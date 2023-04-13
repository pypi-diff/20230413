# Comparing `tmp/jianglab-0.1.3.tar.gz` & `tmp/jianglab-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.3.tar", last modified: Thu Apr 13 13:06:25 2023, max compression
+gzip compressed data, was "jianglab-0.1.4.tar", last modified: Thu Apr 13 14:04:52 2023, max compression
```

## Comparing `jianglab-0.1.3.tar` & `jianglab-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 13:06:25.147261 jianglab-0.1.3/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 13:06:25.146956 jianglab-0.1.3/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)       22 2023-04-13 12:25:42.000000 jianglab-0.1.3/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 13:06:25.146459 jianglab-0.1.3/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 13:06:25.000000 jianglab-0.1.3/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      177 2023-04-13 13:06:25.000000 jianglab-0.1.3/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 13:06:25.000000 jianglab-0.1.3/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       32 2023-04-13 13:06:25.000000 jianglab-0.1.3/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 13:06:25.000000 jianglab-0.1.3/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-13 13:06:25.147380 jianglab-0.1.3/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      771 2023-04-13 13:05:22.000000 jianglab-0.1.3/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 14:04:52.057241 jianglab-0.1.4/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 14:04:52.056865 jianglab-0.1.4/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      976 2023-04-13 13:24:58.000000 jianglab-0.1.4/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 14:04:52.056252 jianglab-0.1.4/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 14:04:51.000000 jianglab-0.1.4/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      177 2023-04-13 14:04:51.000000 jianglab-0.1.4/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 14:04:51.000000 jianglab-0.1.4/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       32 2023-04-13 14:04:51.000000 jianglab-0.1.4/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 14:04:51.000000 jianglab-0.1.4/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-13 14:04:52.057373 jianglab-0.1.4/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      771 2023-04-13 14:03:53.000000 jianglab-0.1.4/setup.py
```

### Comparing `jianglab-0.1.3/PKG-INFO` & `jianglab-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.3/jianglab.egg-info/PKG-INFO` & `jianglab-0.1.4/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.3/setup.py` & `jianglab-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
     ],
```

