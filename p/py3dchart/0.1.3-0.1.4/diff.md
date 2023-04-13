# Comparing `tmp/py3dchart-0.1.3.tar.gz` & `tmp/py3dchart-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.3.tar", last modified: Thu Apr 13 04:02:28 2023, max compression
+gzip compressed data, was "py3dchart-0.1.4.tar", last modified: Thu Apr 13 04:11:43 2023, max compression
```

## Comparing `py3dchart-0.1.3.tar` & `py3dchart-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:02:28.045117 py3dchart-0.1.3/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 04:02:28.044117 py3dchart-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:02:28.043137 py3dchart-0.1.3/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 04:02:27.000000 py3dchart-0.1.3/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-13 04:02:27.000000 py3dchart-0.1.3/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:02:27.000000 py3dchart-0.1.3/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 04:02:27.000000 py3dchart-0.1.3/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 04:02:28.045117 py3dchart-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 04:02:22.000000 py3dchart-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:11:43.389630 py3dchart-0.1.4/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 04:11:43.388628 py3dchart-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 04:11:43.386631 py3dchart-0.1.4/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 04:11:43.389630 py3dchart-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3926 2023-04-13 04:07:05.000000 py3dchart-0.1.4/setup.py
```

### Comparing `py3dchart-0.1.3/LICENSE` & `py3dchart-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.3/PKG-INFO` & `py3dchart-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.3/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.4/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.3/setup.py` & `py3dchart-0.1.4/setup.py`

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
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

