# Comparing `tmp/easytypes-0.5.2.tar.gz` & `tmp/easytypes-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytypes-0.5.2.tar", max compression
+gzip compressed data, was "easytypes-0.5.3.tar", max compression
```

## Comparing `easytypes-0.5.2.tar` & `easytypes-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-12 10:11:15.182833 easytypes-0.5.2/LICENSE
--rw-r--r--   0        0        0     2627 2023-04-12 10:11:15.182833 easytypes-0.5.2/README.md
--rw-r--r--   0        0        0      368 2023-04-12 10:11:15.182833 easytypes-0.5.2/easytypes/__init__.py
--rw-r--r--   0        0        0     4508 2023-04-12 10:11:15.182833 easytypes-0.5.2/easytypes/easytypes_impl.py
--rw-r--r--   0        0        0     4639 2023-04-12 10:11:15.182833 easytypes-0.5.2/easytypes/easytypes_test.py
--rw-r--r--   0        0        0      866 2023-04-12 10:11:15.182833 easytypes-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 easytypes-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 15:46:26.605413 easytypes-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2627 2023-04-13 15:46:26.605413 easytypes-0.5.3/README.md
+-rw-r--r--   0        0        0      368 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/__init__.py
+-rw-r--r--   0        0        0     4449 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/easytypes_impl.py
+-rw-r--r--   0        0        0     4639 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/easytypes_test.py
+-rw-r--r--   0        0        0      866 2023-04-13 15:46:26.605413 easytypes-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 easytypes-0.5.3/PKG-INFO
```

### Comparing `easytypes-0.5.2/LICENSE` & `easytypes-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.2/README.md` & `easytypes-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.2/easytypes/easytypes_impl.py` & `easytypes-0.5.3/easytypes/easytypes_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,18 +102,16 @@
             object.__delattr__(self, attrname)
 
         def _str(self) -> str:
             keys = list(self.__dict__.keys())
             keys.sort()  # We need the results to be repeatable
             return f"<{self.__class__.__name__} {', '.join(f'{k}={self.__dict__[k]!r}' for k in keys)}>"
 
-        methods = {"__init__": _init, "__str__": _str, "__repr__": _str}
-        if chk_r or chk_a or chk_t:
-            methods['__setattr__'] = _setattr
-            methods['__delattr__'] = _delattr
+        methods = {"__init__": _init, "__str__": _str, "__repr__": _str,
+                   "__setattr__": _setattr, "__delattr__": _delattr}
         return type(f"_easy_type.{cls.__name__}", (cls,), methods)
 
     return wrapper
 
 
 fast_type = easy_type_decorator(False, False, False)  # No checks, just the attribute machinery
 unlimited_type = easy_type_decorator(True, False, True)  # Checks on, extra attrs allowed
```

### Comparing `easytypes-0.5.2/easytypes/easytypes_test.py` & `easytypes-0.5.3/easytypes/easytypes_test.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.2/pyproject.toml` & `easytypes-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easytypes"
-version = "0.5.2"
+version = "0.5.3"
 description = "Easy declaration of data structures with runtime type checking"
 authors = ["Reim, Elijah <Elijah.Reim@wartsila.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/e-reim/easytypes"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `easytypes-0.5.2/PKG-INFO` & `easytypes-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytypes
-Version: 0.5.2
+Version: 0.5.3
 Summary: Easy declaration of data structures with runtime type checking
 Home-page: https://github.com/e-reim/easytypes
 License: Apache-2.0
 Author: Reim, Elijah
 Author-email: Elijah.Reim@wartsila.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

