# Comparing `tmp/test_query_tool-0.3.1.tar.gz` & `tmp/test_query_tool-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_query_tool-0.3.1.tar", last modified: Thu Apr 13 12:08:32 2023, max compression
+gzip compressed data, was "test_query_tool-0.3.2.tar", last modified: Thu Apr 13 12:11:16 2023, max compression
```

## Comparing `test_query_tool-0.3.1.tar` & `test_query_tool-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.798216 test_query_tool-0.3.1/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.1/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.1/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:08:32.797803 test_query_tool-0.3.1/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.788468 test_query_tool-0.3.1/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3373 2023-04-13 10:28:20.000000 test_query_tool-0.3.1/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.786528 test_query_tool-0.3.1/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.789131 test_query_tool-0.3.1/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.789799 test_query_tool-0.3.1/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 12:07:36.000000 test_query_tool-0.3.1/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044760 2023-04-13 12:07:36.000000 test_query_tool-0.3.1/query_tool/frontend/dist/assets/index-d72f7278.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 12:07:46.000000 test_query_tool-0.3.1/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 12:07:36.000000 test_query_tool-0.3.1/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.794705 test_query_tool-0.3.1/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.1/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 12:08:32.798367 test_query_tool-0.3.1/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 12:07:52.000000 test_query_tool-0.3.1/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:08:32.797263 test_query_tool-0.3.1/test_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:08:32.000000 test_query_tool-0.3.1/test_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 12:08:32.000000 test_query_tool-0.3.1/test_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 12:08:32.000000 test_query_tool-0.3.1/test_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 12:08:32.000000 test_query_tool-0.3.1/test_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 12:08:32.000000 test_query_tool-0.3.1/test_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.553927 test_query_tool-0.3.2/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.2/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.2/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:11:16.553588 test_query_tool-0.3.2/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.545387 test_query_tool-0.3.2/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3373 2023-04-13 12:10:48.000000 test_query_tool-0.3.2/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.543573 test_query_tool-0.3.2/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.546048 test_query_tool-0.3.2/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.546839 test_query_tool-0.3.2/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 12:07:36.000000 test_query_tool-0.3.2/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044760 2023-04-13 12:07:36.000000 test_query_tool-0.3.2/query_tool/frontend/dist/assets/index-d72f7278.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 12:07:46.000000 test_query_tool-0.3.2/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 12:07:36.000000 test_query_tool-0.3.2/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.551386 test_query_tool-0.3.2/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.2/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 12:11:16.554049 test_query_tool-0.3.2/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 12:10:56.000000 test_query_tool-0.3.2/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:11:16.553080 test_query_tool-0.3.2/test_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:11:16.000000 test_query_tool-0.3.2/test_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 12:11:16.000000 test_query_tool-0.3.2/test_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 12:11:16.000000 test_query_tool-0.3.2/test_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 12:11:16.000000 test_query_tool-0.3.2/test_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 12:11:16.000000 test_query_tool-0.3.2/test_query_tool.egg-info/top_level.txt
```

### Comparing `test_query_tool-0.3.1/LICENSE` & `test_query_tool-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/__init__.py` & `test_query_tool-0.3.2/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/frontend/dist/assets/index-d72f7278.js` & `test_query_tool-0.3.2/query_tool/frontend/dist/assets/index-d72f7278.js`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/frontend/dist/vite.svg` & `test_query_tool-0.3.2/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/services/dimension_service.py` & `test_query_tool-0.3.2/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/services/entities_service.py` & `test_query_tool-0.3.2/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/services/filters_service.py` & `test_query_tool-0.3.2/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/services/query_tool_service.py` & `test_query_tool-0.3.2/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/query_tool/services/register.py` & `test_query_tool-0.3.2/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.1/setup.py` & `test_query_tool-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_query_tool",
-    version="0.3.1",
+    version="0.3.2",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `test_query_tool-0.3.1/test_query_tool.egg-info/SOURCES.txt` & `test_query_tool-0.3.2/test_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

