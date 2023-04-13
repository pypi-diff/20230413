# Comparing `tmp/arraymap-0.1.1.tar.gz` & `tmp/arraymap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.1.tar", last modified: Wed Apr 12 15:54:20 2023, max compression
+gzip compressed data, was "arraymap-0.1.2.tar", last modified: Thu Apr 13 00:33:21 2023, max compression
```

## Comparing `arraymap-0.1.1.tar` & `arraymap-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 15:54:17.000000 arraymap-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 15:54:17.000000 arraymap-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 15:54:20.002659 arraymap-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 15:54:17.000000 arraymap-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    60734 2023-04-12 15:54:17.000000 arraymap-0.1.1/arraymap.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/arraymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 15:54:20.002659 arraymap-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 15:54:17.000000 arraymap-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-12 15:54:17.000000 arraymap-0.1.1/test/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-04-12 15:54:17.000000 arraymap-0.1.1/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 00:33:16.000000 arraymap-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 00:33:16.000000 arraymap-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 00:33:21.326186 arraymap-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 00:33:16.000000 arraymap-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    60830 2023-04-13 00:33:16.000000 arraymap-0.1.2/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 00:33:21.326186 arraymap-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-13 00:33:16.000000 arraymap-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-13 00:33:16.000000 arraymap-0.1.2/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-04-13 00:33:16.000000 arraymap-0.1.2/test/test_unit.py
```

### Comparing `arraymap-0.1.1/LICENSE.md` & `arraymap-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.1/PKG-INFO` & `arraymap-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -31,14 +31,19 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.2
+-------
+
+Corrected segfault resulting from initialization from generators that raise.
+
 
 0.1.1
 -------
 
 Added `__version__` to module; releasing wheels.
```

### Comparing `arraymap-0.1.1/README.md` & `arraymap-0.1.2/arraymap.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: arraymap
+Version: 0.1.2
+Summary: Dictionary-like lookup from NumPy array values to their integer positions
+Home-page: https://github.com/static-frame/arraymap
+Author: Christopher Ariza, Brandt Bucher
+License: MIT
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 
 arraymap
 ============
 
 The ArrayMap library provides dictionary-like lookup from NumPy array values to their integer positions. The hash table design and C implementation is based on [AutoMap](https://github.com/brandtbucher/automap), with extensive additions for direct support of NumPy arrays.
 
 
@@ -20,14 +31,19 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.2
+-------
+
+Corrected segfault resulting from initialization from generators that raise.
+
 
 0.1.1
 -------
 
 Added `__version__` to module; releasing wheels.
```

### Comparing `arraymap-0.1.1/arraymap.c` & `arraymap-0.1.2/arraymap.c`

 * *Files 0% similar despite different names*

```diff
@@ -1185,15 +1185,19 @@
         return -1;
     }
     return self->table[table_pos].keys_pos;
 }
 
 // Insert a key_pos, hash pair into the table. Assumes table already has appropriate size. When inserting a new itme, `hash` is -1, forcing a fresh hash to be computed here. Return 0 on success, -1 on error.
 static int
