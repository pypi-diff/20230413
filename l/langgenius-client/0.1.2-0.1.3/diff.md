# Comparing `tmp/langgenius-client-0.1.2.tar.gz` & `tmp/langgenius-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgenius-client-0.1.2.tar", last modified: Thu Apr 13 08:16:22 2023, max compression
+gzip compressed data, was "langgenius-client-0.1.3.tar", last modified: Thu Apr 13 08:19:49 2023, max compression
```

## Comparing `langgenius-client-0.1.2.tar` & `langgenius-client-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:16:22.799156 langgenius-client-0.1.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1067 2023-04-13 06:24:04.000000 langgenius-client-0.1.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-04-13 07:19:22.000000 langgenius-client-0.1.2/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1661 2023-04-13 08:16:22.799156 langgenius-client-0.1.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1127 2023-04-13 06:41:49.000000 langgenius-client-0.1.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:16:22.791156 langgenius-client-0.1.2/langgenius/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2023-04-13 08:15:41.000000 langgenius-client-0.1.2/langgenius/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2675 2023-04-13 08:02:58.000000 langgenius-client-0.1.2/langgenius/client.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:16:22.795156 langgenius-client-0.1.2/langgenius_client.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1661 2023-04-13 08:16:22.000000 langgenius-client-0.1.2/langgenius_client.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      307 2023-04-13 08:16:22.000000 langgenius-client-0.1.2/langgenius_client.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-13 08:16:22.000000 langgenius-client-0.1.2/langgenius_client.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-13 08:16:22.000000 langgenius-client-0.1.2/langgenius_client.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-04-13 08:16:22.000000 langgenius-client-0.1.2/langgenius_client.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-13 08:16:22.799156 langgenius-client-0.1.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      847 2023-04-13 08:15:57.000000 langgenius-client-0.1.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:16:22.795156 langgenius-client-0.1.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1664 2023-04-13 07:20:55.000000 langgenius-client-0.1.2/tests/test_client.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:19:49.033522 langgenius-client-0.1.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1067 2023-04-13 06:24:04.000000 langgenius-client-0.1.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-04-13 08:18:39.000000 langgenius-client-0.1.3/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1661 2023-04-13 08:19:49.033522 langgenius-client-0.1.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1127 2023-04-13 06:41:49.000000 langgenius-client-0.1.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:19:49.029522 langgenius-client-0.1.3/langgenius_client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-13 08:19:31.000000 langgenius-client-0.1.3/langgenius_client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2675 2023-04-13 08:02:58.000000 langgenius-client-0.1.3/langgenius_client/client.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:19:49.033522 langgenius-client-0.1.3/langgenius_client.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1661 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/langgenius_client.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      321 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/langgenius_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/langgenius_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/langgenius_client.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/langgenius_client.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-13 08:19:49.033522 langgenius-client-0.1.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      854 2023-04-13 08:19:48.000000 langgenius-client-0.1.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-13 08:19:49.033522 langgenius-client-0.1.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1664 2023-04-13 07:20:55.000000 langgenius-client-0.1.3/tests/test_client.py
```

### Comparing `langgenius-client-0.1.2/LICENSE` & `langgenius-client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langgenius-client-0.1.2/PKG-INFO` & `langgenius-client-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgenius-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for interacting with the LangGenius Service-API
 Home-page: https://github.com/langgenius/langgenius-client
 Author: LangGenius
 Author-email: hello@langgenius.ai
 License: MIT
 Keywords: langgenius nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langgenius-client-0.1.2/README.md` & `langgenius-client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langgenius-client-0.1.2/langgenius/client.py` & `langgenius-client-0.1.3/langgenius_client/client.py`

 * *Files identical despite different names*

### Comparing `langgenius-client-0.1.2/langgenius_client.egg-info/PKG-INFO` & `langgenius-client-0.1.3/langgenius_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgenius-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for interacting with the LangGenius Service-API
 Home-page: https://github.com/langgenius/langgenius-client
 Author: LangGenius
 Author-email: hello@langgenius.ai
 License: MIT
 Keywords: langgenius nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langgenius-client-0.1.2/setup.py` & `langgenius-client-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="langgenius-client",
-    version="0.1.2",
+    version="0.1.3",
     author="LangGenius",
     author_email="hello@langgenius.ai",
     description="A package for interacting with the LangGenius Service-API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/langgenius/langgenius-client",
     license='MIT',
-    packages=['langgenius'],
+    packages=['langgenius_client'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
```

### Comparing `langgenius-client-0.1.2/tests/test_client.py` & `langgenius-client-0.1.3/tests/test_client.py`

 * *Files identical despite different names*

