# Comparing `tmp/confguard-1.1.3.tar.gz` & `tmp/confguard-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confguard-1.1.3.tar", last modified: Thu Apr 13 13:41:10 2023, max compression
+gzip compressed data, was "confguard-1.1.4.tar", last modified: Thu Apr 13 14:07:43 2023, max compression
```

## Comparing `confguard-1.1.3.tar` & `confguard-1.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.374081 confguard-1.1.3/
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.3/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.3/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.3/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.3/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 13:41:10.374208 confguard-1.1.3/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.3/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.3/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 13:41:10.375120 confguard-1.1.3/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.3/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.325770 confguard-1.1.3/src/
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.359435 confguard-1.1.3/src/confguard/
--rw-r--r--   0 Q187392    (501) staff       (20)       42 2023-04-13 13:40:26.000000 confguard-1.1.3/src/confguard/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.3/src/confguard/__main__.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/environment.py
--rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/exceptions.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.3/src/confguard/helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7354 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/main.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.3/src/confguard/model.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.366710 confguard-1.1.3/src/confguard.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 13:41:10.000000 confguard-1.1.3/src/confguard.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/entry_points.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.373654 confguard-1.1.3/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_cli.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.913418 confguard-1.1.4/
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.4/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.4/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.4/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.4/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:07:43.913523 confguard-1.1.4/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.4/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.4/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 14:07:43.914145 confguard-1.1.4/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.4/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.894894 confguard-1.1.4/src/
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.905033 confguard-1.1.4/src/confguard/
+-rw-r--r--   0 Q187392    (501) staff       (20)       44 2023-04-13 14:06:45.000000 confguard-1.1.4/src/confguard/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.4/src/confguard/__main__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/exceptions.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.4/src/confguard/helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7516 2023-04-13 14:05:13.000000 confguard-1.1.4/src/confguard/main.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.4/src/confguard/model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.909050 confguard-1.1.4/src/confguard.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/entry_points.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.913042 confguard-1.1.4/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_cli.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_model.py
```

### Comparing `confguard-1.1.3/LICENSE` & `confguard-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/PKG-INFO` & `confguard-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.3
+Version: 1.1.4
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.3/README.md` & `confguard-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/setup.cfg` & `confguard-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confguard
-version = 1.1.3
+version = 1.1.4
 description = "Save configuration files outside project in save place"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/confguard
 classifiers =
```

### Comparing `confguard-1.1.3/src/confguard/adapter.py` & `confguard-1.1.4/src/confguard/adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/src/confguard/environment.py` & `confguard-1.1.4/src/confguard/environment.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/src/confguard/helper.py` & `confguard-1.1.4/src/confguard/helper.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/src/confguard/main.py` & `confguard-1.1.4/src/confguard/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 
 import typer
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.theme import Theme
 
+from confguard import __version__
 from confguard.adapter import TomlRepoConfGuard
 from confguard.environment import CONFGUARD_BKP_DIR, CONFGUARD_CONFIG_FILE, config
 from confguard.exceptions import InvalidConfigError
 from confguard.model import ConfGuard
 
 _log = logging.getLogger(__name__)
 app = typer.Typer(help="Save sensitive configuration in a save place")
@@ -231,9 +232,14 @@
             format=log_fmt,
             level=logging.INFO,
             datefmt="%m-%d %H:%M:%S",
             handlers=[RichHandler(show_time=False, show_path=False, console=console)],
         )
 
 
+@app.command("version", help="Show version")
+def print_version() -> None:
+    typer.echo(f"Confguard version: {__version__}")
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `confguard-1.1.3/src/confguard/model.py` & `confguard-1.1.4/src/confguard/model.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/src/confguard.egg-info/PKG-INFO` & `confguard-1.1.4/src/confguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.3
+Version: 1.1.4
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.3/src/confguard.egg-info/SOURCES.txt` & `confguard-1.1.4/src/confguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/tests/test_adapter.py` & `confguard-1.1.4/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/tests/test_cli.py` & `confguard-1.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/tests/test_helper.py` & `confguard-1.1.4/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.3/tests/test_model.py` & `confguard-1.1.4/tests/test_model.py`

 * *Files identical despite different names*

