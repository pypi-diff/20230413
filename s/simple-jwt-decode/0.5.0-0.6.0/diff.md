# Comparing `tmp/simple_jwt_decode-0.5.0.tar.gz` & `tmp/simple_jwt_decode-0.6.0.tar.gz`

## Comparing `simple_jwt_decode-0.5.0.tar` & `simple_jwt_decode-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/src/simple_jwt/jwt.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/tests/test_jwt.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/README.md
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 simple_jwt_decode-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/jwt.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/tests/test_jwt.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/README.md
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/PKG-INFO
```

### Comparing `simple_jwt_decode-0.5.0/src/simple_jwt/jwt.py` & `simple_jwt_decode-0.6.0/src/simple_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.5.0/tests/test_jwt.py` & `simple_jwt_decode-0.6.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.5.0/.gitignore` & `simple_jwt_decode-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.5.0/LICENSE.txt` & `simple_jwt_decode-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.5.0/README.md` & `simple_jwt_decode-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Simple JWT
-
-[![PyPI - Version](https://img.shields.io/pypi/v/simple-jwt.svg)](https://pypi.org/project/simple-jwt)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-jwt.svg)](https://pypi.org/project/simple-jwt)
+[![PyPI version](https://badge.fury.io/py/simple-jwt-decode.svg)](https://badge.fury.io/py/simple-jwt-decode)
 
 -----
 
 ## Why?
 
 I created this package because I found that I often needed to see the cliams of a JWT token and wether it was expired or not. I didn't need to verify it the signatures. I wanted a package to check if the token was expired, so I could refresh my token or take other actions based off that. Most other packages seemed to require verified signatures or would throw errors if a key was not provided. Just needed a simple package to get the cliams info and if the token was expired. Simple JWT.
```

### Comparing `simple_jwt_decode-0.5.0/pyproject.toml` & `simple_jwt_decode-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.5.0/PKG-INFO` & `simple_jwt_decode-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-jwt-decode
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple Python Package for decoding JWT claims and checking if its expired. No verification of signatures.
 Project-URL: Documentation, https://github.com/u-clarkdeveloper/simple-jwt#readme
 Project-URL: Issues, https://github.com/u-clarkdeveloper/simple-jwt/issues
 Project-URL: Source, https://github.com/u-clarkdeveloper/simple-jwt
 Author-email: Jesse Clark <jesse@clarkdeveloper.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -17,17 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Simple JWT
-
-[![PyPI - Version](https://img.shields.io/pypi/v/simple-jwt.svg)](https://pypi.org/project/simple-jwt)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-jwt.svg)](https://pypi.org/project/simple-jwt)
+[![PyPI version](https://badge.fury.io/py/simple-jwt-decode.svg)](https://badge.fury.io/py/simple-jwt-decode)
 
 -----
 
 ## Why?
 
 I created this package because I found that I often needed to see the cliams of a JWT token and wether it was expired or not. I didn't need to verify it the signatures. I wanted a package to check if the token was expired, so I could refresh my token or take other actions based off that. Most other packages seemed to require verified signatures or would throw errors if a key was not provided. Just needed a simple package to get the cliams info and if the token was expired. Simple JWT.
```

