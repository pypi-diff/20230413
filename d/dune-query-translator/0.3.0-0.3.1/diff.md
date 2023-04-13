# Comparing `tmp/dune_query_translator-0.3.0.tar.gz` & `tmp/dune_query_translator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_query_translator-0.3.0.tar", max compression
+gzip compressed data, was "dune_query_translator-0.3.1.tar", max compression
```

## Comparing `dune_query_translator-0.3.0.tar` & `dune_query_translator-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/LICENSE
--rw-r--r--   0        0        0     1258 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/README.md
--rw-r--r--   0        0        0      431 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/__init__.py
--rw-r--r--   0        0        0      868 2023-04-12 13:20:43.164943 dune_query_translator-0.3.0/dune/translate/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      651 2023-04-12 13:20:43.376957 dune_query_translator-0.3.0/dune/translate/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0    20816 2023-04-12 13:20:43.380957 dune_query_translator-0.3.0/dune/translate/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0        0        0     3124 2023-04-12 13:20:43.380957 dune_query_translator-0.3.0/dune/translate/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3228 2023-04-12 13:20:43.164943 dune_query_translator-0.3.0/dune/translate/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/constants.py
--rw-r--r--   0        0        0      105 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/errors.py
--rw-r--r--   0        0        0    18400 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/helpers.py
--rw-r--r--   0        0        0     2018 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/table_replacements.py
--rw-r--r--   0        0        0     2978 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/dune/translate/translate.py
--rw-r--r--   0        0        0      522 2023-04-12 13:20:22.463545 dune_query_translator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 dune_query_translator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1258 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/README.md
+-rw-r--r--   0        0        0      431 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-13 08:44:13.211611 dune_query_translator-0.3.1/dune/translate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      651 2023-04-13 08:44:13.443610 dune_query_translator-0.3.1/dune/translate/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0    20816 2023-04-13 08:44:13.447610 dune_query_translator-0.3.1/dune/translate/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     3124 2023-04-13 08:44:13.447610 dune_query_translator-0.3.1/dune/translate/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3228 2023-04-13 08:44:13.215611 dune_query_translator-0.3.1/dune/translate/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/constants.py
+-rw-r--r--   0        0        0      105 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/errors.py
+-rw-r--r--   0        0        0    18400 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/helpers.py
+-rw-r--r--   0        0        0     2018 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/table_replacements.py
+-rw-r--r--   0        0        0     2978 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/translate.py
+-rw-r--r--   0        0        0      576 2023-04-13 08:43:47.035824 dune_query_translator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 dune_query_translator-0.3.1/PKG-INFO
```

### Comparing `dune_query_translator-0.3.0/LICENSE` & `dune_query_translator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.0/README.md` & `dune_query_translator-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.0/dune/translate/__pycache__/__init__.cpython-311.pyc` & `dune_query_translator-0.3.1/dune/translate/__pycache__/__init__.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,41 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x16b03664 (Wed Apr 12 13:20:22 2023 UTC)
+moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
 files sz: 431
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640284005a03640384005a
       0464045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('_translate_query', '_clean_dataset'))
+                 4 LOAD_CONST               1 (('_clean_dataset', '_translate_query'))
                  6 IMPORT_NAME              0 (dune.translate.translate)
