# Comparing `tmp/py3dchart-0.1.9.tar.gz` & `tmp/py3dchart-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.9.tar", last modified: Thu Apr 13 06:38:14 2023, max compression
+gzip compressed data, was "py3dchart-0.2.0.tar", last modified: Thu Apr 13 14:20:26 2023, max compression
```

## Comparing `py3dchart-0.1.9.tar` & `py3dchart-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.291044 py3dchart-0.1.9/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 06:38:14.290046 py3dchart-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.262050 py3dchart-0.1.9/py3dchart/
--rw-rw-rw-   0        0        0        0 2023-04-13 06:11:27.000000 py3dchart-0.1.9/py3dchart/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-04-13 06:37:38.000000 py3dchart-0.1.9/py3dchart/chart.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.287007 py3dchart-0.1.9/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:38:14.291044 py3dchart-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     3927 2023-04-13 06:37:32.000000 py3dchart-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.618976 py3dchart-0.2.0/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:20:26.618014 py3dchart-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.590552 py3dchart-0.2.0/py3dchart/
+-rw-rw-rw-   0        0        0       60 2023-04-13 13:56:09.000000 py3dchart-0.2.0/py3dchart/__init__.py
+-rw-rw-rw-   0        0        0     2949 2023-04-13 14:19:22.000000 py3dchart-0.2.0/py3dchart/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:20:26.615526 py3dchart-0.2.0/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 14:20:26.000000 py3dchart-0.2.0/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:20:26.619992 py3dchart-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3927 2023-04-13 14:19:38.000000 py3dchart-0.2.0/setup.py
```

### Comparing `py3dchart-0.1.9/LICENSE` & `py3dchart-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.9/PKG-INFO` & `py3dchart-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.9/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.2.0/py3dchart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.9/setup.py` & `py3dchart-0.2.0/setup.py`

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
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

