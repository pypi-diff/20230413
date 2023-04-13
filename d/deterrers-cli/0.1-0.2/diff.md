# Comparing `tmp/deterrers-cli-0.1.tar.gz` & `tmp/deterrers-cli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-cli-0.1.tar", last modified: Thu Apr 13 21:53:55 2023, max compression
+gzip compressed data, was "deterrers-cli-0.2.tar", last modified: Thu Apr 13 21:56:09 2023, max compression
```

## Comparing `deterrers-cli-0.1.tar` & `deterrers-cli-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:53:55.980478 deterrers-cli-0.1/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.1/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.1/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:53:55.980478 deterrers-cli-0.1/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     1756 2023-04-13 21:53:30.000000 deterrers-cli-0.1/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:53:55.980478 deterrers-cli-0.1/deterrers_cli.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       26 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 21:53:55.000000 deterrers-cli-0.1/deterrers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:53:55.980478 deterrers-cli-0.1/deterrerscli/
--rw-r--r--   0 lars      (1000) lars      (1000)     2272 2023-04-13 21:39:15.000000 deterrers-cli-0.1/deterrerscli/__main__.py
--rw-r--r--   0 lars      (1000) lars      (1000)       26 2023-04-13 21:08:53.000000 deterrers-cli-0.1/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 21:53:55.980478 deterrers-cli-0.1/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-13 21:22:29.000000 deterrers-cli-0.1/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.573636 deterrers-cli-0.2/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.2/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.2/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:56:09.572636 deterrers-cli-0.2/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     1756 2023-04-13 21:53:30.000000 deterrers-cli-0.2/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.572636 deterrers-cli-0.2/deterrers_cli.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       27 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.572636 deterrers-cli-0.2/deterrerscli/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2272 2023-04-13 21:39:15.000000 deterrers-cli-0.2/deterrerscli/__main__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       27 2023-04-13 21:55:40.000000 deterrers-cli-0.2/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 21:56:09.573636 deterrers-cli-0.2/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-13 21:56:01.000000 deterrers-cli-0.2/setup.py
```

### Comparing `deterrers-cli-0.1/LICENSE` & `deterrers-cli-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.1/PKG-INFO` & `deterrers-cli-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.1
+Version: 0.2
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.1/README.md` & `deterrers-cli-0.2/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.1/deterrers_cli.egg-info/PKG-INFO` & `deterrers-cli-0.2/deterrers_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.1
+Version: 0.2
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.1/deterrerscli/__main__.py` & `deterrers-cli-0.2/deterrerscli/__main__.py`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.1/setup.py` & `deterrers-cli-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-cli',
-    version='0.1',
+    version='0.2',
     description='Command line client for DETERRERS',
     url='https://github.com/virtUOS/proteuscmd',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrerscli'],
     license_files=('LICENSE'),
```

