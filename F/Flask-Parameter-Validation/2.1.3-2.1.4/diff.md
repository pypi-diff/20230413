# Comparing `tmp/Flask-Parameter-Validation-2.1.3.tar.gz` & `tmp/Flask-Parameter-Validation-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Parameter-Validation-2.1.3.tar", last modified: Tue Jan 24 14:33:10 2023, max compression
+gzip compressed data, was "Flask-Parameter-Validation-2.1.4.tar", last modified: Thu Apr 13 15:53:05 2023, max compression
```

## Comparing `Flask-Parameter-Validation-2.1.3.tar` & `Flask-Parameter-Validation-2.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:33:10.238068 Flask-Parameter-Validation-2.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:33:10.234068 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-01-24 14:33:10.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-24 14:33:10.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 14:33:10.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 14:33:09.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 14:33:10.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-24 14:33:10.000000 Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-01-24 14:33:10.238068 Flask-Parameter-Validation-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:33:10.234068 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:33:10.238068 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:33:10.238068 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 14:33:10.238068 Flask-Parameter-Validation-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-24 14:32:58.000000 Flask-Parameter-Validation-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/setup.py
```

### Comparing `Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/PKG-INFO` & `Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Parameter-Validation
-Version: 2.1.3
+Version: 2.1.4
 Summary: Get and validate all Flask input parameters with ease.
 Home-page: https://github.com/Ge0rg3/flask-parameter-validation
 Author: George Omnet
 Author-email: flaskparametervalidation@georgeom.net
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -77,29 +77,32 @@
 * int
 * bool
 * float
 * typing.List
 * typing.Union
 * typing.Optional
 * datetime.datetime
+* datetime.date
+* datetime.time
 
 ### Validation
 All parameters can have default values, and automatic validation.  
 `Route`, `Form`, `Json` and `Query` have the following options:
 * default: any, Specifies the default value for the field.
 * min_str_length: int, Specifies the minimum character length for a string input
 * max_str_length: int, Specifies the maximum character length for a string input
 * min_list_length: int, Specifies the minimum number of elements in a list
 * max_list_length: int, Specifies the maximum number of elements in a list
 * min_int: int, Specifies the minimum number for an int input
 * max_int: int, Specifies the maximum number for an int input
 * whitelist: str, A string containing allowed characters for the value
 * blacklist: str, A string containing forbidden characters for the value
 * pattern: str, A regex pattern to test for string matches
-* func: Callable, A function containing a fully customized logic to validate the value
+* func: Callable -> Union[bool, tuple[bool, str]], A function containing a fully customized logic to validate the value
+* datetime_format: str, str: datetime format string ([datetime format codes](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes))
 
 `File` has the following options:
 * content_types: array of strings, an array of allowed content types.
 * min_length: Minimum content-length for a file
 * max_length: Maximum content-length for a file
 
 These validators are passed into the classes in the route function, such as:
```

### Comparing `Flask-Parameter-Validation-2.1.3/Flask_Parameter_Validation.egg-info/SOURCES.txt` & `Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.3/PKG-INFO` & `Flask-Parameter-Validation-2.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Parameter-Validation
-Version: 2.1.3
+Version: 2.1.4
 Summary: Get and validate all Flask input parameters with ease.
 Home-page: https://github.com/Ge0rg3/flask-parameter-validation
 Author: George Omnet
 Author-email: flaskparametervalidation@georgeom.net
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -77,29 +77,32 @@
 * int
 * bool
 * float
 * typing.List
 * typing.Union
 * typing.Optional
 * datetime.datetime
+* datetime.date
+* datetime.time
 
 ### Validation
 All parameters can have default values, and automatic validation.  
 `Route`, `Form`, `Json` and `Query` have the following options:
 * default: any, Specifies the default value for the field.
 * min_str_length: int, Specifies the minimum character length for a string input
 * max_str_length: int, Specifies the maximum character length for a string input
 * min_list_length: int, Specifies the minimum number of elements in a list
 * max_list_length: int, Specifies the maximum number of elements in a list
 * min_int: int, Specifies the minimum number for an int input
 * max_int: int, Specifies the maximum number for an int input
 * whitelist: str, A string containing allowed characters for the value
 * blacklist: str, A string containing forbidden characters for the value
 * pattern: str, A regex pattern to test for string matches
