# Comparing `tmp/gsd-2.8.0.tar.gz` & `tmp/gsd-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-2.8.0.tar", last modified: Fri Feb 24 18:32:54 2023, max compression
+gzip compressed data, was "gsd-2.8.1.tar", last modified: Thu Apr 13 17:58:09 2023, max compression
```

## Comparing `gsd-2.8.0.tar` & `gsd-2.8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:32:54.540664 gsd-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-24 18:32:48.000000 gsd-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-24 18:32:48.000000 gsd-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-24 18:32:54.540664 gsd-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-02-24 18:32:48.000000 gsd-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:32:54.540664 gsd-2.8.0/gsd/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   698624 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (123)    36552 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    70085 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (123)    46531 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:32:54.540664 gsd-2.8.0/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (123)    34320 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-24 18:32:48.000000 gsd-2.8.0/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:32:54.540664 gsd-2.8.0/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-24 18:32:54.000000 gsd-2.8.0/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-24 18:32:48.000000 gsd-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-24 18:32:54.540664 gsd-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-02-24 18:32:48.000000 gsd-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 17:58:00.000000 gsd-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 17:58:00.000000 gsd-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 17:58:09.712750 gsd-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-13 17:58:00.000000 gsd-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   700278 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36552 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    70351 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46531 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (123)    34320 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 17:58:00.000000 gsd-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-13 17:58:09.716750 gsd-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 17:58:00.000000 gsd-2.8.1/setup.py
```

### Comparing `gsd-2.8.0/LICENSE` & `gsd-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/PKG-INFO` & `gsd-2.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.8.0
+Version: 2.8.1
 Summary: General simulation data file format.
 Home-page: https://gsd.readthedocs.io
 Author: Joshua A. Anderson
 Author-email: joaander@umich.edu
 License: BSD - 2 clause
-Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.0/gsd-v2.8.0.tar.gz
+Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.1/gsd-v2.8.1.tar.gz
 Project-URL: Documentation, https://gsd.readthedocs.io
 Project-URL: Source Code, https://github.com/glotzerlab/gsd
 Project-URL: Issue Tracker, https://github.com/glotzerlab/gsd/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gsd-2.8.0/README.md` & `gsd-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/__init__.py` & `gsd-2.8.1/gsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/__main__.py` & `gsd-2.8.1/gsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/fl.c` & `gsd-2.8.1/gsd/fl.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -230,15 +230,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -269,15 +269,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1731,20 +1731,28 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -11996,52 +12004,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12910,28 +12933,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -14358,44 +14381,62 @@
 }
 #endif
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `gsd-2.8.0/gsd/fl.pyx` & `gsd-2.8.1/gsd/fl.pyx`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/gsd.c` & `gsd-2.8.1/gsd/gsd.c`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,24 @@
 
 /// Size of initial frame index
 enum
     {
     GSD_INITIAL_FRAME_INDEX_SIZE = 16
     };
 
-/// Size of write buffer
+/// Initial size of write buffer
 enum
     {
-    GSD_WRITE_BUFFER_SIZE = 16 * 1024 * 1024
+    GSD_INITIAL_WRITE_BUFFER_SIZE = 1024
+    };
+
+/// Maximum size of write buffer
+enum
+    {
+    GSD_MAXIMUM_WRITE_BUFFER_SIZE = 16 * 1024 * 1024
     };
 
 /// Size of copy buffer
 enum
     {
     GSD_COPY_BUFFER_SIZE = 128 * 1024
     };
@@ -1566,15 +1572,15 @@
 
         retval = gsd_index_buffer_allocate(&handle->buffer_index, GSD_INITIAL_FRAME_INDEX_SIZE);
         if (retval != GSD_SUCCESS)
             {
             return retval;
             }
 
-        retval = gsd_byte_buffer_allocate(&handle->write_buffer, GSD_WRITE_BUFFER_SIZE);
+        retval = gsd_byte_buffer_allocate(&handle->write_buffer, GSD_INITIAL_WRITE_BUFFER_SIZE);
         if (retval != GSD_SUCCESS)
             {
             return retval;
             }
 
         handle->frame_names.n_names = 0;
         retval = gsd_byte_buffer_allocate(&handle->frame_names.data, GSD_NAME_SIZE);
@@ -1890,14 +1896,21 @@
     // flush the write buffer
     retval = gsd_flush_write_buffer(handle);
     if (retval != GSD_SUCCESS)
         {
         return retval;
         }
 
+    // sync the data before writing the index
+    retval = fsync(handle->fd);
+    if (retval != 0)
+        {
+        return GSD_ERROR_IO;
+        }
+
     // write the frame index to the file
     if (handle->frame_index.size > 0)
         {
         // ensure there is enough space in the index
         if ((handle->file_index.size + handle->frame_index.size) > handle->file_index.reserved)
             {
             gsd_expand_file_index(handle, handle->file_index.size + handle->frame_index.size);
@@ -1990,18 +2003,18 @@
     entry.id = id;
     entry.type = (uint8_t)type;
     entry.N = N;
     entry.M = M;
     size_t size = N * M * gsd_sizeof_type(type);
 
     // decide whether to write this chunk to the buffer or straight to disk
-    if (size < handle->write_buffer.reserved / 2)
+    if (size < GSD_MAXIMUM_WRITE_BUFFER_SIZE / 2)
         {
         // flush the buffer if this entry won't fit
-        if (size > (handle->write_buffer.reserved - handle->write_buffer.size))
+        if (size > (GSD_MAXIMUM_WRITE_BUFFER_SIZE - handle->write_buffer.size))
             {
             gsd_flush_write_buffer(handle);
             }
 
         entry.location = handle->write_buffer.size;
 
         // add an entry to the buffer index
```

