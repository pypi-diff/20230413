# Comparing `tmp/tokenizer-viz-0.1.2.tar.gz` & `tmp/tokenizer-viz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizer-viz-0.1.2.tar", last modified: Fri Apr  7 20:51:35 2023, max compression
+gzip compressed data, was "tokenizer-viz-0.2.0.tar", last modified: Thu Apr 13 12:57:49 2023, max compression
```

## Comparing `tokenizer-viz-0.1.2.tar` & `tokenizer-viz-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.813204 tokenizer-viz-0.1.2/
--rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.1.2/LICENSE
--rw-r--r--   0 darienschettler   (501) staff       (20)     2975 2023-04-07 20:51:35.813101 tokenizer-viz-0.1.2/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)     2324 2023-04-07 20:51:22.000000 tokenizer-viz-0.1.2/README.md
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-07 20:51:35.813242 tokenizer-viz-0.1.2/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)      956 2023-04-07 20:51:16.000000 tokenizer-viz-0.1.2/setup.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.812254 tokenizer-viz-0.1.2/tokenizer_viz/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-04-07 19:06:23.000000 tokenizer-viz-0.1.2/tokenizer_viz/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2832 2023-04-07 19:42:40.000000 tokenizer-viz-0.1.2/tokenizer_viz/viz_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.812949 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2975 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      263 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/top_level.txt
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.380427 tokenizer-viz-0.2.0/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.2.0/LICENSE
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 12:57:49.380325 tokenizer-viz-0.2.0/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2148 2023-04-13 12:57:10.000000 tokenizer-viz-0.2.0/README.md
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-13 12:57:49.380464 tokenizer-viz-0.2.0/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)      959 2023-04-13 12:40:42.000000 tokenizer-viz-0.2.0/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.379491 tokenizer-viz-0.2.0/tokenizer_viz/
+-rw-r--r--   0 darienschettler   (501) staff       (20)       46 2023-04-13 12:36:19.000000 tokenizer-viz-0.2.0/tokenizer_viz/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     7474 2023-04-13 12:56:37.000000 tokenizer-viz-0.2.0/tokenizer_viz/visualization.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.380165 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      267 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/top_level.txt
```

### Comparing `tokenizer-viz-0.1.2/LICENSE` & `tokenizer-viz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.1.2/setup.py` & `tokenizer-viz-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tokenizer-viz",
-    version="0.1.2",
+    version="0.2.0",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
-    description="A package to visualize tokenization of text using HTML",
+    description="A package to visualize tokenization boundaries using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/tokenizer-viz",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