-insert_obj(FAMObject *self, PyObject *key, Py_ssize_t keys_pos, Py_hash_t hash)
+insert_obj(
+        FAMObject *self,
+        PyObject *key,
+        Py_ssize_t keys_pos,
+        Py_hash_t hash)
 {
     if (hash == -1) {
         hash = PyObject_Hash(key);
         if (hash == -1) {
             return -1;
         }
     }
@@ -1815,66 +1819,71 @@
 
     if (!PyArg_UnpackTuple(args, name, 0, 1, &keys)) {
         return -1;
     }
 
     if (!keys) {
         keys = PyList_New(0);
+        if (!keys) {
+            return -1;
+        }
     }
     else if (PyObject_TypeCheck(keys, &FAMType)) {
         // Use `keys` as old, `self` as new, and fill from old to new. This returns the same error codes as this function.
         return copy_to_new(cls, (FAMObject*)keys, fam);
     }
     else if (PyArray_Check(keys)) {
         PyArrayObject *a = (PyArrayObject *)keys;
         if (PyArray_NDIM(a) != 1) {
             PyErr_SetString(PyExc_TypeError, "Arrays must be 1-dimensional");
             return -1;
         }
         int array_t = PyArray_TYPE(a);
+        keys_size = PyArray_SIZE(a);
+
         if (cls != &AMType &&
                 (PyTypeNum_ISINTEGER(array_t) // signed and unsigned
                 || PyTypeNum_ISFLOAT(array_t)
                 || PyTypeNum_ISFLEXIBLE(array_t))
             ){
             if ((PyArray_FLAGS(a) & NPY_ARRAY_WRITEABLE)) {
                 PyErr_Format(PyExc_TypeError, "Arrays must be immutable when given to a %s", name);
                 return -1;
             }
             keys_array_type = at_to_kat(array_t);
             Py_INCREF(keys);
         }
-        else { // if an AutoMap or an array that we do not custom-hash, we create a list
+        else { // if an AutoMap or an array that we do not handle, create a list
             if (array_t == NPY_DATETIME || array_t == NPY_TIMEDELTA){
                 keys = PySequence_List(keys); // force scalars
             }
             else {
                 keys = PyArray_ToList(a); // converts to objs
             }
+            if (!keys) {
+                return -1;
+            }
         }
-        keys_size = PyArray_SIZE(a);
     }
     else { // assume an arbitrary iterable
         keys = PySequence_List(keys);
+        if (!keys) {
+            return -1;
+        }
         keys_size = PyList_GET_SIZE(keys);
     }
 
-    if (!keys) {
-        return -1;
-    }
-
     fam->keys = keys;
     fam->keys_array_type = keys_array_type;
     fam->keys_size = keys_size;
     fam->key_buffer = NULL;
     key_count_global += keys_size;
 
     // NOTE: on itialization, grow_table() does not use keys
     if (grow_table(fam, keys_size)) {
-        // assume `fam->keys` will be decrefed by the caller
         return -1;
     }
     Py_ssize_t i = 0;
     if (keys_array_type) {
         PyArrayObject *a = (PyArrayObject *)fam->keys;
         int contiguous = PyArray_IS_C_CONTIGUOUS(a);
         switch (keys_array_type) {
```

### Comparing `arraymap-0.1.1/setup.py` & `arraymap-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import typing as tp
 import site
 import os
 
 
-AM_VERSION = "0.1.1"
+AM_VERSION = "0.1.2"
 
 
 with open("README.md") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
```

### Comparing `arraymap-0.1.1/test/test_property.py` & `arraymap-0.1.2/test/test_property.py`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.1/test/test_unit.py` & `arraymap-0.1.2/test/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import sys
 import numpy as np
 
 from arraymap import AutoMap
 from arraymap import FrozenAutoMap
 from arraymap import NonUniqueError
 
+
 def test_version():
     import arraymap
+
     assert isinstance(arraymap.__version__, str)
 
 
 # ------------------------------------------------------------------------------
 
 
 def test_am_extend():
@@ -37,14 +39,28 @@
     # NOTE: exercise x to force seg fault
     assert len(x) == 0
 
 
 # ------------------------------------------------------------------------------
 
 
+def test_fam_constructor_a():
+    with pytest.raises(ZeroDivisionError):
+        fam = FrozenAutoMap((x / 0 for x in range(3)))
+
+
+def test_fam_constructor_b():
+    fam1 = FrozenAutoMap(range(3))
+    fam2 = FrozenAutoMap(fam1)
+    assert list(fam2), [0, 1, 2]
+
+
+# ------------------------------------------------------------------------------
+
+
 def test_fam_constructor_array_int_a1():
     a1 = np.array((10, 20, 30), dtype=np.int64)
     with pytest.raises(TypeError):
         fam = FrozenAutoMap(a1)
 
 
 def test_fam_constructor_array_int_a2():
```

