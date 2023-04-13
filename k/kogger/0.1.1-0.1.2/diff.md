# Comparing `tmp/kogger-0.1.1.tar.gz` & `tmp/kogger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kogger-0.1.1.tar", last modified: Wed Apr 12 07:33:06 2023, max compression
+gzip compressed data, was "kogger-0.1.2.tar", last modified: Thu Apr 13 09:57:58 2023, max compression
```

## Comparing `kogger-0.1.1.tar` & `kogger-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-12 07:33:06.826891 kogger-0.1.1/
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1068 2023-04-12 06:46:05.000000 kogger-0.1.1/LICENSE
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1437 2023-04-12 07:33:06.826891 kogger-0.1.1/PKG-INFO
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1024 2023-04-12 07:27:21.000000 kogger-0.1.1/README.md
-drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-12 07:33:06.826891 kogger-0.1.1/kogger/
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      399 2023-04-12 03:29:37.000000 kogger-0.1.1/kogger/__init__.py
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1183 2023-04-12 03:29:37.000000 kogger-0.1.1/kogger/logger.py
-drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-12 07:33:06.826891 kogger-0.1.1/kogger.egg-info/
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1437 2023-04-12 07:33:06.000000 kogger-0.1.1/kogger.egg-info/PKG-INFO
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      192 2023-04-12 07:33:06.000000 kogger-0.1.1/kogger.egg-info/SOURCES.txt
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)        1 2023-04-12 07:33:06.000000 kogger-0.1.1/kogger.egg-info/dependency_links.txt
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)        7 2023-04-12 07:33:06.000000 kogger-0.1.1/kogger.egg-info/top_level.txt
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)       79 2023-04-12 07:33:06.826891 kogger-0.1.1/setup.cfg
--rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      729 2023-04-12 07:30:25.000000 kogger-0.1.1/setup.py
+drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-13 09:57:58.372570 kogger-0.1.2/
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1068 2023-04-12 06:46:05.000000 kogger-0.1.2/LICENSE
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1437 2023-04-13 09:57:58.372570 kogger-0.1.2/PKG-INFO
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1024 2023-04-12 07:27:21.000000 kogger-0.1.2/README.md
+drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-13 09:57:58.372570 kogger-0.1.2/kogger/
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      399 2023-04-13 09:55:28.000000 kogger-0.1.2/kogger/__init__.py
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1183 2023-04-12 03:29:37.000000 kogger-0.1.2/kogger/logger.py
+drwxrwxr-x   0 bochengzeng  (1000) bochengzeng  (1000)        0 2023-04-13 09:57:58.372570 kogger-0.1.2/kogger.egg-info/
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)     1437 2023-04-13 09:57:58.000000 kogger-0.1.2/kogger.egg-info/PKG-INFO
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      192 2023-04-13 09:57:58.000000 kogger-0.1.2/kogger.egg-info/SOURCES.txt
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)        1 2023-04-13 09:57:58.000000 kogger-0.1.2/kogger.egg-info/dependency_links.txt
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)        7 2023-04-13 09:57:58.000000 kogger-0.1.2/kogger.egg-info/top_level.txt
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)       79 2023-04-13 09:57:58.372570 kogger-0.1.2/setup.cfg
+-rw-rw-r--   0 bochengzeng  (1000) bochengzeng  (1000)      729 2023-04-13 09:57:03.000000 kogger-0.1.2/setup.py
```

### Comparing `kogger-0.1.1/LICENSE` & `kogger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kogger-0.1.1/PKG-INFO` & `kogger-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kogger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A very simple logger.
 Home-page: https://github.com/zengbocheng/kogger.git
 Author: bochengz
 Author-email: bochengzeng@bochengz.top
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kogger-0.1.1/README.md` & `kogger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kogger-0.1.1/kogger/logger.py` & `kogger-0.1.2/kogger/logger.py`

 * *Files identical despite different names*

### Comparing `kogger-0.1.1/kogger.egg-info/PKG-INFO` & `kogger-0.1.2/kogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kogger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A very simple logger.
 Home-page: https://github.com/zengbocheng/kogger.git
 Author: bochengz
 Author-email: bochengzeng@bochengz.top
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kogger-0.1.1/setup.py` & `kogger-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kogger",
-    version="0.1.1",
+    version="0.1.2",
     license='MIT',
     author="bochengz",
     author_email="bochengzeng@bochengz.top",
     description="A very simple logger.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zengbocheng/kogger.git",
```

