# Comparing `tmp/confguard-1.1.5.tar.gz` & `tmp/confguard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confguard-1.1.5.tar", last modified: Thu Apr 13 14:58:34 2023, max compression
+gzip compressed data, was "confguard-1.2.0.tar", last modified: Thu Apr 13 17:07:52 2023, max compression
```

## Comparing `confguard-1.1.5.tar` & `confguard-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.541811 confguard-1.1.5/
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.1.5/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.1.5/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.1.5/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.1.5/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:58:34.541960 confguard-1.1.5/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.1.5/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.1.5/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 14:58:34.542575 confguard-1.1.5/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.1.5/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.511359 confguard-1.1.5/src/
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.533782 confguard-1.1.5/src/confguard/
--rw-r--r--   0 Q187392    (501) staff       (20)       44 2023-04-13 14:57:33.000000 confguard-1.1.5/src/confguard/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.1.5/src/confguard/__main__.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/environment.py
--rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.1.5/src/confguard/exceptions.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2831 2023-04-13 12:56:13.000000 confguard-1.1.5/src/confguard/helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7836 2023-04-13 14:56:07.000000 confguard-1.1.5/src/confguard/main.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8171 2023-04-13 13:41:01.000000 confguard-1.1.5/src/confguard/model.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.538216 confguard-1.1.5/src/confguard.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 14:58:34.000000 confguard-1.1.5/src/confguard.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/entry_points.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 14:58:33.000000 confguard-1.1.5/src/confguard.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 14:58:34.541385 confguard-1.1.5/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_adapter.py
--rw-r--r--   0 Q187392    (501) staff       (20)     7959 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_cli.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3596 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_helper.py
--rw-r--r--   0 Q187392    (501) staff       (20)     8360 2023-01-24 18:57:00.000000 confguard-1.1.5/tests/test_model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 17:07:52.842840 confguard-1.2.0/
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-18 10:14:52.000000 confguard-1.2.0/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)       71 2023-01-24 18:57:00.000000 confguard-1.2.0/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1513 2022-12-18 10:14:52.000000 confguard-1.2.0/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      119 2022-12-18 10:14:52.000000 confguard-1.2.0/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 17:07:52.842952 confguard-1.2.0/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     1395 2023-01-24 18:57:00.000000 confguard-1.2.0/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-18 10:14:52.000000 confguard-1.2.0/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1938 2023-04-13 17:07:52.865327 confguard-1.2.0/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-18 10:14:52.000000 confguard-1.2.0/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 17:07:52.817696 confguard-1.2.0/src/
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 17:07:52.835456 confguard-1.2.0/src/confguard/
+-rw-r--r--   0 Q187392    (501) staff       (20)       44 2023-04-13 17:07:30.000000 confguard-1.2.0/src/confguard/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)       50 2022-12-18 10:14:52.000000 confguard-1.2.0/src/confguard/__main__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3630 2023-01-24 18:57:00.000000 confguard-1.2.0/src/confguard/adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     1740 2023-01-24 18:57:00.000000 confguard-1.2.0/src/confguard/environment.py
+-rw-r--r--   0 Q187392    (501) staff       (20)      363 2023-01-24 18:57:00.000000 confguard-1.2.0/src/confguard/exceptions.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3273 2023-04-13 17:07:05.000000 confguard-1.2.0/src/confguard/helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8029 2023-04-13 17:05:10.000000 confguard-1.2.0/src/confguard/main.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     8929 2023-04-13 17:07:44.000000 confguard-1.2.0/src/confguard/model.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 17:07:52.840129 confguard-1.2.0/src/confguard.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3507 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      592 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       49 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/entry_points.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       28 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-13 17:07:52.000000 confguard-1.2.0/src/confguard.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-13 17:07:52.842167 confguard-1.2.0/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     2714 2023-01-24 18:57:00.000000 confguard-1.2.0/tests/test_adapter.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     7997 2023-04-13 16:38:27.000000 confguard-1.2.0/tests/test_cli.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     4572 2023-04-13 17:07:40.000000 confguard-1.2.0/tests/test_helper.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     9112 2023-04-13 17:07:40.000000 confguard-1.2.0/tests/test_model.py
```

### Comparing `confguard-1.1.5/LICENSE` & `confguard-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/PKG-INFO` & `confguard-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.5
+Version: 1.2.0
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.5/README.md` & `confguard-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/setup.cfg` & `confguard-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confguard
-version = 1.1.5
+version = 1.2.0
 description = "Save configuration files outside project in save place"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/confguard
 classifiers =
