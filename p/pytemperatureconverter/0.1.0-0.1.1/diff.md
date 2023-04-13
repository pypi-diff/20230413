# Comparing `tmp/pytemperatureconverter-0.1.0.tar.gz` & `tmp/pytemperatureconverter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytemperatureconverter-0.1.0.tar", max compression
+gzip compressed data, was "pytemperatureconverter-0.1.1.tar", max compression
```

## Comparing `pytemperatureconverter-0.1.0.tar` & `pytemperatureconverter-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      363 2023-04-13 13:45:21.129362 pytemperatureconverter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 13:44:44.317666 pytemperatureconverter-0.1.0/pytemperatureconverter/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-12 09:24:05.087934 pytemperatureconverter-0.1.0/pytemperatureconverter/functions.py
--rw-r--r--   0        0        0     2933 2023-04-13 13:55:00.840795 pytemperatureconverter-0.1.0/README.md
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 pytemperatureconverter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-04-13 14:10:40.053155 pytemperatureconverter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 13:44:44.317666 pytemperatureconverter-0.1.1/pytemperatureconverter/__init__.py
+-rw-r--r--   0        0        0     1847 2023-04-12 09:24:05.087934 pytemperatureconverter-0.1.1/pytemperatureconverter/functions.py
+-rw-r--r--   0        0        0     2921 2023-04-13 14:00:08.832048 pytemperatureconverter-0.1.1/README.md
+-rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 pytemperatureconverter-0.1.1/PKG-INFO
```

### Comparing `pytemperatureconverter-0.1.0/pytemperatureconverter/functions.py` & `pytemperatureconverter-0.1.1/pytemperatureconverter/functions.py`

 * *Files identical despite different names*

### Comparing `pytemperatureconverter-0.1.0/README.md` & `pytemperatureconverter-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 kelvin_to_rankine(k): Converts Kelvin to Rankine.
 rankine_to_celsius(r): Converts Rankine to Celsius.
 rankine_to_fahrenheit(r): Converts Rankine to Fahrenheit.
 rankine_to_kelvin(r): Converts Rankine to Kelvin.
 
 Each function takes a numeric value as an argument and returns a numeric value as a result. For example:
 
->>> converter.celsius_to_fahrenheit(0)
+converter.celsius_to_fahrenheit(0)
 32.0
->>> converter.fahrenheit_to_kelvin(32)
+converter.fahrenheit_to_kelvin(32)
 273.15
->>> converter.kelvin_to_rankine(273.15)
+converter.kelvin_to_rankine(273.15)
 491.67
 ## Testing
 
 The functions have been tested using pytest.
 ============================= test session starts =============================
 platform win32 -- Python 3.11.0, pytest-7.3.0, pluggy-1.0.0 -- C:\Users\username\AppData\Local\pypoetry\Cache\virtualenvs\pytemperatureconverter-4KrmmL8q-py3.11\Scripts\python.exe
 cachedir: .pytest_cache
```

### Comparing `pytemperatureconverter-0.1.0/PKG-INFO` & `pytemperatureconverter-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytemperatureconverter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Zeeshan Khalid
 Author-email: nszeeshankhalid@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -35,19 +35,19 @@
 kelvin_to_rankine(k): Converts Kelvin to Rankine.
 rankine_to_celsius(r): Converts Rankine to Celsius.
 rankine_to_fahrenheit(r): Converts Rankine to Fahrenheit.
 rankine_to_kelvin(r): Converts Rankine to Kelvin.
 
 Each function takes a numeric value as an argument and returns a numeric value as a result. For example:
 
->>> converter.celsius_to_fahrenheit(0)
+converter.celsius_to_fahrenheit(0)
 32.0
->>> converter.fahrenheit_to_kelvin(32)
+converter.fahrenheit_to_kelvin(32)
 273.15
->>> converter.kelvin_to_rankine(273.15)
+converter.kelvin_to_rankine(273.15)
 491.67
 ## Testing
 
 The functions have been tested using pytest.
 ============================= test session starts =============================
 platform win32 -- Python 3.11.0, pytest-7.3.0, pluggy-1.0.0 -- C:\Users\username\AppData\Local\pypoetry\Cache\virtualenvs\pytemperatureconverter-4KrmmL8q-py3.11\Scripts\python.exe
 cachedir: .pytest_cache
```

