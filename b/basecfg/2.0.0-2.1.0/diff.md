# Comparing `tmp/basecfg-2.0.0.tar.gz` & `tmp/basecfg-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basecfg-2.0.0.tar", last modified: Mon Apr 10 17:10:33 2023, max compression
+gzip compressed data, was "basecfg-2.1.0.tar", last modified: Wed Apr 12 22:16:42 2023, max compression
```

## Comparing `basecfg-2.0.0.tar` & `basecfg-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-10 17:10:06.000000 basecfg-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-10 17:10:33.474110 basecfg-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 17:10:06.000000 basecfg-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-10 17:10:06.000000 basecfg-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:10:33.474110 basecfg-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.470110 basecfg-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/src/basecfg/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 17:10:06.000000 basecfg-2.0.0/src/basecfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-04-10 17:10:06.000000 basecfg-2.0.0/src/basecfg/basecfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/src/basecfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:16:42.058057 basecfg-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-12 22:16:18.000000 basecfg-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-12 22:16:42.058057 basecfg-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 22:16:18.000000 basecfg-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 22:16:18.000000 basecfg-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 22:16:42.058057 basecfg-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:16:42.058057 basecfg-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:16:42.058057 basecfg-2.1.0/src/basecfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 22:16:18.000000 basecfg-2.1.0/src/basecfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18912 2023-04-12 22:16:18.000000 basecfg-2.1.0/src/basecfg/basecfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:16:42.058057 basecfg-2.1.0/src/basecfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-12 22:16:42.000000 basecfg-2.1.0/src/basecfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 22:16:42.000000 basecfg-2.1.0/src/basecfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:16:42.000000 basecfg-2.1.0/src/basecfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 22:16:42.000000 basecfg-2.1.0/src/basecfg.egg-info/top_level.txt
```

### Comparing `basecfg-2.0.0/LICENSE` & `basecfg-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basecfg-2.0.0/PKG-INFO` & `basecfg-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basecfg
-Version: 2.0.0
+Version: 2.1.0
 Summary: typed 12-factor app configuration helper
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/basecfg
 Project-URL: Bug Tracker, https://github.com/edencehealth/basecfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `basecfg-2.0.0/README.md` & `basecfg-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `basecfg-2.0.0/pyproject.toml` & `basecfg-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basecfg"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Ben Burke", email="actualben@users.noreply.github.com" },
 ]
 description = "typed 12-factor app configuration helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `basecfg-2.0.0/src/basecfg/basecfg.py` & `basecfg-2.1.0/src/basecfg/basecfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 module for specifying configuration options as a class with typed members and
 loading the configuration values from json config files, environment variables,
 and command-line arguments
 """
 # pylint: disable=too-many-arguments
 import argparse
 import json
+import logging
 import os
 import re
 from typing import (
     Any,
     Callable,
     Dict,
     List,
@@ -59,14 +60,21 @@
     _optmeta: List[OptionMetadata] = []
     _optmeta_reset: bool = True
     _options: Dict[str, OptionMetadata]
     _prog: Optional[str] = None
     _prog_description: Optional[str] = None
     _prog_epilog: Optional[str] = None
     _version: Optional[str] = None
+    _autoredact_tokens: Sequence[str] = (
+        "key",
+        "pass",
+        "private",
+        "secret",
+        "token",
+    )
 
     def __init__(
         self,
         json_config_path: Optional[str] = None,
         json_required=False,
         envfile_path: Optional[str] = None,
         envfile_required: bool = False,
@@ -255,15 +263,15 @@
             elif option_type == "List[bool]":
                 arg_config["action"] = "append"
                 arg_config["type"] = self._parse_bool
 
             argp.add_argument(
                 arg_name,
                 dest=optname,
-                help=option.doc + f" (default {str(option.default)})",
+                help=option.doc + f" (default: {repr(option.default)})",
                 required=False,
                 choices=option.choices,
                 **arg_config,
             )
 
         return vars(argp.parse_args(args=cli_args))
 
@@ -345,15 +353,15 @@
         with dotenvfh as dotenv:
             for i, line in enumerate(dotenv.readlines()):
                 if empty_line.match(line):
                     continue
                 if "=" not in line:
                     raise ValueError(
                         f'envfile parsing error; file:"{path}" line:{i}; data line '
-                        f'contains no "-" character'
+                        f'contains no "=" character'
                     )
                 key, value = line.split("=", 1)
                 result[key.lower().strip()] = value.strip()
         return result
 
     @staticmethod
     def _list_docker_secrets(
@@ -433,14 +441,48 @@
         """returns the number of configuration options in the class"""
         return len(self._options)
 
     def __iter__(self):
         """returns keys iterator"""
         return iter(self._options.keys())
 
+    def _looks_sensitive(self, keyname: str) -> bool:
+        """
+        returns true of the given keyname appears to refer to a secret that should
+        be redacted when logging the configuration
+        """
+        keyname = keyname.lower()
+        for token in self._autoredact_tokens:
+            if token in keyname:
+                return True
+        return False
+
+    def logcfg(
+        self,
+        cfglogger: logging.Logger,
+        autoredact: bool = True,
+        heading: str = "running configuration:",
+        item_prefix: str = "  ",
+    ):
+        """
+        use the given logger to report the cfg info;
+        if "autoredact" is true, values with names that resemble passwords are redacted;
+        "heading" is logged before the configuration items are reported;
+        "item_prefix" is prepended to each configuration item in the output
+        """
+        cfglogger.info(heading)
+        for key in self:
+            if self._options[key].redact:
+                value = "--REDACTED--"
+            elif autoredact and self._looks_sensitive(key):
+                value = "--AUTO-REDACTED--"
+            else:
+                value = repr(getattr(self, key))
+            cfglogger.info("%s%s: %s", item_prefix, key, value)
+
 
 def opt(
     default: OptType,
     doc: str,
     required: bool = False,
     parser: Optional[Callable[[OptParserInput], OptType]] = None,
     choices: Optional[Sequence[OptType]] = None,
```

### Comparing `basecfg-2.0.0/src/basecfg.egg-info/PKG-INFO` & `basecfg-2.1.0/src/basecfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basecfg
-Version: 2.0.0
+Version: 2.1.0
 Summary: typed 12-factor app configuration helper
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/basecfg
 Project-URL: Bug Tracker, https://github.com/edencehealth/basecfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
```