```

### Comparing `confguard-1.1.5/src/confguard/adapter.py` & `confguard-1.2.0/src/confguard/adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/src/confguard/environment.py` & `confguard-1.2.0/src/confguard/environment.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/src/confguard/helper.py` & `confguard-1.2.0/src/confguard/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,14 +50,34 @@
     name = Path(
         target
     ).name  # Gotcha: source_path.name is not the same as target_path.name
     rel_path = os.path.relpath(target_path, source_path)
     return Path(rel_path) / name
 
 
+def normalize_name(name: str) -> str:
+    if name.startswith("."):
+        return f"dot.{name[1:]}"
+    return name
+
+
+def denormalize_name(name: str) -> str:
+    if name.startswith("dot."):
+        return f".{name[4:]}"
+    return name
+
+
+def normalize_path(path: Path) -> Path:
+    return Path(*[normalize_name(p) for p in path.parts])
+
+
+def denormalize_path(path: Path) -> Path:
+    return Path(*[denormalize_name(p) for p in path.parts])
+
+
 if __name__ == "__main__":
     # Create a list of strings
     files = [
         "file1____________________________________________________________",
         "file2____________________________________________________________",
         "file3____________________________________________________________",
         "file4____________________________________________________________",
```

### Comparing `confguard-1.1.5/src/confguard/main.py` & `confguard-1.2.0/src/confguard/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from rich.logging import RichHandler
 from rich.theme import Theme
 
 from confguard import __version__
 from confguard.adapter import TomlRepoConfGuard
 from confguard.environment import CONFGUARD_BKP_DIR, CONFGUARD_CONFIG_FILE, config
 from confguard.exceptions import InvalidConfigError
+from confguard.helper import normalize_path
 from confguard.model import ConfGuard
 
 _log = logging.getLogger(__name__)
 app = typer.Typer(help="Save sensitive configuration in a save place")
 
 
 @app.command()
@@ -61,25 +62,25 @@
             _log.debug(f"Project is already guarded, but not all files are guarded.")
             _unguard(source_dir)  # get everything back and recreate with new config
 
     _log.info(f"Guarding {source_dir}")
 
     cg.create_sentinel()
     try:
-        cg.create_bkp(cg.source_dir, cg.targets)
+        cg.create_bkp(cg.source_dir, cg.targets, normalizer=lambda x: x)
     except Exception as e:
         typer.secho(f"Error occurred, Aborting: {e}", fg=typer.colors.RED)
         cg.delete_dir(dir_=cg.source_dir / CONFGUARD_BKP_DIR)
         cg.remove_sentinel()
         repo.add(cg)  # save it
         raise typer.Abort(1)
 
     try:
         cg.move_files()
-        cg.create_lk(cg.targets)
+        cg.create_lk(cg.targets, normalizer=normalize_path)
         cg.back_create()
     except Exception as e:
         typer.secho(f"Error occurred, rolling back: {e}", fg=typer.colors.RED)
         cg.remove_lk(cg.targets)
         cg.back_remove()
         cg.restore_bkp(cg.source_dir, cg.targets)
         cg.remove_sentinel()
@@ -123,15 +124,15 @@
             fg=typer.colors.GREEN,
         )
         raise typer.Exit(1)
 
     _log.info(f"Un-guarding {source_dir}")
 
     try:
-        cg.create_bkp(cg.target_dir, cg.files)
+        cg.create_bkp(cg.target_dir, cg.files, normalizer=normalize_path)
     except Exception as e:
         typer.secho(f"Error occurred, Aborting: {e}", fg=typer.colors.RED)
         cg.delete_dir(dir_=cg.target_dir / CONFGUARD_BKP_DIR)
         cg.remove_sentinel()
         repo.add(cg)  # save it
         raise typer.Abort(1)
 
@@ -140,15 +141,15 @@
         cg.back_remove()
         cg.unmove_files()
         cg.remove_sentinel()
     except Exception as e:
         _log.error(f"Error occurred, rolling back: {e}")
         cg.restore_bkp(cg.target_dir, cg.files)
         try:
-            cg.create_lk(cg.files)
+            cg.create_lk(cg.files, normalizer=normalize_path)
         except Exception as e:
             _log.warning(f"Manual intervention required: {e}")
         try:
             cg.back_create()
         except Exception as e:
             _log.error(f"Manual intervention required: {e}")
         raise typer.Abort(1)
@@ -193,15 +194,15 @@
             fg=typer.colors.RED,
         )
         raise typer.Exit(1)
     project = projects[0]
     _log.info(f"Found guarded project files for {project}, re-linking it.")
 
     ConfGuard.restore_toml(source_dir, project)
