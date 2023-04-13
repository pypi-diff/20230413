# Comparing `tmp/CustomGPT-0.1.6.tar.gz` & `tmp/CustomGPT-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomGPT-0.1.6.tar", last modified: Thu Apr 13 15:32:41 2023, max compression
+gzip compressed data, was "CustomGPT-1.0.0.tar", last modified: Thu Apr 13 15:41:11 2023, max compression
```

## Comparing `CustomGPT-0.1.6.tar` & `CustomGPT-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.776317 CustomGPT-0.1.6/
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.775127 CustomGPT-0.1.6/CustomGPT/
--rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-13 15:21:03.000000 CustomGPT-0.1.6/CustomGPT/__init__.py
--rw-r--r--   0 lymengnaret   (501) staff       (20)     5241 2023-04-13 15:29:59.000000 CustomGPT-0.1.6/CustomGPT/custom_gpt.py
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.775951 CustomGPT-0.1.6/CustomGPT.egg-info/
--rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      236 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/SOURCES.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/dependency_links.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/requires.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       10 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/top_level.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-11 20:33:34.000000 CustomGPT-0.1.6/LICENSE
--rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:32:41.776190 CustomGPT-0.1.6/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)     1029 2023-04-13 15:26:03.000000 CustomGPT-0.1.6/README.md
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:32:41.776362 CustomGPT-0.1.6/setup.cfg
--rw-r--r--   0 lymengnaret   (501) staff       (20)      942 2023-04-13 15:30:29.000000 CustomGPT-0.1.6/setup.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:41:11.894611 CustomGPT-1.0.0/
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:41:11.892967 CustomGPT-1.0.0/CustomGPT/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-13 15:21:03.000000 CustomGPT-1.0.0/CustomGPT/__init__.py
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     5241 2023-04-13 15:29:59.000000 CustomGPT-1.0.0/CustomGPT/custom_gpt.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:41:11.894032 CustomGPT-1.0.0/CustomGPT.egg-info/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:41:11.000000 CustomGPT-1.0.0/CustomGPT.egg-info/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      236 2023-04-13 15:41:11.000000 CustomGPT-1.0.0/CustomGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-13 15:41:11.000000 CustomGPT-1.0.0/CustomGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:41:11.000000 CustomGPT-1.0.0/CustomGPT.egg-info/requires.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       10 2023-04-13 15:41:11.000000 CustomGPT-1.0.0/CustomGPT.egg-info/top_level.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-11 20:33:34.000000 CustomGPT-1.0.0/LICENSE
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:41:11.894232 CustomGPT-1.0.0/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1370 2023-04-13 15:40:42.000000 CustomGPT-1.0.0/README.md
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:41:11.894652 CustomGPT-1.0.0/setup.cfg
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      942 2023-04-13 15:40:47.000000 CustomGPT-1.0.0/setup.py
```

### Comparing `CustomGPT-0.1.6/CustomGPT/custom_gpt.py` & `CustomGPT-1.0.0/CustomGPT/custom_gpt.py`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.6/CustomGPT.egg-info/PKG-INFO` & `CustomGPT-1.0.0/CustomGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.6
+Version: 1.0.0
 Summary: A package for interacting with GPT-4 models (and older) without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.6/LICENSE` & `CustomGPT-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.6/PKG-INFO` & `CustomGPT-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.6
+Version: 1.0.0
 Summary: A package for interacting with GPT-4 models (and older) without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CustomGPT-0.1.6/setup.py` & `CustomGPT-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="CustomGPT",
-    version="0.1.6",
+    version="1.0.0",
     description="A package for interacting with GPT-4 models (and older) without using the OpenAI API.",
     author="Lymeng Naret",
     author_email="lymengnaret@yahoo.com",
     url="https://github.com/NLmeng/CustomGPT",
     packages=find_packages(),
     install_requires=[
         "requests==2.28.2",
```

