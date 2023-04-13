# Comparing `tmp/test_query_tool-0.3.4.tar.gz` & `tmp/test_query_tool-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_query_tool-0.3.4.tar", last modified: Thu Apr 13 18:13:05 2023, max compression
+gzip compressed data, was "test_query_tool-0.3.5.tar", last modified: Thu Apr 13 18:16:38 2023, max compression
```

## Comparing `test_query_tool-0.3.4.tar` & `test_query_tool-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.106164 test_query_tool-0.3.4/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.4/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.4/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:13:05.105639 test_query_tool-0.3.4/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.087763 test_query_tool-0.3.4/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3588 2023-04-13 18:04:49.000000 test_query_tool-0.3.4/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.085357 test_query_tool-0.3.4/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.088705 test_query_tool-0.3.4/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.091639 test_query_tool-0.3.4/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044761 2023-04-13 18:12:35.000000 test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-49ab9bc7.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 18:12:35.000000 test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 18:12:47.000000 test_query_tool-0.3.4/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 18:12:34.000000 test_query_tool-0.3.4/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.101921 test_query_tool-0.3.4/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 18:13:05.106359 test_query_tool-0.3.4/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 18:11:47.000000 test_query_tool-0.3.4/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.105065 test_query_tool-0.3.4/test_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.990313 test_query_tool-0.3.5/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.5/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.5/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:16:38.989904 test_query_tool-0.3.5/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.981346 test_query_tool-0.3.5/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 test_query_tool-0.3.5/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.979752 test_query_tool-0.3.5/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.982145 test_query_tool-0.3.5/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.985141 test_query_tool-0.3.5/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044761 2023-04-13 18:12:35.000000 test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-49ab9bc7.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 18:12:35.000000 test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 18:12:47.000000 test_query_tool-0.3.5/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 18:12:34.000000 test_query_tool-0.3.5/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.987593 test_query_tool-0.3.5/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 18:16:38.990422 test_query_tool-0.3.5/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 18:16:12.000000 test_query_tool-0.3.5/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.989400 test_query_tool-0.3.5/test_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/top_level.txt
```

### Comparing `test_query_tool-0.3.4/LICENSE` & `test_query_tool-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/__init__.py` & `test_query_tool-0.3.5/query_tool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     set_component_rerender_count,
 )
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 init()
```

### Comparing `test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-49ab9bc7.js` & `test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-49ab9bc7.js`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/frontend/dist/vite.svg` & `test_query_tool-0.3.5/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/services/dimension_service.py` & `test_query_tool-0.3.5/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/services/entities_service.py` & `test_query_tool-0.3.5/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/services/filters_service.py` & `test_query_tool-0.3.5/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/services/query_tool_service.py` & `test_query_tool-0.3.5/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/query_tool/services/register.py` & `test_query_tool-0.3.5/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.4/setup.py` & `test_query_tool-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_query_tool",
-    version="0.3.4",
+    version="0.3.5",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `test_query_tool-0.3.4/test_query_tool.egg-info/SOURCES.txt` & `test_query_tool-0.3.5/test_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

