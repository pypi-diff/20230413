# Comparing `tmp/mashumaro-3.6.tar.gz` & `tmp/mashumaro-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mashumaro-3.6.tar", last modified: Fri Apr  7 09:26:58 2023, max compression
+gzip compressed data, was "mashumaro-3.7.tar", last modified: Thu Apr 13 17:38:55 2023, max compression
```

## Comparing `mashumaro-3.6.tar` & `mashumaro-3.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.308766 mashumaro-3.6/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    11348 2023-02-06 08:24:36.000000 mashumaro-3.6/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78282 2023-04-07 09:26:58.308555 mashumaro-3.6/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    77363 2023-04-07 09:26:24.000000 mashumaro-3.6/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.302925 mashumaro-3.6/mashumaro/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      258 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1452 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/config.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.304251 mashumaro-3.6/mashumaro/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1013 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      825 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/core/helpers.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.304928 mashumaro-3.6/mashumaro/core/meta/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/meta/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.305865 mashumaro-3.6/mashumaro/core/meta/code/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/meta/code/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    37597 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/core/meta/code/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      707 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/meta/code/lines.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    20883 2023-02-13 10:27:04.000000 mashumaro-3.6/mashumaro/core/meta/helpers.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1366 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/meta/mixin.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.306424 mashumaro-3.6/mashumaro/core/meta/types/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/core/meta/types/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4109 2023-02-13 10:27:04.000000 mashumaro-3.6/mashumaro/core/meta/types/common.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25319 2023-02-13 10:27:04.000000 mashumaro-3.6/mashumaro/core/meta/types/pack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    32058 2023-02-13 10:27:04.000000 mashumaro-3.6/mashumaro/core/meta/types/unpack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      469 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/dialect.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4548 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/exceptions.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1392 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/helper.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.307237 mashumaro-3.6/mashumaro/jsonschema/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      214 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2170 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/annotations.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2353 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      746 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/dialects.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5781 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25664 2023-04-07 09:26:24.000000 mashumaro-3.6/mashumaro/jsonschema/schema.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.308268 mashumaro-3.6/mashumaro/mixins/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1673 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/dict.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      790 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/json.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1558 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/msgpack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1731 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/orjson.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1000 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/orjson.pyi
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1392 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/toml.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1108 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/mixins/yaml.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.6/mashumaro/py.typed
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2249 2023-02-13 10:27:04.000000 mashumaro-3.6/mashumaro/types.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 09:26:58.303925 mashumaro-3.6/mashumaro.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78282 2023-04-07 09:26:58.000000 mashumaro-3.6/mashumaro.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1210 2023-04-07 09:26:58.000000 mashumaro-3.6/mashumaro.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-07 09:26:58.000000 mashumaro-3.6/mashumaro.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-02-06 08:27:56.000000 mashumaro-3.6/mashumaro.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      155 2023-04-07 09:26:58.000000 mashumaro-3.6/mashumaro.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-07 09:26:58.000000 mashumaro-3.6/mashumaro.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      689 2023-04-07 09:26:24.000000 mashumaro-3.6/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-07 09:26:58.308804 mashumaro-3.6/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1463 2023-04-07 09:26:24.000000 mashumaro-3.6/setup.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.211377 mashumaro-3.7/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-13 17:38:38.000000 mashumaro-3.7/LICENSE
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78949 2023-04-13 17:38:55.211162 mashumaro-3.7/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78030 2023-04-13 17:38:38.000000 mashumaro-3.7/README.md
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.205196 mashumaro-3.7/mashumaro/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      258 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1452 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/config.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.206520 mashumaro-3.7/mashumaro/core/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1013 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/const.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      825 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/core/helpers.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.207249 mashumaro-3.7/mashumaro/core/meta/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.208148 mashumaro-3.7/mashumaro/core/meta/code/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/code/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    37703 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/core/meta/code/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      707 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/code/lines.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    20883 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/helpers.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1366 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/mixin.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.208781 mashumaro-3.7/mashumaro/core/meta/types/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/types/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4109 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/common.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25319 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/pack.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    32058 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/unpack.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      469 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/dialect.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4548 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/exceptions.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1472 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/helper.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.209840 mashumaro-3.7/mashumaro/jsonschema/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      214 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2170 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/annotations.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2837 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      746 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/dialects.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5818 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/models.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25682 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/schema.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.210887 mashumaro-3.7/mashumaro/mixins/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1673 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/dict.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      790 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/json.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1558 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/msgpack.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1731 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/orjson.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1000 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1392 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/toml.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1108 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/yaml.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/py.typed
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2249 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/types.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.206105 mashumaro-3.7/mashumaro.egg-info/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78949 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1210 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-02-06 08:27:56.000000 mashumaro-3.7/mashumaro.egg-info/not-zip-safe
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      155 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/requires.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/top_level.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      689 2023-04-07 09:26:24.000000 mashumaro-3.7/pyproject.toml
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-13 17:38:55.211416 mashumaro-3.7/setup.cfg
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1463 2023-04-13 17:38:38.000000 mashumaro-3.7/setup.py
```

### Comparing `mashumaro-3.6/LICENSE` & `mashumaro-3.7/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -171,25 +171,14 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
    Copyright 2017 Alexander Tikhonov
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `mashumaro-3.6/PKG-INFO` & `mashumaro-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.6
+Version: 3.7
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -874,17 +874,18 @@
 object like a function, a class method, a class instance method, an instance
 of a callable class or even a lambda function to be called for serialization.
 
 A value of type `str` sets a specific engine for serialization. Keep in mind
 that all possible engines depend on the data type that this option is used
 with. At this moment there are next serialization engines to choose from:
 
-| Applicable data types      | Supported engines        | Description                                                                                                                                                                                                  |
-|:---------------------------|:-------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `NamedTuple`, `namedtuple` | `as_list`, `as_dict`     | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
+|:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
 In addition, you can pass a field value as is without changes using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
@@ -1985,15 +1986,41 @@
     "items": {
         "$ref": "#/components/schemas/User"
     }
 }
 ```
 </details>
 
