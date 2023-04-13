# Comparing `tmp/types-ujson-5.7.0.2.tar.gz` & `tmp/types-ujson-5.7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ujson-5.7.0.2.tar", last modified: Wed Apr 12 15:15:48 2023, max compression
+gzip compressed data, was "types-ujson-5.7.0.3.tar", last modified: Thu Apr 13 15:15:35 2023, max compression
```

## Comparing `types-ujson-5.7.0.2.tar` & `types-ujson-5.7.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:48.333205 types-ujson-5.7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-12 15:15:47.000000 types-ujson-5.7.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 15:15:47.000000 types-ujson-5.7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-12 15:15:48.333205 types-ujson-5.7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:15:48.333205 types-ujson-5.7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 15:15:47.000000 types-ujson-5.7.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:48.333205 types-ujson-5.7.0.2/types_ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-12 15:15:48.000000 types-ujson-5.7.0.2/types_ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 15:15:48.000000 types-ujson-5.7.0.2/types_ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:15:48.000000 types-ujson-5.7.0.2/types_ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 15:15:48.000000 types-ujson-5.7.0.2/types_ujson.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:48.333205 types-ujson-5.7.0.2/ujson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 15:15:47.000000 types-ujson-5.7.0.2/ujson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-12 15:15:47.000000 types-ujson-5.7.0.2/ujson-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/types_ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/ujson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/ujson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/ujson-stubs/__init__.pyi
```

### Comparing `types-ujson-5.7.0.2/CHANGELOG.md` & `types-ujson-5.7.0.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.7.0.3 (2023-04-13)
+
+Make most ujson.dump() parameters keyword-only (#10044)
+
 ## 5.7.0.2 (2023-04-12)
 
 [ujson] Update stubs with new features (#10035)
 
 ## 5.7.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-ujson-5.7.0.2/PKG-INFO` & `types-ujson-5.7.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.2
+Version: 5.7.0.3
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
+This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
```

### Comparing `types-ujson-5.7.0.2/setup.py` & `types-ujson-5.7.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
+This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.7.0.2",
+      version="5.7.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md",
```

### Comparing `types-ujson-5.7.0.2/types_ujson.egg-info/PKG-INFO` & `types-ujson-5.7.0.3/types_ujson.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.2
+Version: 5.7.0.3
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
+This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
```

### Comparing `types-ujson-5.7.0.2/ujson-stubs/__init__.pyi` & `types-ujson-5.7.0.3/ujson-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     reject_bytes: bool = ...,
     default: Callable[[Incomplete], Incomplete] | None = None,
     separators: tuple[str, str] | None = None,
 ) -> str: ...
 def dump(
     obj: Any,
     fp: IO[str],
+    *,
     ensure_ascii: bool = ...,
     double_precision: int = ...,
     encode_html_chars: bool = ...,
     escape_forward_slashes: bool = ...,
     sort_keys: bool = ...,
     indent: int = ...,
     allow_nan: bool = ...,
```

