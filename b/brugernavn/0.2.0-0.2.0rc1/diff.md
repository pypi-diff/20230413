# Comparing `tmp/brugernavn-0.2.0.tar.gz` & `tmp/brugernavn-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brugernavn-0.2.0.tar", max compression
+gzip compressed data, was "brugernavn-0.2.0rc1.tar", max compression
```

## Comparing `brugernavn-0.2.0.tar` & `brugernavn-0.2.0rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1110 2023-03-04 23:46:25.661963 brugernavn-0.2.0/LICENSE
--rw-r--r--   0        0        0      292 2023-03-04 23:46:25.661963 brugernavn-0.2.0/README.md
--rw-r--r--   0        0        0       35 2023-03-04 23:46:25.661963 brugernavn-0.2.0/brugernavn/__init__.py
--rw-r--r--   0        0        0      809 2023-04-11 22:45:27.179804 brugernavn-0.2.0/brugernavn/__main__.py
--rw-r--r--   0        0        0     2804 2023-04-11 22:45:27.179804 brugernavn-0.2.0/brugernavn/brugernavn.py
--rw-r--r--   0        0        0     8677 2023-03-04 23:46:25.661963 brugernavn-0.2.0/brugernavn/ressources/data.json
--rw-r--r--   0        0        0      325 2023-03-04 23:46:25.661963 brugernavn-0.2.0/brugernavn/ressources/tests.json
--rw-r--r--   0        0        0      441 2023-03-04 23:46:25.661963 brugernavn-0.2.0/brugernavn/test_brugernavn.py
--rw-r--r--   0        0        0      368 2023-04-11 22:45:27.183805 brugernavn-0.2.0/brugernavn/test_typer.py
--rw-r--r--   0        0        0      701 2023-04-13 11:48:04.225190 brugernavn-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 brugernavn-0.2.0/setup.py
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 brugernavn-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0      292 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/README.md
+-rw-r--r--   0        0        0       35 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/brugernavn/__init__.py
+-rw-r--r--   0        0        0      809 2023-03-05 21:51:53.570859 brugernavn-0.2.0rc1/brugernavn/__main__.py
+-rw-r--r--   0        0        0     2804 2023-03-05 21:51:53.614859 brugernavn-0.2.0rc1/brugernavn/brugernavn.py
+-rw-r--r--   0        0        0     8677 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/brugernavn/ressources/data.json
+-rw-r--r--   0        0        0      325 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/brugernavn/ressources/tests.json
+-rw-r--r--   0        0        0      441 2023-03-04 23:46:25.661963 brugernavn-0.2.0rc1/brugernavn/test_brugernavn.py
+-rw-r--r--   0        0        0      368 2023-03-05 21:51:53.562859 brugernavn-0.2.0rc1/brugernavn/test_typer.py
+-rw-r--r--   0        0        0      704 2023-03-06 22:45:53.753105 brugernavn-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 brugernavn-0.2.0rc1/setup.py
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 brugernavn-0.2.0rc1/PKG-INFO
```

### Comparing `brugernavn-0.2.0/LICENSE` & `brugernavn-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `brugernavn-0.2.0/brugernavn/__main__.py` & `brugernavn-0.2.0rc1/brugernavn/__main__.py`

 * *Files identical despite different names*

### Comparing `brugernavn-0.2.0/brugernavn/brugernavn.py` & `brugernavn-0.2.0rc1/brugernavn/brugernavn.py`

 * *Files identical despite different names*

### Comparing `brugernavn-0.2.0/brugernavn/ressources/data.json` & `brugernavn-0.2.0rc1/brugernavn/ressources/data.json`

 * *Files identical despite different names*

### Comparing `brugernavn-0.2.0/pyproject.toml` & `brugernavn-0.2.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brugernavn"
-version = "0.2.0"
+version = "0.2.0rc1"
 readme = "README.md"
 description = "An OSINT tool to search for a username on many websites"
 authors = ["Jonathan Krüger <jonathan.krueger@teckids.org>"]
 license = "MIT"
 repository = "https://edugit.org/pinguin/brugernavn"
 keywords = ["osint", "osint tool", "search", "username"]
 classifiers = [
```

### Comparing `brugernavn-0.2.0/setup.py` & `brugernavn-0.2.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'brugernavn': ['ressources/*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0', 'typer>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'brugernavn',
-    'version': '0.2.0',
+    'version': '0.2.0rc1',
     'description': 'An OSINT tool to search for a username on many websites',
     'long_description': '# Brugernavn\n\nBrugernavn is an OSINT tool to search for user names at websites.\nYou can find the project [here](https://edugit.org/pinguin/brugernavn).\nBrugernavn is licensed under the MIT License, the document can be found [here](https://edugit.org/pinguin/brugernavn/-/blob/master/LICENSE).',
     'author': 'Jonathan Krüger',
     'author_email': 'jonathan.krueger@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://edugit.org/pinguin/brugernavn',
```

### Comparing `brugernavn-0.2.0/PKG-INFO` & `brugernavn-0.2.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brugernavn
-Version: 0.2.0
+Version: 0.2.0rc1
 Summary: An OSINT tool to search for a username on many websites
 Home-page: https://edugit.org/pinguin/brugernavn
 License: MIT
 Keywords: osint,osint tool,search,username
 Author: Jonathan Krüger
 Author-email: jonathan.krueger@teckids.org
 Requires-Python: >=3.9,<4.0
```