-These omitted definitions could be found later in the `Context` object that
+Reference prefix can be changed by using `ref_prefix` parameter:
+
+```python
+print(
+    build_json_schema(
+        List[User],
+        all_refs=True,
+        with_definitions=False,
+        ref_prefix="#/components/responses",
+    ).to_json()
+)
+```
+
+<details>
+<summary>Click to show the result</summary>
+
+```json
+{
+    "type": "array",
+    "items": {
+        "$ref": "#/components/responses/User"
+    }
+}
+```
+</details>
+
+The omitted definitions could be found later in the `Context` object that
 you could have created and passed to the function, but it could be easier
 to use `JSONSchemaBuilder` for that. For example, you might found it handy
 to build OpenAPI Specification step by step passing your models to the builder
 and get all the registered definitions later. This builder has reasonable
 defaults but can be customized if necessary.
 
 ```python
```

### Comparing `mashumaro-3.6/README.md` & `mashumaro-3.7/mashumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: mashumaro
+Version: 3.7
+Summary: Fast serialization library on top of dataclasses
+Home-page: https://github.com/Fatal1ty/mashumaro
+Author: Alexander Tikhonov
+Author-email: random.gauss@gmail.com
+License: Apache License, Version 2.0
+Platform: all
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: orjson
+Provides-Extra: msgpack
+Provides-Extra: yaml
+Provides-Extra: toml
+License-File: LICENSE
+
 # mashumaro
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
@@ -848,17 +874,18 @@
 object like a function, a class method, a class instance method, an instance
 of a callable class or even a lambda function to be called for serialization.
 
 A value of type `str` sets a specific engine for serialization. Keep in mind
 that all possible engines depend on the data type that this option is used
 with. At this moment there are next serialization engines to choose from:
 
-| Applicable data types      | Supported engines        | Description                                                                                                                                                                                                  |
-|:---------------------------|:-------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `NamedTuple`, `namedtuple` | `as_list`, `as_dict`     | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
+|:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
 In addition, you can pass a field value as is without changes using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
@@ -1959,15 +1986,41 @@
     "items": {
         "$ref": "#/components/schemas/User"
     }
 }
 ```
 </details>
 
-These omitted definitions could be found later in the `Context` object that
+Reference prefix can be changed by using `ref_prefix` parameter:
+
+```python
+print(
+    build_json_schema(
+        List[User],
+        all_refs=True,
+        with_definitions=False,
+        ref_prefix="#/components/responses",
+    ).to_json()
+)
+```
+
+<details>
+<summary>Click to show the result</summary>
+
+```json
+{
+    "type": "array",
+    "items": {
+        "$ref": "#/components/responses/User"
+    }
+}
+```
+</details>
+
+The omitted definitions could be found later in the `Context` object that
 you could have created and passed to the function, but it could be easier
 to use `JSONSchemaBuilder` for that. For example, you might found it handy
 to build OpenAPI Specification step by step passing your models to the builder
 and get all the registered definitions later. This builder has reasonable
 defaults but can be customized if necessary.
 
 ```python
```

### Comparing `mashumaro-3.6/mashumaro/config.py` & `mashumaro-3.7/mashumaro/config.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/const.py` & `mashumaro-3.7/mashumaro/core/const.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/helpers.py` & `mashumaro-3.7/mashumaro/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/code/builder.py` & `mashumaro-3.7/mashumaro/core/meta/code/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,14 +705,16 @@
             )
             serialize_by_alias = self.get_config().serialize_by_alias
             omit_none = self._get_dialect_or_config_option("omit_none", False)
             packers = {}
             aliases = {}
             fields_could_be_none = set()
             for fname, ftype in field_types.items():
