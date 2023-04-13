# Comparing `tmp/ansible-variables-0.3.0.tar.gz` & `tmp/ansible-variables-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.3.0.tar", last modified: Thu Apr 13 21:02:39 2023, max compression
+gzip compressed data, was "ansible-variables-0.3.1.tar", last modified: Thu Apr 13 21:13:21 2023, max compression
```

## Comparing `ansible-variables-0.3.0.tar` & `ansible-variables-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.851257 ansible-variables-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 21:02:39.851257 ansible-variables-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.843257 ansible-variables-0.3.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.847257 ansible-variables-0.3.0/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.847257 ansible-variables-0.3.0/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.847257 ansible-variables-0.3.0/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.847257 ansible-variables-0.3.0/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:02:39.000000 ansible-variables-0.3.0/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 21:02:39.851257 ansible-variables-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:02:39.851257 ansible-variables-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-13 21:02:27.000000 ansible-variables-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.511618 ansible-variables-0.3.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.511618 ansible-variables-0.3.1/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/tests/test_utils.py
```

### Comparing `ansible-variables-0.3.0/LICENSE` & `ansible-variables-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/PKG-INFO` & `ansible-variables-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.3.0
-Summary: Variables for Ansible
+Version: 0.3.1
+Summary: Check from where Ansible inventory variables are comming from
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ansible-variables-0.3.0/README.md` & `ansible-variables-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/lib/ansible_variables/cli/variables.py` & `ansible-variables-0.3.1/lib/ansible_variables/cli/variables.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/lib/ansible_variables/utils/vars.py` & `ansible-variables-0.3.1/lib/ansible_variables/utils/vars.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/lib/ansible_variables.egg-info/PKG-INFO` & `ansible-variables-0.3.1/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.3.0
-Summary: Variables for Ansible
+Version: 0.3.1
+Summary: Check from where Ansible inventory variables are comming from
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ansible-variables-0.3.0/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.3.1/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/setup.cfg` & `ansible-variables-0.3.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = ansible-variables
-version = 0.3.0
-description = Variables for Ansible
+version = 0.3.1
+description = Check from where Ansible inventory variables are comming from
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls = 
 	Bug Tracker=https://github.com/hille721/ansible-variables/issues
```

### Comparing `ansible-variables-0.3.0/tests/test_cli.py` & `ansible-variables-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.0/tests/test_utils.py` & `ansible-variables-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

