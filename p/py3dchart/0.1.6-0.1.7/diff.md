# Comparing `tmp/py3dchart-0.1.6.tar.gz` & `tmp/py3dchart-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.1.6.tar", last modified: Thu Apr 13 04:45:29 2023, max compression
+gzip compressed data, was "py3dchart-0.1.7.tar", last modified: Thu Apr 13 05:47:30 2023, max compression
```

## Comparing `py3dchart-0.1.6.tar` & `py3dchart-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:45:29.120989 py3dchart-0.1.6/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 04:45:29.119988 py3dchart-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:45:29.107992 py3dchart-0.1.6/py3dchart/
--rw-rw-rw-   0        0        0       93 2023-04-13 03:47:37.000000 py3dchart-0.1.6/py3dchart/__init__.py
--rw-rw-rw-   0        0        0     1212 2023-04-13 04:44:52.000000 py3dchart-0.1.6/py3dchart/chart.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:45:29.117991 py3dchart-0.1.6/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 04:45:28.000000 py3dchart-0.1.6/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-13 04:45:29.000000 py3dchart-0.1.6/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:45:28.000000 py3dchart-0.1.6/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 04:45:28.000000 py3dchart-0.1.6/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 04:45:29.120989 py3dchart-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     3926 2023-04-13 04:44:45.000000 py3dchart-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:47:30.792416 py3dchart-0.1.7/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 05:47:30.791411 py3dchart-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1244 2023-04-13 05:42:55.000000 py3dchart-0.1.7/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:47:30.789410 py3dchart-0.1.7/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 05:47:30.000000 py3dchart-0.1.7/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 05:47:30.792416 py3dchart-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3926 2023-04-13 05:45:22.000000 py3dchart-0.1.7/setup.py
```

### Comparing `py3dchart-0.1.6/LICENSE` & `py3dchart-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.1.6/PKG-INFO` & `py3dchart-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.6/py3dchart/chart.py` & `py3dchart-0.1.7/chart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tkinter import *
 import numpy
 
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 __author__ = 'WangLvyuan'
 
 class threeDChart:
 
     def pieData(data2):
         rate = []
         s = sum(data2)
@@ -33,10 +33,13 @@
             startPoint += degree
     
         cv.create_oval(center, fill="white")
         cv.create_arc(centerShadow, style="arc", start=71, extent=135)
     
         cv.pack()
         root.mainloop()
+
+def main():
+     print('test main')
 		
 if __name__ == '__main__':
-	print("hello")
+	main()
```

### Comparing `py3dchart-0.1.6/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.1.7/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.1.6/setup.py` & `py3dchart-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'py3dchart'
 DESCRIPTION = 'A simple tool for my classmate to finish their classwork'
 URL = 'https://github.com/Niggoss/Wang-Lvyuan.git'
 EMAIL = 'lvyuanw@gmail.com'
 AUTHOR = 'Wang Lvyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
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
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
-    # py_modules=['chart'],
+    py_modules=['chart'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
```

