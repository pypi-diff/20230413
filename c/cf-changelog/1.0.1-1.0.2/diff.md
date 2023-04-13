# Comparing `tmp/cf_changelog-1.0.1.tar.gz` & `tmp/cf_changelog-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-zzmm531o\cf_changelog-1.0.1.tar", last modified: Thu Apr 13 15:10:56 2023, max compression
+gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-byn3ctrf\cf_changelog-1.0.2.tar", last modified: Thu Apr 13 15:30:09 2023, max compression
```

## Comparing `cf_changelog-1.0.1.tar` & `cf_changelog-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1503 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.1/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-04-13 15:08:38.000000 cf_changelog-1.0.1/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0     1503 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-13 14:53:27.000000 cf_changelog-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog/
+-rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.2/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6601 2023-04-13 15:28:17.000000 cf_changelog-1.0.2/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:30:09.000000 cf_changelog-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-04-13 15:29:00.000000 cf_changelog-1.0.2/setup.py
```

### Comparing `cf_changelog-1.0.1/LICENSE` & `cf_changelog-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.1/PKG-INFO` & `cf_changelog-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_changelog
-Version: 1.0.1
+Version: 1.0.2
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.1/README.md` & `cf_changelog-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.1/cf_changelog/cf_changelog.py` & `cf_changelog-1.0.2/cf_changelog/cf_changelog.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse, os, tempfile, getpass, yaml
 from subprocess import call
 from datetime import datetime
 from schema import Schema, SchemaError
 import git
 from pathlib import Path
+from sys import platform
 
 config_schema = Schema({
     object: list,
     })
 
 def handle_add(args):
     initial_message = '''New:
@@ -102,15 +103,21 @@
     for source_file in source_files:
         full_source_path = Path(args.source_directory) / Path(source_file)
         full_archive_path = Path(target_archive_directory) / Path(source_file)
         print(f"Moving {full_source_path} to {full_archive_path}")
         g.mv(str(full_source_path), str(full_archive_path))
 
 
-EDITOR = os.environ.get('EDITOR', 'notepad')  # that easy!
+EDITOR = os.environ.get('EDITOR', None)  # that easy!
+if EDITOR is None:
+    if platform == "win32":
+        EDITOR = "notepad"
+    else:
+        EDITOR = "vim" # I Hate nano :-)
+
 
 def main():
     parser = argparse.ArgumentParser(description='Handles changelog entries without conflicts')
     parser.add_argument('--source_directory', type=str, nargs=1, 
                         help='directory where developers entries will be stored. You should keep it in the repository together with your code',
                         default="changelog/sources")
     parser.add_argument('--archive_directory', type=str, nargs=1,
```

### Comparing `cf_changelog-1.0.1/cf_changelog.egg-info/PKG-INFO` & `cf_changelog-1.0.2/cf_changelog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-changelog
-Version: 1.0.1
+Version: 1.0.2
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.1/setup.py` & `cf_changelog-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='cf_changelog',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='1.0.1',
+      version='1.0.2',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='https://gitlab.com/salekpawel/cf_changelog',
       packages=['cf_changelog', ],
       license="MIT",
       install_requires=[
```

