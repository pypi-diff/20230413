# Comparing `tmp/pyproject-generator-0.0.1.tar.gz` & `tmp/pyproject-generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.1.tar", last modified: Thu Apr 13 20:57:16 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.2.tar", last modified: Thu Apr 13 21:01:57 2023, max compression
```

## Comparing `pyproject-generator-0.0.1.tar` & `pyproject-generator-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 20:57:16.467127 pyproject-generator-0.0.1/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 20:57:16.467379 pyproject-generator-0.0.1/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.1/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-12 22:11:58.000000 pyproject-generator-0.0.1/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      809 2023-04-13 20:57:16.468963 pyproject-generator-0.0.1/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 20:57:16.452188 pyproject-generator-0.0.1/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 20:57:16.460372 pyproject-generator-0.0.1/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-13 20:46:07.000000 pyproject-generator-0.0.1/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-13 20:36:47.000000 pyproject-generator-0.0.1/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)      799 2023-04-13 20:45:19.000000 pyproject-generator-0.0.1/src/pyproject/cli.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4650 2023-04-13 20:29:53.000000 pyproject-generator-0.0.1/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 20:57:16.465657 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 20:57:16.000000 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      405 2023-04-13 20:57:16.000000 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-13 20:57:16.000000 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-13 20:57:16.000000 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-13 20:57:16.000000 pyproject-generator-0.0.1/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 20:57:16.466699 pyproject-generator-0.0.1/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.1/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879990 pyproject-generator-0.0.2/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 21:01:57.880227 pyproject-generator-0.0.2/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      824 2023-04-13 21:01:57.881625 pyproject-generator-0.0.2/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.864064 pyproject-generator-0.0.2/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.868564 pyproject-generator-0.0.2/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-13 20:46:07.000000 pyproject-generator-0.0.2/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-13 21:01:49.000000 pyproject-generator-0.0.2/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      799 2023-04-13 20:45:19.000000 pyproject-generator-0.0.2/src/pyproject/cli.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4650 2023-04-13 20:29:53.000000 pyproject-generator-0.0.2/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.875109 pyproject-generator-0.0.2/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.2/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.2/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      416 2023-04-13 18:52:00.000000 pyproject-generator-0.0.2/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      632 2023-04-13 17:35:50.000000 pyproject-generator-0.0.2/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.2/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.2/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879034 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      646 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879607 pyproject-generator-0.0.2/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.1/PKG-INFO` & `pyproject-generator-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.1/setup.cfg` & `pyproject-generator-0.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
 [options.package_data]
-pyproject = py.typed
+pyproject = 
+	py.typed
+	templates/*
 
 [options.entry_points]
 console_scripts = 
 	pyproject = pyproject.cli:main
 
 [egg_info]
 tag_build =
```

### Comparing `pyproject-generator-0.0.1/src/pyproject/cli.py` & `pyproject-generator-0.0.2/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.1/src/pyproject/project_builder.py` & `pyproject-generator-0.0.2/src/pyproject/project_builder.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.1/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.2/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