-    _ = _unguard(source_dir)
+    _ = _unguard(source_dir)  # breakpoint here shows restored directory
     return _guard(source_dir)
 
 
 @app.callback(invoke_without_command=True)
 def main(
     ctx: typer.Context,
     verbose: bool = typer.Option(False, "-v", "--verbose", help="verbosity"),
```

### Comparing `confguard-1.1.5/src/confguard/model.py` & `confguard-1.2.0/src/confguard/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import shutil
 import uuid
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Optional
+from typing import Callable, Optional
 
 from confguard.environment import CONFGUARD_BKP_DIR, CONFGUARD_CONFIG_FILE, config
 from confguard.exceptions import BackupExistError, DirectoryNotDeleted
 from confguard.helper import (
     _create_relative_path,
+    denormalize_path,
     is_directory_containing_only,
-    is_directory_empty,
+    normalize_path,
 )
 
 _log = logging.getLogger(__name__)
 
 
 @dataclass(frozen=False, kw_only=True, repr=False)
 class ConfGuard:
@@ -46,53 +47,71 @@
             _log.warning(
                 f"Directory {self.target_dir} still exists. Keeping sentinel in .confguard"
             )
             return
         self.sentinel = None
 
     @staticmethod
-    def _move_files(source_dir: Path, target_dir: Path, targets: list[str]) -> None:
+    def _move_files(
+        source_dir: Path,
+        target_dir: Path,
+        targets: list[str],
+        normalizer: Callable[[Path], Path],
+    ) -> None:
         for rel_path in targets:
-            tgt_path = target_dir / rel_path
+            tgt_path = normalizer(target_dir / rel_path)
             src_path = source_dir / rel_path
 
             if src_path.exists():
                 _log.debug(f"Moving {src_path} to {tgt_path}")
                 tgt_path.parent.exists() or tgt_path.parent.mkdir(parents=True)
                 src_path.rename(tgt_path)
             else:
                 _log.warning(f"{src_path} does not exist")
 
     def move_files(self) -> None:
         assert self.sentinel is not None, "Sentinel not created"
         Path(self.target_dir).mkdir(parents=True, exist_ok=True)
-        self._move_files(self.source_dir, self.target_dir, targets=self.targets)
+        self._move_files(
+            self.source_dir,
+            self.target_dir,
+            targets=self.targets,
+            normalizer=normalize_path,
+        )
 
     def unmove_files(self) -> None:
         """Restore files from confguard directory, based on saved file list"""
-        self._move_files(self.target_dir, self.source_dir, self.files)
+        files = [str(normalize_path(Path(f))) for f in self.files]
+        self._move_files(
+            self.target_dir, self.source_dir, files, normalizer=denormalize_path
+        )
         if is_directory_containing_only(
             self.target_dir, ["_confguard", ".confguard.bkp"]
         ):
             shutil.rmtree(self.target_dir)
         else:
             _log.warning(
                 f"Directory {self.target_dir} is not empty. Please remove manually."
             )
 
     @staticmethod
-    def _create_bkp(source_dir: Path, bkp_dir: Path, targets: list[str]) -> None:
+    def _create_bkp(
+        source_dir: Path,
+        bkp_dir: Path,
+        targets: list[str],
+        normalizer: Callable[[Path], Path],
+    ) -> None:
         try:
             Path(bkp_dir).mkdir(parents=True, exist_ok=False)
         except FileExistsError:
             raise BackupExistError(f"Backup dir {bkp_dir} already exists.")
 
         for rel_path in targets:
-            bkp_path = bkp_dir / rel_path
-            src_path = source_dir / rel_path
+            bkp_path = normalizer(bkp_dir / rel_path)
+            src_path = normalizer(source_dir / rel_path)
 
             if src_path.exists():
                 if not src_path.is_symlink():
                     if src_path.is_file():
                         bkp_path.parent.exists() or bkp_path.parent.mkdir(parents=True)
                         shutil.copy2(src_path, bkp_path)
                     elif src_path.is_dir():
@@ -101,24 +120,31 @@
                     _log.info(
                         f"{src_path} is a symlink. Skipping backup.",
                         extra={"highlighter": None},
                     )
             else:
                 _log.warning(f"{src_path} does not exist")
 
-    def create_bkp(self, dir_: Path, targets: list[str]) -> None:
+    def create_bkp(
+        self, dir_: Path, targets: list[str], normalizer: Callable[[Path], Path]
+    ) -> None:
         bkp_dir = dir_ / CONFGUARD_BKP_DIR
-        self._create_bkp(dir_, bkp_dir, targets)
+        self._create_bkp(dir_, bkp_dir, targets, normalizer=normalizer)
 
     @staticmethod
-    def _restore_bkp(source_dir: Path, bkp_dir: Path, targets: list[str]) -> None:
+    def _restore_bkp(
+        source_dir: Path,
+        bkp_dir: Path,
+        targets: list[str],
+        normalizer: Callable[[Path], Path],
+    ) -> None:
         assert bkp_dir.exists(), f"Backup dir {bkp_dir} does not exist"
         for rel_path in targets:
-            bkp_path = bkp_dir / rel_path
-            src_path = source_dir / rel_path
+            bkp_path = normalizer(bkp_dir / rel_path)
+            src_path = normalizer(source_dir / rel_path)
 
             if bkp_path.exists():
                 if bkp_path.is_file():
                     src_path.parent.exists() or src_path.parent.mkdir(
                         parents=True, exist_ok=True
                     )
 
@@ -141,32 +167,35 @@
                     _log.info(f"Restoring {src_path}.", extra={"highlighter": None})
                     shutil.copytree(bkp_path, src_path, dirs_exist_ok=True)
             else:
                 _log.warning(
                     f"File {bkp_path} does not exist in backup. Cannot restore."
                 )
 
-    def restore_bkp(self, dir_: Path, targets: list[str]) -> None:
+    def restore_bkp(
+        self, dir_: Path, targets: list[str], normalizer: Callable[[Path], Path]
+    ) -> None:
         bkp_dir = dir_ / CONFGUARD_BKP_DIR
-        self._restore_bkp(dir_, bkp_dir, targets)
+        self._restore_bkp(dir_, bkp_dir, targets, normalizer=normalizer)
 
     @staticmethod
     def delete_dir(dir_: Path) -> None:
         try:
             shutil.rmtree(dir_, ignore_errors=False)
         except FileNotFoundError:
             pass
         except Exception:
             raise DirectoryNotDeleted(
                 f"{dir_} could not be deleted. Please delete it manually."
             )
 
-    def create_lk(self, targets: list[str]) -> None:
+    def create_lk(self, targets: list[str], normalizer: Callable[[Path], Path]) -> None:
         for rel_path in targets:
-            tgt_path = self.target_dir / rel_path
+            # tgt_path = self.target_dir / rel_path
+            tgt_path = normalizer(self.target_dir / rel_path)
             src_path = self.source_dir / rel_path
 
             if self.is_relative:
                 tgt_path = _create_relative_path(str(src_path), str(tgt_path))
 
             _log.debug(f"Creating link {src_path} to {tgt_path}")
             src_path.symlink_to(tgt_path)
```

### Comparing `confguard-1.1.5/src/confguard.egg-info/PKG-INFO` & `confguard-1.2.0/src/confguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confguard
-Version: 1.1.5
+Version: 1.2.0
 Summary: "Save configuration files outside project in save place"
 Home-page: https://github.com/sysid/confguard
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `confguard-1.1.5/src/confguard.egg-info/SOURCES.txt` & `confguard-1.2.0/src/confguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/tests/test_adapter.py` & `confguard-1.2.0/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `confguard-1.1.5/tests/test_cli.py` & `confguard-1.2.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,29 +43,29 @@
     confguard = list(Path(config.confguard_path).glob("**/test_proj-*"))
     assert len(confguard) == 1
     confguard = confguard[0]
     assert confguard.is_dir()
     assert confguard.name == cg.sentinel
 
     # then: confguard directory contains the files and dirs
-    assert (confguard / ".envrc").is_file()
-    assert (confguard / ".run").is_dir()
+    assert (confguard / "dot.envrc").is_file()
+    assert (confguard / "dot.run").is_dir()
     assert (confguard / "xxx/xxx.txt").is_file()
 
     # then: .confguard backup exists
     assert (cg.target_dir / CONFGUARD_CONFIG_FILE).with_suffix(".bkp").is_file()
 
     # then: in source dir the files and dirs are replaced by links
     assert (TEST_PROJ / ".envrc").is_symlink()
     assert (TEST_PROJ / ".run").is_symlink()
     assert (TEST_PROJ / "xxx/xxx.txt").is_symlink()
 
     # then: the links point to the confguard directory replacements
-    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / ".envrc")
-    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / ".run")
+    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / "dot.envrc")
+    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / "dot.run")
 
     # then backlink created
     assert Path(confguard / f".{cg.sentinel}.confguard").resolve() == TEST_PROJ
 
 
 def test__unguard():
     # given
