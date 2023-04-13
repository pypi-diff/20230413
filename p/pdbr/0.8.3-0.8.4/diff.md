# Comparing `tmp/pdbr-0.8.3.tar.gz` & `tmp/pdbr-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbr-0.8.3.tar", max compression
+gzip compressed data, was "pdbr-0.8.4.tar", max compression
```

## Comparing `pdbr-0.8.3.tar` & `pdbr-0.8.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-04-12 21:02:07.507291 pdbr-0.8.3/LICENSE
--rw-r--r--   0        0        0     6273 2023-04-12 21:02:07.507291 pdbr-0.8.3/README.md
--rw-r--r--   0        0        0      286 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/__main__.py
--rw-r--r--   0        0        0     1206 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_cm.py
--rw-r--r--   0        0        0     1485 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_console_layout.py
--rw-r--r--   0        0        0    15955 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_pdbr.py
--rw-r--r--   0        0        0     1306 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/cli.py
--rw-r--r--   0        0        0     1421 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/helpers.py
--rw-r--r--   0        0        0        0 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/__init__.py
--rw-r--r--   0        0        0      492 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/django.py
--rw-r--r--   0        0        0      334 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/starlette.py
--rw-r--r--   0        0        0      782 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/runner.py
--rw-r--r--   0        0        0     3242 2023-04-12 21:02:07.523291 pdbr-0.8.3/pdbr/utils.py
--rw-r--r--   0        0        0     1762 2023-04-12 21:02:07.523291 pdbr-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 15:22:51.909584 pdbr-0.8.4/LICENSE
+-rw-r--r--   0        0        0     6273 2023-04-13 15:22:51.909584 pdbr-0.8.4/README.md
+-rw-r--r--   0        0        0      286 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/__main__.py
+-rw-r--r--   0        0        0     1206 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_cm.py
+-rw-r--r--   0        0        0     1485 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_console_layout.py
+-rw-r--r--   0        0        0    15974 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_pdbr.py
+-rw-r--r--   0        0        0     1306 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/cli.py
+-rw-r--r--   0        0        0     1421 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/django.py
+-rw-r--r--   0        0        0      334 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/starlette.py
+-rw-r--r--   0        0        0      782 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/runner.py
+-rw-r--r--   0        0        0     3242 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/utils.py
+-rw-r--r--   0        0        0     1762 2023-04-13 15:22:51.921584 pdbr-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.4/PKG-INFO
```

### Comparing `pdbr-0.8.3/LICENSE` & `pdbr-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/README.md` & `pdbr-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/__main__.py` & `pdbr-0.8.4/pdbr/__main__.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/_cm.py` & `pdbr-0.8.4/pdbr/_cm.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/_console_layout.py` & `pdbr-0.8.4/pdbr/_console_layout.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/_pdbr.py` & `pdbr-0.8.4/pdbr/_pdbr.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
                 self.error(f"{type(e).__qualname__} in onecmd({line!r}): {e}")
                 return False
 
         def _print(self, val, prefix=None, style=None, print_layout=True):
             if val == "--Return--":
                 return
 
-            if isinstance(val, str) and "[" in val:
+            if isinstance(val, str) and ("[0m" in val or "[/" in val):
                 val = markup.render(val)
 
             kwargs = {"style": str(style)} if style else {}
             args = (prefix, val) if prefix else (val,)
             if (
                 show_layouts
                 and print_layout
```

### Comparing `pdbr-0.8.3/pdbr/cli.py` & `pdbr-0.8.4/pdbr/cli.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/helpers.py` & `pdbr-0.8.4/pdbr/helpers.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/runner.py` & `pdbr-0.8.4/pdbr/runner.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pdbr/utils.py` & `pdbr-0.8.4/pdbr/utils.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.3/pyproject.toml` & `pdbr-0.8.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdbr"
-version = "0.8.3"
+version = "0.8.4"
 description = "Pdb with Rich library."
 authors = ["Can Sarigol <ertugrulsarigol@gmail.com>"]
 packages = [
     { include = "pdbr" }
 ]
 readme = "README.md"
 homepage = "https://github.com/cansarigol/pdbr"
@@ -52,15 +52,15 @@
 min_confidence = 80
 paths = ["pdbr", "tests"]
 sort_by_size = true
 verbose = false
 
 [project]
 name = "pdbr"
-version = "0.8.3"
+version = "0.8.4"
 
 [tool.setuptools]
 py-modules = []
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle errors
```

### Comparing `pdbr-0.8.3/PKG-INFO` & `pdbr-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbr
-Version: 0.8.3
+Version: 0.8.4
 Summary: Pdb with Rich library.
 Home-page: https://github.com/cansarigol/pdbr
 Author: Can Sarigol
 Author-email: ertugrulsarigol@gmail.com
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

