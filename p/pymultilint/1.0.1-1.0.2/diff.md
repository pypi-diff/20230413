# Comparing `tmp/pymultilint-1.0.1.tar.gz` & `tmp/pymultilint-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultilint-1.0.1.tar", max compression
+gzip compressed data, was "pymultilint-1.0.2.tar", max compression
```

## Comparing `pymultilint-1.0.1.tar` & `pymultilint-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-13 07:35:00.710831 pymultilint-1.0.1/LICENSE
--rw-r--r--   0        0        0     4518 2023-04-13 07:35:00.710831 pymultilint-1.0.1/README.md
--rwxr-xr-x   0        0        0    18041 2023-04-13 07:35:00.714831 pymultilint-1.0.1/multilint.py
--rw-r--r--   0        0        0     1281 2023-04-13 07:35:00.714831 pymultilint-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 07:38:30.461308 pymultilint-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4518 2023-04-13 07:38:30.461308 pymultilint-1.0.2/README.md
+-rwxr-xr-x   0        0        0    18098 2023-04-13 07:38:30.465308 pymultilint-1.0.2/multilint.py
+-rw-r--r--   0        0        0     1281 2023-04-13 07:38:30.465308 pymultilint-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.2/PKG-INFO
```

### Comparing `pymultilint-1.0.1/LICENSE` & `pymultilint-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.1/README.md` & `pymultilint-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.1/multilint.py` & `pymultilint-1.0.2/multilint.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,16 @@
 
         isort_logger: TextIOLogger = cast(
             TextIOLogger, self.make_logger(TextIOLogger, logging.INFO)
         )
 
         for file in isort_files.find(
             [str(p) for p in self.src_paths]
-            or cast(list[str], DEFAULT_CONFIG.src_paths),
+            # pylint: disable=unsubscriptable-object
+            or cast(Iterable[str], DEFAULT_CONFIG.src_paths),
             DEFAULT_CONFIG,
             [],
             [],
         ):
             try:
                 with patch("sys.stdout", isort_logger):
                     isort_file(file)
```

### Comparing `pymultilint-1.0.1/pyproject.toml` & `pymultilint-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pymultilint"
 packages = [{include = "multilint.py"}]
-version = "1.0.1"
+version = "1.0.2"
 description = "Utility tying multiple code quality tools together"
 authors = ["George Kontridze <george.kontridze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gkze/multilint"
 repository = "https://github.com/gkze/multilint"
 documentation = "https://gkze.github.io/multilint/multilint.html"
```

### Comparing `pymultilint-1.0.1/PKG-INFO` & `pymultilint-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultilint
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility tying multiple code quality tools together
 Home-page: https://github.com/gkze/multilint
 License: MIT
 Keywords: lint,code-quality,tools
 Author: George Kontridze
 Author-email: george.kontridze@gmail.com
 Requires-Python: >=3.8,<4.0
```