@@ -152,31 +152,31 @@
     confguard = list(Path(config.confguard_path).glob("**/test_proj-*"))
     assert len(confguard) == 1
     confguard = confguard[0]
     assert confguard.is_dir()
     assert confguard.name == cg.sentinel
 
     # then: confguard directory contains the files and dirs
-    assert (confguard / ".envrc").is_file()
-    assert (confguard / ".run").is_dir()
+    assert (confguard / "dot.envrc").is_file()
+    assert (confguard / "dot.run").is_dir()
     assert (confguard / "xxx/xxx.txt").is_file()
 
     # then: .confguard backup exists
     assert (cg.target_dir / CONFGUARD_CONFIG_FILE).with_suffix(".bkp").is_file()
 
     # then: in source dir the files and dirs are replaced by links
     assert (TEST_PROJ / ".envrc").is_symlink()
     assert (TEST_PROJ / ".run").is_symlink()
     assert (TEST_PROJ / "xxx/xxx.txt").is_symlink()
 
     # then: the links point to the confguard directory replacements
-    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / ".envrc")
-    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / ".run")
+    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / "dot.envrc")
+    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / "dot.run")
 
-    # then backlink created
+    # # then backlink created
     assert Path(confguard / f".{cg.sentinel}.confguard").resolve() == TEST_PROJ
 
 
 def test_restore_toml():
     # given a guarded project with missing .confguard file
     cg = _guard(source_dir=TEST_PROJ)
     (TEST_PROJ / CONFGUARD_CONFIG_FILE).unlink()
