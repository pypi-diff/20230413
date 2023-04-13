# Comparing `tmp/confguard-1.0.3.tar.gz` & `tmp/confguard-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confguard-1.0.3.tar", last modified: Fri Dec 23 14:09:09 2022, max compression
+gzip compressed data, was "confguard-1.1.3.tar", last modified: Thu Apr 13 13:41:10 2023, max compression
```

## Comparing `confguard-1.0.3.tar` & `confguard-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-23 14:09:09.532295 confguard-1.0.3/
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.0.3/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)       71 2022-12-22 16:07:30.000000 confguard-1.0.3/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.0.3/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.0.3/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2022-12-23 14:09:09.532445 confguard-1.0.3/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     1395 2022-12-23 14:08:12.000000 confguard-1.0.3/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.0.3/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1932 2022-12-23 14:09:09.533121 confguard-1.0.3/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.0.3/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-23 14:09:09.506342 confguard-1.0.3/src/
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-23 14:09:09.527701 confguard-1.0.3/src/confguard/
--rw-r--r--   0 Q187392    (501) staff       (20)       42 2022-12-23 14:08:54.000000 confguard-1.0.3/src/confguard/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.0.3/src/confguard/__main__.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3573 2022-12-22 16:32:03.000000 confguard-1.0.3/src/confguard/adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1740 2022-12-21 17:12:13.000000 confguard-1.0.3/src/confguard/environment.py
--rw-r--r--   0 Q187392    (501) staff       (20)      363 2022-12-21 13:01:33.000000 confguard-1.0.3/src/confguard/exceptions.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2331 2022-12-23 13:59:10.000000 confguard-1.0.3/src/confguard/helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7354 2022-12-23 13:59:10.000000 confguard-1.0.3/src/confguard/main.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7659 2022-12-23 13:59:10.000000 confguard-1.0.3/src/confguard/model.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2022-12-23 14:09:09.531578 confguard-1.0.3/src/confguard.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2022-12-23 14:09:08.000000 confguard-1.0.3/src/confguard.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      511 2022-12-23 14:09:09.000000 confguard-1.0.3/src/confguard.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2022-12-23 14:09:08.000000 confguard-1.0.3/src/confguard.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       49 2022-12-23 14:09:08.000000 confguard-1.0.3/src/confguard.egg-info/entry_points.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       23 2022-12-23 14:09:08.000000 confguard-1.0.3/src/confguard.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2022-12-23 14:09:08.000000 confguard-1.0.3/src/confguard.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.374081 confguard-1.1.3/
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.3/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.3/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.3/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.3/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 13:41:10.374208 confguard-1.1.3/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.3/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.3/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 13:41:10.375120 confguard-1.1.3/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.3/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.325770 confguard-1.1.3/src/
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.359435 confguard-1.1.3/src/confguard/
+-rw-r--r--   0 Q187392    (501) staff       (20)       42 2023-04-13 13:40:26.000000 confguard-1.1.3/src/confguard/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.3/src/confguard/__main__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/exceptions.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.3/src/confguard/helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7354 2023-01-24 18:57:00.000000 confguard-1.1.3/src/confguard/main.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.3/src/confguard/model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.366710 confguard-1.1.3/src/confguard.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 13:41:10.000000 confguard-1.1.3/src/confguard.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/entry_points.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 13:41:09.000000 confguard-1.1.3/src/confguard.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 13:41:10.373654 confguard-1.1.3/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_cli.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.3/tests/test_model.py
```

### Comparing `confguard-1.0.3/LICENSE` & `confguard-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `confguard-1.0.3/PKG-INFO` & `confguard-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.0.3
+Version: 1.1.3
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.0.3/README.md` & `confguard-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `confguard-1.0.3/setup.cfg` & `confguard-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confguard
-version = 1.0.3
+version = 1.1.3
 description = "Save configuration files outside project in save place"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/confguard
 classifiers = 
@@ -19,14 +19,15 @@
 packages = find:
 package_dir = 
 	=src
 install_requires = 
 	pydantic
 	tomlkit
 	typer
+	rich
 include_package_data = True
 python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `confguard-1.0.3/src/confguard/adapter.py` & `confguard-1.1.3/src/confguard/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             files = deserialize_from_base64(self.toml["_internal_"]["files"])
         except NonExistentKey:
             return cg
 
         cg.sentinel = sentinel
         cg.target_dir = config.confguard_path / sentinel
         cg.files = files
+        _log.debug(f"{sentinel=}, {targets=}, {files=}")
         return cg
 
     def add(self, confguard: ConfGuard) -> None:
         if confguard.sentinel is not None:
             if self.toml.get("_internal_") is not None:  # Update
                 self.toml["_internal_"]["sentinel"] = confguard.sentinel
                 self.toml["_internal_"]["files"] = tomlkit.string(
```

### Comparing `confguard-1.0.3/src/confguard/environment.py` & `confguard-1.1.3/src/confguard/environment.py`

 * *Files identical despite different names*

### Comparing `confguard-1.0.3/src/confguard/main.py` & `confguard-1.1.3/src/confguard/main.py`

 * *Files identical despite different names*

### Comparing `confguard-1.0.3/src/confguard/model.py` & `confguard-1.1.3/src/confguard/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import uuid
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional
 
 from confguard.environment import CONFGUARD_BKP_DIR, CONFGUARD_CONFIG_FILE, config
 from confguard.exceptions import BackupExistError, DirectoryNotDeleted
-from confguard.helper import _create_relative_path
+from confguard.helper import (
+    _create_relative_path,
+    is_directory_containing_only,
+    is_directory_empty,
+)
 
 _log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=False, kw_only=True, repr=False)
 class ConfGuard:
     source_dir: Path
@@ -34,14 +38,19 @@
             return
 
         self.sentinel = f"{self.source_dir.name}-{uuid.uuid4().hex[:8]}"
         self.target_dir = config.confguard_path / self.sentinel
         _log.debug(f"Sentinel created: {self.sentinel=}")
 
     def remove_sentinel(self) -> None:
+        if self.target_dir.exists():
+            _log.warning(
+                f"Directory {self.target_dir} still exists. Keeping sentinel in .confguard"
+            )
+            return
         self.sentinel = None
 
     @staticmethod
     def _move_files(source_dir: Path, target_dir: Path, targets: list[str]) -> None:
         for rel_path in targets:
             tgt_path = target_dir / rel_path
             src_path = source_dir / rel_path
@@ -57,15 +66,22 @@
         assert self.sentinel is not None, "Sentinel not created"
         Path(self.target_dir).mkdir(parents=True, exist_ok=True)
         self._move_files(self.source_dir, self.target_dir, targets=self.targets)
 
     def unmove_files(self) -> None:
         """Restore files from confguard directory, based on saved file list"""
         self._move_files(self.target_dir, self.source_dir, self.files)
-        shutil.rmtree(self.target_dir)
+        if is_directory_containing_only(
+            self.target_dir, ["_confguard", ".confguard.bkp"]
+        ):
+            shutil.rmtree(self.target_dir)
+        else:
+            _log.warning(
+                f"Directory {self.target_dir} is not empty. Please remove manually."
+            )
 
     @staticmethod
     def _create_bkp(source_dir: Path, bkp_dir: Path, targets: list[str]) -> None:
         try:
             Path(bkp_dir).mkdir(parents=True, exist_ok=False)
         except FileExistsError:
             raise BackupExistError(f"Backup dir {bkp_dir} already exists.")
```

### Comparing `confguard-1.0.3/src/confguard.egg-info/PKG-INFO` & `confguard-1.1.3/src/confguard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.0.3
+Version: 1.1.3
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

