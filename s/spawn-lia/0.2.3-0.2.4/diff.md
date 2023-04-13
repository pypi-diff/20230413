# Comparing `tmp/spawn-lia-0.2.3.tar.gz` & `tmp/spawn-lia-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.3.tar", last modified: Wed Apr 12 17:14:13 2023, max compression
+gzip compressed data, was "spawn-lia-0.2.4.tar", last modified: Thu Apr 13 17:56:08 2023, max compression
```

## Comparing `spawn-lia-0.2.3.tar` & `spawn-lia-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.3/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/check_git/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/check_git/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/check_git/verify_branch.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 20:03:31.000000 spawn-lia-0.2.3/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1003 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      104 2023-04-08 09:57:30.000000 spawn-lia-0.2.3/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      873 2023-04-08 10:05:19.000000 spawn-lia-0.2.3/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      394 2023-04-08 10:16:41.000000 spawn-lia-0.2.3/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1026 2023-04-08 10:18:13.000000 spawn-lia-0.2.3/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2236 2023-04-12 17:13:06.000000 spawn-lia-0.2.3/lia/conversation/virtualenv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      542 2023-04-12 17:07:04.000000 spawn-lia-0.2.3/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:56:24.000000 spawn-lia-0.2.3/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1774 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/simplify/verify_package.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-12 17:14:03.000000 spawn-lia-0.2.3/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      699 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.3/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     3841 2023-04-07 19:00:56.000000 spawn-lia-0.2.3/tests/test_git_check.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.3/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      772 2023-04-08 10:13:59.000000 spawn-lia-0.2.3/tests/test_venv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-13 17:56:00.000000 spawn-lia-0.2.4/LICENSE.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.4/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.786537 spawn-lia-0.2.4/lia/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.4/lia/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/lia/bounty/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 17:54:43.000000 spawn-lia-0.2.4/lia/bounty/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4815 2023-04-13 17:56:00.000000 spawn-lia-0.2.4/lia/bounty/heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      553 2023-04-12 17:13:31.000000 spawn-lia-0.2.4/lia/bounty/testing.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/lia/check_git/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.4/lia/check_git/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-13 17:56:00.000000 spawn-lia-0.2.4/lia/check_git/verify_branch.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/lia/conversation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 20:03:31.000000 spawn-lia-0.2.4/lia/conversation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1003 2023-04-13 17:56:00.000000 spawn-lia-0.2.4/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      104 2023-04-08 09:57:30.000000 spawn-lia-0.2.4/lia/conversation/decision.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      873 2023-04-08 10:05:19.000000 spawn-lia-0.2.4/lia/conversation/emojis.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      394 2023-04-08 10:16:41.000000 spawn-lia-0.2.4/lia/conversation/end_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1026 2023-04-08 10:18:13.000000 spawn-lia-0.2.4/lia/conversation/start_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2236 2023-04-12 17:13:06.000000 spawn-lia-0.2.4/lia/conversation/virtualenv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      542 2023-04-12 17:07:04.000000 spawn-lia-0.2.4/lia/main.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/lia/simplify/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:56:24.000000 spawn-lia-0.2.4/lia/simplify/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1774 2023-04-13 17:56:00.000000 spawn-lia-0.2.4/lia/simplify/create_venv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-03 18:48:44.000000 spawn-lia-0.2.4/lia/simplify/verify_package.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/lia/support/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 17:55:51.000000 spawn-lia-0.2.4/lia/support/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1256 2023-04-12 17:02:43.000000 spawn-lia-0.2.4/lia/support/deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/spawn_lia.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      809 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-13 17:56:08.000000 spawn-lia-0.2.4/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 17:56:08.789870 spawn-lia-0.2.4/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.4/tests/test_deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     3841 2023-04-07 19:00:56.000000 spawn-lia-0.2.4/tests/test_git_check.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.4/tests/test_heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      772 2023-04-08 10:13:59.000000 spawn-lia-0.2.4/tests/test_venv.py
```

### Comparing `spawn-lia-0.2.3/LICENSE.txt` & `spawn-lia-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/PKG-INFO` & `spawn-lia-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.3
+Version: 0.2.4
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.3/README.md` & `spawn-lia-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/check_git/verify_branch.py` & `spawn-lia-0.2.4/lia/check_git/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.2.4/lia/conversation/ask_to_proceed.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/conversation/emojis.py` & `spawn-lia-0.2.4/lia/conversation/emojis.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/conversation/start_message.py` & `spawn-lia-0.2.4/lia/conversation/start_message.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/conversation/virtualenv.py` & `spawn-lia-0.2.4/lia/conversation/virtualenv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/main.py` & `spawn-lia-0.2.4/lia/main.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/lia/simplify/create_venv.py` & `spawn-lia-0.2.4/lia/simplify/create_venv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/setup.py` & `spawn-lia-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.3/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.2.4/spawn_lia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.3
+Version: 0.2.4
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.3/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.2.4/spawn_lia.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE.txt
 README.md
 setup.py
 lia/__init__.py
 lia/main.py
+lia/bounty/__init__.py
+lia/bounty/heal.py
+lia/bounty/testing.py
 lia/check_git/__init__.py
 lia/check_git/verify_branch.py
 lia/conversation/__init__.py
 lia/conversation/ask_to_proceed.py
 lia/conversation/decision.py
 lia/conversation/emojis.py
 lia/conversation/end_message.py
 lia/conversation/start_message.py
 lia/conversation/virtualenv.py
 lia/simplify/__init__.py
 lia/simplify/create_venv.py
 lia/simplify/verify_package.py
+lia/support/__init__.py
+lia/support/deploy.py
 spawn_lia.egg-info/PKG-INFO
 spawn_lia.egg-info/SOURCES.txt
 spawn_lia.egg-info/dependency_links.txt
 spawn_lia.egg-info/entry_points.txt
 spawn_lia.egg-info/requires.txt
 spawn_lia.egg-info/top_level.txt
 tests/test_deploy.py
```

### Comparing `spawn-lia-0.2.3/tests/test_deploy.py` & `spawn-lia-0.2.4/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/tests/test_git_check.py` & `spawn-lia-0.2.4/tests/test_git_check.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/tests/test_heal.py` & `spawn-lia-0.2.4/tests/test_heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.3/tests/test_venv.py` & `spawn-lia-0.2.4/tests/test_venv.py`

 * *Files identical despite different names*