@@ -206,25 +206,25 @@
     confguard = list(Path(config.confguard_path).glob("**/test_proj-*"))
     assert len(confguard) == 1
     confguard = confguard[0]
     assert confguard.is_dir()
     assert confguard.name == cg.sentinel
 
     # then: confguard directory contains the files and dirs
-    assert (confguard / ".envrc").is_file()
-    assert (confguard / ".run").is_dir()
+    assert (confguard / "dot.envrc").is_file()
+    assert (confguard / "dot.run").is_dir()
     assert (confguard / "xxx/xxx.txt").is_file()
 
     # then: .confguard backup exists
     assert (cg.target_dir / CONFGUARD_CONFIG_FILE).with_suffix(".bkp").is_file()
 
     # then: in source dir the files and dirs are replaced by links
     assert (TEST_PROJ / ".envrc").is_symlink()
     assert (TEST_PROJ / ".run").is_symlink()
     assert (TEST_PROJ / "xxx/xxx.txt").is_symlink()
 
     # then: the links point to the confguard directory replacements
-    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / ".envrc")
-    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / ".run")
+    assert Path(TEST_PROJ / ".envrc").resolve() == Path(confguard / "dot.envrc")
+    assert Path(TEST_PROJ / ".run").resolve() == Path(confguard / "dot.run")
 
     # then backlink created
     assert Path(confguard / f".{cg.sentinel}.confguard").resolve() == TEST_PROJ
```

### Comparing `confguard-1.1.5/tests/test_helper.py` & `confguard-1.2.0/tests/test_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from pathlib import Path
 
 import pytest
 
 # noinspection PyProtectedMember
 from confguard.helper import (
     _create_relative_path,
+    denormalize_name,
+    denormalize_path,
     deserialize_from_base64,
+    normalize_name,
+    normalize_path,
     serialize_to_base64,
 )
 
 _log = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize(
@@ -100,7 +104,43 @@
 X19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19flIxBZmlsZTVfX19fX19f
 X19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX19fX1+UaAFoAmgD
 aARoBWUu
     """
     obj = deserialize_from_base64(serialized)
     print(f"\n{obj}")
     assert obj == FILES
+
+
+def test_normalize_name():
+    assert normalize_name(".xxx") == "dot.xxx"
+    assert normalize_name("xxx") == "xxx"
+
+
+def test_denormalize_name():
+    assert denormalize_name("dot.xxx") == ".xxx"
+    assert denormalize_name("xxx") == "xxx"
+
+
+@pytest.mark.parametrize(
+    ("path", "expected"),
+    (
+        ["xxx/xxx.txt", "xxx/xxx.txt"],
+        [".run", "dot.run"],
+        [".run/.env", "dot.run/dot.env"],
+        ["./.run/.env", "./dot.run/dot.env"],
+    ),
+)
+def test_normalize_path(path, expected):
+    assert normalize_path(Path(path)) == Path(expected)
+
+
+@pytest.mark.parametrize(
+    ("path", "expected"),
+    (
+        ["xxx/xxx.txt", "xxx/xxx.txt"],
+        ["dot.run", ".run"],
+        ["dot.run/dot.env", ".run/.env"],
+        ["./dot.run/dot.env", "./.run/.env"],
+    ),
+)
+def test_denormalize_path(path, expected):
+    assert denormalize_path(Path(path)) == Path(expected)
```

