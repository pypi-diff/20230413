# Comparing `tmp/jianglab-0.1.1.tar.gz` & `tmp/jianglab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.1.tar", last modified: Thu Apr  6 21:41:53 2023, max compression
+gzip compressed data, was "jianglab-0.1.2.tar", last modified: Thu Apr 13 12:51:55 2023, max compression
```

## Comparing `jianglab-0.1.1.tar` & `jianglab-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-06 21:41:53.129237 jianglab-0.1.1/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-06 21:41:53.128909 jianglab-0.1.1/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)        0 2023-04-06 20:59:21.000000 jianglab-0.1.1/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-06 21:41:53.128389 jianglab-0.1.1/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-06 21:41:53.000000 jianglab-0.1.1/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      177 2023-04-06 21:41:53.000000 jianglab-0.1.1/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-06 21:41:53.000000 jianglab-0.1.1/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       24 2023-04-06 21:41:53.000000 jianglab-0.1.1/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-06 21:41:53.000000 jianglab-0.1.1/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-06 21:41:53.129366 jianglab-0.1.1/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      752 2023-04-06 21:40:55.000000 jianglab-0.1.1/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 12:51:55.317004 jianglab-0.1.2/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 12:51:55.316568 jianglab-0.1.2/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       22 2023-04-13 12:25:42.000000 jianglab-0.1.2/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 12:51:55.315748 jianglab-0.1.2/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 12:51:55.000000 jianglab-0.1.2/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      177 2023-04-13 12:51:55.000000 jianglab-0.1.2/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 12:51:55.000000 jianglab-0.1.2/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       35 2023-04-13 12:51:55.000000 jianglab-0.1.2/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 12:51:55.000000 jianglab-0.1.2/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-13 12:51:55.317149 jianglab-0.1.2/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      785 2023-04-13 12:44:54.000000 jianglab-0.1.2/setup.py
```

### Comparing `jianglab-0.1.1/PKG-INFO` & `jianglab-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.1/jianglab.egg-info/PKG-INFO` & `jianglab-0.1.2/jianglab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.1/setup.py` & `jianglab-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
+        "os",
+        "treelib",
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

