# Comparing `tmp/pyProcessAutom-1.4.2.tar.gz` & `tmp/pyProcessAutom-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.4.2.tar", last modified: Thu Apr 13 06:48:46 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.3.tar", last modified: Thu Apr 13 06:53:07 2023, max compression
```

## Comparing `pyProcessAutom-1.4.2.tar` & `pyProcessAutom-1.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:48:46.068482 pyProcessAutom-1.4.2/
--rw-rw-rw-   0        0        0     1885 2023-04-13 06:48:46.067480 pyProcessAutom-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1658 2023-04-13 06:48:12.000000 pyProcessAutom-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:48:46.035489 pyProcessAutom-1.4.2/auto_preprocess/
--rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.2/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4.2/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:48:46.065482 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1885 2023-04-13 06:48:45.000000 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-13 06:48:45.000000 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:48:45.000000 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 06:48:45.000000 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 06:48:45.000000 pyProcessAutom-1.4.2/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:48:46.068482 pyProcessAutom-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-13 06:48:41.000000 pyProcessAutom-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.645584 pyProcessAutom-1.4.3/
+-rw-rw-rw-   0        0        0     1901 2023-04-13 06:53:07.644570 pyProcessAutom-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1674 2023-04-13 06:52:42.000000 pyProcessAutom-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.617113 pyProcessAutom-1.4.3/auto_preprocess/
+-rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.3/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4.3/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.643571 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1901 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:53:07.646582 pyProcessAutom-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-13 06:52:48.000000 pyProcessAutom-1.4.3/setup.py
```

### Comparing `pyProcessAutom-1.4.2/PKG-INFO` & `pyProcessAutom-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.2
+Version: 1.4.3
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -19,15 +19,15 @@
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
-from auto_preprocess import DataPreprocessor
+from auto_preprocess.data_preprocess import DataPreprocessor
 
 # Load data into a pandas DataFrame
 df = pd.read_csv("my_data.csv")
 
 # Preprocess the data using the DataPreprocessor class
 preprocessor = DataPreprocessor(df)
 preprocessor.remove_outliers()
```

### Comparing `pyProcessAutom-1.4.2/README.md` & `pyProcessAutom-1.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
-from auto_preprocess import DataPreprocessor
+from auto_preprocess.data_preprocess import DataPreprocessor
 
 # Load data into a pandas DataFrame
 df = pd.read_csv("my_data.csv")
 
 # Preprocess the data using the DataPreprocessor class
 preprocessor = DataPreprocessor(df)
 preprocessor.remove_outliers()
```

### Comparing `pyProcessAutom-1.4.2/auto_preprocess/data_preprocess.py` & `pyProcessAutom-1.4.3/auto_preprocess/data_preprocess.py`

 * *Files identical despite different names*

### Comparing `pyProcessAutom-1.4.2/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4.3/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.2
+Version: 1.4.3
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -19,15 +19,15 @@
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
-from auto_preprocess import DataPreprocessor
+from auto_preprocess.data_preprocess import DataPreprocessor
 
 # Load data into a pandas DataFrame
 df = pd.read_csv("my_data.csv")
 
 # Preprocess the data using the DataPreprocessor class
 preprocessor = DataPreprocessor(df)
 preprocessor.remove_outliers()
```

