# Comparing `tmp/types-croniter-1.3.2.8.tar.gz` & `tmp/types-croniter-1.3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-croniter-1.3.2.8.tar", last modified: Sun Apr  9 15:13:39 2023, max compression
+gzip compressed data, was "types-croniter-1.3.2.9.tar", last modified: Thu Apr 13 01:12:14 2023, max compression
```

## Comparing `types-croniter-1.3.2.8.tar` & `types-croniter-1.3.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/croniter-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/croniter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-09 15:13:26.000000 types-croniter-1.3.2.8/croniter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-09 15:13:26.000000 types-croniter-1.3.2.8/croniter-stubs/croniter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-09 15:13:38.000000 types-croniter-1.3.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:13:39.447228 types-croniter-1.3.2.8/types_croniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 15:13:39.000000 types-croniter-1.3.2.8/types_croniter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.837728 types-croniter-1.3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/croniter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/croniter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 01:11:59.000000 types-croniter-1.3.2.9/croniter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-13 01:11:59.000000 types-croniter-1.3.2.9/croniter-stubs/croniter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 01:12:14.837728 types-croniter-1.3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/types_croniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/top_level.txt
```

### Comparing `types-croniter-1.3.2.8/CHANGELOG.md` & `types-croniter-1.3.2.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.3.2.9 (2023-04-13)
+
+Delete allowlist for croniter (#10041)
+
+Fixes #10040
+
 ## 1.3.2.8 (2023-04-09)
 
 Update `croniter` to 1.3.10 (#10027)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 1.3.2.7 (2023-03-27)
```

### Comparing `types-croniter-1.3.2.8/PKG-INFO` & `types-croniter-1.3.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.8
+Version: 1.3.2.9
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
+This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
```

### Comparing `types-croniter-1.3.2.8/croniter-stubs/croniter.pyi` & `types-croniter-1.3.2.9/croniter-stubs/croniter.pyi`

 * *Files identical despite different names*

### Comparing `types-croniter-1.3.2.8/setup.py` & `types-croniter-1.3.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
+This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.2.8",
+      version="1.3.2.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md",
```

### Comparing `types-croniter-1.3.2.8/types_croniter.egg-info/PKG-INFO` & `types-croniter-1.3.2.9/types_croniter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.8
+Version: 1.3.2.9
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `02b8f77630c8dbb60a4d00c362d01519e9639591`.
+This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
```

