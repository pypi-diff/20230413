# Comparing `tmp/types-hdbcli-2.15.0.2.tar.gz` & `tmp/types-hdbcli-2.15.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hdbcli-2.15.0.2.tar", last modified: Tue Mar 28 01:19:12 2023, max compression
+gzip compressed data, was "types-hdbcli-2.15.0.3.tar", last modified: Thu Apr 13 12:31:07 2023, max compression
```

## Comparing `types-hdbcli-2.15.0.2.tar` & `types-hdbcli-2.15.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:19:12.386909 types-hdbcli-2.15.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-28 01:19:11.000000 types-hdbcli-2.15.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 01:19:11.000000 types-hdbcli-2.15.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-28 01:19:12.386909 types-hdbcli-2.15.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:19:12.386909 types-hdbcli-2.15.0.2/hdbcli-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 01:19:11.000000 types-hdbcli-2.15.0.2/hdbcli-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-28 01:18:59.000000 types-hdbcli-2.15.0.2/hdbcli-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-03-28 01:18:59.000000 types-hdbcli-2.15.0.2/hdbcli-stubs/dbapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-28 01:18:59.000000 types-hdbcli-2.15.0.2/hdbcli-stubs/resultrow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 01:19:12.386909 types-hdbcli-2.15.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-28 01:19:11.000000 types-hdbcli-2.15.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:19:12.386909 types-hdbcli-2.15.0.2/types_hdbcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-28 01:19:12.000000 types-hdbcli-2.15.0.2/types_hdbcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-28 01:19:12.000000 types-hdbcli-2.15.0.2/types_hdbcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 01:19:12.000000 types-hdbcli-2.15.0.2/types_hdbcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 01:19:12.000000 types-hdbcli-2.15.0.2/types_hdbcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:07.812350 types-hdbcli-2.15.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-13 12:31:07.812350 types-hdbcli-2.15.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:07.812350 types-hdbcli-2.15.0.3/hdbcli-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/hdbcli-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 12:30:41.000000 types-hdbcli-2.15.0.3/hdbcli-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-13 12:30:41.000000 types-hdbcli-2.15.0.3/hdbcli-stubs/dbapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 12:30:41.000000 types-hdbcli-2.15.0.3/hdbcli-stubs/resultrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:31:07.812350 types-hdbcli-2.15.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:07.812350 types-hdbcli-2.15.0.3/types_hdbcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/types_hdbcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/types_hdbcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/types_hdbcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 12:31:07.000000 types-hdbcli-2.15.0.3/types_hdbcli.egg-info/top_level.txt
```

### Comparing `types-hdbcli-2.15.0.2/CHANGELOG.md` & `types-hdbcli-2.15.0.3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.15.0.3 (2023-04-13)
+
+Style: prefer `type[Foo | Bar]` over `type[Foo] | type[Bar]` (#10039)
+
 ## 2.15.0.2 (2023-03-28)
 
 Ran stubdefaulter for `hdbcli` (#9962)
 
 ## 2.15.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-hdbcli-2.15.0.2/PKG-INFO` & `types-hdbcli-2.15.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.15.0.2
+Version: 2.15.0.3
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `72456da2a3546044508828dc9075fa25cbdb3645`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

### Comparing `types-hdbcli-2.15.0.2/hdbcli-stubs/dbapi.pyi` & `types-hdbcli-2.15.0.3/hdbcli-stubs/dbapi.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,12 +125,12 @@
 def DateFromTicks(ticks: float) -> date: ...
 def TimeFromTicks(ticks: float) -> time: ...
 def TimestampFromTicks(ticks: float) -> datetime: ...
 def Binary(data: ReadableBuffer) -> memoryview: ...
 
 Decimal = decimal.Decimal
 
-NUMBER: type[int] | type[float] | type[complex]
-DATETIME: type[date] | type[time] | type[datetime]
+NUMBER: type[int | float | complex]
+DATETIME: type[date | time | datetime]
 STRING = str
 BINARY = memoryview
 ROWID = int
```

### Comparing `types-hdbcli-2.15.0.2/setup.py` & `types-hdbcli-2.15.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `72456da2a3546044508828dc9075fa25cbdb3645`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.2",
+      version="2.15.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md",
```

### Comparing `types-hdbcli-2.15.0.2/types_hdbcli.egg-info/PKG-INFO` & `types-hdbcli-2.15.0.3/types_hdbcli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.15.0.2
+Version: 2.15.0.3
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `72456da2a3546044508828dc9075fa25cbdb3645`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

