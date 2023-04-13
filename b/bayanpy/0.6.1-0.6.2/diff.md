# Comparing `tmp/bayanpy-0.6.1.tar.gz` & `tmp/bayanpy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.1.tar", last modified: Thu Apr 13 14:32:37 2023, max compression
+gzip compressed data, was "bayanpy-0.6.2.tar", last modified: Thu Apr 13 14:40:21 2023, max compression
```

## Comparing `bayanpy-0.6.1.tar` & `bayanpy-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.1/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:32:37.059519 bayanpy-0.6.1/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.1/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51873 2023-04-13 14:28:36.000000 bayanpy-0.6.1/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:28:56.000000 bayanpy-0.6.1/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-13 14:32:37.000000 bayanpy-0.6.1/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-13 14:32:37.059519 bayanpy-0.6.1/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      561 2023-04-13 14:29:14.000000 bayanpy-0.6.1/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.2/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:40:21.572419 bayanpy-0.6.2/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.2/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51873 2023-04-13 14:28:36.000000 bayanpy-0.6.2/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.2/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-13 14:40:21.572419 bayanpy-0.6.2/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      561 2023-04-13 14:39:10.000000 bayanpy-0.6.2/setup.py
```

### Comparing `bayanpy-0.6.1/LICENSE` & `bayanpy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.1/README.md` & `bayanpy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.1/bayanpy/BayanImplied.py` & `bayanpy-0.6.2/bayanpy/BayanImplied.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.1/setup.py` & `bayanpy-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.1", 
+    version="0.6.2", 
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