+                if self.metadatas.get(fname, {}).get("serialize") == "omit":
+                    continue
                 packer, alias, could_be_none = self._get_field_packer(
                     fname, ftype, config
                 )
                 packers[fname] = packer
                 if alias:
                     aliases[fname] = alias
                 if could_be_none:
```

### Comparing `mashumaro-3.6/mashumaro/core/meta/code/lines.py` & `mashumaro-3.7/mashumaro/core/meta/code/lines.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/helpers.py` & `mashumaro-3.7/mashumaro/core/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/mixin.py` & `mashumaro-3.7/mashumaro/core/meta/mixin.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/types/common.py` & `mashumaro-3.7/mashumaro/core/meta/types/common.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/types/pack.py` & `mashumaro-3.7/mashumaro/core/meta/types/pack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/core/meta/types/unpack.py` & `mashumaro-3.7/mashumaro/core/meta/types/unpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/exceptions.py` & `mashumaro-3.7/mashumaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/helper.py` & `mashumaro-3.7/mashumaro/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 NamedTupleDeserializationEngine = Literal["as_dict", "as_list"]
 DateTimeDeserializationEngine = Literal["ciso8601", "pendulum"]
 AnyDeserializationEngine = Literal[
     NamedTupleDeserializationEngine, DateTimeDeserializationEngine
 ]
 
 NamedTupleSerializationEngine = Literal["as_dict", "as_list"]
