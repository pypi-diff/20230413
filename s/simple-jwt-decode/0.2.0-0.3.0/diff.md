# Comparing `tmp/simple_jwt_decode-0.2.0.tar.gz` & `tmp/simple_jwt_decode-0.3.0.tar.gz`

## Comparing `simple_jwt_decode-0.2.0.tar` & `simple_jwt_decode-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/src/simple_jwt/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/src/simple_jwt/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/src/simple_jwt/jwt.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/tests/test_jwt.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/README.md
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 simple_jwt_decode-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/src/simple_jwt/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/src/simple_jwt/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/src/simple_jwt/jwt.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/tests/test_jwt.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/README.md
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 simple_jwt_decode-0.3.0/PKG-INFO
```

### Comparing `simple_jwt_decode-0.2.0/src/simple_jwt/jwt.py` & `simple_jwt_decode-0.3.0/src/simple_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.2.0/tests/test_jwt.py` & `simple_jwt_decode-0.3.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.2.0/.gitignore` & `simple_jwt_decode-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.2.0/LICENSE.txt` & `simple_jwt_decode-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.2.0/README.md` & `simple_jwt_decode-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     - [Decode](#decode)
     - [Expired](#expired)
   - [License](#license)
 
 ## Installation
 
 ```console
-pip install simple-jwt
+pip install simple-jwt-decode
 ```
 
 ## Usage
 
 ### Decode
 ```console
 from simple_jwt import jwt
```

### Comparing `simple_jwt_decode-0.2.0/pyproject.toml` & `simple_jwt_decode-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.2.0/PKG-INFO` & `simple_jwt_decode-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-jwt-decode
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/u-clarkdeveloper/simple-jwt#readme
 Project-URL: Issues, https://github.com/u-clarkdeveloper/simple-jwt/issues
 Project-URL: Source, https://github.com/u-clarkdeveloper/simple-jwt
 Author-email: Jesse Clark <jesse@clarkdeveloper.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
     - [Decode](#decode)
     - [Expired](#expired)
   - [License](#license)
 
 ## Installation
 
 ```console
-pip install simple-jwt
+pip install simple-jwt-decode
 ```
 
 ## Usage
 
 ### Decode
 ```console
 from simple_jwt import jwt
```

