# Comparing `tmp/diff-1c-6.6.5.tar.gz` & `tmp/diff-1c-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diff-1c-6.6.5.tar", last modified: Thu Mar  9 12:15:44 2023, max compression
+gzip compressed data, was "diff-1c-6.6.6.tar", last modified: Thu Apr 13 12:29:02 2023, max compression
```

## Comparing `diff-1c-6.6.5.tar` & `diff-1c-6.6.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:15:44.436370 diff-1c-6.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-09 12:15:44.436370 diff-1c-6.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-09 12:15:18.000000 diff-1c-6.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-09 12:15:18.000000 diff-1c-6.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 12:15:44.436370 diff-1c-6.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:15:44.432370 diff-1c-6.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:15:44.432370 diff-1c-6.6.5/src/diff_1c/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-09 12:15:18.000000 diff-1c-6.6.5/src/diff_1c/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:15:44.436370 diff-1c-6.6.5/src/diff_1c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 12:15:44.000000 diff-1c-6.6.5/src/diff_1c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:15:44.436370 diff-1c-6.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-09 12:15:18.000000 diff-1c-6.6.5/tests/test_diff_1c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:29:02.931809 diff-1c-6.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-13 12:29:02.931809 diff-1c-6.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 12:28:37.000000 diff-1c-6.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 12:28:37.000000 diff-1c-6.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:29:02.931809 diff-1c-6.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:29:02.927809 diff-1c-6.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:29:02.931809 diff-1c-6.6.6/src/diff_1c/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-13 12:28:37.000000 diff-1c-6.6.6/src/diff_1c/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:29:02.931809 diff-1c-6.6.6/src/diff_1c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 12:29:02.000000 diff-1c-6.6.6/src/diff_1c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:29:02.931809 diff-1c-6.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 12:28:37.000000 diff-1c-6.6.6/tests/test_diff_1c.py
```

### Comparing `diff-1c-6.6.5/PKG-INFO` & `diff-1c-6.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diff-1c
-Version: 6.6.5
+Version: 6.6.6
 Summary: Diff utility for 1C:Enterprise
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/diff-1c
 Keywords: 1c,diff,v8reader,v8unpack,gcomp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `diff-1c-6.6.5/README.md` & `diff-1c-6.6.6/README.md`

 * *Files identical despite different names*

### Comparing `diff-1c-6.6.5/pyproject.toml` & `diff-1c-6.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 description = "Diff utility for 1C:Enterprise"
 keywords = ["1c", "diff", "v8reader", "v8unpack", "gcomp"]
 license = {text = "MIT"}
 name = "diff-1c"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "6.6.5"
+version = "6.6.6"
 
 [project.scripts]
 diff-1c = "diff_1c.__main__:run"
 
 [project.urls]
 repository = "https://github.com/Cujoko-Dev/diff-1c"
```

### Comparing `diff-1c-6.6.5/src/diff_1c/main.py` & `diff-1c-6.6.6/src/diff_1c/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,115 +2,153 @@
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 
-from cjk_commons.settings import (SettingsError, get_attribute,
-                                  get_path_attribute, get_settings)
+from cjk_commons.settings import (
+    SettingsError,
+    get_attribute,
+    get_path_attribute,
+    get_settings,
+)
 from loguru import logger
 from parse_1c_build import Parser
 
 from diff_1c.__about__ import APP_AUTHOR, APP_NAME
 
 logger.disable(__name__)
 
 
 class Processor:
     def __init__(self, **kwargs):
         settings_file_path = get_path_attribute(
-            kwargs, 'settings_file_path', default_path=Path('settings.yaml'), is_dir=False, check_if_exists=False)
-        self.settings = get_settings(settings_file_path, app_name=APP_NAME, app_author=APP_AUTHOR)
+            kwargs,
+            "settings_file_path",
+            default_path=Path("settings.yaml"),
+            is_dir=False,
+            check_if_exists=False,
+        )
+        self.settings = get_settings(
+            settings_file_path, app_name=APP_NAME, app_author=APP_AUTHOR
+        )
+
+        self.tool = get_attribute(
+            kwargs, "tool", self.settings, "default_tool", "kdiff3"
+        ).lower()
+        if self.tool not in self.settings["tools"]:
+            raise SettingsError("Tool Incorrect")
 
