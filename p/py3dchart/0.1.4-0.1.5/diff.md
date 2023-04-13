# Comparing `tmp/py3dchart-0.1.4.tar.gz` & `tmp/py3dchart-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.4.tar", last modified: Thu Apr 13 04:11:43 2023, max compression
+gzip compressed data, was "py3dchart-0.1.5.tar", last modified: Thu Apr 13 04:28:15 2023, max compression
```

## Comparing `py3dchart-0.1.4.tar` & `py3dchart-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:11:43.389630 py3dchart-0.1.4/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 04:11:43.388628 py3dchart-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:11:43.386631 py3dchart-0.1.4/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 04:11:43.000000 py3dchart-0.1.4/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 04:11:43.389630 py3dchart-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 04:07:05.000000 py3dchart-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:28:15.737894 py3dchart-0.1.5/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 04:28:15.736896 py3dchart-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 04:28:15.712899 py3dchart-0.1.5/py3dchart/
+-rw-rw-rw-   0        0        0       93 2023-04-13 03:47:37.000000 py3dchart-0.1.5/py3dchart/__init__.py
+-rw-rw-rw-   0        0        0     1212 2023-04-13 04:22:42.000000 py3dchart-0.1.5/py3dchart/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:28:15.734895 py3dchart-0.1.5/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 04:28:15.000000 py3dchart-0.1.5/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-13 04:28:15.000000 py3dchart-0.1.5/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 04:28:15.000000 py3dchart-0.1.5/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 04:28:15.000000 py3dchart-0.1.5/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 04:28:15.737894 py3dchart-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3926 2023-04-13 04:27:48.000000 py3dchart-0.1.5/setup.py
```

### Comparing `py3dchart-0.1.4/LICENSE` & `py3dchart-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.4/PKG-INFO` & `py3dchart-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.4/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.5/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.4/setup.py` & `py3dchart-0.1.5/setup.py`

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
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
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
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
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

