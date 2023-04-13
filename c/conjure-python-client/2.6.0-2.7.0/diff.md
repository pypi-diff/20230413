# Comparing `tmp/conjure-python-client-2.6.0.tar.gz` & `tmp/conjure-python-client-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjure-python-client-2.6.0.tar", last modified: Wed Mar 15 15:34:47 2023, max compression
+gzip compressed data, was "conjure-python-client-2.7.0.tar", last modified: Thu Mar 16 01:26:02 2023, max compression
```

## Comparing `conjure-python-client-2.6.0.tar` & `conjure-python-client-2.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.399025 conjure-python-client-2.6.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2023-03-15 15:34:47.399025 conjure-python-client-2.6.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1041 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.395025 conjure-python-client-2.6.0/conjure_python_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.395025 conjure-python-client-2.6.0/conjure_python_client/_http/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_http/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_http/configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9318 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_http/requests_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.395025 conjure-python-client-2.6.0/conjure_python_client/_lib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_lib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_lib/case.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1379 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_lib/sanitize.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4358 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_lib/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.399025 conjure-python-client-2.6.0/conjure_python_client/_serde/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      748 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_serde/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10956 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_serde/decoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3060 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/_serde/encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/conjure_python_client/py.typed
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.395025 conjure-python-client-2.6.0/conjure_python_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      790 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-03-15 15:34:47.000000 conjure-python-client-2.6.0/conjure_python_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-15 15:34:47.399025 conjure-python-client-2.6.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3446 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 15:34:47.399025 conjure-python-client-2.6.0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6219 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/test/test_http.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      774 2023-03-15 15:34:39.000000 conjure-python-client-2.6.0/test/test_version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.954839 conjure-python-client-2.7.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2023-03-16 01:26:02.954839 conjure-python-client-2.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1041 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/conjure_python_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/conjure_python_client/_http/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_http/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_http/configuration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9318 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_http/requests_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/conjure_python_client/_lib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_lib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_lib/case.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1379 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_lib/sanitize.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4358 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_lib/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/conjure_python_client/_serde/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      748 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_serde/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11006 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_serde/decoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3060 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/_serde/encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/conjure_python_client/py.typed
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/conjure_python_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      790 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-03-16 01:26:02.000000 conjure-python-client-2.7.0/conjure_python_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-16 01:26:02.954839 conjure-python-client-2.7.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3446 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 01:26:02.950839 conjure-python-client-2.7.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6219 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/test/test_http.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      774 2023-03-16 01:25:56.000000 conjure-python-client-2.7.0/test/test_version.py
```

### Comparing `conjure-python-client-2.6.0/LICENSE` & `conjure-python-client-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/PKG-INFO` & `conjure-python-client-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: conjure-python-client
-Version: 2.6.0
+Version: 2.7.0
 Summary: Conjure Python Library
 Home-page: https://github.com/palantir/conjure-python-client
 Author: Palantir Technologies, Inc.
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conjure-python-client-2.6.0/README.md` & `conjure-python-client-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/__init__.py` & `conjure-python-client-2.7.0/conjure_python_client/__init__.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_http/__init__.py` & `conjure-python-client-2.7.0/conjure_python_client/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_http/configuration.py` & `conjure-python-client-2.7.0/conjure_python_client/_http/configuration.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_http/requests_client.py` & `conjure-python-client-2.7.0/conjure_python_client/_http/requests_client.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_lib/__init__.py` & `conjure-python-client-2.7.0/conjure_python_client/_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_lib/case.py` & `conjure-python-client-2.7.0/conjure_python_client/_lib/case.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_lib/sanitize.py` & `conjure-python-client-2.7.0/conjure_python_client/_lib/sanitize.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_lib/types.py` & `conjure-python-client-2.7.0/conjure_python_client/_lib/types.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_serde/__init__.py` & `conjure-python-client-2.7.0/conjure_python_client/_serde/__init__.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_serde/decoder.py` & `conjure-python-client-2.7.0/conjure_python_client/_serde/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,16 @@
         else:
             value = obj[type_of_union]
             field_type = conjure_field_definition.field_type
             deserialized[attribute] = cls.do_decode(value, field_type)
 
         # for backwards compatibility with conjure-python,
         # only pass in arg type_of_union if it is expected
-        if 'type_of_union' in conjure_type.__code__.co_varnames:
+        param_dict = inspect.signature(conjure_type.__init__).parameters
+        if 'type_of_union' in param_dict:
             deserialized['type_of_union'] = type_of_union
         return conjure_type(**deserialized)
 
     @classmethod
     def decode_conjure_enum_type(cls, obj, conjure_type):
         """Decodes json into a conjure enum type.
```

### Comparing `conjure-python-client-2.6.0/conjure_python_client/_serde/encoder.py` & `conjure-python-client-2.7.0/conjure_python_client/_serde/encoder.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/conjure_python_client.egg-info/PKG-INFO` & `conjure-python-client-2.7.0/conjure_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: conjure-python-client
-Version: 2.6.0
+Version: 2.7.0
 Summary: Conjure Python Library
 Home-page: https://github.com/palantir/conjure-python-client
 Author: Palantir Technologies, Inc.
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conjure-python-client-2.6.0/conjure_python_client.egg-info/SOURCES.txt` & `conjure-python-client-2.7.0/conjure_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/setup.py` & `conjure-python-client-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/test/test_http.py` & `conjure-python-client-2.7.0/test/test_http.py`

 * *Files identical despite different names*

### Comparing `conjure-python-client-2.6.0/test/test_version.py` & `conjure-python-client-2.7.0/test/test_version.py`

 * *Files identical despite different names*

