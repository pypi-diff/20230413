# Comparing `tmp/symdexer-0.1.0.tar.gz` & `tmp/symdexer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.1.0.tar", last modified: Thu Apr 13 10:56:14 2023, max compression
+gzip compressed data, was "symdexer-0.1.1.tar", last modified: Thu Apr 13 14:52:26 2023, max compression
```

## Comparing `symdexer-0.1.0.tar` & `symdexer-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.128890 symdexer-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-04-13 09:20:48.000000 symdexer-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      548 2023-04-13 10:56:14.128890 symdexer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-04-13 09:20:48.000000 symdexer-0.1.0/README.md
--rw-rw-rw-   0        0        0      586 2023-04-13 10:55:00.000000 symdexer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 10:56:14.128890 symdexer-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.026863 symdexer-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.097616 symdexer-0.1.0/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0     2327 2023-04-13 10:15:30.000000 symdexer-0.1.0/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     1718 2023-04-13 10:13:35.000000 symdexer-0.1.0/src/symdexer/cache.py
--rw-rw-rw-   0        0        0      564 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     1309 2023-04-13 10:06:06.000000 symdexer-0.1.0/src/symdexer/settings.py
--rw-rw-rw-   0        0        0      979 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.128890 symdexer-0.1.0/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      548 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-13 10:56:14.000000 symdexer-0.1.0/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.260990 symdexer-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 09:20:48.000000 symdexer-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      548 2023-04-13 14:52:26.260990 symdexer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-04-13 09:20:48.000000 symdexer-0.1.1/README.md
+-rw-rw-rw-   0        0        0      586 2023-04-13 14:51:55.000000 symdexer-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:52:26.260990 symdexer-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.207580 symdexer-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.245368 symdexer-0.1.1/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-13 14:51:15.000000 symdexer-0.1.1/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     1718 2023-04-13 10:13:35.000000 symdexer-0.1.1/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     2247 2023-04-13 14:51:11.000000 symdexer-0.1.1/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      564 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     1309 2023-04-13 10:06:06.000000 symdexer-0.1.1/src/symdexer/settings.py
+-rw-rw-rw-   0        0        0      979 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.260990 symdexer-0.1.1/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.1.0/LICENSE.txt` & `symdexer-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.0/PKG-INFO` & `symdexer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.1.0/pyproject.toml` & `symdexer-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `symdexer-0.1.0/src/symdexer/__main__.py` & `symdexer-0.1.1/src/symdexer/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 def find_command(settings_p: str, symbols: list[str], order: list[str]):
     settings = load_settings(settings_p)
 
     if not settings.cache.exists():
         make_cache(settings.cache, settings.packages)
 
     for name, module in search_cache(settings.cache, symbols, order or settings.order):
-        print(f"from {module} import {name}")
+        yield f"from {module} import {name}"
 
 
 def reset_cache_command(settings_p: str):
     settings = load_settings(settings_p)
 
     make_cache(settings.cache, settings.packages)
 
-    print("reseted cached")
+    yield "cache reseted"
 
 
 def init_settings_command(settings_p: str):
     with open(settings_p, "w", encoding="utf-8") as fp:
         fp.write('cache = "symdex.db"\n')
         fp.write('default_order = ["defines", "assigns", "imports"]\n')
         fp.write("\n")
         fp.write("[packages]\n")
         fp.write('package_name = "path/to/package"\n')
 
-    print(f"initialized {settings_p}")
+    yield f"initialized {settings_p}"
 
 
 def main():
     parser = ArgumentParser("symdexer")
 
     parser.add_argument(
         "-s",
@@ -46,38 +46,26 @@
         help="Name of the file to load the settings from",
     )
 
     subp = parser.add_subparsers(required=True, dest="command")
 
     find = subp.add_parser("find", help="Searches the cache for symbols matching a list of patterns")
 
-    find.add_argument(
-        "patterns",
-        metavar="PATTERN",
-        nargs="+",
-        help="The patterns to look for"
-    )
+    find.add_argument("patterns", metavar="PATTERN", nargs="+", help="The patterns to look for")
 
-    find.add_argument(
-        "-o",
-        "--order",
-        metavar="SYM_TYPE",
-        choices=list(SYM_TYPES),
-        nargs="+"
-    )
+    find.add_argument("-o", "--order", metavar="SYM_TYPE", choices=list(SYM_TYPES), nargs="+")
 
     subp.add_parser("reset-cache", help="Determines if the cache should be reset or not")
 
     subp.add_parser("init", help="Creates a new configuration file")
 
     args = parser.parse_args()
 
     if args.command == "find":
-        find_command(args.settings, args.patterns, args.order)
+        res = find_command(args.settings, args.patterns, args.order)
     elif args.command == "reset-cache":
-        reset_cache_command(args.settings)
+        res = reset_cache_command(args.settings)
     elif args.command == "init":
-        init_settings_command(args.settings)
-
+        res = init_settings_command(args.settings)
 
-if __name__ == "__main__":
-    main()
+    for line in res:
+        print(line)
```

### Comparing `symdexer-0.1.0/src/symdexer/cache.py` & `symdexer-0.1.1/src/symdexer/cache.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.0/src/symdexer/modules.py` & `symdexer-0.1.1/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.0/src/symdexer/settings.py` & `symdexer-0.1.1/src/symdexer/settings.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.0/src/symdexer/symbols.py` & `symdexer-0.1.1/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.0/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.1.1/src/symdexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

