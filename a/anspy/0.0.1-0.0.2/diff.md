# Comparing `tmp/anspy-0.0.1.tar.gz` & `tmp/anspy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anspy-0.0.1.tar", last modified: Thu Apr 13 15:04:01 2023, max compression
+gzip compressed data, was "anspy-0.0.2.tar", last modified: Thu Apr 13 15:37:36 2023, max compression
```

## Comparing `anspy-0.0.1.tar` & `anspy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:04:01.752002 anspy-0.0.1/
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1247 2023-04-13 15:04:01.751830 anspy-0.0.1/PKG-INFO
--rw-r--r--   0 inoseizuru   (501) staff       (20)      726 2023-04-13 14:58:10.000000 anspy-0.0.1/README.md
--rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-04-13 15:04:01.752055 anspy-0.0.1/setup.cfg
--rw-r--r--   0 inoseizuru   (501) staff       (20)      950 2023-04-13 15:02:58.000000 anspy-0.0.1/setup.py
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:04:01.750832 anspy-0.0.1/src/
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:04:01.751625 anspy-0.0.1/src/anspy.egg-info/
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1247 2023-04-13 15:04:01.000000 anspy-0.0.1/src/anspy.egg-info/PKG-INFO
--rw-r--r--   0 inoseizuru   (501) staff       (20)      199 2023-04-13 15:04:01.000000 anspy-0.0.1/src/anspy.egg-info/SOURCES.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-04-13 15:04:01.000000 anspy-0.0.1/src/anspy.egg-info/dependency_links.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)       37 2023-04-13 15:04:01.000000 anspy-0.0.1/src/anspy.egg-info/entry_points.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)        6 2023-04-13 15:04:01.000000 anspy-0.0.1/src/anspy.egg-info/top_level.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)      281 2023-04-13 14:27:55.000000 anspy-0.0.1/src/anspy.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:37:36.158160 anspy-0.0.2/
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1247 2023-04-13 15:37:36.157998 anspy-0.0.2/PKG-INFO
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      726 2023-04-13 14:58:10.000000 anspy-0.0.2/README.md
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-04-13 15:37:36.158206 anspy-0.0.2/setup.cfg
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      950 2023-04-13 15:35:18.000000 anspy-0.0.2/setup.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:37:36.156984 anspy-0.0.2/src/
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-13 15:37:36.157784 anspy-0.0.2/src/anspy.egg-info/
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1247 2023-04-13 15:37:36.000000 anspy-0.0.2/src/anspy.egg-info/PKG-INFO
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      199 2023-04-13 15:37:36.000000 anspy-0.0.2/src/anspy.egg-info/SOURCES.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-04-13 15:37:36.000000 anspy-0.0.2/src/anspy.egg-info/dependency_links.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       37 2023-04-13 15:37:36.000000 anspy-0.0.2/src/anspy.egg-info/entry_points.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)        6 2023-04-13 15:37:36.000000 anspy-0.0.2/src/anspy.egg-info/top_level.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      281 2023-04-13 15:34:57.000000 anspy-0.0.2/src/anspy.py
```

### Comparing `anspy-0.0.1/PKG-INFO` & `anspy-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anspy
-Version: 0.0.1
+Version: 0.0.2
 Summary: anspy is a PyPI tool, a terminal version of ChatGPT developed using openai's api and python.
 Home-page: https://github.com/i-inose/anspy
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/anspy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anspy-0.0.1/README.md` & `anspy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `anspy-0.0.1/setup.py` & `anspy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="anspy",
-    version="0.0.1",
+    version="0.0.2",
     author="Izuru Inose",
     author_email="i.inose0304@gmail.com",
     description="anspy is a PyPI tool, a terminal version of ChatGPT developed using openai's api and python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/i-inose/anspy",
     project_urls={
```

### Comparing `anspy-0.0.1/src/anspy.egg-info/PKG-INFO` & `anspy-0.0.2/src/anspy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anspy
-Version: 0.0.1
+Version: 0.0.2
 Summary: anspy is a PyPI tool, a terminal version of ChatGPT developed using openai's api and python.
 Home-page: https://github.com/i-inose/anspy
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/anspy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

