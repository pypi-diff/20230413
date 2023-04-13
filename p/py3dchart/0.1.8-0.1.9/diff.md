# Comparing `tmp/py3dchart-0.1.8.tar.gz` & `tmp/py3dchart-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.8.tar", last modified: Thu Apr 13 06:12:32 2023, max compression
+gzip compressed data, was "py3dchart-0.1.9.tar", last modified: Thu Apr 13 06:38:14 2023, max compression
```

## Comparing `py3dchart-0.1.8.tar` & `py3dchart-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:12:32.668421 py3dchart-0.1.8/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 06:12:32.667451 py3dchart-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:12:32.665417 py3dchart-0.1.8/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 06:12:32.000000 py3dchart-0.1.8/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:12:32.668421 py3dchart-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 06:11:58.000000 py3dchart-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.291044 py3dchart-0.1.9/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 06:38:14.290046 py3dchart-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.262050 py3dchart-0.1.9/py3dchart/
+-rw-rw-rw-   0        0        0        0 2023-04-13 06:11:27.000000 py3dchart-0.1.9/py3dchart/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-04-13 06:37:38.000000 py3dchart-0.1.9/py3dchart/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:38:14.287007 py3dchart-0.1.9/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 06:38:14.000000 py3dchart-0.1.9/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:38:14.291044 py3dchart-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3927 2023-04-13 06:37:32.000000 py3dchart-0.1.9/setup.py
```

### Comparing `py3dchart-0.1.8/LICENSE` & `py3dchart-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.8/PKG-INFO` & `py3dchart-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.8/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.9/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.8/setup.py` & `py3dchart-0.1.9/setup.py`

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
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
@@ -99,17 +99,17 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(exclude=[]),#"tests", "*.tests", "*.tests.*", "tests.*"
     # If your package is a single module, use this instead of 'packages':
-    py_modules=['chart'],
+    # py_modules=['chart'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
```

