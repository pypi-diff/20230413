# Comparing `tmp/dr-lord-of-the-rings-sdk-0.0.1.tar.gz` & `tmp/dr-lord-of-the-rings-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-lord-of-the-rings-sdk-0.0.1.tar", last modified: Wed Apr 12 23:25:39 2023, max compression
+gzip compressed data, was "dr-lord-of-the-rings-sdk-0.0.2.tar", last modified: Wed Apr 12 23:28:14 2023, max compression
```

## Comparing `dr-lord-of-the-rings-sdk-0.0.1.tar` & `dr-lord-of-the-rings-sdk-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:25:39.202636 dr-lord-of-the-rings-sdk-0.0.1/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-12 22:17:43.000000 dr-lord-of-the-rings-sdk-0.0.1/LICENCE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     4280 2023-04-12 23:25:39.202435 dr-lord-of-the-rings-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3369 2023-04-12 23:25:11.000000 dr-lord-of-the-rings-sdk-0.0.1/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:25:39.199188 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     4280 2023-04-12 23:25:39.000000 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      401 2023-04-12 23:25:39.000000 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-12 23:25:39.000000 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-12 23:25:39.000000 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       15 2023-04-12 23:25:39.000000 dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:25:39.200518 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-12 18:49:04.000000 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1728 2023-04-12 22:16:55.000000 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/api_methods.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-12 18:31:50.000000 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/conf.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2454 2023-04-12 23:21:44.000000 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/movies.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1609 2023-04-12 23:17:22.000000 dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/quotes.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-12 23:25:39.202687 dr-lord-of-the-rings-sdk-0.0.1/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1168 2023-04-12 22:32:50.000000 dr-lord-of-the-rings-sdk-0.0.1/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:25:39.201037 dr-lord-of-the-rings-sdk-0.0.1/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-12 18:48:52.000000 dr-lord-of-the-rings-sdk-0.0.1/tests/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2516 2023-04-12 23:20:09.000000 dr-lord-of-the-rings-sdk-0.0.1/tests/test.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:28:14.685991 dr-lord-of-the-rings-sdk-0.0.2/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-12 22:17:43.000000 dr-lord-of-the-rings-sdk-0.0.2/LICENCE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     4279 2023-04-12 23:28:14.685727 dr-lord-of-the-rings-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3368 2023-04-12 23:27:17.000000 dr-lord-of-the-rings-sdk-0.0.2/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:28:14.682210 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     4279 2023-04-12 23:28:14.000000 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      401 2023-04-12 23:28:14.000000 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-12 23:28:14.000000 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-12 23:28:14.000000 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       15 2023-04-12 23:28:14.000000 dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:28:14.683588 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-12 18:49:04.000000 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1728 2023-04-12 22:16:55.000000 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/api_methods.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-12 18:31:50.000000 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/conf.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2454 2023-04-12 23:21:44.000000 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/movies.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1609 2023-04-12 23:17:22.000000 dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/quotes.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-12 23:28:14.686041 dr-lord-of-the-rings-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1168 2023-04-12 23:27:45.000000 dr-lord-of-the-rings-sdk-0.0.2/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-12 23:28:14.684103 dr-lord-of-the-rings-sdk-0.0.2/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-12 18:48:52.000000 dr-lord-of-the-rings-sdk-0.0.2/tests/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2516 2023-04-12 23:20:09.000000 dr-lord-of-the-rings-sdk-0.0.2/tests/test.py
```

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/LICENCE.txt` & `dr-lord-of-the-rings-sdk-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/PKG-INFO` & `dr-lord-of-the-rings-sdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-lord-of-the-rings-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python project using the following import statement:
 
 ```python
 from lotr_sdk.movies import Movie
-from lotr_ssdk.quotes import Quote
+from lotr_sdk.quotes import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
```

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/README.md` & `dr-lord-of-the-rings-sdk-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python project using the following import statement:
 
 ```python
 from lotr_sdk.movies import Movie
-from lotr_ssdk.quotes import Quote
+from lotr_sdk.quotes import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
```

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/dr_lord_of_the_rings_sdk.egg-info/PKG-INFO` & `dr-lord-of-the-rings-sdk-0.0.2/dr_lord_of_the_rings_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-lord-of-the-rings-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python project using the following import statement:
 
 ```python
 from lotr_sdk.movies import Movie
-from lotr_ssdk.quotes import Quote
+from lotr_sdk.quotes import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
```

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/api_methods.py` & `dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/api_methods.py`

 * *Files identical despite different names*

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/movies.py` & `dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/movies.py`

 * *Files identical despite different names*

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/lotr_sdk/quotes.py` & `dr-lord-of-the-rings-sdk-0.0.2/lotr_sdk/quotes.py`

 * *Files identical despite different names*

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/setup.py` & `dr-lord-of-the-rings-sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dr-lord-of-the-rings-sdk',
-    version='0.0.1',
+    version='0.0.2',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
     url='https://github.com/DannyBuffet/Lord-of-the-rings-sdk',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
```

### Comparing `dr-lord-of-the-rings-sdk-0.0.1/tests/test.py` & `dr-lord-of-the-rings-sdk-0.0.2/tests/test.py`

 * *Files identical despite different names*

