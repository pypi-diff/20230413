# Comparing `tmp/strictpy-1.0.0.tar.gz` & `tmp/strictpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictpy-1.0.0.tar", last modified: Wed Apr 12 19:27:46 2023, max compression
+gzip compressed data, was "strictpy-1.1.0.tar", last modified: Thu Apr 13 18:15:29 2023, max compression
```

## Comparing `strictpy-1.0.0.tar` & `strictpy-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:27:46.830418 strictpy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 19:27:33.000000 strictpy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 19:27:46.830418 strictpy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-12 19:27:33.000000 strictpy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 19:27:33.000000 strictpy-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:27:46.830418 strictpy-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:27:46.830418 strictpy-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:27:46.830418 strictpy-1.0.0/src/strictpy/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 19:27:33.000000 strictpy-1.0.0/src/strictpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-12 19:27:33.000000 strictpy-1.0.0/src/strictpy/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 19:27:33.000000 strictpy-1.0.0/src/strictpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-12 19:27:33.000000 strictpy-1.0.0/src/strictpy/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:27:46.830418 strictpy-1.0.0/src/strictpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 19:27:46.000000 strictpy-1.0.0/src/strictpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 19:27:46.000000 strictpy-1.0.0/src/strictpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:27:46.000000 strictpy-1.0.0/src/strictpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 19:27:46.000000 strictpy-1.0.0/src/strictpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:27:46.830418 strictpy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-12 19:27:33.000000 strictpy-1.0.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:29.620903 strictpy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 18:15:20.000000 strictpy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-13 18:15:29.620903 strictpy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-13 18:15:20.000000 strictpy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-13 18:15:20.000000 strictpy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:15:29.620903 strictpy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:29.616903 strictpy-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:29.616903 strictpy-1.1.0/src/strictpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 18:15:20.000000 strictpy-1.1.0/src/strictpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-13 18:15:20.000000 strictpy-1.1.0/src/strictpy/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 18:15:20.000000 strictpy-1.1.0/src/strictpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-13 18:15:20.000000 strictpy-1.1.0/src/strictpy/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:29.620903 strictpy-1.1.0/src/strictpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-13 18:15:29.000000 strictpy-1.1.0/src/strictpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-13 18:15:29.000000 strictpy-1.1.0/src/strictpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:15:29.000000 strictpy-1.1.0/src/strictpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 18:15:29.000000 strictpy-1.1.0/src/strictpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:29.620903 strictpy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 18:15:20.000000 strictpy-1.1.0/tests/test_helpers.py
```

### Comparing `strictpy-1.0.0/LICENSE` & `strictpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strictpy-1.0.0/pyproject.toml` & `strictpy-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "strictpy"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Ishmam Hossain", email="ishmam.dev@gmail.com" },
 ]
 description = "This is a simple decorator that will allow you to implement strict type checking in your everyday cPython functions based on the type hint of the function parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `strictpy-1.0.0/src/strictpy/decorator.py` & `strictpy-1.1.0/src/strictpy/decorator.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                       ensure_type_hints_for,
                       ensure_keyword_only_arguments)
 
 
 def strict(_wrapped_func=None, *,
            force_return_type_check: bool = True) -> Callable:
     def decorator_strict(decorated_func: Callable):
-        ensure_type_hints_for(decorated_func)
+        ensure_type_hints_for(decorated_func, force_return_type_check)
 
         parameter_annotations: dict
         return_type_annotation: dict
         parameter_annotations, return_type_annotation = get_annotations_of(decorated_func)
 
         @functools.wraps(decorated_func)
         def wrapper_strict(*args, **kwargs):
```

### Comparing `strictpy-1.0.0/src/strictpy/helpers.py` & `strictpy-1.1.0/src/strictpy/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 def ensure_param_type_hints(func_signature: inspect.Signature) -> None:
     for name in func_signature.parameters:
         if func_signature.parameters[name].annotation is not _EMPTY:
             continue
         raise TypeHintMissingError(f"parameter type hint cannot be empty for '{name}'")
 
 
-def ensure_type_hints_for(decorated_func: Callable) -> None:
+def ensure_type_hints_for(decorated_func: Callable, force_return_type_check: bool) -> None:
     func_signature = inspect.signature(decorated_func)
     ensure_param_type_hints(func_signature)
-    ensure_return_type_hint(func_signature)
+    if force_return_type_check:
+        ensure_return_type_hint(func_signature)
 
 
 def ensure_keyword_only_arguments(*args: tuple, **_: dict) -> None:
     if (positional_args_len := len(args)) > 0:
         raise PositionalArgumentsNotAllowedException(
             f"Only keyword arguments are expected, "
             f"{positional_args_len} were passed as positional arguments."
@@ -42,10 +43,10 @@
                 f"Expected type of '{param}' is {expected_type}, "
                 f"got {type(received.get(param))} instead."
             )
 
 
 def get_annotations_of(decorated_func: Callable) -> tuple[dict, dict]:
     func_annotations: dict = get_type_hints(decorated_func)
-    return_type_annotation: dict = {'return': func_annotations.pop('return')}
+    return_type_annotation: dict = {'return': func_annotations.pop('return', None)}
     parameter_annotations: dict = func_annotations
     return parameter_annotations, return_type_annotation
```

### Comparing `strictpy-1.0.0/tests/test_helpers.py` & `strictpy-1.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

