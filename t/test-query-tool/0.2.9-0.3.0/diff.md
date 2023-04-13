# Comparing `tmp/test_query_tool-0.2.9.tar.gz` & `tmp/test_query_tool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_query_tool-0.2.9.tar", last modified: Thu Apr 13 09:52:21 2023, max compression
+gzip compressed data, was "test_query_tool-0.3.0.tar", last modified: Thu Apr 13 10:00:04 2023, max compression
```

## Comparing `test_query_tool-0.2.9.tar` & `test_query_tool-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.829266 test_query_tool-0.2.9/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.2.9/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.2.9/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 09:52:21.828988 test_query_tool-0.2.9/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.818754 test_query_tool-0.2.9/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3372 2023-04-06 08:45:04.000000 test_query_tool-0.2.9/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.816763 test_query_tool-0.2.9/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.819704 test_query_tool-0.2.9/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.821821 test_query_tool-0.2.9/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044680 2023-04-13 09:51:46.000000 test_query_tool-0.2.9/query_tool/frontend/dist/assets/index-b14312ff.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 09:51:46.000000 test_query_tool-0.2.9/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 09:52:04.000000 test_query_tool-0.2.9/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 09:51:45.000000 test_query_tool-0.2.9/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.826183 test_query_tool-0.2.9/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.2.9/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 09:52:21.829363 test_query_tool-0.2.9/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 09:52:14.000000 test_query_tool-0.2.9/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 09:52:21.828535 test_query_tool-0.2.9/test_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 09:52:21.000000 test_query_tool-0.2.9/test_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 09:52:21.000000 test_query_tool-0.2.9/test_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 09:52:21.000000 test_query_tool-0.2.9/test_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 09:52:21.000000 test_query_tool-0.2.9/test_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 09:52:21.000000 test_query_tool-0.2.9/test_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.198582 test_query_tool-0.3.0/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.0/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.0/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 10:00:04.198272 test_query_tool-0.3.0/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.168537 test_query_tool-0.3.0/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3372 2023-04-13 09:56:52.000000 test_query_tool-0.3.0/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.165787 test_query_tool-0.3.0/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.172602 test_query_tool-0.3.0/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.183610 test_query_tool-0.3.0/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044680 2023-04-13 09:55:21.000000 test_query_tool-0.3.0/query_tool/frontend/dist/assets/index-b14312ff.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 09:55:21.000000 test_query_tool-0.3.0/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 09:55:37.000000 test_query_tool-0.3.0/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 09:55:21.000000 test_query_tool-0.3.0/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.195230 test_query_tool-0.3.0/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.0/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 10:00:04.198687 test_query_tool-0.3.0/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 09:59:56.000000 test_query_tool-0.3.0/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 10:00:04.197699 test_query_tool-0.3.0/test_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 10:00:04.000000 test_query_tool-0.3.0/test_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 10:00:04.000000 test_query_tool-0.3.0/test_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 10:00:04.000000 test_query_tool-0.3.0/test_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 10:00:04.000000 test_query_tool-0.3.0/test_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 10:00:04.000000 test_query_tool-0.3.0/test_query_tool.egg-info/top_level.txt
```

### Comparing `test_query_tool-0.2.9/LICENSE` & `test_query_tool-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/__init__.py` & `test_query_tool-0.3.0/query_tool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/dist")
     __query_tool_component_function = components.declare_component(
         "query_tool", path=build_dir
     )
 else:
     __query_tool_component_function = components.declare_component(
-        "query_tool", url="http://localhost:4000"
+        "query_tool", url="http://localhost:4001"
     )
 
 
 def __query_builder(
     query=None,
     database_list=None,
     table_list=None,
```

### Comparing `test_query_tool-0.2.9/query_tool/frontend/dist/assets/index-b14312ff.js` & `test_query_tool-0.3.0/query_tool/frontend/dist/assets/index-b14312ff.js`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/frontend/dist/vite.svg` & `test_query_tool-0.3.0/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/services/dimension_service.py` & `test_query_tool-0.3.0/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/services/entities_service.py` & `test_query_tool-0.3.0/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/services/filters_service.py` & `test_query_tool-0.3.0/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/services/query_tool_service.py` & `test_query_tool-0.3.0/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/query_tool/services/register.py` & `test_query_tool-0.3.0/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.2.9/setup.py` & `test_query_tool-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_query_tool",
-    version="0.2.9",
+    version="0.3.0",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `test_query_tool-0.2.9/test_query_tool.egg-info/SOURCES.txt` & `test_query_tool-0.3.0/test_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

