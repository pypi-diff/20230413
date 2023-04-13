# Comparing `tmp/simple_jwt_decode-0.4.0.tar.gz` & `tmp/simple_jwt_decode-0.5.0.tar.gz`

## Comparing `simple_jwt_decode-0.4.0.tar` & `simple_jwt_decode-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/src/simple_jwt/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/src/simple_jwt/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/src/simple_jwt/jwt.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/tests/test_jwt.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/README.md
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 simple_jwt_decode-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/jwt.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/tests/test_jwt.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/README.md
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/PKG-INFO
```

### Comparing `simple_jwt_decode-0.4.0/src/simple_jwt/jwt.py` & `simple_jwt_decode-0.5.0/src/simple_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.4.0/tests/test_jwt.py` & `simple_jwt_decode-0.5.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.4.0/.gitignore` & `simple_jwt_decode-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.4.0/LICENSE.txt` & `simple_jwt_decode-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.4.0/README.md` & `simple_jwt_decode-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.4.0/pyproject.toml` & `simple_jwt_decode-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple-jwt-decode"
 dynamic = ["version"]
-description = ''
+description = 'Simple Python Package for decoding JWT claims and checking if its expired. No verification of signatures.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Jesse Clark", email = "jesse@clarkdeveloper.com" },
 ]
```

### Comparing `simple_jwt_decode-0.4.0/PKG-INFO` & `simple_jwt_decode-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: simple-jwt-decode
-Version: 0.4.0
+Version: 0.5.0
+Summary: Simple Python Package for decoding JWT claims and checking if its expired. No verification of signatures.
 Project-URL: Documentation, https://github.com/u-clarkdeveloper/simple-jwt#readme
 Project-URL: Issues, https://github.com/u-clarkdeveloper/simple-jwt/issues
 Project-URL: Source, https://github.com/u-clarkdeveloper/simple-jwt
 Author-email: Jesse Clark <jesse@clarkdeveloper.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

