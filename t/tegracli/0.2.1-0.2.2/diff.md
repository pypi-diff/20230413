# Comparing `tmp/tegracli-0.2.1.tar.gz` & `tmp/tegracli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.2.1.tar", max compression
+gzip compressed data, was "tegracli-0.2.2.tar", max compression
```

## Comparing `tegracli-0.2.1.tar` & `tegracli-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.1/LICENSE
--rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.1/README.md
--rw-r--r--   0        0        0     1322 2023-04-12 16:01:08.273768 tegracli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.1/tegracli/__init__.py
--rw-r--r--   0        0        0     5336 2023-04-12 16:01:00.081752 tegracli-0.2.1/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.1/tegracli/group.py
--rw-r--r--   0        0        0    12732 2023-04-12 16:01:00.081752 tegracli-0.2.1/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.1/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.1/tegracli/utilities.py
--rw-r--r--   0        0        0     9481 1970-01-01 00:00:00.000000 tegracli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.2/README.md
+-rw-r--r--   0        0        0     1322 2023-04-13 10:33:29.655155 tegracli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.2/tegracli/__init__.py
+-rw-r--r--   0        0        0     5336 2023-04-12 16:01:00.081752 tegracli-0.2.2/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.2/tegracli/group.py
+-rw-r--r--   0        0        0    12773 2023-04-13 10:33:21.255171 tegracli-0.2.2/tegracli/main.py
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.2/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.2/tegracli/utilities.py
+-rw-r--r--   0        0        0     9568 2023-04-13 10:34:10.375085 tegracli-0.2.2/setup.py
+-rw-r--r--   0        0        0     9430 2023-04-13 10:34:10.375756 tegracli-0.2.2/PKG-INFO
```

### Comparing `tegracli-0.2.1/LICENSE` & `tegracli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.1/README.md` & `tegracli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.1/pyproject.toml` & `tegracli-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tegracli"
-version = "0.2.1"
+version = "0.2.2"
 description = "A research-focused Telegram CLI application"
 authors = ["Philipp Kessling <p.kessling@leibniz-hbi.de>", "Felix Münch <f.muench@lebniz-hbi.de>"]
 readme  = "README.md"
 license = "MIT"
 repository  = "https://github.com/Leibniz-HBI/tegracli"
 homepage = "https://pypi.org/project/tegracli/"
 classifiers = [
```

### Comparing `tegracli-0.2.1/tegracli/dispatch.py` & `tegracli-0.2.2/tegracli/dispatch.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.1/tegracli/group.py` & `tegracli-0.2.2/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.1/tegracli/main.py` & `tegracli-0.2.2/tegracli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,17 @@
 
 
 @group.command()
 @click.argument("groups", nargs=-1)
 @click.pass_context
 def run(ctx: click.Context, groups: Tuple[str]):
     """Load a group configuration and run the groups operations."""
-    run_group(ctx.obj["client"], groups)
+    client = ctx.obj["client"]
+    with client:
+        run_group(client, groups)
 
 
 def _handle_group_member(member: str, conf: Group, client: TelegramClient) -> None:
     # check whether member is known already and, thus, present in profiles.jsonl
     # if (yes
     #   load user object
     profile = conf.get_member_profile(member)
```

### Comparing `tegracli-0.2.1/tegracli/utilities.py` & `tegracli-0.2.2/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.1/PKG-INFO` & `tegracli-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: tegracli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A research-focused Telegram CLI application
 Home-page: https://pypi.org/project/tegracli/
 License: MIT
 Author: Philipp Kessling
 Author-email: p.kessling@leibniz-hbi.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: Telethon (>=1.24.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: ujson (>=5.4.0,<6.0.0)
 Project-URL: Repository, https://github.com/Leibniz-HBI/tegracli
```

