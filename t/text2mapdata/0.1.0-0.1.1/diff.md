# Comparing `tmp/text2mapdata-0.1.0.tar.gz` & `tmp/text2mapdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2mapdata-0.1.0.tar", last modified: Thu Apr 13 01:21:53 2023, max compression
+gzip compressed data, was "text2mapdata-0.1.1.tar", last modified: Thu Apr 13 04:25:55 2023, max compression
```

## Comparing `text2mapdata-0.1.0.tar` & `text2mapdata-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/
--rw-r--r--   0 pswia     (1000) pswia     (1000)     1077 2023-04-12 23:36:48.000000 text2mapdata-0.1.0/LICENCE.txt
--rw-r--r--   0 pswia     (1000) pswia     (1000)       31 2023-04-12 23:37:06.000000 text2mapdata-0.1.0/MANIFEST.in
--rw-r--r--   0 pswia     (1000) pswia     (1000)      781 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/PKG-INFO
--rw-r--r--   0 pswia     (1000) pswia     (1000)      143 2023-04-12 23:23:59.000000 text2mapdata-0.1.0/README.md
-drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/examples/
--rw-r--r--   0 pswia     (1000) pswia     (1000)      170 2023-04-13 00:48:28.000000 text2mapdata-0.1.0/examples/map_embedding.py
-drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/fondamental/
--rw-r--r--   0 pswia     (1000) pswia     (1000)     1932 2023-04-12 23:33:53.000000 text2mapdata-0.1.0/fondamental/bases.py
--rw-r--r--   0 pswia     (1000) pswia     (1000)     1858 2023-04-12 23:36:22.000000 text2mapdata-0.1.0/main.py
--rw-r--r--   0 pswia     (1000) pswia     (1000)       38 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/setup.cfg
--rw-r--r--   0 pswia     (1000) pswia     (1000)      934 2023-04-13 01:21:42.000000 text2mapdata-0.1.0/setup.py
-drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 01:21:53.074377 text2mapdata-0.1.0/text2mapdata.egg-info/
--rw-r--r--   0 pswia     (1000) pswia     (1000)      781 2023-04-13 01:21:53.000000 text2mapdata-0.1.0/text2mapdata.egg-info/PKG-INFO
--rw-r--r--   0 pswia     (1000) pswia     (1000)      241 2023-04-13 01:21:53.000000 text2mapdata-0.1.0/text2mapdata.egg-info/SOURCES.txt
--rw-r--r--   0 pswia     (1000) pswia     (1000)        1 2023-04-13 01:21:53.000000 text2mapdata-0.1.0/text2mapdata.egg-info/dependency_links.txt
--rw-r--r--   0 pswia     (1000) pswia     (1000)        1 2023-04-13 01:21:53.000000 text2mapdata-0.1.0/text2mapdata.egg-info/top_level.txt
+drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     1077 2023-04-12 23:36:48.000000 text2mapdata-0.1.1/LICENCE.txt
+-rw-r--r--   0 pswia     (1000) pswia     (1000)       31 2023-04-12 23:37:06.000000 text2mapdata-0.1.1/MANIFEST.in
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     2532 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/PKG-INFO
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     1854 2023-04-13 03:59:05.000000 text2mapdata-0.1.1/README.md
+drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/examples/
+-rw-r--r--   0 pswia     (1000) pswia     (1000)      170 2023-04-13 00:48:28.000000 text2mapdata-0.1.1/examples/map_embedding.py
+drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/fondamental/
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     1932 2023-04-12 23:33:53.000000 text2mapdata-0.1.1/fondamental/bases.py
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     1858 2023-04-12 23:36:22.000000 text2mapdata-0.1.1/main.py
+-rw-r--r--   0 pswia     (1000) pswia     (1000)       38 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/setup.cfg
+-rw-r--r--   0 pswia     (1000) pswia     (1000)      941 2023-04-13 04:25:47.000000 text2mapdata-0.1.1/setup.py
+drwxr-xr-x   0 pswia     (1000) pswia     (1000)        0 2023-04-13 04:25:55.215298 text2mapdata-0.1.1/text2mapdata.egg-info/
+-rw-r--r--   0 pswia     (1000) pswia     (1000)     2532 2023-04-13 04:25:55.000000 text2mapdata-0.1.1/text2mapdata.egg-info/PKG-INFO
+-rw-r--r--   0 pswia     (1000) pswia     (1000)      241 2023-04-13 04:25:55.000000 text2mapdata-0.1.1/text2mapdata.egg-info/SOURCES.txt
+-rw-r--r--   0 pswia     (1000) pswia     (1000)        1 2023-04-13 04:25:55.000000 text2mapdata-0.1.1/text2mapdata.egg-info/dependency_links.txt
+-rw-r--r--   0 pswia     (1000) pswia     (1000)        1 2023-04-13 04:25:55.000000 text2mapdata-0.1.1/text2mapdata.egg-info/top_level.txt
```

### Comparing `text2mapdata-0.1.0/LICENCE.txt` & `text2mapdata-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `text2mapdata-0.1.0/fondamental/bases.py` & `text2mapdata-0.1.1/fondamental/bases.py`

 * *Files identical despite different names*

### Comparing `text2mapdata-0.1.0/main.py` & `text2mapdata-0.1.1/main.py`

 * *Files identical despite different names*

### Comparing `text2mapdata-0.1.0/setup.py` & `text2mapdata-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,17 +12,18 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='text2mapdata',
-  version='0.1.0',
+  version='0.1.1',
   description='A python package to map your own csv files data using Atlas from NOMIC',
-  long_description=open('README.md').read(), # + '\n\n' + open('CHANGELOG.md').read(),
+  long_description=open('README.md').read(),
+  long_description_content_type="text/markdown",
   url='https://github.com/papasega/text2embeddingview',  
   author='Papa Séga WADE',
   author_email='pasega.wade@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='Embedding, Visualization, Map, Text, CSV, Search keywords, dynamic', 
   packages=find_packages(),
```