-        self.tool = get_attribute(kwargs, 'tool', self.settings, 'default_tool', 'kdiff3').lower()
-        if self.tool not in self.settings['tools']:
-            raise SettingsError('Tool Incorrect')
-
-        self.tool_path = Path(self.settings['tools'][self.tool])
+        self.tool_path = Path(self.settings["tools"][self.tool])
         if not self.tool_path.is_file():
-            raise SettingsError('Tool Not Exists')
-
-        self.exclude_file_names = get_attribute(kwargs, 'exclude_file_names', self.settings, 'exclude_file_names', [])
-        self.name_format = get_attribute(kwargs, 'name_format', self.settings, 'name_format', 'tortoisegit').lower()
+            raise SettingsError("Tool Not Exists")
 
-    def run(self, base_file_fullpath: Path, mine_file_fullpath: Path, bname: str = '', yname: str = '') -> None:
+        self.exclude_file_names = get_attribute(
+            kwargs, "exclude_file_names", self.settings, "exclude_file_names", []
+        )
+        self.name_format = get_attribute(
+            kwargs, "name_format", self.settings, "name_format", "tortoisegit"
+        ).lower()
+
+    def run(
+        self,
+        base_file_path: Path,
+        mine_file_path: Path,
+        bname: str = "",
+        yname: str = "",
+    ) -> None:
         # base
         base_is_excluded = False
         if bname:
-            if self.name_format == 'tortoisegit':
-                bname_file_fullpath = Path(bname.split(':')[0])
+            if self.name_format == "tortoisegit":
+                bname_file_path = Path(bname.split(":")[0])
             else:
-                bname_file_fullpath = Path(bname.split(':')[0])
+                bname_file_path = Path(bname.split(":")[0])
         else:
-            bname_file_fullpath = Path.cwd()
-        base_source_dir_fullpath = None
-        if bname_file_fullpath.name not in self.exclude_file_names:
-            base_file_fullpath_suffix = base_file_fullpath.suffix
-            base_temp_file, base_temp_file_fullname = tempfile.mkstemp(base_file_fullpath_suffix)
+            bname_file_path = Path.cwd()
+        base_source_dir_path = None
+        if bname_file_path.name not in self.exclude_file_names:
+            base_file_path_suffix = base_file_path.suffix
+            base_temp_file, base_temp_file_name = tempfile.mkstemp(
+                base_file_path_suffix
+            )
             os.close(base_temp_file)
-            shutil.copyfile(str(base_file_fullpath), base_temp_file_fullname)
-            base_source_dir_fullpath = Path(tempfile.mkdtemp())
-            Parser().run(Path(base_temp_file_fullname), base_source_dir_fullpath)
-            Path(base_temp_file_fullname).unlink()
+            shutil.copyfile(str(base_file_path), base_temp_file_name)
+            base_source_dir_path = Path(tempfile.mkdtemp())
+            Parser().run(Path(base_temp_file_name), base_source_dir_path)
+            Path(base_temp_file_name).unlink()
         else:
             base_is_excluded = True
 
         # mine
         mine_is_excluded = False
         if yname:
-            if self.name_format == 'tortoisegit':
-                yname_file_fullpath = Path(yname.split(':')[0])
+            if self.name_format == "tortoisegit":
+                yname_file_path = Path(yname.split(":")[0])
             else:
-                yname_file_fullpath = Path(yname.split(':')[0])
+                yname_file_path = Path(yname.split(":")[0])
         else:
