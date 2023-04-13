# Comparing `tmp/py3dchart-0.1.7.tar.gz` & `tmp/py3dchart-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.7.tar", last modified: Thu Apr 13 05:47:30 2023, max compression
+gzip compressed data, was "py3dchart-0.1.8.tar", last modified: Thu Apr 13 06:12:32 2023, max compression
```

## Comparing `py3dchart-0.1.7.tar` & `py3dchart-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 05:47:30.792416 py3dchart-0.1.7/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 05:47:30.791411 py3dchart-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.7/README.md
--rw-rw-rw-   0        0        0     1244 2023-04-13 05:42:55.000000 py3dchart-0.1.7/chart.py
-drwxrwxrwx   0        0        0        0 2023-04-13 05:47:30.789410 py3dchart-0.1.7/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 05:47:30.792416 py3dchart-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 05:45:22.000000 py3dchart-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:12:32.668421 py3dchart-0.1.8/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 06:12:32.667451 py3dchart-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:12:32.665417 py3dchart-0.1.8/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:12:32.668421 py3dchart-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3926 2023-04-13 06:11:58.000000 py3dchart-0.1.8/setup.py
```

### Comparing `py3dchart-0.1.7/LICENSE` & `py3dchart-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.7/PKG-INFO` & `py3dchart-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.7/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.8/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.7/setup.py` & `py3dchart-0.1.8/setup.py`

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
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

