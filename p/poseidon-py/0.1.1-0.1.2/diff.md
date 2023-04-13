# Comparing `tmp/poseidon_py-0.1.1.tar.gz` & `tmp/poseidon_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseidon_py-0.1.1.tar", last modified: Fri Apr  7 09:13:20 2023, max compression
+gzip compressed data, was "poseidon_py-0.1.2.tar", last modified: Thu Apr 13 08:18:26 2023, max compression
```

## Comparing `poseidon_py-0.1.1.tar` & `poseidon_py-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/poseidon/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/.git
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/poseidon/sage/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/low_level.sage
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon.sage
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon3_data.sage
--rw-r--r--   0 runner    (1001) docker     (123)    32794 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon4_data.sage
--rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon5_data.sage
--rw-r--r--   0 runner    (1001) docker     (123)    72459 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon9_data.sage
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/poseidon_variant.sage
--rw-r--r--   0 runner    (1001) docker     (123)    59375 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/print_c_round_cst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/print_c_round_cst.sage
--rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/test_clib.sage
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sage/tests.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/poseidon/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/f251.c
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/f251.h
--rw-r--r--   0 runner    (1001) docker     (123)    29612 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/f251_asm.s
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/poseidon.c
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/poseidon.h
--rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/poseidon_rc.c
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/poseidon_rc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-07 09:13:19.000000 poseidon_py-0.1.1/poseidon/sources/test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/poseidon_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/poseidon_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/poseidon_py/c_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/poseidon_py/poseidon_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/poseidon_py/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/poseidon_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-07 09:13:20.000000 poseidon_py-0.1.1/poseidon_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-07 09:13:20.000000 poseidon_py-0.1.1/poseidon_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 09:13:20.000000 poseidon_py-0.1.1/poseidon_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 09:13:20.000000 poseidon_py-0.1.1/poseidon_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 09:13:20.000000 poseidon_py-0.1.1/poseidon_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 09:13:20.408841 poseidon_py-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-07 09:13:18.000000 poseidon_py-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/poseidon/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/poseidon/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/low_level.sage
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon3_data.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    32794 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon4_data.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon5_data.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    72459 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon9_data.sage
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/poseidon_variant.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    59375 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/print_c_round_cst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/print_c_round_cst.sage
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/test_clib.sage
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sage/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/poseidon/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/f251.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/f251.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29612 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/f251_asm.s
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/poseidon.c
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/poseidon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/poseidon_rc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/poseidon_rc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon/sources/test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/poseidon_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon_py/c_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon_py/poseidon_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/poseidon_py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/poseidon_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 08:18:26.000000 poseidon_py-0.1.2/poseidon_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-13 08:18:26.000000 poseidon_py-0.1.2/poseidon_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:18:26.000000 poseidon_py-0.1.2/poseidon_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 08:18:26.000000 poseidon_py-0.1.2/poseidon_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:18:26.106868 poseidon_py-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 08:18:24.000000 poseidon_py-0.1.2/setup.py
```

### Comparing `poseidon_py-0.1.1/PKG-INFO` & `poseidon_py-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: poseidon_py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of Poseidon hash
 Home-page: https://github.com/drknzz/poseidon-py.git
 Author: drknzz
 Author-email: kamil.jankowski.x@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
-Provides-Extra: build
 
 poseidon-py
 ===========
 
 Poseidon hash Python library with Hades permutation `implemented in C <https://github.com/CryptoExperts/poseidon>`_.
 
 Currently, the parameters for poseidon hash are set to define the permutation used in Starknet.
```

### Comparing `poseidon_py-0.1.1/poseidon/README.md` & `poseidon_py-0.1.2/poseidon/README.md`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/low_level.sage` & `poseidon_py-0.1.2/poseidon/sage/low_level.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon3_data.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon3_data.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon4_data.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon4_data.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon5_data.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon5_data.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon9_data.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon9_data.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/poseidon_variant.sage` & `poseidon_py-0.1.2/poseidon/sage/poseidon_variant.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/print_c_round_cst.ipynb` & `poseidon_py-0.1.2/poseidon/sage/print_c_round_cst.ipynb`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/print_c_round_cst.sage` & `poseidon_py-0.1.2/poseidon/sage/print_c_round_cst.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/test_clib.sage` & `poseidon_py-0.1.2/poseidon/sage/test_clib.sage`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sage/tests.ipynb` & `poseidon_py-0.1.2/poseidon/sage/tests.ipynb`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/Makefile` & `poseidon_py-0.1.2/poseidon/sources/Makefile`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/f251.c` & `poseidon_py-0.1.2/poseidon/sources/f251.c`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/f251.h` & `poseidon_py-0.1.2/poseidon/sources/f251.h`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/f251_asm.s` & `poseidon_py-0.1.2/poseidon/sources/f251_asm.s`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/poseidon.c` & `poseidon_py-0.1.2/poseidon/sources/poseidon.c`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/poseidon.h` & `poseidon_py-0.1.2/poseidon/sources/poseidon.h`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/poseidon_rc.c` & `poseidon_py-0.1.2/poseidon/sources/poseidon_rc.c`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon/sources/test.c` & `poseidon_py-0.1.2/poseidon/sources/test.c`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon_py/c_bindings.py` & `poseidon_py-0.1.2/poseidon_py/c_bindings.py`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon_py/poseidon_hash.py` & `poseidon_py-0.1.2/poseidon_py/poseidon_hash.py`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon_py/utils.py` & `poseidon_py-0.1.2/poseidon_py/utils.py`

 * *Files identical despite different names*

### Comparing `poseidon_py-0.1.1/poseidon_py.egg-info/PKG-INFO` & `poseidon_py-0.1.2/poseidon_py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: poseidon-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of Poseidon hash
 Home-page: https://github.com/drknzz/poseidon-py.git
 Author: drknzz
 Author-email: kamil.jankowski.x@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
-Provides-Extra: build
 
 poseidon-py
 ===========
 
 Poseidon hash Python library with Hades permutation `implemented in C <https://github.com/CryptoExperts/poseidon>`_.
 
 Currently, the parameters for poseidon hash are set to define the permutation used in Starknet.
```

### Comparing `poseidon_py-0.1.1/poseidon_py.egg-info/SOURCES.txt` & `poseidon_py-0.1.2/poseidon_py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,8 @@
 poseidon_py/__init__.py
 poseidon_py/c_bindings.py
 poseidon_py/poseidon_hash.py
 poseidon_py/utils.py
 poseidon_py.egg-info/PKG-INFO
 poseidon_py.egg-info/SOURCES.txt
 poseidon_py.egg-info/dependency_links.txt
-poseidon_py.egg-info/requires.txt
 poseidon_py.egg-info/top_level.txt
```

### Comparing `poseidon_py-0.1.1/setup.py` & `poseidon_py-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,21 +28,20 @@
 
 if __name__ == "__main__":
     with open("README.rst", encoding="utf-8") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="poseidon_py",
-        version="0.1.1",
+        version="0.1.2",
         description="Python implementation of Poseidon hash",
         long_description=long_description,
         author="drknzz",
         author_email="kamil.jankowski.x@gmail.com",
         url="https://github.com/drknzz/poseidon-py.git",
-        extras_require={"build": ["make"]},
         ext_modules=[PoseidonExtension()],
         cmdclass={
             "build_py": BuildPy,
             "build_ext": BuildPoseidon,
         },
         python_requires=">=3.9",
         packages=["poseidon_py"],
```

