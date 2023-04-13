# Comparing `tmp/confguard-1.1.4.tar.gz` & `tmp/confguard-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confguard-1.1.4.tar", last modified: Thu Apr 13 14:07:43 2023, max compression
+gzip compressed data, was "confguard-1.1.5.tar", last modified: Thu Apr 13 14:58:34 2023, max compression
```

## Comparing `confguard-1.1.4.tar` & `confguard-1.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.913418 confguard-1.1.4/
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.4/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.4/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.4/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.4/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:07:43.913523 confguard-1.1.4/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.4/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.4/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 14:07:43.914145 confguard-1.1.4/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.4/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.894894 confguard-1.1.4/src/
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.905033 confguard-1.1.4/src/confguard/
--rw-r--r--   0 Q187392    (501) staff       (20)       44 2023-04-13 14:06:45.000000 confguard-1.1.4/src/confguard/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.4/src/confguard/__main__.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/environment.py
--rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.4/src/confguard/exceptions.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.4/src/confguard/helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7516 2023-04-13 14:05:13.000000 confguard-1.1.4/src/confguard/main.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.4/src/confguard/model.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.909050 confguard-1.1.4/src/confguard.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/entry_points.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 14:07:43.000000 confguard-1.1.4/src/confguard.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:07:43.913042 confguard-1.1.4/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_cli.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.4/tests/test_model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.541811 confguard-1.1.5/
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.5/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.5/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.5/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.5/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:58:34.541960 confguard-1.1.5/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.5/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.5/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 14:58:34.542575 confguard-1.1.5/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.5/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.511359 confguard-1.1.5/src/
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.533782 confguard-1.1.5/src/confguard/
+-rw-r--r--   0 Q187392    (501) staff       (20)       44 2023-04-13 14:57:33.000000 confguard-1.1.5/src/confguard/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.5/src/confguard/__main__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/exceptions.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.5/src/confguard/helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7836 2023-04-13 14:56:07.000000 confguard-1.1.5/src/confguard/main.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.5/src/confguard/model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.538216 confguard-1.1.5/src/confguard.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 14:58:34.000000 confguard-1.1.5/src/confguard.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/entry_points.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.541385 confguard-1.1.5/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_cli.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_model.py
```

### Comparing `confguard-1.1.4/LICENSE` & `confguard-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/PKG-INFO` & `confguard-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.4
+Version: 1.1.5
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.4/README.md` & `confguard-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/setup.cfg` & `confguard-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confguard
-version = 1.1.4
+version = 1.1.5
 description = "Save configuration files outside project in save place"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/confguard
 classifiers =
```

### Comparing `confguard-1.1.4/src/confguard/adapter.py` & `confguard-1.1.5/src/confguard/adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/src/confguard/environment.py` & `confguard-1.1.5/src/confguard/environment.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/src/confguard/helper.py` & `confguard-1.1.5/src/confguard/helper.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/src/confguard/main.py` & `confguard-1.1.5/src/confguard/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -197,17 +197,19 @@
     _log.info(f"Found guarded project files for {project}, re-linking it.")
 
     ConfGuard.restore_toml(source_dir, project)
     _ = _unguard(source_dir)
     return _guard(source_dir)
 
 
-@app.callback()
+@app.callback(invoke_without_command=True)
 def main(
+    ctx: typer.Context,
     verbose: bool = typer.Option(False, "-v", "--verbose", help="verbosity"),
+    version: bool = typer.Option(False, "-V", "--version", help="show version"),
 ):
     # log_fmt = r"%(asctime)-15s %(levelname)-7s %(message)s"
     log_fmt = r"%(message)s"
     # https://github.com/Textualize/rich/issues/1161#issuecomment-813882224
     # https://stackoverflow.com/questions/69348880/is-it-possible-to-use-background-aware-color-choices
     console = Console(
         theme=Theme(
@@ -230,16 +232,20 @@
     else:
         logging.basicConfig(
             format=log_fmt,
             level=logging.INFO,
             datefmt="%m-%d %H:%M:%S",
             handlers=[RichHandler(show_time=False, show_path=False, console=console)],
         )
+    if ctx.invoked_subcommand is None and version:
+        ctx.invoke(print_version)
+    if ctx.invoked_subcommand is None and not version:
+        typer.echo(ctx.get_help())
 
 
-@app.command("version", help="Show version")
+@app.command("version", help="Show version", hidden=True)
 def print_version() -> None:
     typer.echo(f"Confguard version: {__version__}")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `confguard-1.1.4/src/confguard/model.py` & `confguard-1.1.5/src/confguard/model.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/src/confguard.egg-info/PKG-INFO` & `confguard-1.1.5/src/confguard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.4
+Version: 1.1.5
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.4/src/confguard.egg-info/SOURCES.txt` & `confguard-1.1.5/src/confguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/tests/test_adapter.py` & `confguard-1.1.5/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/tests/test_cli.py` & `confguard-1.1.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/tests/test_helper.py` & `confguard-1.1.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.4/tests/test_model.py` & `confguard-1.1.5/tests/test_model.py`

 * *Files identical despite different names*

