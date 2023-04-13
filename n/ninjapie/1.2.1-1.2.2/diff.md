# Comparing `tmp/ninjapie-1.2.1.tar.gz` & `tmp/ninjapie-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.2.1.tar", last modified: Tue Apr 11 17:16:00 2023, max compression
+gzip compressed data, was "ninjapie-1.2.2.tar", last modified: Thu Apr 13 14:59:07 2023, max compression
```

## Comparing `ninjapie-1.2.1.tar` & `ninjapie-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.2.1/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 17:16:00.393218 ninjapie-1.2.1/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6330 2023-04-10 08:16:09.000000 ninjapie-1.2.1/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:43:40.000000 ninjapie-1.2.1/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5087 2023-04-11 17:15:38.000000 ninjapie-1.2.1/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    28191 2023-04-10 16:28:24.000000 ninjapie-1.2.1/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19502 2023-04-11 07:40:23.000000 ninjapie-1.2.1/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.2.1/ninjapie/path.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-11 17:15:52.000000 ninjapie-1.2.1/ninjapie/version.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       29 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-11 17:15:52.000000 ninjapie-1.2.1/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-11 17:16:00.393218 ninjapie-1.2.1/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-13 14:59:07.776579 ninjapie-1.2.2/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.2.2/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-13 14:59:07.776579 ninjapie-1.2.2/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6330 2023-04-10 08:16:09.000000 ninjapie-1.2.2/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-13 14:59:07.773246 ninjapie-1.2.2/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:43:40.000000 ninjapie-1.2.2/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5087 2023-04-11 17:15:38.000000 ninjapie-1.2.2/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    28431 2023-04-13 14:58:49.000000 ninjapie-1.2.2/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19502 2023-04-11 07:40:23.000000 ninjapie-1.2.2/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.2.2/ninjapie/path.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-13 14:58:58.000000 ninjapie-1.2.2/ninjapie/version.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-13 14:59:07.776579 ninjapie-1.2.2/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-13 14:59:07.000000 ninjapie-1.2.2/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-13 14:59:07.000000 ninjapie-1.2.2/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-13 14:59:07.000000 ninjapie-1.2.2/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-13 14:59:07.000000 ninjapie-1.2.2/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       20 2023-04-13 14:59:07.000000 ninjapie-1.2.2/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-13 14:58:58.000000 ninjapie-1.2.2/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-13 14:59:07.776579 ninjapie-1.2.2/setup.cfg
```

### Comparing `ninjapie-1.2.1/LICENSE` & `ninjapie-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.1/PKG-INFO` & `ninjapie-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.2.1/README.md` & `ninjapie-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.1/ninjapie/__main__.py` & `ninjapie-1.2.2/ninjapie/__main__.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.1/ninjapie/env.py` & `ninjapie-1.2.2/ninjapie/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 from glob import glob
-import importlib
+import importlib.util
 import os
+import sys
 
 from ninjapie.path import BuildPath, SourcePath
 from ninjapie.generator import BuildEdge, Generator
 
 
 class Env:
     """
@@ -256,16 +257,22 @@
         """
 
         old_cwd = self.cur_dir
         self._cwd.path += '/' + dir
 
         gen._add_build_file(self.cur_dir + '/build.py')
 
+        # import module
         mod_path = self.cur_dir[2:].replace('/', '.')
-        sub = importlib.import_module(mod_path + '.build')
+        spec = importlib.util.spec_from_file_location(mod_path, self.cur_dir + '/build.py')
+        sub = importlib.util.module_from_spec(spec)
+        sys.modules[spec.name] = sub
+        spec.loader.exec_module(sub)
+
+        # call build function in module
         res = sub.build(gen, self)
 
         self._cwd.path = old_cwd
         return res
 
     def glob(self, gen: Generator, pattern: str) -> list[SourcePath]:
         """
```

### Comparing `ninjapie-1.2.1/ninjapie/generator.py` & `ninjapie-1.2.2/ninjapie/generator.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.1/ninjapie/path.py` & `ninjapie-1.2.2/ninjapie/path.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.1/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.2.2/ninjapie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.2.1/pyproject.toml` & `ninjapie-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.2.1"
+version = "1.2.2"
 description = "Ninja-based build system with a Python API"
 readme = "README.md"
 authors = [{ name = "Nils Asmussen", email = "nils.asmussen@barkhauseninstitut.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -30,15 +30,15 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["coverage*", "tests*"]
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

