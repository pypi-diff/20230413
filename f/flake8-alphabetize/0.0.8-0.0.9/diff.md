# Comparing `tmp/flake8_alphabetize-0.0.8.tar.gz` & `tmp/flake8_alphabetize-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_alphabetize-0.0.8.tar", last modified: Sun Apr 11 09:48:35 2021, max compression
+gzip compressed data, was "dist/flake8_alphabetize-0.0.9.tar", last modified: Sun Apr 11 11:02:20 2021, max compression
```

## Comparing `flake8_alphabetize-0.0.8.tar` & `flake8_alphabetize-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 09:48:35.434026 flake8_alphabetize-0.0.8/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       54 2021-04-09 21:14:51.000000 flake8_alphabetize-0.0.8/MANIFEST.in
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      902 2021-04-11 09:48:35.438026 flake8_alphabetize-0.0.8/PKG-INFO
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 09:48:35.438026 flake8_alphabetize-0.0.8/alphabetize/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      208 2021-04-10 13:50:04.000000 flake8_alphabetize-0.0.8/alphabetize/__init__.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      497 2021-04-11 09:48:35.438026 flake8_alphabetize-0.0.8/alphabetize/_version.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     5296 2021-04-11 09:45:41.000000 flake8_alphabetize-0.0.8/alphabetize/core.py
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 09:48:35.434026 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      902 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/PKG-INFO
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      366 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/SOURCES.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)        1 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/dependency_links.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       49 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/entry_points.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       32 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/requires.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       12 2021-04-11 09:48:35.000000 flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/top_level.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      452 2021-04-11 09:48:35.438026 flake8_alphabetize-0.0.8/setup.cfg
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1322 2021-04-10 14:49:37.000000 flake8_alphabetize-0.0.8/setup.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    70238 2021-04-10 11:00:11.000000 flake8_alphabetize-0.0.8/versioneer.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       54 2021-04-09 21:14:51.000000 flake8_alphabetize-0.0.9/MANIFEST.in
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      902 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/PKG-INFO
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/alphabetize/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      208 2021-04-10 13:50:04.000000 flake8_alphabetize-0.0.9/alphabetize/__init__.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      497 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/alphabetize/_version.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     5351 2021-04-11 11:00:52.000000 flake8_alphabetize-0.0.9/alphabetize/core.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      902 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/PKG-INFO
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      366 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)        1 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       49 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/entry_points.txt
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       32 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/requires.txt
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       12 2021-04-11 11:02:20.000000 flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/top_level.txt
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      452 2021-04-11 11:02:20.767860 flake8_alphabetize-0.0.9/setup.cfg
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1322 2021-04-10 14:49:37.000000 flake8_alphabetize-0.0.9/setup.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    70238 2021-04-10 11:00:11.000000 flake8_alphabetize-0.0.9/versioneer.py
```

### Comparing `flake8_alphabetize-0.0.8/PKG-INFO` & `flake8_alphabetize-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_alphabetize
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python style checker for alphabetizing import and __all__.
 Home-page: https://github.com/tlocke/flake8_alphabetize
 Author: Tony Locke
 Author-email: tlocke@tlocke.org.uk
 License: Unlicense
 Description: 
         A Flake8 style checker for alphabetizing import and \_\_all\_\_. Please see the
```

### Comparing `flake8_alphabetize-0.0.8/alphabetize/core.py` & `flake8_alphabetize-0.0.9/alphabetize/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,28 @@
     def __iter__(self):
         errors = _find_errors(Alphabetize.app_names, self.tree)
         return iter(errors)
 
     @staticmethod
     def add_options(option_manager):
         option_manager.add_option(
-            "--application-package-names",
+            "--application-names",
             type="string",
-            metavar="IMPORT_NAMES",
+            metavar="APPLICATION_NAMES",
             default="",
             parse_from_config=True,
             help="Comma-separated list of package names. If an import is for a "
             "package in this list, it'll be in the application group of imports. "
             "Eg. 'myapp'.",
         )
 
     @classmethod
     def parse_options(cls, options):
-        cls.app_names = options.application_package_names
+        names = options.application_names
+        cls.app_names = [] if (names is None or names == "") else [names]
 
 
 def _make_error(node, code, message):
     return (node.lineno, node.col_offset, f"AZ{code} {message}", Alphabetize)
 
 
 class GroupEnum(IntEnum):
@@ -92,19 +93,19 @@
         if self.module_name == "__future__":
             group = GroupEnum.FUTURE
         elif in_stdlib(self.module_name):
             group = GroupEnum.STDLIB
         elif level > 0:
             group = GroupEnum.APPLICATION
         else:
+            group = GroupEnum.THIRD_PARTY
             for name in app_names:
                 if name == self.module_name or self.module_name.startswith(f"{name}."):
                     group = GroupEnum.APPLICATION
                     break
-            group = GroupEnum.THIRD_PARTY
 
         if group == GroupEnum.STDLIB:
             self.sorter = group, self.node_type, self.module_name
         else:
             m = self.module_name
             first_dot = m.find(".")
             top_name = m if first_dot == -1 else m[:first_dot]
```

### Comparing `flake8_alphabetize-0.0.8/flake8_alphabetize.egg-info/PKG-INFO` & `flake8_alphabetize-0.0.9/flake8_alphabetize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-alphabetize
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python style checker for alphabetizing import and __all__.
 Home-page: https://github.com/tlocke/flake8_alphabetize
 Author: Tony Locke
 Author-email: tlocke@tlocke.org.uk
 License: Unlicense
 Description: 
         A Flake8 style checker for alphabetizing import and \_\_all\_\_. Please see the
```

### Comparing `flake8_alphabetize-0.0.8/setup.py` & `flake8_alphabetize-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `flake8_alphabetize-0.0.8/versioneer.py` & `flake8_alphabetize-0.0.9/versioneer.py`

 * *Files identical despite different names*

