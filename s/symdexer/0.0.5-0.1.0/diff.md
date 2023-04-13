# Comparing `tmp/symdexer-0.0.5.tar.gz` & `tmp/symdexer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.0.5.tar", last modified: Thu Apr 13 02:32:17 2023, max compression
+gzip compressed data, was "symdexer-0.1.0.tar", last modified: Thu Apr 13 10:56:14 2023, max compression
```

## Comparing `symdexer-0.0.5.tar` & `symdexer-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:32:17.744585 symdexer-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      548 2023-04-13 02:32:17.743583 symdexer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-04-13 01:29:38.000000 symdexer-0.0.5/README.md
--rw-rw-rw-   0        0        0      438 2023-04-13 02:31:54.000000 symdexer-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 02:32:17.744585 symdexer-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 02:32:17.708585 symdexer-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 02:32:17.721583 symdexer-0.0.5/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.0.5/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0     1173 2023-04-13 01:58:49.000000 symdexer-0.0.5/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     1435 2023-04-13 02:25:32.000000 symdexer-0.0.5/src/symdexer/cache.py
--rw-rw-rw-   0        0        0      564 2023-04-13 01:01:39.000000 symdexer-0.0.5/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     1510 2023-04-13 02:24:54.000000 symdexer-0.0.5/src/symdexer/settings.py
--rw-rw-rw-   0        0        0      979 2023-04-13 02:29:44.000000 symdexer-0.0.5/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:32:17.740585 symdexer-0.0.5/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      548 2023-04-13 02:32:17.000000 symdexer-0.0.5/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-13 02:32:17.000000 symdexer-0.0.5/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:32:17.000000 symdexer-0.0.5/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 02:32:17.000000 symdexer-0.0.5/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.128890 symdexer-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 09:20:48.000000 symdexer-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      548 2023-04-13 10:56:14.128890 symdexer-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-04-13 09:20:48.000000 symdexer-0.1.0/README.md
+-rw-rw-rw-   0        0        0      586 2023-04-13 10:55:00.000000 symdexer-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:56:14.128890 symdexer-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.026863 symdexer-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.097616 symdexer-0.1.0/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0     2327 2023-04-13 10:15:30.000000 symdexer-0.1.0/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     1718 2023-04-13 10:13:35.000000 symdexer-0.1.0/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0      564 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     1309 2023-04-13 10:06:06.000000 symdexer-0.1.0/src/symdexer/settings.py
+-rw-rw-rw-   0        0        0      979 2023-04-13 09:20:48.000000 symdexer-0.1.0/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:56:14.128890 symdexer-0.1.0/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-04-13 10:56:14.000000 symdexer-0.1.0/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 10:56:13.000000 symdexer-0.1.0/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.0.5/LICENSE.txt` & `symdexer-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.0.5/PKG-INFO` & `symdexer-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.0.5
+Version: 0.1.0
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.0.5/src/symdexer/cache.py` & `symdexer-0.1.0/src/symdexer/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,15 +35,24 @@
     for symbol, sym_type in iter_symbols(module):
         db.execute(
             "INSERT OR IGNORE INTO Symbol (name, type, module) VALUES (?, ? ,?)",
             (symbol, sym_type, module.name),
         )
 
 
-def search_cache(file: Path, symbol: str, order: list[str]) -> Generator[tuple[str, str], None, None]:
+def search_cache(file: Path, symbols: list[str], order: list[str]) -> Generator[tuple[str, str], None, None]:
     with sqlite3.connect(file) as db:
-        for sym_type in order:
-            cursor = db.execute(
-                "SELECT name, module FROM Symbol WHERE name LIKE ? AND type = ?",
-                (symbol, sym_type),
-            )
-            yield from cursor.fetchall()
+        orders = " OR ".join("type = ?" for _ in order)
+        patterns = " OR ".join("name LIKE ?" for _ in symbols)
+        cursor = db.execute(
+            f"""
+            SELECT GROUP_CONCAT(name, ", ") as names, module
+            FROM Symbol
+            WHERE ({patterns}) AND ({orders})
+            GROUP BY
+                module
+            ORDER BY
+                LENGTH(module) + LENGTH(names) ASC
+            """,
+            (*symbols, *order),
+        )
+        return cursor.fetchall()
```

### Comparing `symdexer-0.0.5/src/symdexer/modules.py` & `symdexer-0.1.0/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.0.5/src/symdexer/settings.py` & `symdexer-0.1.0/src/symdexer/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,40 +16,35 @@
     packages: list[Path]
 
 
 def load_settings(file: str):
     path = Path(file)
 
     if not path.is_file():
-        with path.open("w", encoding="utf-8") as fp:
-            fp.write('cache = "symdex.db"\n')
-            fp.write('order = ["defines", "assigns", "imports"]\n')
-            fp.write("\n")
-            fp.write("[packages]\n")
-            fp.write('package_name = "path/to/package"\n')
+        raise FileNotFoundError(f"settings file `{file}` does not exist")
 
     with path.open("rb") as fp:
         data = tomllib.load(fp)
 
-        if any(sym_type not in SYM_TYPES for sym_type in data["order"]):
+        if any(sym_type not in SYM_TYPES for sym_type in data["default_order"]):
             raise ValueError(f"invalid symbol type in order, values must be {list(SYM_TYPES)}")
 
-        return Settings(Path(data["cache"]), data["order"], list(load_packages(data["packages"])))
+        return Settings(Path(data["cache"]), data["default_order"], list(load_packages(data["packages"])))
 
 
 def load_packages(packages: dict[str, str]):
     for name, path in packages.items():
         if path:
             p = Path(path)
 
             if not p.is_dir():
-                raise ImportError(f"package {name} must be a folder")
+                raise ImportError(f"package `{name}` must be a folder")
 
             yield p
             continue
 
         p = Path(importlib.import_module(name).__file__)
 
         if not p.is_file() or p.name.lower() != "__init__.py":
-            raise ImportError(f"module {name} is not a package")
+            raise ImportError(f"module `{name}` is not a package")
 
         yield p.parent
```

### Comparing `symdexer-0.0.5/src/symdexer/symbols.py` & `symdexer-0.1.0/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.0.5/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.1.0/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.0.5
+Version: 0.1.0
 Summary: A CLI for finding symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

