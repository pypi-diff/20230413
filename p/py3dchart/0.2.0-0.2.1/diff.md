# Comparing `tmp/py3dchart-0.2.0.tar.gz` & `tmp/py3dchart-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.2.0.tar", last modified: Thu Apr 13 14:20:26 2023, max compression
+gzip compressed data, was "py3dchart-0.2.1.tar", last modified: Thu Apr 13 14:22:41 2023, max compression
```

## Comparing `py3dchart-0.2.0.tar` & `py3dchart-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.618976 py3dchart-0.2.0/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 14:20:26.618014 py3dchart-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.590552 py3dchart-0.2.0/py3dchart/
--rw-rw-rw-   0        0        0       60 2023-04-13 13:56:09.000000 py3dchart-0.2.0/py3dchart/__init__.py
--rw-rw-rw-   0        0        0     2949 2023-04-13 14:19:22.000000 py3dchart-0.2.0/py3dchart/chart.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.615526 py3dchart-0.2.0/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 14:20:26.619992 py3dchart-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3927 2023-04-13 14:19:38.000000 py3dchart-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.717187 py3dchart-0.2.1/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:22:41.716187 py3dchart-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.699185 py3dchart-0.2.1/py3dchart/
+-rw-rw-rw-   0        0        0       60 2023-04-13 13:56:09.000000 py3dchart-0.2.1/py3dchart/__init__.py
+-rw-rw-rw-   0        0        0     3031 2023-04-13 14:22:13.000000 py3dchart-0.2.1/py3dchart/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.713191 py3dchart-0.2.1/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:22:41.718194 py3dchart-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3927 2023-04-13 14:22:20.000000 py3dchart-0.2.1/setup.py
```

### Comparing `py3dchart-0.2.0/LICENSE` & `py3dchart-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.2.0/PKG-INFO` & `py3dchart-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.2.0/py3dchart/chart.py` & `py3dchart-0.2.1/py3dchart/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from tkinter import *
 import numpy
 import math
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'WangLvyuan'
 
 class chart3d:
     fontSize = 12
     x1 = 20
     y1 = 20
     x2 = 220
     y2 = 220
 
+    def fontSize(self, num):
+         chart3d.fontSize = num
+         return
+
     def x1(self, num):
          chart3d.x1 = num
          return
     
     def x2(self, num):
          chart3d.x2 = num
          return
```

### Comparing `py3dchart-0.2.0/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.2.1/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.2.0/setup.py` & `py3dchart-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'py3dchart'
 DESCRIPTION = 'A simple tool for my classmate to finish their classwork'
 URL = 'https://github.com/Niggoss/Wang-Lvyuan.git'
 EMAIL = 'lvyuanw@gmail.com'
 AUTHOR = 'Wang Lvyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

