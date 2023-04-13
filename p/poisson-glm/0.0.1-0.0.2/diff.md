# Comparing `tmp/poisson-glm-0.0.1.tar.gz` & `tmp/poisson-glm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poisson-glm-0.0.1.tar", last modified: Mon Apr 10 18:15:34 2023, max compression
+gzip compressed data, was "poisson-glm-0.0.2.tar", last modified: Thu Apr 13 01:15:21 2023, max compression
```

## Comparing `poisson-glm-0.0.1.tar` & `poisson-glm-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 meina      (501) staff       (20)        0 2023-04-10 18:15:34.246874 poisson-glm-0.0.1/
--rw-r--r--   0 meina      (501) staff       (20)     1062 2023-04-10 11:36:24.000000 poisson-glm-0.0.1/LICENSE
--rw-r--r--   0 meina      (501) staff       (20)      519 2023-04-10 18:15:34.246723 poisson-glm-0.0.1/PKG-INFO
--rw-r--r--   0 meina      (501) staff       (20)       12 2023-04-10 11:36:24.000000 poisson-glm-0.0.1/README.md
-drwxr-xr-x   0 meina      (501) staff       (20)        0 2023-04-10 18:15:34.246596 poisson-glm-0.0.1/poisson_glm.egg-info/
--rw-r--r--   0 meina      (501) staff       (20)      519 2023-04-10 18:15:34.000000 poisson-glm-0.0.1/poisson_glm.egg-info/PKG-INFO
--rw-r--r--   0 meina      (501) staff       (20)      200 2023-04-10 18:15:34.000000 poisson-glm-0.0.1/poisson_glm.egg-info/SOURCES.txt
--rw-r--r--   0 meina      (501) staff       (20)        1 2023-04-10 18:15:34.000000 poisson-glm-0.0.1/poisson_glm.egg-info/dependency_links.txt
--rw-r--r--   0 meina      (501) staff       (20)       33 2023-04-10 18:15:34.000000 poisson-glm-0.0.1/poisson_glm.egg-info/requires.txt
--rw-r--r--   0 meina      (501) staff       (20)        1 2023-04-10 18:15:34.000000 poisson-glm-0.0.1/poisson_glm.egg-info/top_level.txt
--rw-r--r--   0 meina      (501) staff       (20)       38 2023-04-10 18:15:34.246915 poisson-glm-0.0.1/setup.cfg
--rw-r--r--   0 meina      (501) staff       (20)      774 2023-04-10 12:00:57.000000 poisson-glm-0.0.1/setup.py
+drwxr-xr-x   0 meina      (501) staff       (20)        0 2023-04-13 01:15:21.487179 poisson-glm-0.0.2/
+-rw-r--r--   0 meina      (501) staff       (20)     1062 2023-04-10 11:36:24.000000 poisson-glm-0.0.2/LICENSE
+-rw-r--r--   0 meina      (501) staff       (20)      630 2023-04-13 01:15:21.487024 poisson-glm-0.0.2/PKG-INFO
+-rw-r--r--   0 meina      (501) staff       (20)      534 2023-04-13 01:05:37.000000 poisson-glm-0.0.2/README.md
+drwxr-xr-x   0 meina      (501) staff       (20)        0 2023-04-13 01:15:21.486897 poisson-glm-0.0.2/poisson_glm.egg-info/
+-rw-r--r--   0 meina      (501) staff       (20)      630 2023-04-13 01:15:21.000000 poisson-glm-0.0.2/poisson_glm.egg-info/PKG-INFO
+-rw-r--r--   0 meina      (501) staff       (20)      200 2023-04-13 01:15:21.000000 poisson-glm-0.0.2/poisson_glm.egg-info/SOURCES.txt
+-rw-r--r--   0 meina      (501) staff       (20)        1 2023-04-13 01:15:21.000000 poisson-glm-0.0.2/poisson_glm.egg-info/dependency_links.txt
+-rw-r--r--   0 meina      (501) staff       (20)       33 2023-04-13 01:15:21.000000 poisson-glm-0.0.2/poisson_glm.egg-info/requires.txt
+-rw-r--r--   0 meina      (501) staff       (20)        1 2023-04-13 01:15:21.000000 poisson-glm-0.0.2/poisson_glm.egg-info/top_level.txt
+-rw-r--r--   0 meina      (501) staff       (20)       38 2023-04-13 01:15:21.487227 poisson-glm-0.0.2/setup.cfg
+-rw-r--r--   0 meina      (501) staff       (20)      885 2023-04-13 01:12:06.000000 poisson-glm-0.0.2/setup.py
```

### Comparing `poisson-glm-0.0.1/LICENSE` & `poisson-glm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poisson-glm-0.0.1/PKG-INFO` & `poisson-glm-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: poisson-glm
-Version: 0.0.1
-Summary: Poisson GLM package for investigating spike trains in RGCs population
+Version: 0.0.2
+Summary: Poisson GLM package for investigating spike trains in RGCs population. The model can use either radial basis function or raised cosine bumps, since both were built for comparisons.
 Author: Meina Lin Wei
 Author-email: meina.lw12@gmail.com
 Keywords: python,poissonGLM
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `poisson-glm-0.0.1/poisson_glm.egg-info/PKG-INFO` & `poisson-glm-0.0.2/poisson_glm.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: poisson-glm
-Version: 0.0.1
-Summary: Poisson GLM package for investigating spike trains in RGCs population
+Version: 0.0.2
+Summary: Poisson GLM package for investigating spike trains in RGCs population. The model can use either radial basis function or raised cosine bumps, since both were built for comparisons.
 Author: Meina Lin Wei
 Author-email: meina.lw12@gmail.com
 Keywords: python,poissonGLM
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `poisson-glm-0.0.1/setup.py` & `poisson-glm-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
-DESCRIPTION = 'Poisson GLM package for investigating spike trains in RGCs population'
+VERSION = '0.0.2'
+DESCRIPTION = 'Poisson GLM package for investigating spike trains in RGCs population. The model can use either radial basis function or raised cosine bumps, since both were built for comparisons.'
 
 # Setting up
 setup(
     name="poisson-glm",
     version=VERSION,
     author="Meina Lin Wei",
     author_email="meina.lw12@gmail.com",
```

