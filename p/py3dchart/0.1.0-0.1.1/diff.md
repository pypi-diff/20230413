# Comparing `tmp/py3dchart-0.1.0.tar.gz` & `tmp/py3dchart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.0.tar", last modified: Thu Apr 13 03:12:55 2023, max compression
+gzip compressed data, was "py3dchart-0.1.1.tar", last modified: Thu Apr 13 03:37:38 2023, max compression
```

## Comparing `py3dchart-0.1.0.tar` & `py3dchart-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:12:55.413079 py3dchart-0.1.0/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 03:12:55.412085 py3dchart-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:12:55.410115 py3dchart-0.1.0/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 03:12:55.000000 py3dchart-0.1.0/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-13 03:12:55.000000 py3dchart-0.1.0/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:12:55.000000 py3dchart-0.1.0/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 03:12:55.000000 py3dchart-0.1.0/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 03:12:55.413079 py3dchart-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 03:12:28.000000 py3dchart-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:37:38.444323 py3dchart-0.1.1/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 03:37:38.443323 py3dchart-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 03:37:38.441306 py3dchart-0.1.1/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 03:37:38.000000 py3dchart-0.1.1/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-13 03:37:38.000000 py3dchart-0.1.1/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:37:38.000000 py3dchart-0.1.1/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 03:37:38.000000 py3dchart-0.1.1/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:37:38.444323 py3dchart-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3926 2023-04-13 03:35:11.000000 py3dchart-0.1.1/setup.py
```

### Comparing `py3dchart-0.1.0/LICENSE` & `py3dchart-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.0/PKG-INFO` & `py3dchart-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.0/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.1/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.0/setup.py` & `py3dchart-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'py3dchart'
 DESCRIPTION = 'A simple tool for my classmate to finish their classwork'
 URL = 'https://github.com/Niggoss/Wang-Lvyuan.git'
 EMAIL = 'lvyuanw@gmail.com'
 AUTHOR = 'Wang Lvyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

