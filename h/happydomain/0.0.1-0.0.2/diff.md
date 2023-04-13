# Comparing `tmp/happydomain-0.0.1.tar.gz` & `tmp/happydomain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.1.tar", last modified: Wed Apr 12 14:30:00 2023, max compression
+gzip compressed data, was "happydomain-0.0.2.tar", last modified: Thu Apr 13 01:11:47 2023, max compression
```

## Comparing `happydomain-0.0.1.tar` & `happydomain-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:30:00.943946 happydomain-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-12 14:29:11.000000 happydomain-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-12 14:30:00.943946 happydomain-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-12 14:29:11.000000 happydomain-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:30:00.927946 happydomain-0.0.1/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-12 14:29:11.000000 happydomain-0.0.1/happydomain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:30:00.939946 happydomain-0.0.1/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-12 14:30:00.000000 happydomain-0.0.1/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-12 14:30:00.000000 happydomain-0.0.1/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:30:00.000000 happydomain-0.0.1/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-12 14:30:00.000000 happydomain-0.0.1/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 14:30:00.000000 happydomain-0.0.1/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-12 14:29:11.000000 happydomain-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 14:30:00.947945 happydomain-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-12 14:29:11.000000 happydomain-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.806336 happydomain-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 01:11:39.000000 happydomain-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 01:11:47.802337 happydomain-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 01:11:39.000000 happydomain-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.790337 happydomain-0.0.2/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.802337 happydomain-0.0.2/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 01:11:39.000000 happydomain-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 01:11:47.806336 happydomain-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 01:11:39.000000 happydomain-0.0.2/setup.py
```

### Comparing `happydomain-0.0.1/LICENSE` & `happydomain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.1/PKG-INFO` & `happydomain-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.1/happydomain/__init__.py` & `happydomain-0.0.2/happydomain/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,9 +26,7 @@
 # computer knowledge. Users are therefore encouraged to load and test the
 # software's suitability as regards their requirements in conditions enabling
 # the security of their systems and/or data to be ensured and, more generally,
 # to use and operate it in the same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
-
-version = "0.1"
```

### Comparing `happydomain-0.0.1/happydomain.egg-info/PKG-INFO` & `happydomain-0.0.2/happydomain.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.1/pyproject.toml` & `happydomain-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.1/setup.py` & `happydomain-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.1.0"
+version = "0.0.2"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

