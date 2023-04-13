# Comparing `tmp/easyvalid_data_validator-0.1.2.tar.gz` & `tmp/easyvalid_data_validator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyvalid_data_validator-0.1.2.tar", max compression
+gzip compressed data, was "easyvalid_data_validator-0.1.3.tar", max compression
```

## Comparing `easyvalid_data_validator-0.1.2.tar` & `easyvalid_data_validator-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-0.1.2/easyvalid_data_validator/__init__.py
--rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-0.1.2/easyvalid_data_validator/common.py
--rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.2/easyvalid_data_validator/constraints.py
--rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-0.1.2/easyvalid_data_validator/customexceptions/__init__.py
--rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.2/easyvalid_data_validator/customexceptions/array.py
--rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.2/easyvalid_data_validator/customexceptions/common.py
--rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.2/easyvalid_data_validator/customexceptions/integer.py
--rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.2/easyvalid_data_validator/customexceptions/string.py
--rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/__init__.py
--rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/array.py
--rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/boolean.py
--rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/dictionary.py
--rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/float.py
--rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/integer.py
--rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/string.py
--rw-r--r--   0        0        0     6775 2023-04-06 17:19:24.062391 easyvalid_data_validator-0.1.2/easyvalid_data_validator/validator.py
--rw-r--r--   0        0        0      410 2023-04-13 08:14:34.719802 easyvalid_data_validator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2390 2023-03-09 23:36:23.123574 easyvalid_data_validator-0.1.2/README.md
--rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 easyvalid_data_validator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-0.1.3/easyvalid_data_validator/__init__.py
+-rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-0.1.3/easyvalid_data_validator/common.py
+-rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.3/easyvalid_data_validator/constraints.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/__init__.py
+-rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/array.py
+-rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/common.py
+-rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/integer.py
+-rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/string.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/__init__.py
+-rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/array.py
+-rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/boolean.py
+-rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/dictionary.py
+-rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/float.py
+-rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/integer.py
+-rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/string.py
+-rw-r--r--   0        0        0     6775 2023-04-06 17:19:24.062391 easyvalid_data_validator-0.1.3/easyvalid_data_validator/validator.py
+-rw-r--r--   0        0        0      410 2023-04-13 08:16:54.033553 easyvalid_data_validator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-04-13 08:16:35.139598 easyvalid_data_validator-0.1.3/README.md
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 easyvalid_data_validator-0.1.3/PKG-INFO
```

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/common.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/common.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/constraints.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/constraints.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/array.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/array.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/float.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/float.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/integer.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/integer.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/datacheckers/string.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/string.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/easyvalid_data_validator/validator.py` & `easyvalid_data_validator-0.1.3/easyvalid_data_validator/validator.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.2/README.md` & `easyvalid_data_validator-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 ## Installation
 
-You can install it directly from PyPi
+You can install it directly from PyPi https://pypi.org/project/easyvalid-data-validator/
 ```bash
   pip install easyvalid-data-validator
 ```
     
 ## Tests
 
 All functions are fully tested
 
-You are able to run tests on your own by using this command being in package directory
+You are able to run tests on your own cloning repo and using it's environment:
+```
+  git clone https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR.git
+  cd EASYVALID_DATA_VALIDATOR
+  poetry update
+  poetry shell
+```
 
+And then:
 ```bash
   poetry run python -m unittest discover -v
 ```
 or
 ```bash
   poetry run pytest
 ```
```

### Comparing `easyvalid_data_validator-0.1.2/PKG-INFO` & `easyvalid_data_validator-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: easyvalid-data-validator
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 ## Installation
 
-You can install it directly from PyPi
+You can install it directly from PyPi https://pypi.org/project/easyvalid-data-validator/
 ```bash
   pip install easyvalid-data-validator
 ```
     
 ## Tests
 
 All functions are fully tested
 
-You are able to run tests on your own by using this command being in package directory
+You are able to run tests on your own cloning repo and using it's environment:
+```
+  git clone https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR.git
+  cd EASYVALID_DATA_VALIDATOR
+  poetry update
+  poetry shell
+```
 
+And then:
 ```bash
   poetry run python -m unittest discover -v
 ```
 or
 ```bash
   poetry run pytest
 ```
```