-AnySerializationEngine = NamedTupleSerializationEngine
+OmitSerializationEngine = Literal["omit"]
+AnySerializationEngine = Union[
+    NamedTupleSerializationEngine, OmitSerializationEngine
+]
 
 
 T = TypeVar("T")
 
 
 def field_options(
     serialize: Optional[
```

### Comparing `mashumaro-3.6/mashumaro/jsonschema/annotations.py` & `mashumaro-3.7/mashumaro/jsonschema/annotations.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/jsonschema/builder.py` & `mashumaro-3.7/mashumaro/jsonschema/builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,29 +16,35 @@
 def build_json_schema(
     instance_type: Type,
     context: Optional[Context] = None,
     with_definitions: bool = True,
     all_refs: Optional[bool] = None,
     with_dialect_uri: bool = False,
     dialect: Optional[JSONSchemaDialect] = None,
+    ref_prefix: Optional[str] = None,
 ) -> JSONSchema:
     if context is None:
         context = Context()
     else:
         context = Context(
             dialect=context.dialect,
             definitions=context.definitions,
             all_refs=context.all_refs,
+            ref_prefix=context.ref_prefix,
         )
     if dialect is not None:
         context.dialect = dialect
     if all_refs is not None:
         context.all_refs = all_refs
     elif context.all_refs is None:
         context.all_refs = context.dialect.all_refs
+    if ref_prefix is not None:
+        context.ref_prefix = ref_prefix.rstrip("/")
+    elif context.ref_prefix is None:
+        context.ref_prefix = context.dialect.definitions_root_pointer
     instance = Instance(instance_type)
     schema = get_schema(instance, context, with_dialect_uri=with_dialect_uri)
     if with_definitions and context.definitions:
         schema.definitions = context.definitions
     return schema
 
 
@@ -53,18 +59,25 @@
 
 
 class JSONSchemaBuilder:
     def __init__(
         self,
         dialect: JSONSchemaDialect = DRAFT_2020_12,
         all_refs: Optional[bool] = None,
+        ref_prefix: Optional[str] = None,
     ):
         if all_refs is None:
             all_refs = dialect.all_refs
-        self.context = Context(dialect=dialect, all_refs=all_refs)
+        if ref_prefix is None:
+            ref_prefix = dialect.definitions_root_pointer
+        self.context = Context(
+            dialect=dialect,
+            all_refs=all_refs,
+            ref_prefix=ref_prefix.rstrip("/"),
+        )
 
     def build(self, instance_type: Type) -> JSONSchema:
         return build_json_schema(
             instance_type=instance_type,
             context=self.context,
             with_definitions=False,
         )
```

### Comparing `mashumaro-3.6/mashumaro/jsonschema/dialects.py` & `mashumaro-3.7/mashumaro/jsonschema/dialects.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/jsonschema/models.py` & `mashumaro-3.7/mashumaro/jsonschema/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,7 +184,8 @@
 
 
 @dataclass
 class Context:
     dialect: JSONSchemaDialect = DRAFT_2020_12
     definitions: Dict[str, JSONSchema] = field(default_factory=dict)
     all_refs: Optional[bool] = None
+    ref_prefix: Optional[str] = None
```

### Comparing `mashumaro-3.6/mashumaro/jsonschema/schema.py` & `mashumaro-3.7/mashumaro/jsonschema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,31 +293,30 @@
             override = field_schema_overrides.get(f_name)
             f_instance = instance.copy(type=f_type, name=f_name)
             if override:
                 f_schema = JSONSchema.from_dict(override)
             else:
                 override_field_instance_type_if_needed(instance, f_instance)
                 f_schema = get_schema(f_instance, ctx)
+            if f_instance.alias:
+                f_name = f_instance.alias
             if f_default is not MISSING:
                 f_schema.default = f_default
             else:
                 required.append(f_name)
-            if f_instance.alias:
-                properties[f_instance.alias] = f_schema
+            properties[f_name] = f_schema
         if properties:
             schema.properties = properties
         if required:
             schema.required = required
         if ctx.all_refs:
             ctx.definitions[instance.origin_type.__name__] = schema
+            ref_prefix = ctx.ref_prefix or ctx.dialect.definitions_root_pointer
             return JSONSchema(
-                reference=(
-                    f"{ctx.dialect.definitions_root_pointer}/"
-                    f"{instance.origin_type.__name__}"
-                )
+                reference=f"{ref_prefix}/{instance.origin_type.__name__}"
             )
         else:
             return schema
 
 
 @register
 def on_any(instance: Instance, ctx: Context) -> Optional[JSONSchema]:
```

### Comparing `mashumaro-3.6/mashumaro/mixins/dict.py` & `mashumaro-3.7/mashumaro/mixins/dict.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/json.py` & `mashumaro-3.7/mashumaro/mixins/json.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/msgpack.py` & `mashumaro-3.7/mashumaro/mixins/msgpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/orjson.py` & `mashumaro-3.7/mashumaro/mixins/orjson.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/orjson.pyi` & `mashumaro-3.7/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/toml.py` & `mashumaro-3.7/mashumaro/mixins/toml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/mixins/yaml.py` & `mashumaro-3.7/mashumaro/mixins/yaml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro/types.py` & `mashumaro-3.7/mashumaro/types.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/mashumaro.egg-info/PKG-INFO` & `mashumaro-3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: mashumaro
-Version: 3.6
-Summary: Fast serialization library on top of dataclasses
-Home-page: https://github.com/Fatal1ty/mashumaro
-Author: Alexander Tikhonov
-Author-email: random.gauss@gmail.com
-License: Apache License, Version 2.0
-Platform: all
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: orjson
-Provides-Extra: msgpack
-Provides-Extra: yaml
-Provides-Extra: toml
-License-File: LICENSE
-
 # mashumaro
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
@@ -874,17 +848,18 @@
 object like a function, a class method, a class instance method, an instance
 of a callable class or even a lambda function to be called for serialization.
 
 A value of type `str` sets a specific engine for serialization. Keep in mind
 that all possible engines depend on the data type that this option is used
 with. At this moment there are next serialization engines to choose from:
 
-| Applicable data types      | Supported engines        | Description                                                                                                                                                                                                  |
-|:---------------------------|:-------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `NamedTuple`, `namedtuple` | `as_list`, `as_dict`     | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
+|:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
+| `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
 In addition, you can pass a field value as is without changes using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
@@ -1985,15 +1960,41 @@
     "items": {
         "$ref": "#/components/schemas/User"
     }
 }
 ```
 </details>
 
-These omitted definitions could be found later in the `Context` object that
+Reference prefix can be changed by using `ref_prefix` parameter:
+
+```python
+print(
+    build_json_schema(
+        List[User],
+        all_refs=True,
+        with_definitions=False,
+        ref_prefix="#/components/responses",
+    ).to_json()
+)
+```
+
+<details>
+<summary>Click to show the result</summary>
+
+```json
+{
+    "type": "array",
+    "items": {
+        "$ref": "#/components/responses/User"
+    }
+}
+```
+</details>
+
+The omitted definitions could be found later in the `Context` object that
 you could have created and passed to the function, but it could be easier
 to use `JSONSchemaBuilder` for that. For example, you might found it handy
 to build OpenAPI Specification step by step passing your models to the builder
 and get all the registered definitions later. This builder has reasonable
 defaults but can be customized if necessary.
 
 ```python
```

### Comparing `mashumaro-3.6/mashumaro.egg-info/SOURCES.txt` & `mashumaro-3.7/mashumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/pyproject.toml` & `mashumaro-3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mashumaro-3.6/setup.py` & `mashumaro-3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="mashumaro",
-    version="3.6",
+    version="3.7",
     description="Fast serialization library on top of dataclasses",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
```