### Comparing `gsd-2.8.0/gsd/gsd.h` & `gsd-2.8.1/gsd/gsd.h`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/hoomd.py` & `gsd-2.8.1/gsd/hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/libgsd.pxd` & `gsd-2.8.1/gsd/libgsd.pxd`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/pygsd.py` & `gsd-2.8.1/gsd/pygsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from __future__ import division
 import logging
 import numpy
 import struct
 from collections import namedtuple
 import sys
 
-__version__ = "2.8.0"
+__version__ = "2.8.1"
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
```

### Comparing `gsd-2.8.0/gsd/pytest_plugin_validate.py` & `gsd-2.8.1/gsd/pytest_plugin_validate.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/test/conftest.py` & `gsd-2.8.1/gsd/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/test/test_fl.py` & `gsd-2.8.1/gsd/test/test_fl.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/test/test_gsd_v1.gsd` & `gsd-2.8.1/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/test/test_hoomd.py` & `gsd-2.8.1/gsd/test/test_hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd/test/test_largefile.py` & `gsd-2.8.1/gsd/test/test_largefile.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/gsd.egg-info/PKG-INFO` & `gsd-2.8.1/gsd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.8.0
+Version: 2.8.1
 Summary: General simulation data file format.
 Home-page: https://gsd.readthedocs.io
 Author: Joshua A. Anderson
 Author-email: joaander@umich.edu
 License: BSD - 2 clause
-Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.0/gsd-v2.8.0.tar.gz
+Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.1/gsd-v2.8.1.tar.gz
 Project-URL: Documentation, https://gsd.readthedocs.io
 Project-URL: Source Code, https://github.com/glotzerlab/gsd
 Project-URL: Issue Tracker, https://github.com/glotzerlab/gsd/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gsd-2.8.0/gsd.egg-info/SOURCES.txt` & `gsd-2.8.1/gsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/pyproject.toml` & `gsd-2.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/setup.cfg` & `gsd-2.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gsd-2.8.0/setup.py` & `gsd-2.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     with open(readme_file) as f:
         readme = f.read()
 except ImportError:
     readme = desc
 
 
 setup(name='gsd',
-      version='2.8.0',
+      version='2.8.1',
       description=desc,
       long_description=readme,
       long_description_content_type='text/markdown',
       license='BSD - 2 clause',
       author='Joshua A. Anderson',
       author_email='joaander@umich.edu',
       url='https://gsd.readthedocs.io',
-      download_url='https://github.com/glotzerlab/gsd/releases/download/v2.8.0'
-                   '/gsd-v2.8.0.tar.gz',
+      download_url='https://github.com/glotzerlab/gsd/releases/download/v2.8.1'
+                   '/gsd-v2.8.1.tar.gz',
       project_urls={
           "Documentation": "https://gsd.readthedocs.io",
           "Source Code": "https://github.com/glotzerlab/gsd",
           "Issue Tracker": "https://github.com/glotzerlab/gsd/issues",
       },
 
       classifiers=[
```

