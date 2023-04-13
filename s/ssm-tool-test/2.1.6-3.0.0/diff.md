# Comparing `tmp/ssm_tool_test-2.1.6.tar.gz` & `tmp/ssm_tool_test-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm_tool_test-2.1.6.tar", last modified: Wed Mar 22 17:35:13 2023, max compression
+gzip compressed data, was "ssm_tool_test-3.0.0.tar", last modified: Thu Apr 13 18:32:04 2023, max compression
```

## Comparing `ssm_tool_test-2.1.6.tar` & `ssm_tool_test-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1068 2023-03-06 16:20:43.000000 ssm_tool_test-2.1.6/LICENSE
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1291 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/PKG-INFO
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      754 2023-03-09 19:14:10.000000 ssm_tool_test-2.1.6/README.md
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      715 2023-03-09 16:38:43.000000 ssm_tool_test-2.1.6/pyproject.toml
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       38 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/setup.cfg
-drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/src/
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        5 2023-03-22 17:33:17.000000 ssm_tool_test-2.1.6/src/VERSION
-drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/src/ssm_tool_test/
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-06 16:03:31.000000 ssm_tool_test-2.1.6/src/ssm_tool_test/__init__.py
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     3615 2023-03-22 17:33:11.000000 ssm_tool_test-2.1.6/src/ssm_tool_test/ssm.py
-drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-22 17:35:13.265495 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1291 2023-03-22 17:35:13.000000 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/PKG-INFO
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      303 2023-03-22 17:35:13.000000 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/SOURCES.txt
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        1 2023-03-22 17:35:13.000000 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/dependency_links.txt
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       15 2023-03-22 17:35:13.000000 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/requires.txt
--rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       14 2023-03-22 17:35:13.000000 ssm_tool_test-2.1.6/src/ssm_tool_test.egg-info/top_level.txt
+drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1068 2023-03-06 16:20:43.000000 ssm_tool_test-3.0.0/LICENSE
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1164 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/PKG-INFO
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      627 2023-04-13 18:31:54.000000 ssm_tool_test-3.0.0/README.md
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      712 2023-04-13 18:31:29.000000 ssm_tool_test-3.0.0/pyproject.toml
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       38 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/setup.cfg
+drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/src/
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        5 2023-04-13 18:29:05.000000 ssm_tool_test-3.0.0/src/VERSION
+drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/src/ssm_tool_test/
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        0 2023-03-06 16:03:31.000000 ssm_tool_test-3.0.0/src/ssm_tool_test/__init__.py
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1264 2023-04-13 18:31:50.000000 ssm_tool_test-3.0.0/src/ssm_tool_test/ssm.py
+drwxrwxr-x   0 davidroldan  (1000) davidroldan  (1000)        0 2023-04-13 18:32:04.957627 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)     1164 2023-04-13 18:32:04.000000 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/PKG-INFO
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)      303 2023-04-13 18:32:04.000000 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)        1 2023-04-13 18:32:04.000000 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       12 2023-04-13 18:32:04.000000 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/requires.txt
+-rw-rw-r--   0 davidroldan  (1000) davidroldan  (1000)       14 2023-04-13 18:32:04.000000 ssm_tool_test-3.0.0/src/ssm_tool_test.egg-info/top_level.txt
```

### Comparing `ssm_tool_test-2.1.6/LICENSE` & `ssm_tool_test-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm_tool_test-2.1.6/pyproject.toml` & `ssm_tool_test-3.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools >= 66.1.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssm_tool_test"
 dynamic = ["version"]
 dependencies = [
-  "boto3==1.18.44"
+  "aiobotocore"
 ]
 authors = [
   { name="Roldan Author", email="jdroldan@playvox.com" },
 ]
 description = "A small example package to get ssm parameters from aws"
 readme = "README.md"
 requires-python = ">=3.7"
```