-* func: Callable, A function containing a fully customized logic to validate the value
+* func: Callable -> Union[bool, tuple[bool, str]], A function containing a fully customized logic to validate the value
+* datetime_format: str, str: datetime format string ([datetime format codes](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes))
 
 `File` has the following options:
 * content_types: array of strings, an array of allowed content types.
 * min_length: Minimum content-length for a file
 * max_length: Maximum content-length for a file
 
 These validators are passed into the classes in the route function, such as:
```

### Comparing `Flask-Parameter-Validation-2.1.3/README.md` & `Flask-Parameter-Validation-2.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,29 +59,32 @@
 * int
 * bool
 * float
 * typing.List
 * typing.Union
 * typing.Optional
 * datetime.datetime
+* datetime.date
+* datetime.time
 
 ### Validation
 All parameters can have default values, and automatic validation.  
 `Route`, `Form`, `Json` and `Query` have the following options:
 * default: any, Specifies the default value for the field.
 * min_str_length: int, Specifies the minimum character length for a string input
 * max_str_length: int, Specifies the maximum character length for a string input
 * min_list_length: int, Specifies the minimum number of elements in a list
 * max_list_length: int, Specifies the maximum number of elements in a list
 * min_int: int, Specifies the minimum number for an int input
 * max_int: int, Specifies the maximum number for an int input
 * whitelist: str, A string containing allowed characters for the value
 * blacklist: str, A string containing forbidden characters for the value
 * pattern: str, A regex pattern to test for string matches
-* func: Callable, A function containing a fully customized logic to validate the value
+* func: Callable -> Union[bool, tuple[bool, str]], A function containing a fully customized logic to validate the value
+* datetime_format: str, str: datetime format string ([datetime format codes](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes))
 
 `File` has the following options:
 * content_types: array of strings, an array of allowed content types.
 * min_length: Minimum content-length for a file
 * max_length: Maximum content-length for a file
 
 These validators are passed into the classes in the route function, such as:
```

### Comparing `Flask-Parameter-Validation-2.1.3/flask_parameter_validation/exceptions/exceptions.py` & `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/file.py` & `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/file.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_types/query.py` & `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/query.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.3/flask_parameter_validation/parameter_validation.py` & `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,19 @@
                 user_inputs = [user_input]
         else:
             user_inputs = [user_input]
             expected_input_types = [expected_input_type]
 
         # Perform automatic type conversion for parameter types (i.e. "true" -> True)
         for count, value in enumerate(user_inputs):
-            user_inputs[count] = expected_delivery_type.convert(
-                value, expected_input_types)
+            try:
+                user_inputs[count] = expected_delivery_type.convert(
+                    value, expected_input_types)
+            except ValueError as e:
+                raise ValidationError(str(e), expected_name, expected_input_type)
 
         # Validate that user type(s) match expected type(s)
         validation_success = all(
             type(inp) in expected_input_types for inp in user_inputs)
 
         # Validate that if lists are required, lists are given
         if expected_input_type_str.startswith("typing.List"):
@@ -152,8 +155,10 @@
         # Validate parameter-specific requirements are met
         try:
             expected_delivery_type.validate(user_input)
         except ValueError as e:
             raise ValidationError(str(e), expected_name, expected_input_type)
 
         # Return input back to parent function
-        return user_input
+        if len(user_inputs) == 1:
+            return user_inputs[0]
+        return user_inputs
```

### Comparing `Flask-Parameter-Validation-2.1.3/setup.py` & `Flask-Parameter-Validation-2.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='Flask-Parameter-Validation',
-    version='2.1.3',
+    version='2.1.4',
     url='https://github.com/Ge0rg3/flask-parameter-validation',
     license='MIT',
     author='George Omnet',
     author_email='flaskparametervalidation@georgeom.net',
     description='Get and validate all Flask input parameters with ease.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

