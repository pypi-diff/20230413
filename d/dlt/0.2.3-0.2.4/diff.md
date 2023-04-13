# Comparing `tmp/dlt-0.2.3.tar.gz` & `tmp/dlt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlt-0.2.3.tar", last modified: Wed Feb 14 14:58:56 2018, max compression
+gzip compressed data, was "dlt-0.2.4.tar", last modified: Thu Apr 13 10:16:22 2023, max compression
```

## Comparing `dlt-0.2.3.tar` & `dlt-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hiroyuki827   (501) staff       (20)        0 2018-02-14 14:58:56.000000 dlt-0.2.3/
--rw-r--r--   0 hiroyuki827   (501) staff       (20)      697 2018-02-14 14:58:56.000000 dlt-0.2.3/PKG-INFO
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)     1085 2018-01-25 03:33:06.000000 dlt-0.2.3/LICENSE.md
-drwxr-xr-x   0 hiroyuki827   (501) staff       (20)        0 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt/
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)     1349 2018-01-25 03:33:06.000000 dlt-0.2.3/dlt/fashion_mnist.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)      166 2018-01-25 03:39:08.000000 dlt-0.2.3/dlt/__init__.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)    10235 2018-02-14 14:57:07.000000 dlt-0.2.3/dlt/utils.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)     5297 2018-01-30 08:29:01.000000 dlt-0.2.3/dlt/cifar.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)      927 2018-01-30 08:30:39.000000 dlt-0.2.3/dlt/mnist.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)       37 2018-01-25 03:33:06.000000 dlt-0.2.3/MANIFEST.in
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)     1920 2018-02-14 14:45:42.000000 dlt-0.2.3/README.md
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)      839 2018-02-14 14:58:12.000000 dlt-0.2.3/setup.py
--rwxr-xr-x   0 hiroyuki827   (501) staff       (20)       70 2018-02-14 14:58:56.000000 dlt-0.2.3/setup.cfg
-drwxr-xr-x   0 hiroyuki827   (501) staff       (20)        0 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/
--rw-r--r--   0 hiroyuki827   (501) staff       (20)      697 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/PKG-INFO
--rw-r--r--   0 hiroyuki827   (501) staff       (20)      261 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/SOURCES.txt
--rw-r--r--   0 hiroyuki827   (501) staff       (20)       47 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/requires.txt
--rw-r--r--   0 hiroyuki827   (501) staff       (20)        4 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/top_level.txt
--rw-r--r--   0 hiroyuki827   (501) staff       (20)        1 2018-02-14 14:58:56.000000 dlt-0.2.3/dlt.egg-info/dependency_links.txt
+drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.515210 dlt-0.2.4/
+-rwxr-xr-x   0 burnash    (501) staff       (20)     1085 2018-01-25 03:33:06.000000 dlt-0.2.4/LICENSE.md
+-rwxr-xr-x   0 burnash    (501) staff       (20)       37 2018-01-25 03:33:06.000000 dlt-0.2.4/MANIFEST.in
+-rw-r--r--   0 burnash    (501) staff       (20)      690 2023-04-13 10:16:22.515334 dlt-0.2.4/PKG-INFO
+-rwxr-xr-x   0 burnash    (501) staff       (20)     1920 2018-02-14 14:45:42.000000 dlt-0.2.4/README.md
+drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.513721 dlt-0.2.4/dlt/
+-rwxr-xr-x   0 burnash    (501) staff       (20)      485 2023-04-13 10:15:44.000000 dlt-0.2.4/dlt/__init__.py
+-rwxr-xr-x   0 burnash    (501) staff       (20)     5297 2018-01-30 08:29:01.000000 dlt-0.2.4/dlt/cifar.py
+-rwxr-xr-x   0 burnash    (501) staff       (20)     1349 2018-01-25 03:33:06.000000 dlt-0.2.4/dlt/fashion_mnist.py
+-rwxr-xr-x   0 burnash    (501) staff       (20)      927 2018-01-30 08:30:39.000000 dlt-0.2.4/dlt/mnist.py
+-rwxr-xr-x   0 burnash    (501) staff       (20)    10235 2018-02-14 14:57:07.000000 dlt-0.2.4/dlt/utils.py
+drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.515004 dlt-0.2.4/dlt.egg-info/
+-rw-r--r--   0 burnash    (501) staff       (20)      690 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/PKG-INFO
+-rw-r--r--   0 burnash    (501) staff       (20)      261 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/SOURCES.txt
+-rw-r--r--   0 burnash    (501) staff       (20)        1 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/dependency_links.txt
+-rw-r--r--   0 burnash    (501) staff       (20)       47 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/requires.txt
+-rw-r--r--   0 burnash    (501) staff       (20)        4 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/top_level.txt
+-rwxr-xr-x   0 burnash    (501) staff       (20)       70 2023-04-13 10:16:22.515727 dlt-0.2.4/setup.cfg
+-rwxr-xr-x   0 burnash    (501) staff       (20)      839 2023-04-13 09:44:49.000000 dlt-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dlt-0.2.3/PKG-INFO` & `dlt-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: dlt
-Version: 0.2.3
+Version: 0.2.4
 Summary: The  package to visualize the result for the learners of the deep learning 
 Home-page: https://github.com/hiroyuki827/deep_learning_tools
-Author: Hioyuki Fuchiue
-Author-email: hiroyuki.fuchiue.827@gmail.com
+Author: David Walz
+Maintainer: Hioyuki Fuchiue
+Maintainer-email: hiroyuki.fuchiue.827@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dlt-0.2.3/LICENSE.md` & `dlt-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/dlt/fashion_mnist.py` & `dlt-0.2.4/dlt/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/dlt/utils.py` & `dlt-0.2.4/dlt/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/dlt/cifar.py` & `dlt-0.2.4/dlt/cifar.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/dlt/mnist.py` & `dlt-0.2.4/dlt/mnist.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/README.md` & `dlt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.3/setup.py` & `dlt-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dlt',
-    version='0.2.3',
+    version='0.2.4',
     packages=['dlt'],
     url='https://github.com/hiroyuki827/deep_learning_tools',
     license='MIT',
     author='David Walz',
     maintainer='Hioyuki Fuchiue',
     maintainer_email='hiroyuki.fuchiue.827@gmail.com',
     description='The  package to visualize the result for the learners of the deep learning ',
```

### Comparing `dlt-0.2.3/dlt.egg-info/PKG-INFO` & `dlt-0.2.4/dlt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: dlt
-Version: 0.2.3
+Version: 0.2.4
 Summary: The  package to visualize the result for the learners of the deep learning 
 Home-page: https://github.com/hiroyuki827/deep_learning_tools
-Author: Hioyuki Fuchiue
-Author-email: hiroyuki.fuchiue.827@gmail.com
+Author: David Walz
+Maintainer: Hioyuki Fuchiue
+Maintainer-email: hiroyuki.fuchiue.827@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

