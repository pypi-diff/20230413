# Comparing `tmp/retroperm-0.0.0.tar.gz` & `tmp/retroperm-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retroperm-0.0.0.tar", last modified: Thu Apr 13 10:00:04 2023, max compression
+gzip compressed data, was "retroperm-0.0.1.tar", last modified: Thu Apr 13 10:08:45 2023, max compression
```

## Comparing `retroperm-0.0.0.tar` & `retroperm-0.0.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1069 2023-03-24 14:47:52.000000 retroperm-0.0.0/LICENSE
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      627 2023-04-13 10:00:04.631225 retroperm-0.0.0/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.0.0/README.md
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/retroperm/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.0.0/retroperm/__init__.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/retroperm/analysis/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.0.0/retroperm/analysis/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.0.0/retroperm/analysis/functions.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.0.0/retroperm/analysis/permfinder.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.0.0/retroperm/analysis/resolver.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.0.0/retroperm/analysis/utils.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.0.0/retroperm/analysis/utils_angrmgmt.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     5909 2023-04-13 05:42:14.000000 retroperm-0.0.0/retroperm/project.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/retroperm/rules/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       23 2023-04-11 22:53:49.000000 retroperm-0.0.0/retroperm/rules/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      412 2023-04-04 07:23:47.000000 retroperm-0.0.0/retroperm/rules/data.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.0.0/retroperm/rules/default_rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2537 2023-04-13 05:40:22.000000 retroperm-0.0.0/retroperm/rules/filesystem_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.0.0/retroperm/rules/pathrules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      947 2023-04-12 04:17:48.000000 retroperm-0.0.0/retroperm/rules/rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.0.0/retroperm/rules/ruleList.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.0.0/retroperm/rules/rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.0.0/retroperm/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/retroperm.egg-info/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      627 2023-04-13 10:00:04.000000 retroperm-0.0.0/retroperm.egg-info/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      702 2023-04-13 10:00:04.000000 retroperm-0.0.0/retroperm.egg-info/SOURCES.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-04-13 10:00:04.000000 retroperm-0.0.0/retroperm.egg-info/dependency_links.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       12 2023-04-13 10:00:04.000000 retroperm-0.0.0/retroperm.egg-info/requires.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-04-13 10:00:04.000000 retroperm-0.0.0/retroperm.egg-info/top_level.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      529 2023-04-13 10:00:04.635225 retroperm-0.0.0/setup.cfg
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.0.0/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:00:04.631225 retroperm-0.0.0/tests/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2113 2023-04-13 05:45:01.000000 retroperm-0.0.0/tests/test_project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.477744 retroperm-0.0.1/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.0.1/LICENSE
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 10:08:45.477744 retroperm-0.0.1/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.0.1/README.md
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-04-13 09:57:58.000000 retroperm-0.0.1/pyproject.toml
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.0.1/retroperm/__init__.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/analysis/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.0.1/retroperm/analysis/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.0.1/retroperm/analysis/functions.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.0.1/retroperm/analysis/permfinder.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.0.1/retroperm/analysis/resolver.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.0.1/retroperm/analysis/utils.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.0.1/retroperm/analysis/utils_angrmgmt.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     5909 2023-04-13 05:42:14.000000 retroperm-0.0.1/retroperm/project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/rules/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       23 2023-04-11 22:53:49.000000 retroperm-0.0.1/retroperm/rules/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      412 2023-04-04 07:23:47.000000 retroperm-0.0.1/retroperm/rules/data.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.0.1/retroperm/rules/default_rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2537 2023-04-13 05:40:22.000000 retroperm-0.0.1/retroperm/rules/filesystem_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.0.1/retroperm/rules/pathrules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      947 2023-04-12 04:17:48.000000 retroperm-0.0.1/retroperm/rules/rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.0.1/retroperm/rules/ruleList.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.0.1/retroperm/rules/rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.0.1/retroperm/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm.egg-info/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      717 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/SOURCES.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/dependency_links.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       12 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/requires.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/top_level.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      529 2023-04-13 10:08:45.477744 retroperm-0.0.1/setup.cfg
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.0.1/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.477744 retroperm-0.0.1/tests/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2113 2023-04-13 05:45:01.000000 retroperm-0.0.1/tests/test_project.py
```

### Comparing `retroperm-0.0.0/PKG-INFO` & `retroperm-0.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.0
-Summary: A retro permission library
+Version: 0.0.1
+Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
+Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
-Classifier: License :: OSI Approved :: BSD License
+Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
+Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Retroperm
 A platform-agnostic retroactive effective permission generation system for compiled executables built using angr
 
 ## Developer Install
```

### Comparing `retroperm-0.0.0/retroperm/analysis/functions.py` & `retroperm-0.0.1/retroperm/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/analysis/permfinder.py` & `retroperm-0.0.1/retroperm/analysis/permfinder.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/analysis/resolver.py` & `retroperm-0.0.1/retroperm/analysis/resolver.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/analysis/utils.py` & `retroperm-0.0.1/retroperm/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/analysis/utils_angrmgmt.py` & `retroperm-0.0.1/retroperm/analysis/utils_angrmgmt.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/project.py` & `retroperm-0.0.1/retroperm/project.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/rules/filesystem_rule.py` & `retroperm-0.0.1/retroperm/rules/filesystem_rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/rules/rule.py` & `retroperm-0.0.1/retroperm/rules/rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm/rules/ruleList.py` & `retroperm-0.0.1/retroperm/rules/ruleList.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/retroperm.egg-info/PKG-INFO` & `retroperm-0.0.1/retroperm.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.0
-Summary: A retro permission library
+Version: 0.0.1
+Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
+Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
-Classifier: License :: OSI Approved :: BSD License
+Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
+Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Retroperm
 A platform-agnostic retroactive effective permission generation system for compiled executables built using angr
 
 ## Developer Install
```

### Comparing `retroperm-0.0.0/retroperm.egg-info/SOURCES.txt` & `retroperm-0.0.1/retroperm.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 retroperm/__init__.py
 retroperm/project.py
 retroperm/setup.py
 retroperm.egg-info/PKG-INFO
 retroperm.egg-info/SOURCES.txt
```

### Comparing `retroperm-0.0.0/setup.cfg` & `retroperm-0.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.0/tests/test_project.py` & `retroperm-0.0.1/tests/test_project.py`

 * *Files identical despite different names*