-                 8 IMPORT_FROM              1 (_translate_query)
-                10 STORE_NAME               1 (_translate_query)
-                12 IMPORT_FROM              2 (_clean_dataset)
-                14 STORE_NAME               2 (_clean_dataset)
+                 8 IMPORT_FROM              1 (_clean_dataset)
+                10 STORE_NAME               1 (_clean_dataset)
+                12 IMPORT_FROM              2 (_translate_query)
+                14 STORE_NAME               2 (_translate_query)
                 16 POP_TOP
    
      4          18 LOAD_CONST               2 (<code object migrate_spark, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/__init__.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 STORE_NAME               3 (migrate_spark)
    
      9          24 LOAD_CONST               3 (<code object migrate_postgres, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/__init__.py", line 9>)
                 26 MAKE_FUNCTION            0
                 28 STORE_NAME               4 (migrate_postgres)
                 30 LOAD_CONST               4 (None)
                 32 RETURN_VALUE
    consts
       0
-      ('_translate_query', '_clean_dataset')
+      ('_clean_dataset', '_translate_query')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c006401ac02a6020000ab02000000
@@ -95,15 +95,15 @@
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/__init__.py'
          name       'migrate_postgres'
          firstlineno 9
          lnotab 0x02021e01
       None
-   names      ('dune.translate.translate', '_translate_query', '_clean_dataset', 'migrate_spark', 'migrate_postgres')
+   names      ('dune.translate.translate', '_clean_dataset', '_translate_query', 'migrate_spark', 'migrate_postgres')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020110030605
```

### Comparing `dune_query_translator-0.3.0/dune/translate/__pycache__/errors.cpython-311.pyc` & `dune_query_translator-0.3.1/dune/translate/__pycache__/errors.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x16b03664 (Wed Apr 12 13:20:22 2023 UTC)
+moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_query_translator-0.3.0/dune/translate/__pycache__/helpers.cpython-311.pyc` & `dune_query_translator-0.3.1/dune/translate/__pycache__/helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x16b03664 (Wed Apr 12 13:20:22 2023 UTC)
+moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
 files sz: 18400
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `dune_query_translator-0.3.0/dune/translate/__pycache__/table_replacements.cpython-311.pyc` & `dune_query_translator-0.3.1/dune/translate/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x16b03664 (Wed Apr 12 13:20:22 2023 UTC)
+moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_query_translator-0.3.0/dune/translate/__pycache__/translate.cpython-311.pyc` & `dune_query_translator-0.3.1/dune/translate/__pycache__/translate.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x16b03664 (Wed Apr 12 13:20:22 2023 UTC)
+moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
 files sz: 2978
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -34,36 +34,36 @@
                 32 LOAD_CONST               3 (('DuneTranslationError',))
                 34 IMPORT_NAME              3 (dune.translate.errors)
                 36 IMPORT_FROM              4 (DuneTranslationError)
                 38 STORE_NAME               4 (DuneTranslationError)
                 40 POP_TOP
    
      7          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('add_warnings_and_banner', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder'))
+                44 LOAD_CONST               4 (('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms'))
                 46 IMPORT_NAME              5 (dune.translate.helpers)
                 48 IMPORT_FROM              6 (add_warnings_and_banner)
                 50 STORE_NAME               6 (add_warnings_and_banner)
-                52 IMPORT_FROM              7 (fix_bytearray_lower)
-                54 STORE_NAME               7 (fix_bytearray_lower)
-                56 IMPORT_FROM              8 (fix_bytearray_param)
-                58 STORE_NAME               8 (fix_bytearray_param)
-                60 IMPORT_FROM              9 (prep_query)
-                62 STORE_NAME               9 (prep_query)
-                64 IMPORT_FROM             10 (double_quoted_param_left_placeholder)
-                66 STORE_NAME              10 (double_quoted_param_left_placeholder)
-                68 IMPORT_FROM             11 (double_quoted_param_right_placeholder)
-                70 STORE_NAME              11 (double_quoted_param_right_placeholder)
-                72 IMPORT_FROM             12 (sqlglot_postgres_transforms)
-                74 STORE_NAME              12 (sqlglot_postgres_transforms)
-                76 IMPORT_FROM             13 (sqlglot_spark_transforms)
-                78 STORE_NAME              13 (sqlglot_spark_transforms)
-                80 IMPORT_FROM             14 (single_quoted_param_left_placeholder)
-                82 STORE_NAME              14 (single_quoted_param_left_placeholder)
-                84 IMPORT_FROM             15 (single_quoted_param_right_placeholder)
-                86 STORE_NAME              15 (single_quoted_param_right_placeholder)
+                52 IMPORT_FROM              7 (double_quoted_param_left_placeholder)
+                54 STORE_NAME               7 (double_quoted_param_left_placeholder)
+                56 IMPORT_FROM              8 (double_quoted_param_right_placeholder)
+                58 STORE_NAME               8 (double_quoted_param_right_placeholder)
+                60 IMPORT_FROM              9 (fix_bytearray_lower)
+                62 STORE_NAME               9 (fix_bytearray_lower)
+                64 IMPORT_FROM             10 (fix_bytearray_param)
+                66 STORE_NAME              10 (fix_bytearray_param)
+                68 IMPORT_FROM             11 (prep_query)
+                70 STORE_NAME              11 (prep_query)
+                72 IMPORT_FROM             12 (single_quoted_param_left_placeholder)
+                74 STORE_NAME              12 (single_quoted_param_left_placeholder)
+                76 IMPORT_FROM             13 (single_quoted_param_right_placeholder)
+                78 STORE_NAME              13 (single_quoted_param_right_placeholder)
+                80 IMPORT_FROM             14 (sqlglot_postgres_transforms)
+                82 STORE_NAME              14 (sqlglot_postgres_transforms)
+                84 IMPORT_FROM             15 (sqlglot_spark_transforms)
+                86 STORE_NAME              15 (sqlglot_spark_transforms)
                 88 POP_TOP
    
     21          90 LOAD_CONST               5 (<code object _clean_dataset, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/translate.py", line 21>)
                 92 MAKE_FUNCTION            0
                 94 STORE_NAME              16 (_clean_dataset)
    
     28          96 LOAD_CONST               7 ((None,))
@@ -73,15 +73,15 @@
                104 LOAD_CONST               1 (None)
                106 RETURN_VALUE
    consts
       0
       None
       ('ParseError',)
       ('DuneTranslationError',)
-      ('add_warnings_and_banner', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder')
+      ('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms')
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700640144005d1c7d017c017c00a00000000000000000000000000000
@@ -390,15 +390,15 @@
          name       '_translate_query'
          firstlineno 28
          lnotab
             0x020202024a010eff10031e033c030c0120010c022c0120032e04340132
             01320132fc02081e011e02200212051c0128012801320132fb0208160102
             01020102fd100526ef
       (None,)
-   names      ('re', 'sqlglot', 'ParseError', 'dune.translate.errors', 'DuneTranslationError', 'dune.translate.helpers', 'add_warnings_and_banner', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', '_clean_dataset', '_translate_query')
+   names      ('re', 'sqlglot', 'ParseError', 'dune.translate.errors', 'DuneTranslationError', 'dune.translate.helpers', 'add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', '_clean_dataset', '_translate_query')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/translate.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201080208010c020c01300e0607
```

### Comparing `dune_query_translator-0.3.0/dune/translate/helpers.py` & `dune_query_translator-0.3.1/dune/translate/helpers.py`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.0/dune/translate/table_replacements.py` & `dune_query_translator-0.3.1/dune/translate/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.0/dune/translate/translate.py` & `dune_query_translator-0.3.1/dune/translate/translate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import sqlglot
 from sqlglot import ParseError
 
 from dune.translate.errors import DuneTranslationError
 from dune.translate.helpers import (
     add_warnings_and_banner,
+    double_quoted_param_left_placeholder,
+    double_quoted_param_right_placeholder,
     fix_bytearray_lower,
     fix_bytearray_param,
     prep_query,
-    double_quoted_param_left_placeholder,
-    double_quoted_param_right_placeholder,
-    sqlglot_postgres_transforms,
-    sqlglot_spark_transforms,
     single_quoted_param_left_placeholder,
     single_quoted_param_right_placeholder,
+    sqlglot_postgres_transforms,
+    sqlglot_spark_transforms,
 )
 
 
 def _clean_dataset(dataset):
     for d in ("gnosis", "optimism", "bnb", "polygon", "ethereum"):
         if d in dataset.lower():
             return d
```

### Comparing `dune_query_translator-0.3.0/pyproject.toml` & `dune_query_translator-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "dune-query-translator"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlglot = "^11.4.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 ruff = "^0.0.259"
 black = "^23.1.0"
-isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 # Same as Black.
 line-length = 120
+select = [
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "I",   # isort
+]
```

### Comparing `dune_query_translator-0.3.0/PKG-INFO` & `dune_query_translator-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-query-translator
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.4.4,<12.0.0)
```

