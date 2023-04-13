# Comparing `tmp/symdexer-0.1.1.tar.gz` & `tmp/symdexer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.1.1.tar", last modified: Thu Apr 13 14:52:26 2023, max compression
+gzip compressed data, was "symdexer-0.1.2.tar", last modified: Thu Apr 13 19:02:59 2023, max compression
```

## Comparing `symdexer-0.1.1.tar` & `symdexer-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.260990 symdexer-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-04-13 09:20:48.000000 symdexer-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      548 2023-04-13 14:52:26.260990 symdexer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-04-13 09:20:48.000000 symdexer-0.1.1/README.md
--rw-rw-rw-   0        0        0      586 2023-04-13 14:51:55.000000 symdexer-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:52:26.260990 symdexer-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.207580 symdexer-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.245368 symdexer-0.1.1/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-13 14:51:15.000000 symdexer-0.1.1/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     1718 2023-04-13 10:13:35.000000 symdexer-0.1.1/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     2247 2023-04-13 14:51:11.000000 symdexer-0.1.1/src/symdexer/main.py
--rw-rw-rw-   0        0        0      564 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     1309 2023-04-13 10:06:06.000000 symdexer-0.1.1/src/symdexer/settings.py
--rw-rw-rw-   0        0        0      979 2023-04-13 09:20:48.000000 symdexer-0.1.1/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:52:26.260990 symdexer-0.1.1/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      548 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 14:52:26.000000 symdexer-0.1.1/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.172071 symdexer-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      548 2023-04-13 19:02:59.171071 symdexer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-04-13 01:29:38.000000 symdexer-0.1.2/README.md
+-rw-rw-rw-   0        0        0      586 2023-04-13 19:01:36.000000 symdexer-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:02:59.172071 symdexer-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.138076 symdexer-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.153070 symdexer-0.1.2/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.1.2/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.1.2/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     1718 2023-04-13 17:01:00.000000 symdexer-0.1.2/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     2243 2023-04-13 17:04:05.000000 symdexer-0.1.2/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      564 2023-04-13 01:01:39.000000 symdexer-0.1.2/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     1309 2023-04-13 17:01:00.000000 symdexer-0.1.2/src/symdexer/settings.py
+-rw-rw-rw-   0        0        0      979 2023-04-13 02:29:44.000000 symdexer-0.1.2/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.169071 symdexer-0.1.2/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.1.1/LICENSE.txt` & `symdexer-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.1/PKG-INFO` & `symdexer-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.1.1/pyproject.toml` & `symdexer-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `symdexer-0.1.1/src/symdexer/cache.py` & `symdexer-0.1.2/src/symdexer/cache.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.1/src/symdexer/main.py` & `symdexer-0.1.2/src/symdexer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,15 @@
         default="symdexer.toml",
         help="Name of the file to load the settings from",
     )
 
     subp = parser.add_subparsers(required=True, dest="command")
 
     find = subp.add_parser("find", help="Searches the cache for symbols matching a list of patterns")
-
     find.add_argument("patterns", metavar="PATTERN", nargs="+", help="The patterns to look for")
-
     find.add_argument("-o", "--order", metavar="SYM_TYPE", choices=list(SYM_TYPES), nargs="+")
 
     subp.add_parser("reset-cache", help="Determines if the cache should be reset or not")
 
     subp.add_parser("init", help="Creates a new configuration file")
 
     args = parser.parse_args()
```

### Comparing `symdexer-0.1.1/src/symdexer/modules.py` & `symdexer-0.1.2/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.1/src/symdexer/settings.py` & `symdexer-0.1.2/src/symdexer/settings.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.1/src/symdexer/symbols.py` & `symdexer-0.1.2/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.1/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.1.2/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

