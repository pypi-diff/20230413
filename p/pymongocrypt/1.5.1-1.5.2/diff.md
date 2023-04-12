# Comparing `tmp/pymongocrypt-1.5.1.tar.gz` & `tmp/pymongocrypt-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongocrypt-1.5.1.tar", last modified: Mon Feb  6 20:37:25 2023, max compression
+gzip compressed data, was "pymongocrypt-1.5.2.tar", last modified: Wed Apr 12 21:57:19 2023, max compression
```

## Comparing `pymongocrypt-1.5.1.tar` & `pymongocrypt-1.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-02-06 20:37:25.192347 pymongocrypt-1.5.1/
--rw-r--r--   0 mci        (500) admin       (80)    11357 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/LICENSE
--rw-r--r--   0 mci        (500) admin       (80)     8823 2023-02-06 20:37:25.192116 pymongocrypt-1.5.1/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)     7381 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/README.rst
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-02-06 20:37:25.189798 pymongocrypt-1.5.1/pymongocrypt/
--rw-r--r--   0 mci        (500) admin       (80)      687 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/__init__.py
--rw-r--r--   0 mci        (500) admin       (80)     2053 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/auto_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)     3156 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/binary.py
--rw-r--r--   0 mci        (500) admin       (80)    56936 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/binding.py
--rw-r--r--   0 mci        (500) admin       (80)     2073 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/compat.py
--rw-r--r--   0 mci        (500) admin       (80)     5119 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/credentials.py
--rw-r--r--   0 mci        (500) admin       (80)     6157 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/crypto.py
--rw-r--r--   0 mci        (500) admin       (80)     1393 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/errors.py
--rw-r--r--   0 mci        (500) admin       (80)    11125 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/explicit_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)    32890 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/mongocrypt.py
--rw-r--r--   0 mci        (500) admin       (80)     4850 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/state_machine.py
--rw-r--r--   0 mci        (500) admin       (80)      642 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/pymongocrypt/version.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-02-06 20:37:25.191126 pymongocrypt-1.5.1/pymongocrypt.egg-info/
--rw-r--r--   0 mci        (500) admin       (80)     8823 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)      622 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/SOURCES.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/dependency_links.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/not-zip-safe
--rw-r--r--   0 mci        (500) admin       (80)       49 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/requires.txt
--rw-r--r--   0 mci        (500) admin       (80)       13 2023-02-06 20:37:25.000000 pymongocrypt-1.5.1/pymongocrypt.egg-info/top_level.txt
--rw-r--r--   0 mci        (500) admin       (80)       38 2023-02-06 20:37:25.192403 pymongocrypt-1.5.1/setup.cfg
--rw-r--r--   0 mci        (500) admin       (80)     3368 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/setup.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-02-06 20:37:25.191791 pymongocrypt-1.5.1/test/
--rw-r--r--   0 mci        (500) admin       (80)     2398 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/test/test_binding.py
--rw-r--r--   0 mci        (500) admin       (80)     3479 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/test/test_crypto.py
--rw-r--r--   0 mci        (500) admin       (80)    35775 2023-02-06 20:37:21.000000 pymongocrypt-1.5.1/test/test_mongocrypt.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.230714 pymongocrypt-1.5.2/
+-rw-r--r--   0 mci        (500) admin       (80)    11357 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/LICENSE
+-rw-r--r--   0 mci        (500) admin       (80)     8823 2023-04-12 21:57:19.230465 pymongocrypt-1.5.2/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)     7381 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/README.rst
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.228023 pymongocrypt-1.5.2/pymongocrypt/
+-rw-r--r--   0 mci        (500) admin       (80)      687 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/__init__.py
+-rw-r--r--   0 mci        (500) admin       (80)     2053 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/auto_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)     3156 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/binary.py
+-rw-r--r--   0 mci        (500) admin       (80)    56936 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     2073 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/compat.py
+-rw-r--r--   0 mci        (500) admin       (80)     5119 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/credentials.py
+-rw-r--r--   0 mci        (500) admin       (80)     6157 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)     1393 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/errors.py
+-rw-r--r--   0 mci        (500) admin       (80)    11125 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/explicit_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)    32890 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/mongocrypt.py
+-rw-r--r--   0 mci        (500) admin       (80)     4850 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/state_machine.py
+-rw-r--r--   0 mci        (500) admin       (80)      642 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/version.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.229454 pymongocrypt-1.5.2/pymongocrypt.egg-info/
+-rw-r--r--   0 mci        (500) admin       (80)     8823 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)      622 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/not-zip-safe
+-rw-r--r--   0 mci        (500) admin       (80)      148 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/requires.txt
+-rw-r--r--   0 mci        (500) admin       (80)       13 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/top_level.txt
+-rw-r--r--   0 mci        (500) admin       (80)       38 2023-04-12 21:57:19.230773 pymongocrypt-1.5.2/setup.cfg
+-rw-r--r--   0 mci        (500) admin       (80)     3560 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/setup.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.230132 pymongocrypt-1.5.2/test/
+-rw-r--r--   0 mci        (500) admin       (80)     2398 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     3479 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)    35775 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_mongocrypt.py
```

### Comparing `pymongocrypt-1.5.1/LICENSE` & `pymongocrypt-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/PKG-INFO` & `pymongocrypt-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymongocrypt-1.5.1/README.rst` & `pymongocrypt-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/__init__.py` & `pymongocrypt-1.5.2/pymongocrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/auto_encrypter.py` & `pymongocrypt-1.5.2/pymongocrypt/auto_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/binary.py` & `pymongocrypt-1.5.2/pymongocrypt/binary.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/binding.py` & `pymongocrypt-1.5.2/pymongocrypt/binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/compat.py` & `pymongocrypt-1.5.2/pymongocrypt/compat.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/credentials.py` & `pymongocrypt-1.5.2/pymongocrypt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/crypto.py` & `pymongocrypt-1.5.2/pymongocrypt/crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/errors.py` & `pymongocrypt-1.5.2/pymongocrypt/errors.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/explicit_encrypter.py` & `pymongocrypt-1.5.2/pymongocrypt/explicit_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/mongocrypt.py` & `pymongocrypt-1.5.2/pymongocrypt/mongocrypt.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/state_machine.py` & `pymongocrypt-1.5.2/pymongocrypt/state_machine.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/pymongocrypt/version.py` & `pymongocrypt-1.5.2/pymongocrypt/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 _MIN_LIBMONGOCRYPT_VERSION = '1.7.0'
```

### Comparing `pymongocrypt-1.5.1/pymongocrypt.egg-info/PKG-INFO` & `pymongocrypt-1.5.2/pymongocrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymongocrypt-1.5.1/pymongocrypt.egg-info/SOURCES.txt` & `pymongocrypt-1.5.2/pymongocrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/setup.py` & `pymongocrypt-1.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,21 @@
     version=version['__version__'],
     description="Python bindings for libmongocrypt",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(exclude=['test']),
     package_data={'pymongocrypt': ['*.dll', '*.so', '*.dylib']},
     zip_safe=False,
     # Note cryptography is uncapped because it does not follow semver.
-    install_requires=["cffi>=1.12.0,<2", "cryptography>=2.0", "requests<3.0.0"],
+    install_requires=[
+        "cffi>=1.12.0,<2",
+        "cryptography>=2.0",
+        # cryptography 40 dropped support for PyPy <7.3.10.
+        "cryptography<40;platform_python_implementation=='PyPy' and implementation_version<'7.3.10'",
+        "requests<3.0.0"
+    ],
     author="Shane Harvey",
     author_email="mongodb-user@googlegroups.com",
     url="https://github.com/mongodb/libmongocrypt/tree/master/bindings/python",
     keywords=["mongo", "mongodb", "pymongocrypt", "pymongo", "mongocrypt",
               "bson"],
     test_suite="test",
     license="Apache License, Version 2.0",
```

### Comparing `pymongocrypt-1.5.1/test/test_binding.py` & `pymongocrypt-1.5.2/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/test/test_crypto.py` & `pymongocrypt-1.5.2/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.1/test/test_mongocrypt.py` & `pymongocrypt-1.5.2/test/test_mongocrypt.py`

 * *Files identical despite different names*