-            yname_file_fullpath = Path.cwd()
-        mine_source_dir_fullpath = None
-        if yname_file_fullpath.name not in self.exclude_file_names:
-            mine_file_fullpath_suffix = mine_file_fullpath.suffix
-            mine_temp_file, mine_temp_file_fullname = tempfile.mkstemp(mine_file_fullpath_suffix)
+            yname_file_path = Path.cwd()
+        mine_source_dir_path = None
+        if yname_file_path.name not in self.exclude_file_names:
+            mine_file_path_suffix = mine_file_path.suffix
+            mine_temp_file, mine_temp_file_name = tempfile.mkstemp(
+                mine_file_path_suffix
+            )
             os.close(mine_temp_file)
-            shutil.copyfile(str(mine_file_fullpath), mine_temp_file_fullname)
-            mine_source_dir_fullpath = Path(tempfile.mkdtemp())
-            Parser().run(Path(mine_temp_file_fullname), mine_source_dir_fullpath)
-            Path(mine_temp_file_fullname).unlink()
+            shutil.copyfile(str(mine_file_path), mine_temp_file_name)
+            mine_source_dir_path = Path(tempfile.mkdtemp())
+            Parser().run(Path(mine_temp_file_name), mine_source_dir_path)
+            Path(mine_temp_file_name).unlink()
         else:
             mine_is_excluded = True
 
         tool_args = [str(self.tool_path)]
-        if self.tool == 'kdiff3':
+        if self.tool == "kdiff3":
             # base
             if base_is_excluded:
-                tool_args += ['--cs', 'EncodingForA=UTF-8', str(base_file_fullpath)]
+                tool_args += ["--cs", "EncodingForA=UTF-8", str(base_file_path)]
             else:
-                tool_args += ['--cs', 'EncodingForA=windows-1251', str(base_source_dir_fullpath)]
+                tool_args += [
+                    "--cs",
+                    "EncodingForA=windows-1251",
+                    str(base_source_dir_path),
+                ]
             if bname is not None:
-                tool_args += ['--L1', bname]
+                tool_args += ["--L1", bname]
 
             # mine
             if mine_is_excluded:
-                tool_args += ['--cs', 'EncodingForB=UTF-8', str(mine_file_fullpath)]
+                tool_args += ["--cs", "EncodingForB=UTF-8", str(mine_file_path)]
             else:
-                tool_args += ['--cs', 'EncodingForB=windows-1251', str(mine_source_dir_fullpath)]
+                tool_args += [
+                    "--cs",
+                    "EncodingForB=windows-1251",
+                    str(mine_source_dir_path),
+                ]
             if yname is not None:
-                tool_args += ['--L2', yname]
+                tool_args += ["--L2", yname]
         exit_code = subprocess.check_call(tool_args)
         if not exit_code == 0:
-            raise Exception(f'Diff files \'{base_file_fullpath}\' and \'{mine_file_fullpath}\' failed')
+            raise Exception(
+                f"Diff files '{base_file_path}' and '{mine_file_path}' failed"
+            )
 
 
 def run(args) -> None:
-    logger.enable('cjk_commons')
-    logger.enable('parse_1c_build')
+    logger.enable("cjk_commons")
+    logger.enable("parse_1c_build")
     logger.enable(__name__)
+
     try:
         processor = Processor(name_format=args.name_format, tool=args.tool)
 
-        base_file_fullpath = Path(args.base)
-        mine_file_fullpath = Path(args.mine)
+        base_file_path = Path(args.base)
+        mine_file_path = Path(args.mine)
         bname = args.bname
         yname = args.yname
 
-        processor.run(base_file_fullpath, mine_file_fullpath, bname, yname)
+        processor.run(base_file_path, mine_file_path, bname, yname)
     except Exception as e:
         logger.exception(e)
         sys.exit(1)
```

### Comparing `diff-1c-6.6.5/src/diff_1c.egg-info/PKG-INFO` & `diff-1c-6.6.6/src/diff_1c.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diff-1c
-Version: 6.6.5
+Version: 6.6.6
 Summary: Diff utility for 1C:Enterprise
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/diff-1c
 Keywords: 1c,diff,v8reader,v8unpack,gcomp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

