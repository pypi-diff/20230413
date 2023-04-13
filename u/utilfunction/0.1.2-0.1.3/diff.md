# Comparing `tmp/utilfunction-0.1.2.tar.gz` & `tmp/utilfunction-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilfunction-0.1.2.tar", last modified: Fri Apr  7 12:07:48 2023, max compression
+gzip compressed data, was "utilfunction-0.1.3.tar", last modified: Thu Apr 13 09:26:30 2023, max compression
```

## Comparing `utilfunction-0.1.2.tar` & `utilfunction-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 12:07:48.854316 utilfunction-0.1.2/
--rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3326 2023-04-07 12:07:48.853059 utilfunction-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2023-04-07 12:06:39.000000 utilfunction-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 12:07:48.854316 utilfunction-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-04-07 12:07:34.000000 utilfunction-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:07:48.836902 utilfunction-0.1.2/utilfunction/
--rw-rw-rw-   0        0        0      834 2023-04-07 12:07:32.000000 utilfunction-0.1.2/utilfunction/__init__.py
--rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.2/utilfunction/astyper.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.2/utilfunction/path_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:07:48.850628 utilfunction-0.1.2/utilfunction.egg-info/
--rw-rw-rw-   0        0        0     3326 2023-04-07 12:07:48.000000 utilfunction-0.1.2/utilfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-07 12:07:48.000000 utilfunction-0.1.2/utilfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 12:07:48.000000 utilfunction-0.1.2/utilfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-07 12:07:48.000000 utilfunction-0.1.2/utilfunction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.438453 utilfunction-0.1.3/
+-rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3506 2023-04-13 09:26:30.437445 utilfunction-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2023-04-13 09:26:05.000000 utilfunction-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:26:30.438453 utilfunction-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-04-13 09:24:23.000000 utilfunction-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.414820 utilfunction-0.1.3/utilfunction/
+-rw-rw-rw-   0        0        0      880 2023-04-13 09:23:10.000000 utilfunction-0.1.3/utilfunction/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.3/utilfunction/astyper.py
+-rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.3/utilfunction/beep.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.3/utilfunction/path_finder.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:26:30.434234 utilfunction-0.1.3/utilfunction.egg-info/
+-rw-rw-rw-   0        0        0     3506 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 09:26:30.000000 utilfunction-0.1.3/utilfunction.egg-info/top_level.txt
```

### Comparing `utilfunction-0.1.2/LICENSE` & `utilfunction-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.2/PKG-INFO` & `utilfunction-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+Development Status :: 3 - Alpha
+
 # util-function
 ![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
@@ -46,17 +48,31 @@
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
 
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
-from utilfunction import col_converter
+from utilfunction import col_convert
+
+df_has_converted_col = col_convert(df, "embedding_arrays")
+```
+
+
+
+`beep.py` - function: beep <br>
+Make beep
+```python
+from utilfunction import beep
+
+beep()
 
-nii_file_list = col_converter(df, "embedding_arrays")
+sec=10
+feq=800
+beep(sec, feq)
 ```
 
 <br>
 
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
```

### Comparing `utilfunction-0.1.2/README.md` & `utilfunction-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+Development Status :: 3 - Alpha
+
 # util-function
 ![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
@@ -25,17 +27,31 @@
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
 
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
-from utilfunction import col_converter
+from utilfunction import col_convert
+
+df_has_converted_col = col_convert(df, "embedding_arrays")
+```
+
+
+
+`beep.py` - function: beep <br>
+Make beep
+```python
+from utilfunction import beep
+
+beep()
 
-nii_file_list = col_converter(df, "embedding_arrays")
+sec=10
+feq=800
+beep(sec, feq)
 ```
 
 <br>
 
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
```

### Comparing `utilfunction-0.1.2/setup.py` & `utilfunction-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="utilfunction",
-    version="0.1.2",
+    version="0.1.3",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/DSDanielPark/utilfunction",
     packages=find_packages(),
     python_requires=">=3.6",
-    install_requires=[],
+    install_requires=["pandas", "numpy"],
     keywords="Utils, Utility, Preprocessing, Analysis",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

### Comparing `utilfunction-0.1.2/utilfunction/__init__.py` & `utilfunction-0.1.3/utilfunction/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from utilfunction.path_finder import find_path
-from utilfunction.astyper import col_convert
-
-
 # coding=utf-8
 # Copyright 2023 parkminwoo Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,11 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # # limitations under the License.
 
-__all__ = ["find_path", "col_convert"]
 
-__version__ = "0.1.2"
+from utilfunction.path_finder import find_path
+from utilfunction.astyper import col_convert
+from utilfunction.beep import beep
+
+
+__all__ = ["find_path", "col_convert", "beep"]
+
+__version__ = "0.1.3"
 __author__ = "MinWoo Park <parkminwoo1991@gmail.com>"
```

### Comparing `utilfunction-0.1.2/utilfunction/astyper.py` & `utilfunction-0.1.3/utilfunction/astyper.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.2/utilfunction/path_finder.py` & `utilfunction-0.1.3/utilfunction/path_finder.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.2/utilfunction.egg-info/PKG-INFO` & `utilfunction-0.1.3/utilfunction.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+Development Status :: 3 - Alpha
+
 # util-function
 ![Util-Func](https://img.shields.io/badge/pypi-utilfunction-blue)
 ![Pypi Version](https://img.shields.io/pypi/v/utilfunction.svg)
 [![Contributor Covenant](https://img.shields.io/badge/contributor%20covenant-v2.0%20adopted-black.svg)](code_of_conduct.md)
 [![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8-black.svg)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 
@@ -46,17 +48,31 @@
 nii_file_list = find_path('./home', 'file', 'mask.nii.gz')
 ```
 
 
 `astyper.py` - function: col_converter <br>
 Restores a column whose array is stored as a string type back to an array type.
 ```python
-from utilfunction import col_converter
+from utilfunction import col_convert
+
+df_has_converted_col = col_convert(df, "embedding_arrays")
+```
+
+
+
+`beep.py` - function: beep <br>
+Make beep
+```python
+from utilfunction import beep
+
+beep()
 
-nii_file_list = col_converter(df, "embedding_arrays")
+sec=10
+feq=800
+beep(sec, feq)
 ```
 
 <br>
 
 # How to Contribute
 Please create a pull request for any function that is useful and simple to reuse. Create a function, and write a tutorial with the same name as the function in the doc folder. Any snippet that you are comfortable with and use often will do. However, some contents may be revised and adjusted later for convenience.
```

