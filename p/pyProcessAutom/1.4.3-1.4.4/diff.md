# Comparing `tmp/pyProcessAutom-1.4.3.tar.gz` & `tmp/pyProcessAutom-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.4.3.tar", last modified: Thu Apr 13 06:53:07 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.4.tar", last modified: Thu Apr 13 09:17:54 2023, max compression
```

## Comparing `pyProcessAutom-1.4.3.tar` & `pyProcessAutom-1.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.645584 pyProcessAutom-1.4.3/
--rw-rw-rw-   0        0        0     1901 2023-04-13 06:53:07.644570 pyProcessAutom-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1674 2023-04-13 06:52:42.000000 pyProcessAutom-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.617113 pyProcessAutom-1.4.3/auto_preprocess/
--rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.3/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4.3/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:07.643571 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1901 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 06:53:07.000000 pyProcessAutom-1.4.3/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:53:07.646582 pyProcessAutom-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-13 06:52:48.000000 pyProcessAutom-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.507016 pyProcessAutom-1.4.4/
+-rw-rw-rw-   0        0        0     1897 2023-04-13 09:17:54.506017 pyProcessAutom-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1670 2023-04-13 09:17:34.000000 pyProcessAutom-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.462017 pyProcessAutom-1.4.4/auto_preprocess/
+-rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.4/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4.4/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.503044 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1897 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:17:54.508017 pyProcessAutom-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-13 09:16:36.000000 pyProcessAutom-1.4.4/setup.py
```

### Comparing `pyProcessAutom-1.4.3/PKG-INFO` & `pyProcessAutom-1.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.3
+Version: 1.4.4
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Data Preprocessing Library
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
-pip install data-preprocessing
+pip install pyProcessAutom
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
```

### Comparing `pyProcessAutom-1.4.3/README.md` & `pyProcessAutom-1.4.4/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+Metadata-Version: 2.1
+Name: pyProcessAutom
+Version: 1.4.4
+Summary: A data preprocessing library
+Home-page: UNKNOWN
+Author: Aryan Sakhala
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 Data Preprocessing Library
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
-pip install data-preprocessing
+pip install pyProcessAutom
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
@@ -34,8 +44,9 @@
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
 * scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
 * label_encode(): Encodes all columns with binary categories using label encoding.
 * impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
-This project is licensed under the MIT License - see the LICENSE.txt file for details.
+This project is licensed under the MIT License - see the LICENSE.txt file for details.
+
```

### Comparing `pyProcessAutom-1.4.3/auto_preprocess/data_preprocess.py` & `pyProcessAutom-1.4.4/auto_preprocess/data_preprocess.py`

 * *Files identical despite different names*

### Comparing `pyProcessAutom-1.4.3/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-Metadata-Version: 2.1
-Name: pyProcessAutom
-Version: 1.4.3
-Summary: A data preprocessing library
-Home-page: UNKNOWN
-Author: Aryan Sakhala
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Data Preprocessing Library
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
-pip install data-preprocessing
+pip install pyProcessAutom
 ```
 # Usage
 To use this library, simply import the DataPreprocessor class from the data_preprocess module and instantiate it with a pandas DataFrame. You can then call various methods of the DataPreprocessor class to preprocess the data.
 
 Here's an example of how to use this library:
 ```
 import pandas as pd
@@ -44,9 +34,8 @@
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
 * scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
 * label_encode(): Encodes all columns with binary categories using label encoding.
 * impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
-This project is licensed under the MIT License - see the LICENSE.txt file for details.
-
+This project is licensed under the MIT License - see the LICENSE.txt file for details.
```

