# Comparing `tmp/databind.core-4.2.3.tar.gz` & `tmp/databind.core-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.3.tar", max compression
+gzip compressed data, was "databind.core-4.2.4.tar", max compression
```

## Comparing `databind.core-4.2.3.tar` & `databind.core-4.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1727 2023-04-12 21:58:45.391794 databind.core-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     1245 2023-03-01 15:01:37.487224 databind.core-4.2.3/readme.md
--rw-r--r--   0        0        0       22 2023-04-12 21:58:45.391794 databind.core-4.2.3/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/context.py
--rw-r--r--   0        0        0     4869 2023-04-12 21:47:28.043974 databind.core-4.2.3/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/py.typed
--rw-r--r--   0        0        0    15320 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/schema.py
--rw-r--r--   0        0        0    26830 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-04-12 21:58:57.866877 databind.core-4.2.3/setup.py
--rw-r--r--   0        0        0     2343 2023-04-12 21:58:57.867233 databind.core-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1727 2023-04-12 22:47:04.968499 databind.core-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1245 2023-03-01 15:01:37.487224 databind.core-4.2.4/readme.md
+-rw-r--r--   0        0        0       22 2023-04-12 22:47:04.968499 databind.core-4.2.4/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5558 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/context.py
+-rw-r--r--   0        0        0     4869 2023-04-12 21:47:28.043974 databind.core-4.2.4/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15234 2023-04-12 22:46:53.368366 databind.core-4.2.4/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26830 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-04-12 22:47:18.282069 databind.core-4.2.4/setup.py
+-rw-r--r--   0        0        0     2343 2023-04-12 22:47:18.282426 databind.core-4.2.4/PKG-INFO
```

### Comparing `databind.core-4.2.3/pyproject.toml` & `databind.core-4.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.3"
+version = "4.2.4"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
@@ -14,15 +14,15 @@
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
 Deprecated = "^1.2.12"
 nr-date = "^2.0.0"
 nr-stream = "^1.0.0"
-typeapi = "^1.2.1"
+typeapi = "^1.4.2"
 typing-extensions = ">=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
```

### Comparing `databind.core-4.2.3/readme.md` & `databind.core-4.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/context.py` & `databind.core-4.2.4/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/converter.py` & `databind.core-4.2.4/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/dataclasses.py` & `databind.core-4.2.4/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/dataclasses.pyi` & `databind.core-4.2.4/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/mapper.py` & `databind.core-4.2.4/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/schema.py` & `databind.core-4.2.4/src/databind/core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,19 +227,15 @@
             if field.name in fields:
                 # Subclasses override their parent's fields.
                 continue
             if field_origin[field.name] != hint.type:
                 # If this field does not belong to the current type
                 continue
 
-            field_hint = (
-                TypeHint(field.type)
-                .evaluate(eval_context_by_type[field_origin[field.name]])
-                .parameterize(parameter_map)
-            )
+            field_hint = TypeHint(field.type, field_origin[field.name]).evaluate().parameterize(parameter_map)
 
             # NOTE(NiklasRosenstein): In Python 3.6, Mypy complains about "Callable does not accept self argument",
             #       but we also cannot ignore it because of warn_unused_ignores.
             _field_default_factory = getattr(field, "default_factory")
 
             default = NotSet.Value if field.default == MISSING else field.default
             default_factory = NotSet.Value if _field_default_factory == MISSING else _field_default_factory
```

### Comparing `databind.core-4.2.3/src/databind/core/settings.py` & `databind.core-4.2.4/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/union.py` & `databind.core-4.2.4/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/src/databind/core/utils.py` & `databind.core-4.2.4/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.3/setup.py` & `databind.core-4.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Deprecated>=1.2.12,<2.0.0',
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
- 'typeapi>=1.2.1,<2.0.0',
+ 'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.3',
+    'version': '4.2.4',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.3/PKG-INFO` & `databind.core-4.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.3
+Version: 4.2.4
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: nr-stream (>=1.0.0,<2.0.0)
-Requires-Dist: typeapi (>=1.2.1,<2.0.0)
+Requires-Dist: typeapi (>=1.4.2,<2.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
 
 # databind.core
```

