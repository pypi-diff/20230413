# Comparing `tmp/retroperm-0.0.1.tar.gz` & `tmp/retroperm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retroperm-0.0.1.tar", last modified: Thu Apr 13 10:08:45 2023, max compression
+gzip compressed data, was "retroperm-0.0.2.tar", last modified: Thu Apr 13 11:20:19 2023, max compression
```

## Comparing `retroperm-0.0.1.tar` & `retroperm-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.477744 retroperm-0.0.1/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.0.1/LICENSE
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 10:08:45.477744 retroperm-0.0.1/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.0.1/README.md
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-04-13 09:57:58.000000 retroperm-0.0.1/pyproject.toml
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.0.1/retroperm/__init__.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/analysis/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.0.1/retroperm/analysis/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.0.1/retroperm/analysis/functions.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.0.1/retroperm/analysis/permfinder.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.0.1/retroperm/analysis/resolver.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.0.1/retroperm/analysis/utils.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.0.1/retroperm/analysis/utils_angrmgmt.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     5909 2023-04-13 05:42:14.000000 retroperm-0.0.1/retroperm/project.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm/rules/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       23 2023-04-11 22:53:49.000000 retroperm-0.0.1/retroperm/rules/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      412 2023-04-04 07:23:47.000000 retroperm-0.0.1/retroperm/rules/data.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.0.1/retroperm/rules/default_rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2537 2023-04-13 05:40:22.000000 retroperm-0.0.1/retroperm/rules/filesystem_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.0.1/retroperm/rules/pathrules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      947 2023-04-12 04:17:48.000000 retroperm-0.0.1/retroperm/rules/rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.0.1/retroperm/rules/ruleList.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.0.1/retroperm/rules/rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.0.1/retroperm/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.473744 retroperm-0.0.1/retroperm.egg-info/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      717 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/SOURCES.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/dependency_links.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       12 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/requires.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-04-13 10:08:45.000000 retroperm-0.0.1/retroperm.egg-info/top_level.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      529 2023-04-13 10:08:45.477744 retroperm-0.0.1/setup.cfg
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.0.1/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 10:08:45.477744 retroperm-0.0.1/tests/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2113 2023-04-13 05:45:01.000000 retroperm-0.0.1/tests/test_project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.980797 retroperm-0.0.2/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.0.2/LICENSE
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 11:20:19.980797 retroperm-0.0.2/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.0.2/README.md
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-04-13 11:19:35.000000 retroperm-0.0.2/pyproject.toml
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.976797 retroperm-0.0.2/retroperm/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.0.2/retroperm/__init__.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.980797 retroperm-0.0.2/retroperm/analysis/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.0.2/retroperm/analysis/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.0.2/retroperm/analysis/functions.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.0.2/retroperm/analysis/permfinder.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.0.2/retroperm/analysis/resolver.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.0.2/retroperm/analysis/utils.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.0.2/retroperm/analysis/utils_angrmgmt.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     5909 2023-04-13 11:18:32.000000 retroperm-0.0.2/retroperm/project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.980797 retroperm-0.0.2/retroperm/rules/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       23 2023-04-11 22:53:49.000000 retroperm-0.0.2/retroperm/rules/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      614 2023-04-13 10:13:49.000000 retroperm-0.0.2/retroperm/rules/data.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.0.2/retroperm/rules/default_rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2537 2023-04-13 05:40:22.000000 retroperm-0.0.2/retroperm/rules/filesystem_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.0.2/retroperm/rules/pathrules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      947 2023-04-12 04:17:48.000000 retroperm-0.0.2/retroperm/rules/rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.0.2/retroperm/rules/ruleList.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.0.2/retroperm/rules/rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.0.2/retroperm/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.976797 retroperm-0.0.2/retroperm.egg-info/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 11:20:19.000000 retroperm-0.0.2/retroperm.egg-info/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      717 2023-04-13 11:20:19.000000 retroperm-0.0.2/retroperm.egg-info/SOURCES.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-04-13 11:20:19.000000 retroperm-0.0.2/retroperm.egg-info/dependency_links.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       12 2023-04-13 11:20:19.000000 retroperm-0.0.2/retroperm.egg-info/requires.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-04-13 11:20:19.000000 retroperm-0.0.2/retroperm.egg-info/top_level.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      529 2023-04-13 11:20:19.980797 retroperm-0.0.2/setup.cfg
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.0.2/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:20:19.980797 retroperm-0.0.2/tests/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2113 2023-04-13 05:45:01.000000 retroperm-0.0.2/tests/test_project.py
```

### Comparing `retroperm-0.0.1/LICENSE` & `retroperm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/PKG-INFO` & `retroperm-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.0.1/pyproject.toml` & `retroperm-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retroperm"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Saketh Reddy", email="yssaketh@gmail.com" },
 ]
 description = "A retroactive effective binary permission deduction tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `retroperm-0.0.1/retroperm/analysis/functions.py` & `retroperm-0.0.2/retroperm/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/analysis/permfinder.py` & `retroperm-0.0.2/retroperm/analysis/permfinder.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/analysis/resolver.py` & `retroperm-0.0.2/retroperm/analysis/resolver.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/analysis/utils.py` & `retroperm-0.0.2/retroperm/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/analysis/utils_angrmgmt.py` & `retroperm-0.0.2/retroperm/analysis/utils_angrmgmt.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/project.py` & `retroperm-0.0.2/retroperm/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 import angr
-from reference.utils_angrmgmt import string_at_addr
 from .analysis.utils import get_arg_locations
+from .analysis.utils_angrmgmt import string_at_addr
 from .rules.data import important_func_args
 from .rules import Rule, default_rules
 import pyvex
 
 import logging
 
 logging.getLogger('angr.analyses.reaching_definitions').setLevel(logging.FATAL)
```

### Comparing `retroperm-0.0.1/retroperm/rules/filesystem_rule.py` & `retroperm-0.0.2/retroperm/rules/filesystem_rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/rules/rule.py` & `retroperm-0.0.2/retroperm/rules/rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm/rules/ruleList.py` & `retroperm-0.0.2/retroperm/rules/ruleList.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/retroperm.egg-info/PKG-INFO` & `retroperm-0.0.2/retroperm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.0.1/retroperm.egg-info/SOURCES.txt` & `retroperm-0.0.2/retroperm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/setup.cfg` & `retroperm-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.1/tests/test_project.py` & `retroperm-0.0.2/tests/test_project.py`

 * *Files identical despite different names*

