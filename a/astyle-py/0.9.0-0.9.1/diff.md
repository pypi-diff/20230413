# Comparing `tmp/astyle_py-0.9.0.tar.gz` & `tmp/astyle_py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astyle_py-0.9.0.tar", last modified: Wed Aug 31 16:03:16 2022, max compression
+gzip compressed data, was "astyle_py-0.9.1.tar", last modified: Thu Apr 13 14:18:42 2023, max compression
```

## Comparing `astyle_py-0.9.0.tar` & `astyle_py-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:03:16.537079 astyle_py-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-08-31 16:03:06.000000 astyle_py-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2022-08-31 16:03:16.537079 astyle_py-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2022-08-31 16:03:06.000000 astyle_py-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:03:16.537079 astyle_py-0.9.0/astyle_py/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/args.py
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/astyle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/files_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   395039 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/libastyle.wasm
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-08-31 16:03:06.000000 astyle_py-0.9.0/astyle_py/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:03:16.537079 astyle_py-0.9.0/astyle_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-31 16:03:16.000000 astyle_py-0.9.0/astyle_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-31 16:03:06.000000 astyle_py-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-08-31 16:03:16.537079 astyle_py-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-31 16:03:06.000000 astyle_py-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:03:16.537079 astyle_py-0.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-08-31 16:03:06.000000 astyle_py-0.9.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-08-31 16:03:06.000000 astyle_py-0.9.0/test/test_astyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-08-31 16:03:06.000000 astyle_py-0.9.0/test/test_files_iter.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-08-31 16:03:06.000000 astyle_py-0.9.0/test/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:18:42.704817 astyle_py-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 14:18:29.000000 astyle_py-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-13 14:18:42.704817 astyle_py-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-13 14:18:29.000000 astyle_py-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:18:42.704817 astyle_py-0.9.1/astyle_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/astyle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/files_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   395039 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/libastyle.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-13 14:18:29.000000 astyle_py-0.9.1/astyle_py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:18:42.704817 astyle_py-0.9.1/astyle_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 14:18:42.000000 astyle_py-0.9.1/astyle_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 14:18:29.000000 astyle_py-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-13 14:18:42.704817 astyle_py-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 14:18:29.000000 astyle_py-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:18:42.704817 astyle_py-0.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 14:18:29.000000 astyle_py-0.9.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 14:18:29.000000 astyle_py-0.9.1/test/test_astyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-13 14:18:29.000000 astyle_py-0.9.1/test/test_files_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 14:18:29.000000 astyle_py-0.9.1/test/test_sample.py
```

### Comparing `astyle_py-0.9.0/LICENSE` & `astyle_py-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/PKG-INFO` & `astyle_py-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astyle_py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Astyle, wrapped in a python package.
 Home-page: https://github.com/igrr/astyle_py
 Author: Ivan Grokhotkov
 Author-email: ivan@espressif.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `astyle_py-0.9.0/README.md` & `astyle_py-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py/__main__.py` & `astyle_py-0.9.1/astyle_py/__main__.py`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py/args.py` & `astyle_py-0.9.1/astyle_py/args.py`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py/astyle_wrapper.py` & `astyle_py-0.9.1/astyle_py/astyle_wrapper.py`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py/files_iter.py` & `astyle_py-0.9.1/astyle_py/files_iter.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return any((re.search(regex, fname_match) for regex in patterns))
 
 
 def iterate_files(args: AstyleArgs) -> Generator[FileItem, None, None]:
     if args.rules is None:
         yield from iterate_files_simple(args.files, args.exclude_list, args.options)
     else:
-        raise NotImplementedError('args.rules not implemented yet')
+        yield from iterate_files_rules(args.files, args.rules)
 
 
 def iterate_files_simple(
     files: List[str], exclude_list: List[str], options: List[str]
 ) -> Generator[FileItem, None, None]:
     exclude_regexes = [re.compile(pattern_to_regex(p)) for p in exclude_list]
```

### Comparing `astyle_py-0.9.0/astyle_py/libastyle.wasm` & `astyle_py-0.9.1/astyle_py/libastyle.wasm`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py/utils.py` & `astyle_py-0.9.1/astyle_py/utils.py`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/astyle_py.egg-info/PKG-INFO` & `astyle_py-0.9.1/astyle_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astyle-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Astyle, wrapped in a python package.
 Home-page: https://github.com/igrr/astyle_py
 Author: Ivan Grokhotkov
 Author-email: ivan@espressif.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `astyle_py-0.9.0/setup.cfg` & `astyle_py-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/test/test_args.py` & `astyle_py-0.9.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `astyle_py-0.9.0/test/test_files_iter.py` & `astyle_py-0.9.1/test/test_files_iter.py`

 * *Files identical despite different names*

