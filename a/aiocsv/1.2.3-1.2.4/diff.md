# Comparing `tmp/aiocsv-1.2.3.tar.gz` & `tmp/aiocsv-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocsv-1.2.3.tar", last modified: Wed Oct 26 10:17:55 2022, max compression
+gzip compressed data, was "aiocsv-1.2.4.tar", last modified: Thu Apr 13 02:00:11 2023, max compression
```

## Comparing `aiocsv-1.2.3.tar` & `aiocsv-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-10-26 10:17:55.552840 aiocsv-1.2.3/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6638 2022-10-26 10:17:55.552840 aiocsv-1.2.3/PKG-INFO
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-10-26 10:17:55.552840 aiocsv-1.2.3/aiocsv/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      540 2022-10-26 10:15:12.000000 aiocsv-1.2.3/aiocsv/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)   324840 2022-10-26 10:10:41.000000 aiocsv-1.2.3/aiocsv/_parser.c
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      185 2022-04-16 11:11:11.000000 aiocsv-1.2.3/aiocsv/_parser.pyi
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6782 2021-05-07 22:10:44.000000 aiocsv-1.2.3/aiocsv/_parser.pyx
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6193 2021-05-07 22:10:44.000000 aiocsv-1.2.3/aiocsv/parser.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      332 2022-04-16 11:08:09.000000 aiocsv-1.2.3/aiocsv/protocols.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2022-04-16 11:11:31.000000 aiocsv-1.2.3/aiocsv/py.typed
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3044 2021-05-07 22:14:03.000000 aiocsv-1.2.3/aiocsv/readers.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3376 2021-05-07 22:10:44.000000 aiocsv-1.2.3/aiocsv/writers.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-10-26 10:17:55.552840 aiocsv-1.2.3/aiocsv.egg-info/
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     6638 2022-10-26 10:17:55.000000 aiocsv-1.2.3/aiocsv.egg-info/PKG-INFO
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)      370 2022-10-26 10:17:55.000000 aiocsv-1.2.3/aiocsv.egg-info/SOURCES.txt
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)        1 2022-10-26 10:17:55.000000 aiocsv-1.2.3/aiocsv.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2021-05-02 14:00:52.000000 aiocsv-1.2.3/aiocsv.egg-info/not-zip-safe
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)       46 2022-10-26 10:17:55.000000 aiocsv-1.2.3/aiocsv.egg-info/requires.txt
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)        7 2022-10-26 10:17:55.000000 aiocsv-1.2.3/aiocsv.egg-info/top_level.txt
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1060 2020-07-31 13:37:51.000000 aiocsv-1.2.3/license.md
--rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     6110 2021-05-08 00:01:28.000000 aiocsv-1.2.3/readme.md
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2022-10-26 10:17:55.552840 aiocsv-1.2.3/setup.cfg
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1588 2022-10-26 10:15:20.000000 aiocsv-1.2.3/setup.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-13 02:00:11.337509 aiocsv-1.2.4/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6638 2023-04-13 02:00:11.337509 aiocsv-1.2.4/PKG-INFO
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-13 02:00:11.333509 aiocsv-1.2.4/aiocsv/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      540 2023-04-13 01:59:44.000000 aiocsv-1.2.4/aiocsv/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12763 2022-10-27 10:01:48.000000 aiocsv-1.2.4/aiocsv/_nparser.c
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)   456174 2023-04-13 01:15:38.000000 aiocsv-1.2.4/aiocsv/_parser.c
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      185 2022-04-16 11:11:11.000000 aiocsv-1.2.4/aiocsv/_parser.pyi
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6782 2021-05-07 22:10:44.000000 aiocsv-1.2.4/aiocsv/_parser.pyx
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6193 2021-05-07 22:10:44.000000 aiocsv-1.2.4/aiocsv/parser.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      332 2022-04-16 11:08:09.000000 aiocsv-1.2.4/aiocsv/protocols.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2022-04-16 11:11:31.000000 aiocsv-1.2.4/aiocsv/py.typed
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3044 2021-05-07 22:14:03.000000 aiocsv-1.2.4/aiocsv/readers.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3376 2021-05-07 22:10:44.000000 aiocsv-1.2.4/aiocsv/writers.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-13 02:00:11.337509 aiocsv-1.2.4/aiocsv.egg-info/
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     6638 2023-04-13 02:00:11.000000 aiocsv-1.2.4/aiocsv.egg-info/PKG-INFO
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)      495 2023-04-13 02:00:11.000000 aiocsv-1.2.4/aiocsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-04-13 02:00:11.000000 aiocsv-1.2.4/aiocsv.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2021-05-02 14:00:52.000000 aiocsv-1.2.4/aiocsv.egg-info/not-zip-safe
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)       46 2023-04-13 02:00:11.000000 aiocsv-1.2.4/aiocsv.egg-info/requires.txt
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)        7 2023-04-13 02:00:11.000000 aiocsv-1.2.4/aiocsv.egg-info/top_level.txt
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1060 2020-07-31 13:37:51.000000 aiocsv-1.2.4/license.md
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     6110 2021-05-08 00:01:28.000000 aiocsv-1.2.4/readme.md
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-04-13 02:00:11.337509 aiocsv-1.2.4/setup.cfg
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1588 2023-04-13 01:59:56.000000 aiocsv-1.2.4/setup.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-13 02:00:11.337509 aiocsv-1.2.4/tests/
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1431 2020-08-01 11:03:26.000000 aiocsv-1.2.4/tests/test_dialects.py
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1674 2020-08-01 21:13:34.000000 aiocsv-1.2.4/tests/test_dict.py
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1048 2021-04-17 13:29:26.000000 aiocsv-1.2.4/tests/test_newlines.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5443 2021-05-07 22:10:44.000000 aiocsv-1.2.4/tests/test_parser.py
+-rw-rw-r--   0 mikolaj   (1000) mikolaj   (1000)     1364 2020-08-01 10:59:00.000000 aiocsv-1.2.4/tests/test_simple.py
```

### Comparing `aiocsv-1.2.3/PKG-INFO` & `aiocsv-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocsv
-Version: 1.2.3
+Version: 1.2.4
 Summary: Asynchronous CSV reading/writing
 Home-page: https://github.com/MKuranowski/aiocsv
 Author: Mikołaj Kuranowski
 Author-email: mkuranowski@gmail.com
 License: MIT
 Keywords: async asynchronous aiofiles csv tsv
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiocsv-1.2.3/aiocsv/__init__.py` & `aiocsv-1.2.4/aiocsv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __title__ = "aiocsv"
 __description__ = "Asynchronous CSV reading/writing"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 __url__ = "https://github.com/MKuranowski/aiocsv"
 __author__ = "Mikołaj Kuranowski"
 __email__ = "".join(chr(i) for i in [109, 107, 117, 114, 97, 110, 111, 119, 115, 107, 105,
                                      64, 103, 109, 97, 105, 108, 46, 99, 111, 109])
 
-__copyright__ = "© Copyright 2020-2021 Mikołaj Kuranowski"
+__copyright__ = "© Copyright 2020-2023 Mikołaj Kuranowski"
 __license__ = "MIT"
 
 from .readers import AsyncReader, AsyncDictReader
 from .writers import AsyncWriter, AsyncDictWriter
```

### Comparing `aiocsv-1.2.3/aiocsv/_parser.c` & `aiocsv-1.2.4/aiocsv/_parser.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 3.0.0b2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "aiocsv._parser",
         "sources": [
             "aiocsv/_parser.pyx"
@@ -11,28 +11,40 @@
     "module_name": "aiocsv._parser"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "3_0_0b2"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000B2
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -43,31 +55,90 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -84,76 +155,98 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PYSTON_VERSION)
+#elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
   #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
   #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
@@ -189,36 +282,34 @@
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
@@ -234,45 +325,67 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -294,78 +407,116 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -380,36 +531,36 @@
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
         PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
         PyCodeObject* co=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
         if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
         if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
         if (!(nlocals=PyLong_FromLong(l))) goto end;
         if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
         if (!(stacksize=PyLong_FromLong(s))) goto end;
         if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
@@ -447,78 +598,157 @@
         Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return co;
     }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -541,86 +771,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
   #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+  #define CYTHON_PEP393_ENABLED 1
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -641,16 +951,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -661,25 +977,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -689,19 +1010,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -817,29 +1133,39 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -857,15 +1183,21 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -944,30 +1276,31 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "aiocsv/_parser.pyx",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* #### Code section: numeric_typedefs ### */
+/* #### Code section: complex_type_declarations ### */
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser;
 struct __pyx_t_6aiocsv_7_parser_CDialect;
 
 /* "aiocsv/_parser.pyx":6
  * 
@@ -1032,94 +1365,158 @@
   struct __pyx_t_6aiocsv_7_parser_CDialect __pyx_v_dialect;
   int __pyx_v_force_save_cell;
   int __pyx_v_numeric_cell;
   PyObject *__pyx_v_pydialect;
   PyObject *__pyx_v_reader;
   PyObject *__pyx_v_row;
   enum __pyx_t_6aiocsv_7_parser_ParserState __pyx_v_state;
-  PyObject *__pyx_t_0;
-  Py_ssize_t __pyx_t_1;
+  int __pyx_t_0;
+  PyObject *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
-  void *__pyx_t_3;
-  int __pyx_t_4;
+  Py_ssize_t __pyx_t_3;
+  void *__pyx_t_4;
   Py_ssize_t __pyx_t_5;
 };
 
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
@@ -1143,26 +1540,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1184,125 +1581,137 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
-
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
+#endif
+#endif
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
+
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
+#endif
+
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+#else
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
+#endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
@@ -1323,32 +1732,42 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
 /* CoroutineBase.proto */
-typedef PyObject *(*__pyx_coroutine_body_t)(PyObject *, PyThreadState *, PyObject *);
+struct __pyx_CoroutineObject;
+typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
 #if CYTHON_USE_EXC_INFO_STACK
 #define __Pyx_ExcInfoStruct  _PyErr_StackItem
 #else
 typedef struct {
     PyObject *exc_type;
     PyObject *exc_value;
     PyObject *exc_traceback;
 } __Pyx_ExcInfoStruct;
 #endif
-typedef struct {
+typedef struct __pyx_CoroutineObject {
     PyObject_HEAD
     __pyx_coroutine_body_t body;
     PyObject *closure;
     __Pyx_ExcInfoStruct gi_exc_state;
     PyObject *gi_weakreflist;
     PyObject *classobj;
     PyObject *yieldfrom;
@@ -1405,44 +1824,38 @@
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
 
 /* PatchGeneratorABC.proto */
 static int __Pyx_patch_abc(void);
 
 /* Coroutine.proto */
 #define __Pyx_Coroutine_USED
-static PyTypeObject *__pyx_CoroutineType = 0;
-static PyTypeObject *__pyx_CoroutineAwaitType = 0;
-#define __Pyx_Coroutine_CheckExact(obj) (Py_TYPE(obj) == __pyx_CoroutineType)
+#define __Pyx_Coroutine_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_CoroutineType)
 #define __Pyx_Coroutine_Check(obj) __Pyx_Coroutine_CheckExact(obj)
-#define __Pyx_CoroutineAwait_CheckExact(obj) (Py_TYPE(obj) == __pyx_CoroutineAwaitType)
+#define __Pyx_CoroutineAwait_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_CoroutineAwaitType)
 #define __Pyx_Coroutine_New(body, code, closure, name, qualname, module_name)\
     __Pyx__Coroutine_New(__pyx_CoroutineType, body, code, closure, name, qualname, module_name)
-static int __pyx_Coroutine_init(void);
+static int __pyx_Coroutine_init(PyObject *module);
 static PyObject *__Pyx__Coroutine_await(PyObject *coroutine);
 typedef struct {
     PyObject_HEAD
     PyObject *coroutine;
 } __pyx_CoroutineAwaitObject;
 static PyObject *__Pyx_CoroutineAwait_Close(__pyx_CoroutineAwaitObject *self, PyObject *arg);
 static PyObject *__Pyx_CoroutineAwait_Throw(__pyx_CoroutineAwaitObject *self, PyObject *args);
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* GetAwaitIter.proto */
 static CYTHON_INLINE PyObject *__Pyx_Coroutine_GetAwaitableIter(PyObject *o);
 static PyObject *__Pyx__Coroutine_GetAwaitableIter(PyObject *o);
 
 /* CoroutineYieldFrom.proto */
 static CYTHON_INLINE PyObject* __Pyx_Coroutine_Yield_From(__pyx_CoroutineObject *gen, PyObject *source);
 
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
 /* unicode_iter.proto */
 static CYTHON_INLINE int __Pyx_init_unicode_iteration(
     PyObject* ustring, Py_ssize_t *length, void** data, int *kind);
 
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
@@ -1456,112 +1869,420 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* IncludeStringH.proto */
-#include <string.h>
+/* UnicodeConcatInPlace.proto */
+# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
+    #if CYTHON_REFNANNY
+        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right, __pyx_refnanny)
+    #else
+        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right)
+    #endif
+    static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
+        #if CYTHON_REFNANNY
+        , void* __pyx_refnanny
+        #endif
+    );
+#else
+#define __Pyx_PyUnicode_ConcatInPlace __Pyx_PyUnicode_Concat
+#endif
+#define __Pyx_PyUnicode_ConcatInPlaceSafe(left, right) ((unlikely((left) == Py_None) || unlikely((right) == Py_None)) ?\
+    PyNumber_InPlaceAdd(left, right) : __Pyx_PyUnicode_ConcatInPlace(left, right))
+
+/* pybytes_as_double.proto */
+static double __Pyx_SlowPyString_AsDouble(PyObject *obj);
+static double __Pyx__PyBytes_AsDouble(PyObject *obj, const char* start, Py_ssize_t length);
+static CYTHON_INLINE double __Pyx_PyBytes_AsDouble(PyObject *obj) {
+    return __Pyx__PyBytes_AsDouble(obj, PyBytes_AS_STRING(obj), PyBytes_GET_SIZE(obj));
+}
+static CYTHON_INLINE double __Pyx_PyByteArray_AsDouble(PyObject *obj) {
+    return __Pyx__PyBytes_AsDouble(obj, PyByteArray_AS_STRING(obj), PyByteArray_GET_SIZE(obj));
+}
+
+/* pyunicode_as_double.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static const char* __Pyx__PyUnicode_AsDouble_Copy(const void* data, const int kind, char* buffer, Py_ssize_t start, Py_ssize_t end) {
+    int last_was_punctuation;
+    Py_ssize_t i;
+    last_was_punctuation = 1;
+    for (i=start; i <= end; i++) {
+        Py_UCS4 chr = PyUnicode_READ(kind, data, i);
+        int is_punctuation = (chr == '_') | (chr == '.');
+        *buffer = (char)chr;
+        buffer += (chr != '_');
+        if (unlikely(chr > 127)) goto parse_failure;
+        if (unlikely(last_was_punctuation & is_punctuation)) goto parse_failure;
+        last_was_punctuation = is_punctuation;
+    }
+    if (unlikely(last_was_punctuation)) goto parse_failure;
+    *buffer = '\0';
+    return buffer;
+parse_failure:
+    return NULL;
+}
+static double __Pyx__PyUnicode_AsDouble_inf_nan(const void* data, int kind, Py_ssize_t start, Py_ssize_t length) {
+    int matches = 1;
+    Py_UCS4 chr;
+    Py_UCS4 sign = PyUnicode_READ(kind, data, start);
+    int is_signed = (sign == '-') | (sign == '+');
+    start += is_signed;
+    length -= is_signed;
+    switch (PyUnicode_READ(kind, data, start)) {
+        #ifdef Py_NAN
+        case 'n':
+        case 'N':
+            if (unlikely(length != 3)) goto parse_failure;
+            chr = PyUnicode_READ(kind, data, start+1);
+            matches &= (chr == 'a') | (chr == 'A');
+            chr = PyUnicode_READ(kind, data, start+2);
+            matches &= (chr == 'n') | (chr == 'N');
+            if (unlikely(!matches)) goto parse_failure;
+            return (sign == '-') ? -Py_NAN : Py_NAN;
+        #endif
+        case 'i':
+        case 'I':
+            if (unlikely(length < 3)) goto parse_failure;
+            chr = PyUnicode_READ(kind, data, start+1);
+            matches &= (chr == 'n') | (chr == 'N');
+            chr = PyUnicode_READ(kind, data, start+2);
+            matches &= (chr == 'f') | (chr == 'F');
+            if (likely(length == 3 && matches))
+                return (sign == '-') ? -Py_HUGE_VAL : Py_HUGE_VAL;
+            if (unlikely(length != 8)) goto parse_failure;
+            chr = PyUnicode_READ(kind, data, start+3);
+            matches &= (chr == 'i') | (chr == 'I');
+            chr = PyUnicode_READ(kind, data, start+4);
+            matches &= (chr == 'n') | (chr == 'N');
+            chr = PyUnicode_READ(kind, data, start+5);
+            matches &= (chr == 'i') | (chr == 'I');
+            chr = PyUnicode_READ(kind, data, start+6);
+            matches &= (chr == 't') | (chr == 'T');
+            chr = PyUnicode_READ(kind, data, start+7);
+            matches &= (chr == 'y') | (chr == 'Y');
+            if (unlikely(!matches)) goto parse_failure;
+            return (sign == '-') ? -Py_HUGE_VAL : Py_HUGE_VAL;
+        case '.': case '0': case '1': case '2': case '3': case '4': case '5': case '6': case '7': case '8': case '9':
+            break;
+        default:
+            goto parse_failure;
+    }
+    return 0.0;
+parse_failure:
+    return -1.0;
+}
+static double __Pyx_PyUnicode_AsDouble_WithSpaces(PyObject *obj) {
+    double value;
+    const char *last;
+    char *end;
+    Py_ssize_t start, length = PyUnicode_GET_LENGTH(obj);
+    const int kind = PyUnicode_KIND(obj);
+    const void* data = PyUnicode_DATA(obj);
+    start = 0;
+    while (Py_UNICODE_ISSPACE(PyUnicode_READ(kind, data, start)))
+        start++;
+    while (start < length - 1 && Py_UNICODE_ISSPACE(PyUnicode_READ(kind, data, length - 1)))
+        length--;
+    length -= start;
+    if (unlikely(length <= 0)) goto fallback;
+    value = __Pyx__PyUnicode_AsDouble_inf_nan(data, kind, start, length);
+    if (unlikely(value == -1.0)) goto fallback;
+    if (value != 0.0) return value;
+    if (length < 40) {
+        char number[40];
+        last = __Pyx__PyUnicode_AsDouble_Copy(data, kind, number, start, start + length);
+        if (unlikely(!last)) goto fallback;
+        value = PyOS_string_to_double(number, &end, NULL);
+    } else {
+        char *number = (char*) PyMem_Malloc((length + 1) * sizeof(char));
+        if (unlikely(!number)) goto fallback;
+        last = __Pyx__PyUnicode_AsDouble_Copy(data, kind, number, start, start + length);
+        if (unlikely(!last)) {
+            PyMem_Free(number);
+            goto fallback;
+        }
+        value = PyOS_string_to_double(number, &end, NULL);
+        PyMem_Free(number);
+    }
+    if (likely(end == last) || (value == (double)-1 && PyErr_Occurred())) {
+        return value;
+    }
+fallback:
+    return __Pyx_SlowPyString_AsDouble(obj);
+}
+#endif
+static CYTHON_INLINE double __Pyx_PyUnicode_AsDouble(PyObject *obj) {
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+    if (unlikely(__Pyx_PyUnicode_READY(obj) == -1))
+        return (double)-1;
+    if (likely(PyUnicode_IS_ASCII(obj))) {
+        const char *s;
+        Py_ssize_t length;
+        s = PyUnicode_AsUTF8AndSize(obj, &length);
+        return __Pyx__PyBytes_AsDouble(obj, s, length);
+    }
+    return __Pyx_PyUnicode_AsDouble_WithSpaces(obj);
+#else
+    return __Pyx_SlowPyString_AsDouble(obj);
+#endif
+}
 
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
 /* StopAsyncIteration.proto */
 #define __Pyx_StopAsyncIteration_USED
 static PyObject *__Pyx_PyExc_StopAsyncIteration;
-static int __pyx_StopAsyncIteration_init(void);
+static int __pyx_StopAsyncIteration_init(PyObject *module);
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* pep479.proto */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
+#endif
+
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* UnicodeAsUCS4.proto */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* ObjectAsUCS4.proto */
 #define __Pyx_PyObject_AsPy_UCS4(x)\
     (likely(PyUnicode_Check(x)) ? __Pyx_PyUnicode_AsPy_UCS4(x) : __Pyx__PyObject_AsPy_UCS4(x))
 static Py_UCS4 __Pyx__PyObject_AsPy_UCS4(PyObject*);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_Occurred(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* ReturnWithStopIteration.proto */
 #define __Pyx_ReturnWithStopIteration(value)\
     if (value == Py_None) PyErr_SetNone(PyExc_StopIteration); else __Pyx__ReturnWithStopIteration(value)
 static void __Pyx__ReturnWithStopIteration(PyObject* value);
 
 /* AsyncGenerator.proto */
 #define __Pyx_AsyncGen_USED
 typedef struct {
     __pyx_CoroutineObject coro;
     PyObject *ag_finalizer;
     int ag_hooks_inited;
     int ag_closed;
+    int ag_running_async;
 } __pyx_PyAsyncGenObject;
 static PyTypeObject *__pyx__PyAsyncGenWrappedValueType = 0;
 static PyTypeObject *__pyx__PyAsyncGenASendType = 0;
 static PyTypeObject *__pyx__PyAsyncGenAThrowType = 0;
 static PyTypeObject *__pyx_AsyncGenType = 0;
-#define __Pyx_AsyncGen_CheckExact(obj) (Py_TYPE(obj) == __pyx_AsyncGenType)
+#define __Pyx_AsyncGen_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_AsyncGenType)
 #define __pyx_PyAsyncGenASend_CheckExact(o)\
-                    (Py_TYPE(o) == __pyx__PyAsyncGenASendType)
+                    __Pyx_IS_TYPE(o, __pyx__PyAsyncGenASendType)
 #define __pyx_PyAsyncGenAThrow_CheckExact(o)\
-                    (Py_TYPE(o) == __pyx__PyAsyncGenAThrowType)
+                    __Pyx_IS_TYPE(o, __pyx__PyAsyncGenAThrowType)
 static PyObject *__Pyx_async_gen_anext(PyObject *o);
 static CYTHON_INLINE PyObject *__Pyx_async_gen_asend_iternext(PyObject *o);
 static PyObject *__Pyx_async_gen_asend_send(PyObject *o, PyObject *arg);
 static PyObject *__Pyx_async_gen_asend_close(PyObject *o, PyObject *args);
 static PyObject *__Pyx_async_gen_athrow_close(PyObject *o, PyObject *args);
 static PyObject *__Pyx__PyAsyncGenValueWrapperNew(PyObject *val);
 static __pyx_CoroutineObject *__Pyx_AsyncGen_New(
@@ -1569,122 +2290,439 @@
             PyObject *name, PyObject *qualname, PyObject *module_name) {
     __pyx_PyAsyncGenObject *gen = PyObject_GC_New(__pyx_PyAsyncGenObject, __pyx_AsyncGenType);
     if (unlikely(!gen))
         return NULL;
     gen->ag_finalizer = NULL;
     gen->ag_closed = 0;
     gen->ag_hooks_inited = 0;
+    gen->ag_running_async = 0;
     return __Pyx__Coroutine_NewInit((__pyx_CoroutineObject*)gen, body, code, closure, name, qualname, module_name);
 }
-static int __pyx_AsyncGen_init(void);
+static int __pyx_AsyncGen_init(PyObject *module);
 static void __Pyx_PyAsyncGen_Fini(void);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
 
-/* Module declarations from 'aiocsv._parser' */
-static PyTypeObject *__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser = 0;
+/* Module declarations from "aiocsv._parser" */
 static struct __pyx_t_6aiocsv_7_parser_CDialect __pyx_f_6aiocsv_7_parser_get_dialect(PyObject *); /*proto*/
+/* #### Code section: typeinfo ### */
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "aiocsv._parser"
 extern int __pyx_module_is_main_aiocsv___parser;
 int __pyx_module_is_main_aiocsv___parser = 0;
 
-/* Implementation of 'aiocsv._parser' */
+/* Implementation of "aiocsv._parser" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_RuntimeError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k__2[] = "";
 static const char __pyx_k__3[] = "'";
+static const char __pyx_k__5[] = "*";
+static const char __pyx_k__7[] = "?";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_csv[] = "csv";
 static const char __pyx_k_row[] = "row";
 static const char __pyx_k_wtf[] = "wtf";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_cell[] = "cell";
 static const char __pyx_k_char[] = "char";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_send[] = "send";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_Error[] = "Error";
 static const char __pyx_k_await[] = "__await__";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_throw[] = "throw";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_parser[] = "parser";
 static const char __pyx_k_reader[] = "reader";
 static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_dialect[] = "dialect";
+static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_quoting[] = "quoting";
 static const char __pyx_k_delimiter[] = "delimiter";
+static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pydialect[] = "pydialect";
 static const char __pyx_k_quotechar[] = "quotechar";
 static const char __pyx_k_QUOTE_NONE[] = "QUOTE_NONE";
 static const char __pyx_k_escapechar[] = "escapechar";
 static const char __pyx_k_doublequote[] = "doublequote";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_numeric_cell[] = "numeric_cell";
 static const char __pyx_k_aiocsv__parser[] = "aiocsv._parser";
 static const char __pyx_k_expected_after[] = "' expected after '";
 static const char __pyx_k_force_save_cell[] = "force_save_cell";
 static const char __pyx_k_QUOTE_NONNUMERIC[] = "QUOTE_NONNUMERIC";
 static const char __pyx_k_skipinitialspace[] = "skipinitialspace";
 static const char __pyx_k_aiocsv__parser_pyx[] = "aiocsv/_parser.pyx";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static PyObject *__pyx_n_s_Error;
-static PyObject *__pyx_n_s_QUOTE_NONE;
-static PyObject *__pyx_n_s_QUOTE_NONNUMERIC;
-static PyObject *__pyx_n_s_RuntimeError;
-static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_kp_u__3;
-static PyObject *__pyx_n_s_aiocsv__parser;
-static PyObject *__pyx_kp_s_aiocsv__parser_pyx;
-static PyObject *__pyx_n_s_args;
-static PyObject *__pyx_n_s_await;
-static PyObject *__pyx_n_s_cell;
-static PyObject *__pyx_n_s_char;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_close;
-static PyObject *__pyx_n_s_csv;
-static PyObject *__pyx_n_s_data;
-static PyObject *__pyx_n_s_delimiter;
-static PyObject *__pyx_n_s_dialect;
-static PyObject *__pyx_n_s_doublequote;
-static PyObject *__pyx_n_s_escapechar;
-static PyObject *__pyx_kp_u_expected_after;
-static PyObject *__pyx_n_s_force_save_cell;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_numeric_cell;
-static PyObject *__pyx_n_s_parser;
-static PyObject *__pyx_n_s_pydialect;
-static PyObject *__pyx_n_s_quotechar;
-static PyObject *__pyx_n_s_quoting;
-static PyObject *__pyx_n_s_read;
-static PyObject *__pyx_n_s_reader;
-static PyObject *__pyx_n_s_row;
-static PyObject *__pyx_n_s_send;
-static PyObject *__pyx_n_s_skipinitialspace;
-static PyObject *__pyx_n_s_state;
-static PyObject *__pyx_n_s_strict;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_throw;
-static PyObject *__pyx_n_u_wtf;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_6aiocsv_7_parser_parser(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_reader, PyObject *__pyx_v_pydialect); /* proto */
 static PyObject *__pyx_tp_new_6aiocsv_7_parser___pyx_scope_struct__parser(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_2048;
-static PyObject *__pyx_codeobj_;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser;
+  #endif
+  PyTypeObject *__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser;
+  PyObject *__pyx_n_s_Error;
+  PyObject *__pyx_n_s_QUOTE_NONE;
+  PyObject *__pyx_n_s_QUOTE_NONNUMERIC;
+  PyObject *__pyx_n_s_RuntimeError;
+  PyObject *__pyx_kp_u__2;
+  PyObject *__pyx_kp_u__3;
+  PyObject *__pyx_n_s__5;
+  PyObject *__pyx_n_s__7;
+  PyObject *__pyx_n_s_aiocsv__parser;
+  PyObject *__pyx_kp_s_aiocsv__parser_pyx;
+  PyObject *__pyx_n_s_args;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_await;
+  PyObject *__pyx_n_s_cell;
+  PyObject *__pyx_n_s_char;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_close;
+  PyObject *__pyx_n_s_csv;
+  PyObject *__pyx_n_s_data;
+  PyObject *__pyx_n_s_delimiter;
+  PyObject *__pyx_n_s_dialect;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_doublequote;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_escapechar;
+  PyObject *__pyx_kp_u_expected_after;
+  PyObject *__pyx_n_s_force_save_cell;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_numeric_cell;
+  PyObject *__pyx_n_s_parser;
+  PyObject *__pyx_n_s_pydialect;
+  PyObject *__pyx_n_s_quotechar;
+  PyObject *__pyx_n_s_quoting;
+  PyObject *__pyx_n_s_read;
+  PyObject *__pyx_n_s_reader;
+  PyObject *__pyx_n_s_row;
+  PyObject *__pyx_n_s_send;
+  PyObject *__pyx_n_s_skipinitialspace;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_state;
+  PyObject *__pyx_n_s_strict;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_throw;
+  PyObject *__pyx_n_u_wtf;
+  PyObject *__pyx_int_2048;
+  PyObject *__pyx_codeobj_;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__6;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser);
+  Py_CLEAR(clear_module_state->__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Error);
+  Py_CLEAR(clear_module_state->__pyx_n_s_QUOTE_NONE);
+  Py_CLEAR(clear_module_state->__pyx_n_s_QUOTE_NONNUMERIC);
+  Py_CLEAR(clear_module_state->__pyx_n_s_RuntimeError);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__2);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s__5);
+  Py_CLEAR(clear_module_state->__pyx_n_s__7);
+  Py_CLEAR(clear_module_state->__pyx_n_s_aiocsv__parser);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_aiocsv__parser_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_args);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_await);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cell);
+  Py_CLEAR(clear_module_state->__pyx_n_s_char);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_csv);
+  Py_CLEAR(clear_module_state->__pyx_n_s_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_delimiter);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dialect);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_doublequote);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_escapechar);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_expected_after);
+  Py_CLEAR(clear_module_state->__pyx_n_s_force_save_cell);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numeric_cell);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parser);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pydialect);
+  Py_CLEAR(clear_module_state->__pyx_n_s_quotechar);
+  Py_CLEAR(clear_module_state->__pyx_n_s_quoting);
+  Py_CLEAR(clear_module_state->__pyx_n_s_read);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reader);
+  Py_CLEAR(clear_module_state->__pyx_n_s_row);
+  Py_CLEAR(clear_module_state->__pyx_n_s_send);
+  Py_CLEAR(clear_module_state->__pyx_n_s_skipinitialspace);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_strict);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_throw);
+  Py_CLEAR(clear_module_state->__pyx_n_u_wtf);
+  Py_CLEAR(clear_module_state->__pyx_int_2048);
+  Py_CLEAR(clear_module_state->__pyx_codeobj_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser);
+  Py_VISIT(traverse_module_state->__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Error);
+  Py_VISIT(traverse_module_state->__pyx_n_s_QUOTE_NONE);
+  Py_VISIT(traverse_module_state->__pyx_n_s_QUOTE_NONNUMERIC);
+  Py_VISIT(traverse_module_state->__pyx_n_s_RuntimeError);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__2);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s__5);
+  Py_VISIT(traverse_module_state->__pyx_n_s__7);
+  Py_VISIT(traverse_module_state->__pyx_n_s_aiocsv__parser);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_aiocsv__parser_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_args);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_await);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cell);
+  Py_VISIT(traverse_module_state->__pyx_n_s_char);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_csv);
+  Py_VISIT(traverse_module_state->__pyx_n_s_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_delimiter);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dialect);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_doublequote);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_escapechar);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_expected_after);
+  Py_VISIT(traverse_module_state->__pyx_n_s_force_save_cell);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numeric_cell);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parser);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pydialect);
+  Py_VISIT(traverse_module_state->__pyx_n_s_quotechar);
+  Py_VISIT(traverse_module_state->__pyx_n_s_quoting);
+  Py_VISIT(traverse_module_state->__pyx_n_s_read);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reader);
+  Py_VISIT(traverse_module_state->__pyx_n_s_row);
+  Py_VISIT(traverse_module_state->__pyx_n_s_send);
+  Py_VISIT(traverse_module_state->__pyx_n_s_skipinitialspace);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_strict);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_throw);
+  Py_VISIT(traverse_module_state->__pyx_n_u_wtf);
+  Py_VISIT(traverse_module_state->__pyx_int_2048);
+  Py_VISIT(traverse_module_state->__pyx_codeobj_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser __pyx_mstate_global->__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser
+#endif
+#define __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser __pyx_mstate_global->__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser
+#define __pyx_n_s_Error __pyx_mstate_global->__pyx_n_s_Error
+#define __pyx_n_s_QUOTE_NONE __pyx_mstate_global->__pyx_n_s_QUOTE_NONE
+#define __pyx_n_s_QUOTE_NONNUMERIC __pyx_mstate_global->__pyx_n_s_QUOTE_NONNUMERIC
+#define __pyx_n_s_RuntimeError __pyx_mstate_global->__pyx_n_s_RuntimeError
+#define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
+#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
+#define __pyx_n_s__5 __pyx_mstate_global->__pyx_n_s__5
+#define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
+#define __pyx_n_s_aiocsv__parser __pyx_mstate_global->__pyx_n_s_aiocsv__parser
+#define __pyx_kp_s_aiocsv__parser_pyx __pyx_mstate_global->__pyx_kp_s_aiocsv__parser_pyx
+#define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_await __pyx_mstate_global->__pyx_n_s_await
+#define __pyx_n_s_cell __pyx_mstate_global->__pyx_n_s_cell
+#define __pyx_n_s_char __pyx_mstate_global->__pyx_n_s_char
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
+#define __pyx_n_s_csv __pyx_mstate_global->__pyx_n_s_csv
+#define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
+#define __pyx_n_s_delimiter __pyx_mstate_global->__pyx_n_s_delimiter
+#define __pyx_n_s_dialect __pyx_mstate_global->__pyx_n_s_dialect
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_doublequote __pyx_mstate_global->__pyx_n_s_doublequote
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_escapechar __pyx_mstate_global->__pyx_n_s_escapechar
+#define __pyx_kp_u_expected_after __pyx_mstate_global->__pyx_kp_u_expected_after
+#define __pyx_n_s_force_save_cell __pyx_mstate_global->__pyx_n_s_force_save_cell
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_numeric_cell __pyx_mstate_global->__pyx_n_s_numeric_cell
+#define __pyx_n_s_parser __pyx_mstate_global->__pyx_n_s_parser
+#define __pyx_n_s_pydialect __pyx_mstate_global->__pyx_n_s_pydialect
+#define __pyx_n_s_quotechar __pyx_mstate_global->__pyx_n_s_quotechar
+#define __pyx_n_s_quoting __pyx_mstate_global->__pyx_n_s_quoting
+#define __pyx_n_s_read __pyx_mstate_global->__pyx_n_s_read
+#define __pyx_n_s_reader __pyx_mstate_global->__pyx_n_s_reader
+#define __pyx_n_s_row __pyx_mstate_global->__pyx_n_s_row
+#define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
+#define __pyx_n_s_skipinitialspace __pyx_mstate_global->__pyx_n_s_skipinitialspace
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
+#define __pyx_n_s_strict __pyx_mstate_global->__pyx_n_s_strict
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
+#define __pyx_n_u_wtf __pyx_mstate_global->__pyx_n_u_wtf
+#define __pyx_int_2048 __pyx_mstate_global->__pyx_int_2048
+#define __pyx_codeobj_ __pyx_mstate_global->__pyx_codeobj_
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+/* #### Code section: module_code ### */
 
 /* "aiocsv/_parser.pyx":33
  * 
  * 
  * cdef CDialect get_dialect(object pydialect):             # <<<<<<<<<<<<<<
  *     cdef CDialect d
  * 
@@ -1710,41 +2748,41 @@
  *     # Bools
  *     d.skipinitialspace = <bint?>pydialect.skipinitialspace             # <<<<<<<<<<<<<<
  *     d.doublequote = <bint?>pydialect.doublequote
  *     d.strict = <bint?>pydialect.strict
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pydialect, __pyx_n_s_skipinitialspace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_d.skipinitialspace = __pyx_t_2;
 
   /* "aiocsv/_parser.pyx":38
  *     # Bools
  *     d.skipinitialspace = <bint?>pydialect.skipinitialspace
  *     d.doublequote = <bint?>pydialect.doublequote             # <<<<<<<<<<<<<<
  *     d.strict = <bint?>pydialect.strict
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pydialect, __pyx_n_s_doublequote); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_d.doublequote = __pyx_t_2;
 
   /* "aiocsv/_parser.pyx":39
  *     d.skipinitialspace = <bint?>pydialect.skipinitialspace
  *     d.doublequote = <bint?>pydialect.doublequote
  *     d.strict = <bint?>pydialect.strict             # <<<<<<<<<<<<<<
  * 
  *     # Quoting
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pydialect, __pyx_n_s_strict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_d.strict = __pyx_t_2;
 
   /* "aiocsv/_parser.pyx":42
  * 
  *     # Quoting
  *     if pydialect.quoting == csv.QUOTE_NONE:             # <<<<<<<<<<<<<<
@@ -1757,15 +2795,15 @@
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_QUOTE_NONE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
     /* "aiocsv/_parser.pyx":43
  *     # Quoting
  *     if pydialect.quoting == csv.QUOTE_NONE:
  *         d.quoting = ReadQuoting.NONE             # <<<<<<<<<<<<<<
@@ -1797,15 +2835,15 @@
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_QUOTE_NONNUMERIC); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_2) {
 
     /* "aiocsv/_parser.pyx":45
  *         d.quoting = ReadQuoting.NONE
  *     elif pydialect.quoting == csv.QUOTE_NONNUMERIC:
  *         d.quoting = ReadQuoting.NONNUMERIC             # <<<<<<<<<<<<<<
@@ -1859,15 +2897,15 @@
  *     d.escapechar = <Py_UCS4?>pydialect.escapechar[0] \
  *         if pydialect.escapechar is not None else u'\0'
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pydialect, __pyx_n_s_quotechar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 != Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if ((__pyx_t_2 != 0)) {
+  if (__pyx_t_2) {
 
     /* "aiocsv/_parser.pyx":51
  *     # Chars
  *     d.delimiter = <Py_UCS4?>pydialect.delimiter[0]
  *     d.quotechar = <Py_UCS4?>pydialect.quotechar[0] \             # <<<<<<<<<<<<<<
  *         if pydialect.quotechar is not None else u'\0'
  *     d.escapechar = <Py_UCS4?>pydialect.escapechar[0] \
@@ -1892,15 +2930,15 @@
  * 
  *     return d
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pydialect, __pyx_n_s_escapechar); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = (__pyx_t_4 != Py_None);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if ((__pyx_t_2 != 0)) {
+  if (__pyx_t_2) {
 
     /* "aiocsv/_parser.pyx":53
  *     d.quotechar = <Py_UCS4?>pydialect.quotechar[0] \
  *         if pydialect.quotechar is not None else u'\0'
  *     d.escapechar = <Py_UCS4?>pydialect.escapechar[0] \             # <<<<<<<<<<<<<<
  *         if pydialect.escapechar is not None else u'\0'
  * 
@@ -1937,15 +2975,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_WriteUnraisable("aiocsv._parser.get_dialect", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_AddTraceback("aiocsv._parser.get_dialect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6aiocsv_7_parser_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
@@ -1954,66 +2992,84 @@
  * 
  * async def parser(reader, pydialect):             # <<<<<<<<<<<<<<
  *     cdef unicode data = <unicode?>(await reader.read(READ_SIZE))
  *     cdef CDialect dialect = get_dialect(pydialect)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6aiocsv_7_parser_1parser(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_6aiocsv_7_parser_1parser = {"parser", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6aiocsv_7_parser_1parser, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6aiocsv_7_parser_1parser(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6aiocsv_7_parser_1parser(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_6aiocsv_7_parser_1parser = {"parser", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6aiocsv_7_parser_1parser, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6aiocsv_7_parser_1parser(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_reader = 0;
   PyObject *__pyx_v_pydialect = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parser (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_reader,&__pyx_n_s_pydialect,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_reader,&__pyx_n_s_pydialect,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reader)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_reader)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pydialect)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pydialect)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("parser", 1, 2, 2, 1); __PYX_ERR(0, 59, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parser") < 0)) __PYX_ERR(0, 59, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "parser") < 0)) __PYX_ERR(0, 59, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_reader = values[0];
     __pyx_v_pydialect = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("parser", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 59, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("parser", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 59, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aiocsv._parser.parser", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6aiocsv_7_parser_parser(__pyx_self, __pyx_v_reader, __pyx_v_pydialect);
 
@@ -2032,15 +3088,15 @@
   __Pyx_RefNannySetupContext("parser", 0);
   __pyx_cur_scope = (struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *)__pyx_tp_new_6aiocsv_7_parser___pyx_scope_struct__parser(__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 59, __pyx_L1_error)
   } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_reader = __pyx_v_reader;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_reader);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_reader);
   __pyx_cur_scope->__pyx_v_pydialect = __pyx_v_pydialect;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_pydialect);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_pydialect);
@@ -2051,40 +3107,42 @@
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("aiocsv._parser.parser", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_gb_6aiocsv_7_parser_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *__pyx_cur_scope = ((struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  Py_ssize_t __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  void *__pyx_t_8;
-  int __pyx_t_9;
-  int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  int __pyx_t_12;
-  Py_ssize_t __pyx_t_13;
-  int __pyx_t_14;
-  Py_UCS4 __pyx_t_15;
-  PyObject *__pyx_t_16 = NULL;
+  struct __pyx_t_6aiocsv_7_parser_CDialect __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
+  Py_ssize_t __pyx_t_9;
+  void *__pyx_t_10;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  int __pyx_t_13;
+  Py_ssize_t __pyx_t_14;
+  int __pyx_t_15;
+  double __pyx_t_16;
+  Py_UCS4 __pyx_t_17;
+  PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parser", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
@@ -2105,28 +3163,33 @@
  *     cdef unicode data = <unicode?>(await reader.read(READ_SIZE))             # <<<<<<<<<<<<<<
  *     cdef CDialect dialect = get_dialect(pydialect)
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_reader, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_int_2048) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_int_2048);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_int_2048};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_r);
   if (likely(__pyx_r)) {
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
@@ -2137,30 +3200,31 @@
     if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 60, __pyx_L1_error)
     __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
   } else {
     __pyx_t_1 = NULL;
     if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
   }
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_1;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_data = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "aiocsv/_parser.pyx":61
  * async def parser(reader, pydialect):
  *     cdef unicode data = <unicode?>(await reader.read(READ_SIZE))
  *     cdef CDialect dialect = get_dialect(pydialect)             # <<<<<<<<<<<<<<
  * 
  *     cdef ParserState state = ParserState.AFTER_DELIM
  */
-  __pyx_cur_scope->__pyx_v_dialect = __pyx_f_6aiocsv_7_parser_get_dialect(__pyx_cur_scope->__pyx_v_pydialect);
+  __pyx_t_5 = __pyx_f_6aiocsv_7_parser_get_dialect(__pyx_cur_scope->__pyx_v_pydialect); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_cur_scope->__pyx_v_dialect = __pyx_t_5;
 
   /* "aiocsv/_parser.pyx":63
  *     cdef CDialect dialect = get_dialect(pydialect)
  * 
  *     cdef ParserState state = ParserState.AFTER_DELIM             # <<<<<<<<<<<<<<
  * 
  *     cdef list row = []
@@ -2213,44 +3277,44 @@
  * 
  *     # Iterate while the reader gives out data
  *     while data:             # <<<<<<<<<<<<<<
  * 
  *         # Iterate charachter-by-charachter over the input file
  */
   while (1) {
-    __pyx_t_4 = (__pyx_cur_scope->__pyx_v_data != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_cur_scope->__pyx_v_data) != 0);
-    if (!__pyx_t_4) break;
+    __pyx_t_6 = (__pyx_cur_scope->__pyx_v_data != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_cur_scope->__pyx_v_data) != 0);
+    if (!__pyx_t_6) break;
 
     /* "aiocsv/_parser.pyx":76
  *         # Iterate charachter-by-charachter over the input file
  *         # and update the parser state
  *         for char in data:             # <<<<<<<<<<<<<<
  * 
  *             # Switch case depedning on the state
  */
     if (unlikely(__pyx_cur_scope->__pyx_v_data == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
       __PYX_ERR(0, 76, __pyx_L1_error)
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_data);
-    __pyx_t_5 = __pyx_cur_scope->__pyx_v_data;
-    __pyx_t_10 = __Pyx_init_unicode_iteration(__pyx_t_5, (&__pyx_t_7), (&__pyx_t_8), (&__pyx_t_9)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 76, __pyx_L1_error)
-    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_7; __pyx_t_11++) {
-      __pyx_t_6 = __pyx_t_11;
-      __pyx_cur_scope->__pyx_v_char = __Pyx_PyUnicode_READ(__pyx_t_9, __pyx_t_8, __pyx_t_6);
+    __pyx_t_7 = __pyx_cur_scope->__pyx_v_data;
+    __pyx_t_11 = __Pyx_init_unicode_iteration(__pyx_t_7, (&__pyx_t_9), (&__pyx_t_10), (&__pyx_t_4)); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 76, __pyx_L1_error)
+    for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_9; __pyx_t_12++) {
+      __pyx_t_8 = __pyx_t_12;
+      __pyx_cur_scope->__pyx_v_char = __Pyx_PyUnicode_READ(__pyx_t_4, __pyx_t_10, __pyx_t_8);
 
       /* "aiocsv/_parser.pyx":80
  *             # Switch case depedning on the state
  * 
  *             if state == ParserState.EAT_NEWLINE:             # <<<<<<<<<<<<<<
  *                 if char == u'\r' or char == u'\n':
  *                     continue
  */
-      __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_state == __pyx_e_6aiocsv_7_parser_EAT_NEWLINE) != 0);
-      if (__pyx_t_4) {
+      __pyx_t_6 = (__pyx_cur_scope->__pyx_v_state == __pyx_e_6aiocsv_7_parser_EAT_NEWLINE);
+      if (__pyx_t_6) {
 
         /* "aiocsv/_parser.pyx":81
  * 
  *             if state == ParserState.EAT_NEWLINE:
  *                 if char == u'\r' or char == u'\n':             # <<<<<<<<<<<<<<
  *                     continue
  *                 state = ParserState.AFTER_ROW
@@ -2300,48 +3364,48 @@
       /* "aiocsv/_parser.pyx":86
  *             # (fallthrough)
  * 
  *             if state == ParserState.AFTER_ROW:             # <<<<<<<<<<<<<<
  *                 yield row
  *                 row = []
  */
-      __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_state == __pyx_e_6aiocsv_7_parser_AFTER_ROW) != 0);
-      if (__pyx_t_4) {
+      __pyx_t_6 = (__pyx_cur_scope->__pyx_v_state == __pyx_e_6aiocsv_7_parser_AFTER_ROW);
+      if (__pyx_t_6) {
 
         /* "aiocsv/_parser.pyx":87
  * 
  *             if state == ParserState.AFTER_ROW:
  *                 yield row             # <<<<<<<<<<<<<<
  *                 row = []
  *                 state = ParserState.AFTER_DELIM
  */
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_row);
         __pyx_r = __pyx_cur_scope->__pyx_v_row;
-        __Pyx_XGIVEREF(__pyx_t_5);
-        __pyx_cur_scope->__pyx_t_0 = __pyx_t_5;
-        __pyx_cur_scope->__pyx_t_1 = __pyx_t_6;
-        __pyx_cur_scope->__pyx_t_2 = __pyx_t_7;
-        __pyx_cur_scope->__pyx_t_3 = __pyx_t_8;
-        __pyx_cur_scope->__pyx_t_4 = __pyx_t_9;
-        __pyx_cur_scope->__pyx_t_5 = __pyx_t_11;
+        __pyx_cur_scope->__pyx_t_0 = __pyx_t_4;
+        __Pyx_XGIVEREF(__pyx_t_7);
+        __pyx_cur_scope->__pyx_t_1 = __pyx_t_7;
+        __pyx_cur_scope->__pyx_t_2 = __pyx_t_8;
+        __pyx_cur_scope->__pyx_t_3 = __pyx_t_9;
+        __pyx_cur_scope->__pyx_t_4 = __pyx_t_10;
+        __pyx_cur_scope->__pyx_t_5 = __pyx_t_12;
         __Pyx_XGIVEREF(__pyx_r);
         __Pyx_RefNannyFinishContext();
         __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
         /* return from async generator, yielding value */
         __pyx_generator->resume_label = 2;
         return __Pyx__PyAsyncGenValueWrapperNew(__pyx_r);
         __pyx_L11_resume_from_yield:;
-        __pyx_t_5 = __pyx_cur_scope->__pyx_t_0;
-        __pyx_cur_scope->__pyx_t_0 = 0;
-        __Pyx_XGOTREF(__pyx_t_5);
-        __pyx_t_6 = __pyx_cur_scope->__pyx_t_1;
-        __pyx_t_7 = __pyx_cur_scope->__pyx_t_2;
-        __pyx_t_8 = __pyx_cur_scope->__pyx_t_3;
-        __pyx_t_9 = __pyx_cur_scope->__pyx_t_4;
-        __pyx_t_11 = __pyx_cur_scope->__pyx_t_5;
+        __pyx_t_4 = __pyx_cur_scope->__pyx_t_0;
+        __pyx_t_7 = __pyx_cur_scope->__pyx_t_1;
+        __pyx_cur_scope->__pyx_t_1 = 0;
+        __Pyx_XGOTREF(__pyx_t_7);
+        __pyx_t_8 = __pyx_cur_scope->__pyx_t_2;
+        __pyx_t_9 = __pyx_cur_scope->__pyx_t_3;
+        __pyx_t_10 = __pyx_cur_scope->__pyx_t_4;
+        __pyx_t_12 = __pyx_cur_scope->__pyx_t_5;
         if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 87, __pyx_L1_error)
 
         /* "aiocsv/_parser.pyx":88
  *             if state == ParserState.AFTER_ROW:
  *                 yield row
  *                 row = []             # <<<<<<<<<<<<<<
  *                 state = ParserState.AFTER_DELIM
@@ -2385,24 +3449,23 @@
         /* "aiocsv/_parser.pyx":96
  * 
  *                 # 1. We were asked to skip whitespace right after the delimiter
  *                 if dialect.skipinitialspace and char == u' ':             # <<<<<<<<<<<<<<
  *                     force_save_cell = True
  * 
  */
-        __pyx_t_12 = (__pyx_cur_scope->__pyx_v_dialect.skipinitialspace != 0);
-        if (__pyx_t_12) {
+        if (__pyx_cur_scope->__pyx_v_dialect.skipinitialspace) {
         } else {
-          __pyx_t_4 = __pyx_t_12;
+          __pyx_t_6 = __pyx_cur_scope->__pyx_v_dialect.skipinitialspace;
           goto __pyx_L13_bool_binop_done;
         }
-        __pyx_t_12 = ((__pyx_cur_scope->__pyx_v_char == 32) != 0);
-        __pyx_t_4 = __pyx_t_12;
+        __pyx_t_13 = (__pyx_cur_scope->__pyx_v_char == 32);
+        __pyx_t_6 = __pyx_t_13;
         __pyx_L13_bool_binop_done:;
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":97
  *                 # 1. We were asked to skip whitespace right after the delimiter
  *                 if dialect.skipinitialspace and char == u' ':
  *                     force_save_cell = True             # <<<<<<<<<<<<<<
  * 
  *                 # 2. Empty field + End of row
@@ -2425,49 +3488,48 @@
  *                 elif char == u'\r' or char == u'\n':             # <<<<<<<<<<<<<<
  *                     if len(row) > 0 or force_save_cell:
  *                         row.append(cell)
  */
         switch (__pyx_cur_scope->__pyx_v_char) {
           case 13:
           case 10:
-          __pyx_t_4 = 1;
+          __pyx_t_6 = 1;
           break;
           default:
-          __pyx_t_4 = 0;
+          __pyx_t_6 = 0;
           break;
         }
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":101
  *                 # 2. Empty field + End of row
  *                 elif char == u'\r' or char == u'\n':
  *                     if len(row) > 0 or force_save_cell:             # <<<<<<<<<<<<<<
  *                         row.append(cell)
  *                     state = ParserState.EAT_NEWLINE
  */
-          __pyx_t_13 = PyList_GET_SIZE(__pyx_cur_scope->__pyx_v_row); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 101, __pyx_L1_error)
-          __pyx_t_12 = ((__pyx_t_13 > 0) != 0);
-          if (!__pyx_t_12) {
+          __pyx_t_14 = PyList_GET_SIZE(__pyx_cur_scope->__pyx_v_row); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 101, __pyx_L1_error)
+          __pyx_t_13 = (__pyx_t_14 > 0);
+          if (!__pyx_t_13) {
           } else {
-            __pyx_t_4 = __pyx_t_12;
+            __pyx_t_6 = __pyx_t_13;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_12 = (__pyx_cur_scope->__pyx_v_force_save_cell != 0);
-          __pyx_t_4 = __pyx_t_12;
+          __pyx_t_6 = __pyx_cur_scope->__pyx_v_force_save_cell;
           __pyx_L16_bool_binop_done:;
-          if (__pyx_t_4) {
+          if (__pyx_t_6) {
 
             /* "aiocsv/_parser.pyx":102
  *                 elif char == u'\r' or char == u'\n':
  *                     if len(row) > 0 or force_save_cell:
  *                         row.append(cell)             # <<<<<<<<<<<<<<
  *                     state = ParserState.EAT_NEWLINE
  * 
  */
-            __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 102, __pyx_L1_error)
+            __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 102, __pyx_L1_error)
 
             /* "aiocsv/_parser.pyx":101
  *                 # 2. Empty field + End of row
  *                 elif char == u'\r' or char == u'\n':
  *                     if len(row) > 0 or force_save_cell:             # <<<<<<<<<<<<<<
  *                         row.append(cell)
  *                     state = ParserState.EAT_NEWLINE
@@ -2496,25 +3558,25 @@
         /* "aiocsv/_parser.pyx":106
  * 
  *                 # 3. Empty field
  *                 elif char == dialect.delimiter:             # <<<<<<<<<<<<<<
  *                     row.append(cell)
  *                     cell = u""
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":107
  *                 # 3. Empty field
  *                 elif char == dialect.delimiter:
  *                     row.append(cell)             # <<<<<<<<<<<<<<
  *                     cell = u""
  *                     force_save_cell = False
  */
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 107, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 107, __pyx_L1_error)
 
           /* "aiocsv/_parser.pyx":108
  *                 elif char == dialect.delimiter:
  *                     row.append(cell)
  *                     cell = u""             # <<<<<<<<<<<<<<
  *                     force_save_cell = False
  *                     # state stays unchanged (AFTER_DELIM)
@@ -2546,24 +3608,24 @@
         /* "aiocsv/_parser.pyx":113
  * 
  *                 # 4. Start of a quoted cell
  *                 elif char == dialect.quotechar and dialect.quoting != ReadQuoting.NONE:             # <<<<<<<<<<<<<<
  *                     state = ParserState.IN_CELL_QUOTED
  * 
  */
-        __pyx_t_12 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar) != 0);
-        if (__pyx_t_12) {
+        __pyx_t_13 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar);
+        if (__pyx_t_13) {
         } else {
-          __pyx_t_4 = __pyx_t_12;
+          __pyx_t_6 = __pyx_t_13;
           goto __pyx_L18_bool_binop_done;
         }
-        __pyx_t_12 = ((__pyx_cur_scope->__pyx_v_dialect.quoting != __pyx_e_6aiocsv_7_parser_NONE) != 0);
-        __pyx_t_4 = __pyx_t_12;
+        __pyx_t_13 = (__pyx_cur_scope->__pyx_v_dialect.quoting != __pyx_e_6aiocsv_7_parser_NONE);
+        __pyx_t_6 = __pyx_t_13;
         __pyx_L18_bool_binop_done:;
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":114
  *                 # 4. Start of a quoted cell
  *                 elif char == dialect.quotechar and dialect.quoting != ReadQuoting.NONE:
  *                     state = ParserState.IN_CELL_QUOTED             # <<<<<<<<<<<<<<
  * 
  *                 # 5. Start of an escape in an unqoted field
@@ -2583,16 +3645,16 @@
         /* "aiocsv/_parser.pyx":117
  * 
  *                 # 5. Start of an escape in an unqoted field
  *                 elif char == dialect.escapechar:             # <<<<<<<<<<<<<<
  *                     state = ParserState.ESCAPE
  * 
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":118
  *                 # 5. Start of an escape in an unqoted field
  *                 elif char == dialect.escapechar:
  *                     state = ParserState.ESCAPE             # <<<<<<<<<<<<<<
  * 
  *                 # 6. Start of an unquoted field
@@ -2615,15 +3677,15 @@
  *                     cell += char             # <<<<<<<<<<<<<<
  *                     state = ParserState.IN_CELL
  *                     numeric_cell = dialect.quoting == ReadQuoting.NONNUMERIC
  */
         /*else*/ {
           __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_1));
           __Pyx_GIVEREF(__pyx_t_1);
           __pyx_t_1 = 0;
 
@@ -2663,39 +3725,44 @@
  *                 if char == u'\r' or char == u'\n':             # <<<<<<<<<<<<<<
  *                     row.append(float(cell) if numeric_cell else cell)
  * 
  */
         switch (__pyx_cur_scope->__pyx_v_char) {
           case 13:
           case 10:
-          __pyx_t_4 = 1;
+          __pyx_t_6 = 1;
           break;
           default:
-          __pyx_t_4 = 0;
+          __pyx_t_6 = 0;
           break;
         }
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":131
  *                 # 1. End of a row
  *                 if char == u'\r' or char == u'\n':
  *                     row.append(float(cell) if numeric_cell else cell)             # <<<<<<<<<<<<<<
  * 
  *                     cell = u""
  */
-          if ((__pyx_cur_scope->__pyx_v_numeric_cell != 0)) {
-            __pyx_t_2 = __Pyx_PyNumber_Float(__pyx_cur_scope->__pyx_v_cell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+          if (__pyx_cur_scope->__pyx_v_numeric_cell) {
+            if (unlikely(__pyx_cur_scope->__pyx_v_cell == Py_None)) {
+              PyErr_SetString(PyExc_TypeError, "float() argument must be a string or a number, not 'NoneType'");
+              __PYX_ERR(0, 131, __pyx_L1_error)
+            }
+            __pyx_t_16 = __Pyx_PyUnicode_AsDouble(__pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_16 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
+            __pyx_t_2 = PyFloat_FromDouble(__pyx_t_16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             __pyx_t_1 = __pyx_t_2;
             __pyx_t_2 = 0;
           } else {
             __Pyx_INCREF(__pyx_cur_scope->__pyx_v_cell);
             __pyx_t_1 = __pyx_cur_scope->__pyx_v_cell;
           }
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 131, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_1); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 131, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           /* "aiocsv/_parser.pyx":133
  *                     row.append(float(cell) if numeric_cell else cell)
  * 
  *                     cell = u""             # <<<<<<<<<<<<<<
  *                     force_save_cell = False
@@ -2746,34 +3813,39 @@
         /* "aiocsv/_parser.pyx":139
  * 
  *                 # 2. End of a cell
  *                 elif char == dialect.delimiter:             # <<<<<<<<<<<<<<
  *                     row.append(float(cell) if numeric_cell else cell)  # type: ignore
  * 
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":140
  *                 # 2. End of a cell
  *                 elif char == dialect.delimiter:
  *                     row.append(float(cell) if numeric_cell else cell)  # type: ignore             # <<<<<<<<<<<<<<
  * 
  *                     cell = u""
  */
-          if ((__pyx_cur_scope->__pyx_v_numeric_cell != 0)) {
-            __pyx_t_2 = __Pyx_PyNumber_Float(__pyx_cur_scope->__pyx_v_cell); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
+          if (__pyx_cur_scope->__pyx_v_numeric_cell) {
+            if (unlikely(__pyx_cur_scope->__pyx_v_cell == Py_None)) {
+              PyErr_SetString(PyExc_TypeError, "float() argument must be a string or a number, not 'NoneType'");
+              __PYX_ERR(0, 140, __pyx_L1_error)
+            }
+            __pyx_t_16 = __Pyx_PyUnicode_AsDouble(__pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_16 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 140, __pyx_L1_error)
+            __pyx_t_2 = PyFloat_FromDouble(__pyx_t_16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             __pyx_t_1 = __pyx_t_2;
             __pyx_t_2 = 0;
           } else {
             __Pyx_INCREF(__pyx_cur_scope->__pyx_v_cell);
             __pyx_t_1 = __pyx_cur_scope->__pyx_v_cell;
           }
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 140, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_1); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 140, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           /* "aiocsv/_parser.pyx":142
  *                     row.append(float(cell) if numeric_cell else cell)  # type: ignore
  * 
  *                     cell = u""             # <<<<<<<<<<<<<<
  *                     force_save_cell = False
@@ -2824,16 +3896,16 @@
         /* "aiocsv/_parser.pyx":148
  * 
  *                 # 3. Start of an espace
  *                 elif char == dialect.escapechar:             # <<<<<<<<<<<<<<
  *                     state = ParserState.ESCAPE
  * 
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":149
  *                 # 3. Start of an espace
  *                 elif char == dialect.escapechar:
  *                     state = ParserState.ESCAPE             # <<<<<<<<<<<<<<
  * 
  *                 # 4. Normal char
@@ -2856,15 +3928,15 @@
  *                     cell += char             # <<<<<<<<<<<<<<
  * 
  *             elif state == ParserState.ESCAPE:
  */
         /*else*/ {
           __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_2));
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
         }
@@ -2885,15 +3957,15 @@
  *             elif state == ParserState.ESCAPE:
  *                 cell += char             # <<<<<<<<<<<<<<
  *                 state = ParserState.IN_CELL
  * 
  */
         __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
         __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_1));
         __Pyx_GIVEREF(__pyx_t_1);
         __pyx_t_1 = 0;
 
@@ -2919,16 +3991,16 @@
         /* "aiocsv/_parser.pyx":163
  * 
  *                 # 1. Start of an escape
  *                 if char == dialect.escapechar:             # <<<<<<<<<<<<<<
  *                     state = ParserState.ESCAPE_QUOTED
  * 
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.escapechar);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":164
  *                 # 1. Start of an escape
  *                 if char == dialect.escapechar:
  *                     state = ParserState.ESCAPE_QUOTED             # <<<<<<<<<<<<<<
  * 
  *                 # 2. Quotechar
@@ -2948,46 +4020,45 @@
         /* "aiocsv/_parser.pyx":167
  * 
  *                 # 2. Quotechar
  *                 elif dialect.quoting != ReadQuoting.NONE and char == dialect.quotechar and \             # <<<<<<<<<<<<<<
  *                         dialect.doublequote:
  *                     state = ParserState.QUOTE_IN_QUOTED
  */
-        __pyx_t_12 = ((__pyx_cur_scope->__pyx_v_dialect.quoting != __pyx_e_6aiocsv_7_parser_NONE) != 0);
-        if (__pyx_t_12) {
+        __pyx_t_13 = (__pyx_cur_scope->__pyx_v_dialect.quoting != __pyx_e_6aiocsv_7_parser_NONE);
+        if (__pyx_t_13) {
         } else {
-          __pyx_t_4 = __pyx_t_12;
+          __pyx_t_6 = __pyx_t_13;
           goto __pyx_L22_bool_binop_done;
         }
-        __pyx_t_12 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar) != 0);
-        if (__pyx_t_12) {
+        __pyx_t_13 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar);
+        if (__pyx_t_13) {
         } else {
-          __pyx_t_4 = __pyx_t_12;
+          __pyx_t_6 = __pyx_t_13;
           goto __pyx_L22_bool_binop_done;
         }
 
         /* "aiocsv/_parser.pyx":168
  *                 # 2. Quotechar
  *                 elif dialect.quoting != ReadQuoting.NONE and char == dialect.quotechar and \
  *                         dialect.doublequote:             # <<<<<<<<<<<<<<
  *                     state = ParserState.QUOTE_IN_QUOTED
  * 
  */
-        __pyx_t_12 = (__pyx_cur_scope->__pyx_v_dialect.doublequote != 0);
-        __pyx_t_4 = __pyx_t_12;
+        __pyx_t_6 = __pyx_cur_scope->__pyx_v_dialect.doublequote;
         __pyx_L22_bool_binop_done:;
 
         /* "aiocsv/_parser.pyx":167
  * 
  *                 # 2. Quotechar
  *                 elif dialect.quoting != ReadQuoting.NONE and char == dialect.quotechar and \             # <<<<<<<<<<<<<<
  *                         dialect.doublequote:
  *                     state = ParserState.QUOTE_IN_QUOTED
  */
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":169
  *                 elif dialect.quoting != ReadQuoting.NONE and char == dialect.quotechar and \
  *                         dialect.doublequote:
  *                     state = ParserState.QUOTE_IN_QUOTED             # <<<<<<<<<<<<<<
  * 
  *                 # 3. Every other char
@@ -3010,15 +4081,15 @@
  *                     cell += char             # <<<<<<<<<<<<<<
  * 
  *             elif state == ParserState.ESCAPE_QUOTED:
  */
         /*else*/ {
           __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_2));
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
         }
@@ -3039,15 +4110,15 @@
  *             elif state == ParserState.ESCAPE_QUOTED:
  *                 cell += char             # <<<<<<<<<<<<<<
  *                 state = ParserState.IN_CELL_QUOTED
  * 
  */
         __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
         __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_1));
         __Pyx_GIVEREF(__pyx_t_1);
         __pyx_t_1 = 0;
 
@@ -3073,27 +4144,27 @@
         /* "aiocsv/_parser.pyx":184
  * 
  *                 # 1. Double-quote
  *                 if char == dialect.quotechar:             # <<<<<<<<<<<<<<
  *                     cell += char
  *                     state = ParserState.IN_CELL_QUOTED
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.quotechar);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":185
  *                 # 1. Double-quote
  *                 if char == dialect.quotechar:
  *                     cell += char             # <<<<<<<<<<<<<<
  *                     state = ParserState.IN_CELL_QUOTED
  * 
  */
           __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_2));
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
 
@@ -3122,30 +4193,30 @@
  *                 elif char == u'\r' or char == u'\n':             # <<<<<<<<<<<<<<
  *                     row.append(cell)
  *                     cell = u""
  */
         switch (__pyx_cur_scope->__pyx_v_char) {
           case 13:
           case 10:
-          __pyx_t_4 = 1;
+          __pyx_t_6 = 1;
           break;
           default:
-          __pyx_t_4 = 0;
+          __pyx_t_6 = 0;
           break;
         }
-        if (__pyx_t_4) {
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":190
  *                 # 2. End of a row
  *                 elif char == u'\r' or char == u'\n':
  *                     row.append(cell)             # <<<<<<<<<<<<<<
  *                     cell = u""
  *                     force_save_cell = False
  */
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 190, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 190, __pyx_L1_error)
 
           /* "aiocsv/_parser.pyx":191
  *                 elif char == u'\r' or char == u'\n':
  *                     row.append(cell)
  *                     cell = u""             # <<<<<<<<<<<<<<
  *                     force_save_cell = False
  *                     state = ParserState.EAT_NEWLINE
@@ -3186,25 +4257,25 @@
         /* "aiocsv/_parser.pyx":196
  * 
  *                 # 3. End of a cell
  *                 elif char == dialect.delimiter:             # <<<<<<<<<<<<<<
  *                     row.append(cell)
  *                     cell = u""
  */
-        __pyx_t_4 = ((__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter) != 0);
-        if (__pyx_t_4) {
+        __pyx_t_6 = (__pyx_cur_scope->__pyx_v_char == __pyx_cur_scope->__pyx_v_dialect.delimiter);
+        if (__pyx_t_6) {
 
           /* "aiocsv/_parser.pyx":197
  *                 # 3. End of a cell
  *                 elif char == dialect.delimiter:
  *                     row.append(cell)             # <<<<<<<<<<<<<<
  *                     cell = u""
  *                     force_save_cell = False
  */
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
 
           /* "aiocsv/_parser.pyx":198
  *                 elif char == dialect.delimiter:
  *                     row.append(cell)
  *                     cell = u""             # <<<<<<<<<<<<<<
  *                     force_save_cell = False
  *                     state = ParserState.AFTER_DELIM
@@ -3248,15 +4319,15 @@
  *                     cell += char             # <<<<<<<<<<<<<<
  *                     state = ParserState.IN_CELL
  * 
  */
         /*else*/ {
           __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_cur_scope->__pyx_v_cell, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_cell);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_cell, ((PyObject*)__pyx_t_1));
           __Pyx_GIVEREF(__pyx_t_1);
           __pyx_t_1 = 0;
 
@@ -3272,16 +4343,15 @@
           /* "aiocsv/_parser.pyx":207
  *                     state = ParserState.IN_CELL
  * 
  *                     if dialect.strict:             # <<<<<<<<<<<<<<
  *                         raise csv.Error(
  *                             f"'{dialect.delimiter}' expected after '{dialect.quotechar}'"
  */
-          __pyx_t_4 = (__pyx_cur_scope->__pyx_v_dialect.strict != 0);
-          if (unlikely(__pyx_t_4)) {
+          if (unlikely(__pyx_cur_scope->__pyx_v_dialect.strict)) {
 
             /* "aiocsv/_parser.pyx":208
  * 
  *                     if dialect.strict:
  *                         raise csv.Error(             # <<<<<<<<<<<<<<
  *                             f"'{dialect.delimiter}' expected after '{dialect.quotechar}'"
  *                         )
@@ -3297,61 +4367,66 @@
  *                         raise csv.Error(
  *                             f"'{dialect.delimiter}' expected after '{dialect.quotechar}'"             # <<<<<<<<<<<<<<
  *                         )
  * 
  */
             __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_13 = 0;
-            __pyx_t_15 = 127;
+            __pyx_t_14 = 0;
+            __pyx_t_17 = 127;
             __Pyx_INCREF(__pyx_kp_u__3);
-            __pyx_t_13 += 1;
+            __pyx_t_14 += 1;
             __Pyx_GIVEREF(__pyx_kp_u__3);
             PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__3);
-            __pyx_t_16 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_dialect.delimiter); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 209, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
-            __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) : __pyx_t_15;
-            __pyx_t_13 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
-            __Pyx_GIVEREF(__pyx_t_16);
-            PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_16);
-            __pyx_t_16 = 0;
+            __pyx_t_18 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_dialect.delimiter); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 209, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_18);
+            __pyx_t_17 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_17) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_17;
+            __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+            __Pyx_GIVEREF(__pyx_t_18);
+            PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_18);
+            __pyx_t_18 = 0;
             __Pyx_INCREF(__pyx_kp_u_expected_after);
-            __pyx_t_13 += 18;
+            __pyx_t_14 += 18;
             __Pyx_GIVEREF(__pyx_kp_u_expected_after);
             PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_expected_after);
-            __pyx_t_16 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_dialect.quotechar); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 209, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
-            __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) : __pyx_t_15;
-            __pyx_t_13 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
-            __Pyx_GIVEREF(__pyx_t_16);
-            PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_16);
-            __pyx_t_16 = 0;
+            __pyx_t_18 = PyUnicode_FromOrdinal(__pyx_cur_scope->__pyx_v_dialect.quotechar); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 209, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_18);
+            __pyx_t_17 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) > __pyx_t_17) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_18) : __pyx_t_17;
+            __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_18);
+            __Pyx_GIVEREF(__pyx_t_18);
+            PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_18);
+            __pyx_t_18 = 0;
             __Pyx_INCREF(__pyx_kp_u__3);
-            __pyx_t_13 += 1;
+            __pyx_t_14 += 1;
             __Pyx_GIVEREF(__pyx_kp_u__3);
             PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u__3);
-            __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_2, 5, __pyx_t_13, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 209, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
+            __pyx_t_18 = __Pyx_PyUnicode_Join(__pyx_t_2, 5, __pyx_t_14, __pyx_t_17); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 209, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_18);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __pyx_t_2 = NULL;
+            __pyx_t_11 = 0;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
               __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
               if (likely(__pyx_t_2)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
                 __Pyx_INCREF(__pyx_t_2);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
+                __pyx_t_11 = 1;
               }
             }
-            __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_16) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_16);
-            __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_18};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_1);
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            }
             __Pyx_Raise(__pyx_t_1, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __PYX_ERR(0, 208, __pyx_L1_error)
 
             /* "aiocsv/_parser.pyx":207
  *                     state = ParserState.IN_CELL
  * 
@@ -3385,40 +4460,45 @@
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __PYX_ERR(0, 213, __pyx_L1_error)
         break;
       }
       __pyx_L7_continue:;
     }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "aiocsv/_parser.pyx":216
  * 
  *         # Read more data
  *         data = <unicode?>(await reader.read(READ_SIZE))             # <<<<<<<<<<<<<<
  * 
  *     if cell or force_save_cell:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_reader, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = NULL;
+    __pyx_t_18 = NULL;
+    __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_16)) {
+      __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_18)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_16);
+        __Pyx_INCREF(__pyx_t_18);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
       }
     }
-    __pyx_t_1 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_16, __pyx_int_2048) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_int_2048);
-    __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_18, __pyx_int_2048};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XGOTREF(__pyx_r);
     if (likely(__pyx_r)) {
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
@@ -3429,15 +4509,15 @@
       if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 216, __pyx_L1_error)
       __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
     } else {
       __pyx_t_1 = NULL;
       if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 216, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 216, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_1;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_data);
     __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_data, ((PyObject*)__pyx_t_3));
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_t_3 = 0;
@@ -3446,42 +4526,46 @@
   /* "aiocsv/_parser.pyx":218
  *         data = <unicode?>(await reader.read(READ_SIZE))
  * 
  *     if cell or force_save_cell:             # <<<<<<<<<<<<<<
  *         row.append(float(cell) if numeric_cell else cell)
  *     if row:
  */
-  __pyx_t_12 = (__pyx_cur_scope->__pyx_v_cell != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_cur_scope->__pyx_v_cell) != 0);
-  if (!__pyx_t_12) {
+  __pyx_t_13 = (__pyx_cur_scope->__pyx_v_cell != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_cur_scope->__pyx_v_cell) != 0);
+  if (!__pyx_t_13) {
   } else {
-    __pyx_t_4 = __pyx_t_12;
+    __pyx_t_6 = __pyx_t_13;
     goto __pyx_L29_bool_binop_done;
   }
-  __pyx_t_12 = (__pyx_cur_scope->__pyx_v_force_save_cell != 0);
-  __pyx_t_4 = __pyx_t_12;
+  __pyx_t_6 = __pyx_cur_scope->__pyx_v_force_save_cell;
   __pyx_L29_bool_binop_done:;
-  if (__pyx_t_4) {
+  if (__pyx_t_6) {
 
     /* "aiocsv/_parser.pyx":219
  * 
  *     if cell or force_save_cell:
  *         row.append(float(cell) if numeric_cell else cell)             # <<<<<<<<<<<<<<
  *     if row:
  *         yield row
  */
-    if ((__pyx_cur_scope->__pyx_v_numeric_cell != 0)) {
-      __pyx_t_1 = __Pyx_PyNumber_Float(__pyx_cur_scope->__pyx_v_cell); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    if (__pyx_cur_scope->__pyx_v_numeric_cell) {
+      if (unlikely(__pyx_cur_scope->__pyx_v_cell == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "float() argument must be a string or a number, not 'NoneType'");
+        __PYX_ERR(0, 219, __pyx_L1_error)
+      }
+      __pyx_t_16 = __Pyx_PyUnicode_AsDouble(__pyx_cur_scope->__pyx_v_cell); if (unlikely(__pyx_t_16 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble(__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_3 = __pyx_t_1;
       __pyx_t_1 = 0;
     } else {
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_cell);
       __pyx_t_3 = __pyx_cur_scope->__pyx_v_cell;
     }
-    __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_row, __pyx_t_3); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "aiocsv/_parser.pyx":218
  *         data = <unicode?>(await reader.read(READ_SIZE))
  * 
  *     if cell or force_save_cell:             # <<<<<<<<<<<<<<
  *         row.append(float(cell) if numeric_cell else cell)
@@ -3492,16 +4576,16 @@
   /* "aiocsv/_parser.pyx":220
  *     if cell or force_save_cell:
  *         row.append(float(cell) if numeric_cell else cell)
  *     if row:             # <<<<<<<<<<<<<<
  *         yield row
  * 
  */
-  __pyx_t_4 = (PyList_GET_SIZE(__pyx_cur_scope->__pyx_v_row) != 0);
-  if (__pyx_t_4) {
+  __pyx_t_6 = (PyList_GET_SIZE(__pyx_cur_scope->__pyx_v_row) != 0);
+  if (__pyx_t_6) {
 
     /* "aiocsv/_parser.pyx":221
  *         row.append(float(cell) if numeric_cell else cell)
  *     if row:
  *         yield row             # <<<<<<<<<<<<<<
  * 
  */
@@ -3534,19 +4618,20 @@
  *     cdef CDialect dialect = get_dialect(pydialect)
  */
 
   /* function exit code */
   PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(1);
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_16);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_18);
   __Pyx_AddTraceback("parser", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
@@ -3556,36 +4641,48 @@
 }
 
 static struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *__pyx_freelist_6aiocsv_7_parser___pyx_scope_struct__parser[8];
 static int __pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser = 0;
 
 static PyObject *__pyx_tp_new_6aiocsv_7_parser___pyx_scope_struct__parser(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser)))) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((int)(__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser)))) {
     o = (PyObject*)__pyx_freelist_6aiocsv_7_parser___pyx_scope_struct__parser[--__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser];
     memset(o, 0, sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
+  #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_6aiocsv_7_parser___pyx_scope_struct__parser(PyObject *o) {
   struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *p = (struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_6aiocsv_7_parser___pyx_scope_struct__parser) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_cell);
   Py_CLEAR(p->__pyx_v_data);
   Py_CLEAR(p->__pyx_v_pydialect);
   Py_CLEAR(p->__pyx_v_reader);
   Py_CLEAR(p->__pyx_v_row);
-  Py_CLEAR(p->__pyx_t_0);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser)))) {
+  Py_CLEAR(p->__pyx_t_1);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((int)(__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser)))) {
     __pyx_freelist_6aiocsv_7_parser___pyx_scope_struct__parser[__pyx_freecount_6aiocsv_7_parser___pyx_scope_struct__parser++] = ((struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_6aiocsv_7_parser___pyx_scope_struct__parser(PyObject *o, visitproc v, void *a) {
@@ -3598,18 +4695,33 @@
     e = (*v)(p->__pyx_v_reader, a); if (e) return e;
   }
   if (p->__pyx_v_row) {
     e = (*v)(p->__pyx_v_row, a); if (e) return e;
   }
   return 0;
 }
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_6aiocsv_7_parser___pyx_scope_struct__parser},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_6aiocsv_7_parser___pyx_scope_struct__parser},
+  {Py_tp_new, (void *)__pyx_tp_new_6aiocsv_7_parser___pyx_scope_struct__parser},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser_spec = {
+  "aiocsv._parser.__pyx_scope_struct__parser",
+  sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser = {
   PyVarObject_HEAD_INIT(0, 0)
-  "aiocsv._parser.__pyx_scope_struct__parser", /*tp_name*/
+  "aiocsv._parser.""__pyx_scope_struct__parser", /*tp_name*/
   sizeof(struct __pyx_obj_6aiocsv_7_parser___pyx_scope_struct__parser), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_6aiocsv_7_parser___pyx_scope_struct__parser, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -3629,150 +4741,144 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_6aiocsv_7_parser___pyx_scope_struct__parser, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_6aiocsv_7_parser___pyx_scope_struct__parser, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__parser(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__parser},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "_parser",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
-  {&__pyx_n_s_QUOTE_NONE, __pyx_k_QUOTE_NONE, sizeof(__pyx_k_QUOTE_NONE), 0, 0, 1, 1},
-  {&__pyx_n_s_QUOTE_NONNUMERIC, __pyx_k_QUOTE_NONNUMERIC, sizeof(__pyx_k_QUOTE_NONNUMERIC), 0, 0, 1, 1},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
-  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-  {&__pyx_n_s_aiocsv__parser, __pyx_k_aiocsv__parser, sizeof(__pyx_k_aiocsv__parser), 0, 0, 1, 1},
-  {&__pyx_kp_s_aiocsv__parser_pyx, __pyx_k_aiocsv__parser_pyx, sizeof(__pyx_k_aiocsv__parser_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {&__pyx_n_s_await, __pyx_k_await, sizeof(__pyx_k_await), 0, 0, 1, 1},
-  {&__pyx_n_s_cell, __pyx_k_cell, sizeof(__pyx_k_cell), 0, 0, 1, 1},
-  {&__pyx_n_s_char, __pyx_k_char, sizeof(__pyx_k_char), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
-  {&__pyx_n_s_csv, __pyx_k_csv, sizeof(__pyx_k_csv), 0, 0, 1, 1},
-  {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {&__pyx_n_s_delimiter, __pyx_k_delimiter, sizeof(__pyx_k_delimiter), 0, 0, 1, 1},
-  {&__pyx_n_s_dialect, __pyx_k_dialect, sizeof(__pyx_k_dialect), 0, 0, 1, 1},
-  {&__pyx_n_s_doublequote, __pyx_k_doublequote, sizeof(__pyx_k_doublequote), 0, 0, 1, 1},
-  {&__pyx_n_s_escapechar, __pyx_k_escapechar, sizeof(__pyx_k_escapechar), 0, 0, 1, 1},
-  {&__pyx_kp_u_expected_after, __pyx_k_expected_after, sizeof(__pyx_k_expected_after), 0, 1, 0, 0},
-  {&__pyx_n_s_force_save_cell, __pyx_k_force_save_cell, sizeof(__pyx_k_force_save_cell), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_numeric_cell, __pyx_k_numeric_cell, sizeof(__pyx_k_numeric_cell), 0, 0, 1, 1},
-  {&__pyx_n_s_parser, __pyx_k_parser, sizeof(__pyx_k_parser), 0, 0, 1, 1},
-  {&__pyx_n_s_pydialect, __pyx_k_pydialect, sizeof(__pyx_k_pydialect), 0, 0, 1, 1},
-  {&__pyx_n_s_quotechar, __pyx_k_quotechar, sizeof(__pyx_k_quotechar), 0, 0, 1, 1},
-  {&__pyx_n_s_quoting, __pyx_k_quoting, sizeof(__pyx_k_quoting), 0, 0, 1, 1},
-  {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
-  {&__pyx_n_s_reader, __pyx_k_reader, sizeof(__pyx_k_reader), 0, 0, 1, 1},
-  {&__pyx_n_s_row, __pyx_k_row, sizeof(__pyx_k_row), 0, 0, 1, 1},
-  {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
-  {&__pyx_n_s_skipinitialspace, __pyx_k_skipinitialspace, sizeof(__pyx_k_skipinitialspace), 0, 0, 1, 1},
-  {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
-  {&__pyx_n_s_strict, __pyx_k_strict, sizeof(__pyx_k_strict), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
-  {&__pyx_n_u_wtf, __pyx_k_wtf, sizeof(__pyx_k_wtf), 0, 1, 0, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
+    {&__pyx_n_s_QUOTE_NONE, __pyx_k_QUOTE_NONE, sizeof(__pyx_k_QUOTE_NONE), 0, 0, 1, 1},
+    {&__pyx_n_s_QUOTE_NONNUMERIC, __pyx_k_QUOTE_NONNUMERIC, sizeof(__pyx_k_QUOTE_NONNUMERIC), 0, 0, 1, 1},
+    {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+    {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
+    {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
+    {&__pyx_n_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 1},
+    {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
+    {&__pyx_n_s_aiocsv__parser, __pyx_k_aiocsv__parser, sizeof(__pyx_k_aiocsv__parser), 0, 0, 1, 1},
+    {&__pyx_kp_s_aiocsv__parser_pyx, __pyx_k_aiocsv__parser_pyx, sizeof(__pyx_k_aiocsv__parser_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_await, __pyx_k_await, sizeof(__pyx_k_await), 0, 0, 1, 1},
+    {&__pyx_n_s_cell, __pyx_k_cell, sizeof(__pyx_k_cell), 0, 0, 1, 1},
+    {&__pyx_n_s_char, __pyx_k_char, sizeof(__pyx_k_char), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+    {&__pyx_n_s_csv, __pyx_k_csv, sizeof(__pyx_k_csv), 0, 0, 1, 1},
+    {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+    {&__pyx_n_s_delimiter, __pyx_k_delimiter, sizeof(__pyx_k_delimiter), 0, 0, 1, 1},
+    {&__pyx_n_s_dialect, __pyx_k_dialect, sizeof(__pyx_k_dialect), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_doublequote, __pyx_k_doublequote, sizeof(__pyx_k_doublequote), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_escapechar, __pyx_k_escapechar, sizeof(__pyx_k_escapechar), 0, 0, 1, 1},
+    {&__pyx_kp_u_expected_after, __pyx_k_expected_after, sizeof(__pyx_k_expected_after), 0, 1, 0, 0},
+    {&__pyx_n_s_force_save_cell, __pyx_k_force_save_cell, sizeof(__pyx_k_force_save_cell), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_numeric_cell, __pyx_k_numeric_cell, sizeof(__pyx_k_numeric_cell), 0, 0, 1, 1},
+    {&__pyx_n_s_parser, __pyx_k_parser, sizeof(__pyx_k_parser), 0, 0, 1, 1},
+    {&__pyx_n_s_pydialect, __pyx_k_pydialect, sizeof(__pyx_k_pydialect), 0, 0, 1, 1},
+    {&__pyx_n_s_quotechar, __pyx_k_quotechar, sizeof(__pyx_k_quotechar), 0, 0, 1, 1},
+    {&__pyx_n_s_quoting, __pyx_k_quoting, sizeof(__pyx_k_quoting), 0, 0, 1, 1},
+    {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
+    {&__pyx_n_s_reader, __pyx_k_reader, sizeof(__pyx_k_reader), 0, 0, 1, 1},
+    {&__pyx_n_s_row, __pyx_k_row, sizeof(__pyx_k_row), 0, 0, 1, 1},
+    {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
+    {&__pyx_n_s_skipinitialspace, __pyx_k_skipinitialspace, sizeof(__pyx_k_skipinitialspace), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
+    {&__pyx_n_s_strict, __pyx_k_strict, sizeof(__pyx_k_strict), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
+    {&__pyx_n_u_wtf, __pyx_k_wtf, sizeof(__pyx_k_wtf), 0, 1, 0, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 213, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "aiocsv/_parser.pyx":213
  * 
@@ -3788,32 +4894,39 @@
   /* "aiocsv/_parser.pyx":59
  * 
  * 
  * async def parser(reader, pydialect):             # <<<<<<<<<<<<<<
  *     cdef unicode data = <unicode?>(await reader.read(READ_SIZE))
  *     cdef CDialect dialect = get_dialect(pydialect)
  */
-  __pyx_tuple__5 = PyTuple_Pack(10, __pyx_n_s_reader, __pyx_n_s_pydialect, __pyx_n_s_data, __pyx_n_s_dialect, __pyx_n_s_state, __pyx_n_s_row, __pyx_n_s_cell, __pyx_n_s_force_save_cell, __pyx_n_s_numeric_cell, __pyx_n_s_char); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(2, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aiocsv__parser_pyx, __pyx_n_s_parser, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(10, __pyx_n_s_reader, __pyx_n_s_pydialect, __pyx_n_s_data, __pyx_n_s_dialect, __pyx_n_s_state, __pyx_n_s_row, __pyx_n_s_cell, __pyx_n_s_force_save_cell, __pyx_n_s_numeric_cell, __pyx_n_s_char); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_ASYNC_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aiocsv__parser_pyx, __pyx_n_s_parser, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_2048 = PyInt_FromLong(2048); if (unlikely(!__pyx_int_2048)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  return 0;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -3846,22 +4959,33 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser.tp_print = 0;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser_spec, NULL); if (unlikely(!__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser)) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser_spec, __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  #else
+  __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser = &__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser.tp_dictoffset && __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser->tp_dictoffset && __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_6aiocsv_7_parser___pyx_scope_struct__parser = &__pyx_type_6aiocsv_7_parser___pyx_scope_struct__parser;
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3886,14 +5010,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec__parser(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__parser},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "_parser",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -3936,42 +5109,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -3979,28 +5166,62 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__parser(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module '_parser' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("_parser", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _parser pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -4011,143 +5232,152 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_parser", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_aiocsv___parser) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "aiocsv._parser")) {
-      if (unlikely(PyDict_SetItemString(modules, "aiocsv._parser", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "aiocsv._parser", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "aiocsv/_parser.pyx":1
  * import csv             # <<<<<<<<<<<<<<
  * 
  * DEF READ_SIZE = 2048
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_csv, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_csv, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_csv, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_csv, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "aiocsv/_parser.pyx":59
  * 
  * 
  * async def parser(reader, pydialect):             # <<<<<<<<<<<<<<
  *     cdef unicode data = <unicode?>(await reader.read(READ_SIZE))
  *     cdef CDialect dialect = get_dialect(pydialect)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6aiocsv_7_parser_1parser, NULL, __pyx_n_s_aiocsv__parser); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parser, __pyx_t_1) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6aiocsv_7_parser_1parser, __Pyx_CYFUNCTION_COROUTINE, __pyx_n_s_parser, NULL, __pyx_n_s_aiocsv__parser, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parser, __pyx_t_2) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "aiocsv/_parser.pyx":1
  * import csv             # <<<<<<<<<<<<<<
  * 
  * DEF READ_SIZE = 2048
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init aiocsv._parser", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init aiocsv._parser");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#if _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -4159,32 +5389,103 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
@@ -4230,14 +5531,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -4251,15 +5560,15 @@
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (!j) return NULL;
+    if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -4312,103 +5621,252 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return m->sq_item(o, i);
+            return sm->sq_item(o, i);
         }
     }
 #else
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
 }
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
 }
 #endif
 
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
 #endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
 #endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
     }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
     } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
     }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
 #endif
 }
 
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -4444,25 +5902,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -4488,19 +5958,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -4531,51 +6002,29 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -4596,15 +6045,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -4612,15 +6060,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -4683,15 +6131,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
@@ -4705,43 +6152,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
     self = PyCFunction_GET_SELF(func);
@@ -4754,98 +6172,278 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
 #endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
+    }
 #endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
         }
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
+
+/* FixUpExtensionType */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
 #else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
 }
 #endif
 
+/* FetchSharedCythonModule */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
 /* FetchCommonType */
+static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
-    PyObject* fake_module;
-    PyTypeObject* cached_type = NULL;
-    fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
-    if (!fake_module) return NULL;
-    Py_INCREF(fake_module);
-    cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
     if (cached_type) {
-        if (!PyType_Check((PyObject*)cached_type)) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s is not a type object",
-                type->tp_name);
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
             goto bad;
         }
-        if (cached_type->tp_basicsize != type->tp_basicsize) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s has the wrong size, try recompiling",
-                type->tp_name);
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
             goto bad;
         }
-    } else {
-        if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-        PyErr_Clear();
-        if (PyType_Ready(type) < 0) goto bad;
-        if (PyObject_SetAttrString(fake_module, type->tp_name, (PyObject*) type) < 0)
-            goto bad;
-        Py_INCREF(type);
-        cached_type = type;
+        goto done;
     }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
 done:
-    Py_DECREF(fake_module);
-    return cached_type;
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
+#endif
 
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -4970,69 +6568,94 @@
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
 
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
         exc_info = exc_info->previous_item;
     }
     return exc_info;
 }
 #endif
 
 /* SaveResetException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
     *type = exc_info->exc_type;
     *value = exc_info->exc_value;
     *tb = exc_info->exc_traceback;
-    #else
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
     *type = tstate->exc_type;
     *value = tstate->exc_value;
     *tb = tstate->exc_traceback;
-    #endif
     Py_XINCREF(*type);
     Py_XINCREF(*value);
     Py_XINCREF(*tb);
+  #endif
 }
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = type;
@@ -5045,37 +6668,52 @@
     tstate->exc_type = type;
     tstate->exc_value = value;
     tstate->exc_traceback = tb;
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+  #endif
 }
 #endif
 
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        tmp_tb = PyException_GetTraceback(tmp_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
     exc_info->exc_value = *value;
     exc_info->exc_traceback = *tb;
-    #else
+  #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = *type;
     tstate->exc_value = *value;
     tstate->exc_traceback = *tb;
-    #endif
+  #endif
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -5083,18 +6721,31 @@
     PyErr_SetExcInfo(*type, *value, *tb);
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
     PyObject **dictptr, *dict;
     int meth_found = 0;
     assert (*method == NULL);
     if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
@@ -5103,19 +6754,21 @@
     }
     if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
         return 0;
     }
     descr = _PyType_Lookup(tp, name);
     if (likely(descr != NULL)) {
         Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
         #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
         #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
         #endif
 #else
         #ifdef __Pyx_CyFunction_USED
         if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
         #else
         if (likely(PyFunction_Check(descr)))
         #endif
@@ -5148,26 +6801,28 @@
         return 1;
     }
     if (f != NULL) {
         attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
         Py_DECREF(descr);
         goto try_unpack;
     }
-    if (descr != NULL) {
+    if (likely(descr != NULL)) {
         *method = descr;
         return 0;
     }
+    type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 #else
     attr = __Pyx_PyObject_GetAttrStr(obj, name);
     goto try_unpack;
 #endif
 try_unpack:
 #if CYTHON_UNPACK_METHODS
@@ -5197,42 +6852,48 @@
         Py_DECREF(method);
         return result;
     }
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
 /* CoroutineBase */
-#include <structmember.h>
 #include <frameobject.h>
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
-static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
+static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
+    CYTHON_UNUSED_VAR(__pyx_tstate);
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
         Py_XDECREF(ev);
         Py_INCREF(Py_None);
         *pvalue = Py_None;
         return 0;
     }
     if (likely(et == PyExc_StopIteration)) {
         if (!ev) {
             Py_INCREF(Py_None);
             value = Py_None;
         }
 #if PY_VERSION_HEX >= 0x030300A0
-        else if (Py_TYPE(ev) == (PyTypeObject*)PyExc_StopIteration) {
+        else if (likely(__Pyx_IS_TYPE(ev, (PyTypeObject*)PyExc_StopIteration))) {
             value = ((PyStopIterationObject *)ev)->value;
             Py_INCREF(value);
             Py_DECREF(ev);
         }
 #endif
         else if (unlikely(PyTuple_Check(ev))) {
             if (PyTuple_GET_SIZE(ev) >= 1) {
@@ -5288,28 +6949,33 @@
     }
 #endif
     *pvalue = value;
     return 0;
 }
 static CYTHON_INLINE
 void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_CLEAR(exc_state->exc_value);
+#else
     PyObject *t, *v, *tb;
     t = exc_state->exc_type;
     v = exc_state->exc_value;
     tb = exc_state->exc_traceback;
     exc_state->exc_type = NULL;
     exc_state->exc_value = NULL;
     exc_state->exc_traceback = NULL;
     Py_XDECREF(t);
     Py_XDECREF(v);
     Py_XDECREF(tb);
+#endif
 }
 #define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyRunningError(CYTHON_UNUSED __pyx_CoroutineObject *gen) {
+static void __Pyx__Coroutine_AlreadyRunningError(__pyx_CoroutineObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
         msg = "coroutine already executing";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
@@ -5317,16 +6983,17 @@
     #endif
     } else {
         msg = "generator already executing";
     }
     PyErr_SetString(PyExc_ValueError, msg);
 }
 #define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_NotStartedError(CYTHON_UNUSED PyObject *gen) {
+static void __Pyx__Coroutine_NotStartedError(PyObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check(gen)) {
         msg = "can't send non-None value to a just-started coroutine";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact(gen)) {
@@ -5334,15 +7001,17 @@
     #endif
     } else {
         msg = "can't send non-None value to a just-started generator";
     }
     PyErr_SetString(PyExc_TypeError, msg);
 }
 #define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyTerminatedError(CYTHON_UNUSED PyObject *gen, PyObject *value, CYTHON_UNUSED int closing) {
+static void __Pyx__Coroutine_AlreadyTerminatedError(PyObject *gen, PyObject *value, int closing) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    CYTHON_MAYBE_UNUSED_VAR(closing);
     #ifdef __Pyx_Coroutine_USED
     if (!closing && __Pyx_Coroutine_Check(gen)) {
         PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
     } else
     #endif
     if (value) {
         #ifdef __Pyx_AsyncGen_USED
@@ -5371,27 +7040,36 @@
 #if CYTHON_FAST_THREAD_STATE
     __Pyx_PyThreadState_assign
     tstate = __pyx_tstate;
 #else
     tstate = __Pyx_PyThreadState_Current;
 #endif
     exc_state = &self->gi_exc_state;
-    if (exc_state->exc_type) {
-        #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+    if (exc_state->exc_value) {
+        #if CYTHON_COMPILING_IN_PYPY
+        #else
+        PyObject *exc_tb;
+        #if PY_VERSION_HEX >= 0x030B00a4
+        exc_tb = PyException_GetTraceback(exc_state->exc_value);
         #else
-        if (exc_state->exc_traceback) {
-            PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
+        exc_tb = exc_state->exc_traceback;
+        #endif
+        if (exc_tb) {
+            PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
             PyFrameObject *f = tb->tb_frame;
             assert(f->f_back == NULL);
             #if PY_VERSION_HEX >= 0x030B00A1
             f->f_back = PyThreadState_GetFrame(tstate);
             #else
             Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
             #endif
+            #if PY_VERSION_HEX >= 0x030B00a4
+            Py_DECREF(exc_tb);
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -5399,37 +7077,48 @@
         __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     } else {
         __Pyx_Coroutine_ExceptionClear(exc_state);
         __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     }
 #endif
     self->is_running = 1;
-    retval = self->body((PyObject *) self, tstate, value);
+    retval = self->body(self, tstate, value);
     self->is_running = 0;
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state = &self->gi_exc_state;
     tstate->exc_info = exc_state->previous_item;
     exc_state->previous_item = NULL;
     __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
 #endif
     return retval;
 }
 static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
-    PyObject *exc_tb = exc_state->exc_traceback;
-    if (likely(exc_tb)) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+#if CYTHON_COMPILING_IN_PYPY
+    CYTHON_UNUSED_VAR(exc_state);
 #else
+    PyObject *exc_tb;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    if (!exc_state->exc_value) return;
+    exc_tb = PyException_GetTraceback(exc_state->exc_value);
+    #else
+    exc_tb = exc_state->exc_traceback;
+    #endif
+    if (likely(exc_tb)) {
         PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
         PyFrameObject *f = tb->tb_frame;
         Py_CLEAR(f->f_back);
-#endif
+        #if PY_VERSION_HEX >= 0x030B00a4
+        Py_DECREF(exc_tb);
+        #endif
     }
+#endif
 }
 static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_MethodReturn(CYTHON_UNUSED PyObject* gen, PyObject *retval) {
+PyObject *__Pyx_Coroutine_MethodReturn(PyObject* gen, PyObject *retval) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if (unlikely(!retval)) {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         if (!__Pyx_PyErr_Occurred()) {
             PyObject *exc = PyExc_StopIteration;
             #ifdef __Pyx_AsyncGen_USED
             if (__Pyx_AsyncGen_CheckExact(gen))
@@ -5506,15 +7195,15 @@
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyCoro_CheckExact(yf)) {
             ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         {
             if (value == Py_None)
-                ret = Py_TYPE(yf)->tp_iternext(yf);
+                ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
             else
                 ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
         }
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
@@ -5553,24 +7242,23 @@
     if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
         retval = __Pyx_async_gen_athrow_close(yf, NULL);
     } else
     #endif
     {
         PyObject *meth;
         gen->is_running = 1;
-        meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_close);
+        meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_close);
         if (unlikely(!meth)) {
-            if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+            if (unlikely(PyErr_Occurred())) {
                 PyErr_WriteUnraisable(yf);
             }
-            PyErr_Clear();
         } else {
-            retval = PyObject_CallFunction(meth, NULL);
+            retval = __Pyx_PyObject_CallNoArg(meth);
             Py_DECREF(meth);
-            if (!retval)
+            if (unlikely(!retval))
                 err = -1;
         }
         gen->is_running = 0;
     }
     Py_XDECREF(retval);
     return err;
 }
@@ -5593,24 +7281,25 @@
         } else
         #endif
         #ifdef __Pyx_Coroutine_USED
         if (__Pyx_Coroutine_Check(yf)) {
             ret = __Pyx_Coroutine_Send(yf, Py_None);
         } else
         #endif
-            ret = Py_TYPE(yf)->tp_iternext(yf);
+            ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
         return __Pyx_Coroutine_FinishDelegation(gen);
     }
     return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
 }
-static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_Coroutine_Close(self);
 }
 static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject *retval, *raised_exception;
     PyObject *yf = gen->yieldfrom;
     int err = 0;
@@ -5683,30 +7372,30 @@
             ) {
             ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
         #ifdef __Pyx_Coroutine_USED
         } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
             ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
         #endif
         } else {
-            PyObject *meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_throw);
+            PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_throw);
             if (unlikely(!meth)) {
                 Py_DECREF(yf);
-                if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+                if (unlikely(PyErr_Occurred())) {
                     gen->is_running = 0;
                     return NULL;
                 }
-                PyErr_Clear();
                 __Pyx_Coroutine_Undelegate(gen);
                 gen->is_running = 0;
                 goto throw_here;
             }
             if (likely(args)) {
-                ret = PyObject_CallObject(meth, args);
+                ret = __Pyx_PyObject_Call(meth, args, NULL);
             } else {
-                ret = PyObject_CallFunctionObjArgs(meth, typ, val, tb, NULL);
+                PyObject *cargs[4] = {NULL, typ, val, tb};
+                ret = __Pyx_PyObject_FastCall(meth, cargs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
             }
             Py_DECREF(meth);
         }
         gen->is_running = 0;
         Py_DECREF(yf);
         if (!ret) {
             ret = __Pyx_Coroutine_FinishDelegation(gen);
@@ -5717,22 +7406,26 @@
     __Pyx_Raise(typ, val, tb, NULL);
     return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
 }
 static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
     PyObject *typ;
     PyObject *val = NULL;
     PyObject *tb = NULL;
-    if (!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb))
+    if (unlikely(!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb)))
         return NULL;
     return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
 }
 static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_VISIT(exc_state->exc_value);
+#else
     Py_VISIT(exc_state->exc_type);
     Py_VISIT(exc_state->exc_value);
     Py_VISIT(exc_state->exc_traceback);
+#endif
     return 0;
 }
 static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
     Py_VISIT(gen->closure);
     Py_VISIT(gen->classobj);
     Py_VISIT(gen->yieldfrom);
     return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
@@ -5759,18 +7452,18 @@
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject_GC_UnTrack(gen);
     if (gen->gi_weakreflist != NULL)
         PyObject_ClearWeakRefs(self);
     if (gen->resume_label >= 0) {
         PyObject_GC_Track(self);
 #if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
-        if (PyObject_CallFinalizerFromDealloc(self))
+        if (unlikely(PyObject_CallFinalizerFromDealloc(self)))
 #else
         Py_TYPE(gen)->tp_del(self);
-        if (Py_REFCNT(self) > 0)
+        if (unlikely(Py_REFCNT(self) > 0))
 #endif
         {
             return;
         }
         PyObject_GC_UnTrack(self);
     }
 #ifdef __Pyx_AsyncGen_USED
@@ -5778,15 +7471,15 @@
         /* We have to handle this case for asynchronous generators
            right here, because this code has to be between UNTRACK
            and GC_Del. */
         Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
     }
 #endif
     __Pyx_Coroutine_clear(self);
-    PyObject_GC_Del(gen);
+    __Pyx_PyHeapTypeObject_GC_Del(gen);
 }
 static void __Pyx_Coroutine_del(PyObject *self) {
     PyObject *error_type, *error_value, *error_traceback;
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     __Pyx_PyThreadState_declare
     if (gen->resume_label < 0) {
         return;
@@ -5857,15 +7550,15 @@
         } else {
             Py_DECREF(res);
         }
     }
     __Pyx_ErrRestore(error_type, error_value, error_traceback);
 #if !CYTHON_USE_TP_FINALIZE
     assert(Py_REFCNT(self) > 0);
-    if (--self->ob_refcnt == 0) {
+    if (likely(--self->ob_refcnt == 0)) {
         return;
     }
     {
         Py_ssize_t refcnt = Py_REFCNT(self);
         _Py_NewReference(self);
         __Pyx_SET_REFCNT(self, refcnt);
     }
@@ -5877,73 +7570,72 @@
 #ifdef COUNT_ALLOCS
     --Py_TYPE(self)->tp_frees;
     --Py_TYPE(self)->tp_allocs;
 #endif
 #endif
 }
 static PyObject *
-__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_name;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__name__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_name;
     Py_INCREF(value);
-    self->gi_name = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_name, value);
     return 0;
 }
 static PyObject *
-__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_qualname;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__qualname__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_qualname;
     Py_INCREF(value);
-    self->gi_qualname = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_qualname, value);
     return 0;
 }
 static PyObject *
-__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *frame = self->gi_frame;
+    CYTHON_UNUSED_VAR(context);
     if (!frame) {
         if (unlikely(!self->gi_code)) {
             Py_RETURN_NONE;
         }
         frame = (PyObject *) PyFrame_New(
             PyThreadState_Get(),            /*PyThreadState *tstate,*/
             (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
@@ -5971,17 +7663,21 @@
     gen->body = body;
     gen->closure = closure;
     Py_XINCREF(closure);
     gen->is_running = 0;
     gen->resume_label = 0;
     gen->classobj = NULL;
     gen->yieldfrom = NULL;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    gen->gi_exc_state.exc_value = NULL;
+    #else
     gen->gi_exc_state.exc_type = NULL;
     gen->gi_exc_state.exc_value = NULL;
     gen->gi_exc_state.exc_traceback = NULL;
+    #endif
 #if CYTHON_USE_EXC_INFO_STACK
     gen->gi_exc_state.previous_item = NULL;
 #endif
     gen->gi_weakreflist = NULL;
     Py_XINCREF(qualname);
     gen->gi_qualname = qualname;
     Py_XINCREF(name);
@@ -5994,22 +7690,24 @@
     PyObject_GC_Track(gen);
     return gen;
 }
 
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -6098,15 +7796,15 @@
 #endif
 static int __Pyx_patch_abc(void) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
     static int abc_patched = 0;
     if (CYTHON_REGISTER_ABCS && !abc_patched) {
         PyObject *module;
         module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
-        if (!module) {
+        if (unlikely(!module)) {
             PyErr_WriteUnraisable(NULL);
             if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
                     ((PY_MAJOR_VERSION >= 3) ?
                         "Cython module failed to register with collections.abc module" :
                         "Cython module failed to register with collections module"), 1) < 0)) {
                 return -1;
             }
@@ -6132,15 +7830,15 @@
     return 0;
 }
 
 /* Coroutine */
 static void __Pyx_CoroutineAwait_dealloc(PyObject *self) {
     PyObject_GC_UnTrack(self);
     Py_CLEAR(((__pyx_CoroutineAwaitObject*)self)->coroutine);
-    PyObject_GC_Del(self);
+    __Pyx_PyHeapTypeObject_GC_Del(self);
 }
 static int __Pyx_CoroutineAwait_traverse(__pyx_CoroutineAwaitObject *self, visitproc visit, void *arg) {
     Py_VISIT(self->coroutine);
     return 0;
 }
 static int __Pyx_CoroutineAwait_clear(__pyx_CoroutineAwaitObject *self) {
     Py_CLEAR(self->coroutine);
@@ -6151,39 +7849,72 @@
 }
 static PyObject *__Pyx_CoroutineAwait_Send(__pyx_CoroutineAwaitObject *self, PyObject *value) {
     return __Pyx_Coroutine_Send(self->coroutine, value);
 }
 static PyObject *__Pyx_CoroutineAwait_Throw(__pyx_CoroutineAwaitObject *self, PyObject *args) {
     return __Pyx_Coroutine_Throw(self->coroutine, args);
 }
-static PyObject *__Pyx_CoroutineAwait_Close(__pyx_CoroutineAwaitObject *self, CYTHON_UNUSED PyObject *arg) {
+static PyObject *__Pyx_CoroutineAwait_Close(__pyx_CoroutineAwaitObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_Coroutine_Close(self->coroutine);
 }
 static PyObject *__Pyx_CoroutineAwait_self(PyObject *self) {
     Py_INCREF(self);
     return self;
 }
 #if !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_CoroutineAwait_no_new(CYTHON_UNUSED PyTypeObject *type, CYTHON_UNUSED PyObject *args, CYTHON_UNUSED PyObject *kwargs) {
+static PyObject *__Pyx_CoroutineAwait_no_new(PyTypeObject *type, PyObject *args, PyObject *kwargs) {
+    CYTHON_UNUSED_VAR(type);
+    CYTHON_UNUSED_VAR(args);
+    CYTHON_UNUSED_VAR(kwargs);
     PyErr_SetString(PyExc_TypeError, "cannot instantiate type, use 'await coroutine' instead");
     return NULL;
 }
 #endif
+static PyObject *__Pyx_CoroutineAwait_reduce_ex(__pyx_CoroutineAwaitObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
+    PyErr_Format(PyExc_TypeError, "cannot pickle '%.200s' object",
+                         Py_TYPE(self)->tp_name);
+    return NULL;
+}
 static PyMethodDef __pyx_CoroutineAwait_methods[] = {
     {"send", (PyCFunction) __Pyx_CoroutineAwait_Send, METH_O,
      (char*) PyDoc_STR("send(arg) -> send 'arg' into coroutine,\nreturn next yielded value or raise StopIteration.")},
     {"throw", (PyCFunction) __Pyx_CoroutineAwait_Throw, METH_VARARGS,
      (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in coroutine,\nreturn next yielded value or raise StopIteration.")},
     {"close", (PyCFunction) __Pyx_CoroutineAwait_Close, METH_NOARGS,
      (char*) PyDoc_STR("close() -> raise GeneratorExit inside coroutine.")},
+    {"__reduce_ex__", (PyCFunction) __Pyx_CoroutineAwait_reduce_ex, METH_O, 0},
+    {"__reduce__", (PyCFunction) __Pyx_CoroutineAwait_reduce_ex, METH_NOARGS, 0},
     {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CoroutineAwaitType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CoroutineAwait_dealloc},
+    {Py_tp_traverse, (void *)__Pyx_CoroutineAwait_traverse},
+    {Py_tp_clear, (void *)__Pyx_CoroutineAwait_clear},
+#if !CYTHON_COMPILING_IN_PYPY
+    {Py_tp_new, (void *)__Pyx_CoroutineAwait_no_new},
+#endif
+    {Py_tp_methods, (void *)__pyx_CoroutineAwait_methods},
+    {Py_tp_iter, (void *)__Pyx_CoroutineAwait_self},
+    {Py_tp_iternext, (void *)__Pyx_CoroutineAwait_Next},
+    {0, 0},
+};
+static PyType_Spec __pyx_CoroutineAwaitType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "coroutine_wrapper",
+    sizeof(__pyx_CoroutineAwaitObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
+    __pyx_CoroutineAwaitType_slots
+};
+#else
 static PyTypeObject __pyx_CoroutineAwaitType_type = {
     PyVarObject_HEAD_INIT(0, 0)
-    "coroutine_wrapper",
+    __PYX_TYPE_MODULE_PREFIX "coroutine_wrapper",
     sizeof(__pyx_CoroutineAwaitObject),
     0,
     (destructor) __Pyx_CoroutineAwait_dealloc,
     0,
     0,
     0,
     0,
@@ -6234,30 +7965,35 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
+#endif
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
     Py_INCREF(coroutine);
     await->coroutine = coroutine;
     PyObject_GC_Track(await);
     return (PyObject*)await;
 }
 #endif
 #if PY_VERSION_HEX < 0x030500B1
-static PyObject *__Pyx_Coroutine_await_method(PyObject *coroutine, CYTHON_UNUSED PyObject *arg) {
+static PyObject *__Pyx_Coroutine_await_method(PyObject *coroutine, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx__Coroutine_await(coroutine);
 }
 #endif
 #if defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static PyObject *__Pyx_Coroutine_await(PyObject *coroutine) {
     if (unlikely(!coroutine || !__Pyx_Coroutine_Check(coroutine))) {
         PyErr_SetString(PyExc_TypeError, "invalid input, expected coroutine");
@@ -6293,39 +8029,64 @@
     {0, 0, 0, 0}
 };
 static PyMemberDef __pyx_Coroutine_memberlist[] = {
     {(char *) "cr_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
     {(char*) "cr_await", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
      (char*) PyDoc_STR("object being awaited, or None")},
     {(char*) "cr_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
-    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), PY_WRITE_RESTRICTED, 0},
+    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyGetSetDef __pyx_Coroutine_getsets[] = {
     {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the coroutine"), 0},
     {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the coroutine"), 0},
     {(char *) "cr_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
      (char*) PyDoc_STR("Frame of the coroutine"), 0},
     {0, 0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CoroutineType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
+    {Py_am_await, (void *)&__Pyx_Coroutine_await},
+    {Py_tp_traverse, (void *)__Pyx_Coroutine_traverse},
+    {Py_tp_methods, (void *)__pyx_Coroutine_methods},
+    {Py_tp_members, (void *)__pyx_Coroutine_memberlist},
+    {Py_tp_getset, (void *)__pyx_Coroutine_getsets},
+    {Py_tp_getattro, (void *) __Pyx_PyObject_GenericGetAttrNoDict},
+#if CYTHON_USE_TP_FINALIZE
+    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
+#endif
+    {0, 0},
+};
+static PyType_Spec __pyx_CoroutineType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "coroutine",
+    sizeof(__pyx_CoroutineObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    __pyx_CoroutineType_slots
+};
+#else
 #if CYTHON_USE_ASYNC_SLOTS
 static __Pyx_PyAsyncMethodsStruct __pyx_Coroutine_as_async = {
     __Pyx_Coroutine_await,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030A00A3
     0,
 #endif
 };
 #endif
 static PyTypeObject __pyx_CoroutineType_type = {
     PyVarObject_HEAD_INIT(0, 0)
-    "coroutine",
+    __PYX_TYPE_MODULE_PREFIX "coroutine",
     sizeof(__pyx_CoroutineObject),
     0,
     (destructor) __Pyx_Coroutine_dealloc,
     0,
     0,
     0,
 #if CYTHON_USE_ASYNC_SLOTS
@@ -6386,87 +8147,76 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
-static int __pyx_Coroutine_init(void) {
+#endif
+static int __pyx_Coroutine_init(PyObject *module) {
+    CYTHON_MAYBE_UNUSED_VAR(module);
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CoroutineType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CoroutineType_spec, NULL);
+#else
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
+#endif
     if (unlikely(!__pyx_CoroutineType))
         return -1;
 #ifdef __Pyx_IterableCoroutine_USED
-    if (unlikely(__pyx_IterableCoroutine_init() == -1))
+    if (unlikely(__pyx_IterableCoroutine_init(module) == -1))
         return -1;
 #endif
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CoroutineAwaitType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CoroutineAwaitType_spec, NULL);
+#else
     __pyx_CoroutineAwaitType = __Pyx_FetchCommonType(&__pyx_CoroutineAwaitType_type);
+#endif
     if (unlikely(!__pyx_CoroutineAwaitType))
         return -1;
     return 0;
 }
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* GetAwaitIter */
 static CYTHON_INLINE PyObject *__Pyx_Coroutine_GetAwaitableIter(PyObject *o) {
 #ifdef __Pyx_Coroutine_USED
     if (__Pyx_Coroutine_Check(o)) {
         return __Pyx_NewRef(o);
     }
 #endif
     return __Pyx__Coroutine_GetAwaitableIter(o);
 }
 static void __Pyx_Coroutine_AwaitableIterError(PyObject *source) {
 #if PY_VERSION_HEX >= 0x030600B3 || defined(_PyErr_FormatFromCause)
-    _PyErr_FormatFromCause(
-        PyExc_TypeError,
-        "'async for' received an invalid object "
-        "from __anext__: %.100s",
-        Py_TYPE(source)->tp_name);
+    __Pyx_TypeName source_type_name = __Pyx_PyType_GetName(Py_TYPE(source));
+    _PyErr_FormatFromCause(PyExc_TypeError,
+        "'async for' received an invalid object from __anext__: " __Pyx_FMT_TYPENAME, source_type_name);
+    __Pyx_DECREF_TypeName(source_type_name);
 #elif PY_MAJOR_VERSION >= 3
     PyObject *exc, *val, *val2, *tb;
+    __Pyx_TypeName source_type_name = __Pyx_PyType_GetName(Py_TYPE(source));
     assert(PyErr_Occurred());
     PyErr_Fetch(&exc, &val, &tb);
     PyErr_NormalizeException(&exc, &val, &tb);
     if (tb != NULL) {
         PyException_SetTraceback(val, tb);
         Py_DECREF(tb);
     }
     Py_DECREF(exc);
     assert(!PyErr_Occurred());
-    PyErr_Format(
-        PyExc_TypeError,
-        "'async for' received an invalid object "
-        "from __anext__: %.100s",
-        Py_TYPE(source)->tp_name);
+    PyErr_Format(PyExc_TypeError,
+        "'async for' received an invalid object from __anext__: " __Pyx_FMT_TYPENAME, source_type_name);
+    __Pyx_DECREF_TypeName(source_type_name);
     PyErr_Fetch(&exc, &val2, &tb);
     PyErr_NormalizeException(&exc, &val2, &tb);
     Py_INCREF(val);
     PyException_SetCause(val2, val);
     PyException_SetContext(val2, val);
     PyErr_Restore(exc, val2, tb);
 #else
@@ -6503,17 +8253,18 @@
         Py_DECREF(method);
     }
     if (unlikely(!res)) {
         __Pyx_Coroutine_AwaitableIterError(obj);
         goto bad;
     }
     if (unlikely(!PyIter_Check(res))) {
+        __Pyx_TypeName res_type_name = __Pyx_PyType_GetName(Py_TYPE(res));
         PyErr_Format(PyExc_TypeError,
-                     "__await__() returned non-iterator of type '%.100s'",
-                     Py_TYPE(res)->tp_name);
+            "__await__() returned non-iterator of type '" __Pyx_FMT_TYPENAME "'", res_type_name);
+        __Pyx_DECREF_TypeName(res_type_name);
         Py_CLEAR(res);
     } else {
         int is_coroutine = 0;
         #ifdef __Pyx_Coroutine_USED
         is_coroutine |= __Pyx_Coroutine_Check(res);
         #endif
         #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
@@ -6525,36 +8276,35 @@
             PyErr_SetString(PyExc_TypeError,
                             "__await__() returned a coroutine");
             Py_CLEAR(res);
         }
     }
     return res;
 slot_error:
-    PyErr_Format(PyExc_TypeError,
-                 "object %.100s can't be used in 'await' expression",
-                 Py_TYPE(obj)->tp_name);
+    {
+        __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+        PyErr_Format(PyExc_TypeError,
+            "object " __Pyx_FMT_TYPENAME " can't be used in 'await' expression", obj_type_name);
+        __Pyx_DECREF_TypeName(obj_type_name);
+    }
 bad:
     return NULL;
 }
 
 /* CoroutineYieldFrom */
 static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
     PyObject *retval;
     PyObject *source_gen = __Pyx__Coroutine_GetAwaitableIter(source);
     if (unlikely(!source_gen)) {
         return NULL;
     }
     if (__Pyx_Coroutine_Check(source_gen)) {
         retval = __Pyx_Generator_Next(source_gen);
     } else {
-#if CYTHON_USE_TYPE_SLOTS
-        retval = Py_TYPE(source_gen)->tp_iternext(source_gen);
-#else
-        retval = PyIter_Next(source_gen);
-#endif
+        retval = __Pyx_PyObject_GetIterNextFunc(source_gen)(source_gen);
     }
     if (retval) {
         gen->yieldfrom = source_gen;
         return retval;
     }
     Py_DECREF(source_gen);
     return NULL;
@@ -6579,66 +8329,259 @@
     if (retval) {
         Py_INCREF(source);
         gen->yieldfrom = source;
     }
     return retval;
 }
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
 /* unicode_iter */
 static CYTHON_INLINE int __Pyx_init_unicode_iteration(
     PyObject* ustring, Py_ssize_t *length, void** data, int *kind) {
-#if CYTHON_PEP393_ENABLED
+#if CYTHON_COMPILING_IN_LIMITED_API
+    *kind   = 0;
+    *length = PyUnicode_GetLength(ustring);
+    *data   = (void*)ustring;
+#elif CYTHON_PEP393_ENABLED
     if (unlikely(__Pyx_PyUnicode_READY(ustring) < 0)) return -1;
     *kind   = PyUnicode_KIND(ustring);
     *length = PyUnicode_GET_LENGTH(ustring);
     *data   = PyUnicode_DATA(ustring);
 #else
     *kind   = 0;
     *length = PyUnicode_GET_SIZE(ustring);
     *data   = (void*)PyUnicode_AS_UNICODE(ustring);
 #endif
     return 0;
 }
 
+/* UnicodeConcatInPlace */
+# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
+static int
+__Pyx_unicode_modifiable(PyObject *unicode)
+{
+    if (Py_REFCNT(unicode) != 1)
+        return 0;
+    if (!PyUnicode_CheckExact(unicode))
+        return 0;
+    if (PyUnicode_CHECK_INTERNED(unicode))
+        return 0;
+    return 1;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
+        #if CYTHON_REFNANNY
+        , void* __pyx_refnanny
+        #endif
+    ) {
+    PyObject *left = *p_left;
+    Py_ssize_t left_len, right_len, new_len;
+    if (unlikely(__Pyx_PyUnicode_READY(left) == -1))
+        return NULL;
+    if (unlikely(__Pyx_PyUnicode_READY(right) == -1))
+        return NULL;
+    left_len = PyUnicode_GET_LENGTH(left);
+    if (left_len == 0) {
+        Py_INCREF(right);
+        return right;
+    }
+    right_len = PyUnicode_GET_LENGTH(right);
+    if (right_len == 0) {
+        Py_INCREF(left);
+        return left;
+    }
+    if (unlikely(left_len > PY_SSIZE_T_MAX - right_len)) {
+        PyErr_SetString(PyExc_OverflowError,
+                        "strings are too large to concat");
+        return NULL;
+    }
+    new_len = left_len + right_len;
+    if (__Pyx_unicode_modifiable(left)
+            && PyUnicode_CheckExact(right)
+            && PyUnicode_KIND(right) <= PyUnicode_KIND(left)
+            && !(PyUnicode_IS_ASCII(left) && !PyUnicode_IS_ASCII(right))) {
+        __Pyx_GIVEREF(*p_left);
+        if (unlikely(PyUnicode_Resize(p_left, new_len) != 0)) {
+            __Pyx_GOTREF(*p_left);
+            return NULL;
+        }
+        __Pyx_INCREF(*p_left);
+        _PyUnicode_FastCopyCharacters(*p_left, left_len, right, 0, right_len);
+        return *p_left;
+    } else {
+        return __Pyx_PyUnicode_Concat(left, right);
+    }
+  }
+#endif
+
+/* pybytes_as_double */
+static double __Pyx_SlowPyString_AsDouble(PyObject *obj) {
+    PyObject *float_value;
+#if PY_MAJOR_VERSION >= 3
+    float_value = PyFloat_FromString(obj);
+#else
+    float_value = PyFloat_FromString(obj, 0);
+#endif
+    if (likely(float_value)) {
+        double value = PyFloat_AS_DOUBLE(float_value);
+        Py_DECREF(float_value);
+        return value;
+    }
+    return (double)-1;
+}
+static const char* __Pyx__PyBytes_AsDouble_Copy(const char* start, char* buffer, Py_ssize_t length) {
+    int last_was_punctuation = 1;
+    Py_ssize_t i;
+    for (i=0; i < length; i++) {
+        char chr = start[i];
+        int is_punctuation = (chr == '_') | (chr == '.') | (chr == 'e') | (chr == 'E');
+        *buffer = chr;
+        buffer += (chr != '_');
+        if (unlikely(last_was_punctuation & is_punctuation)) goto parse_failure;
+        last_was_punctuation = is_punctuation;
+    }
+    if (unlikely(last_was_punctuation)) goto parse_failure;
+    *buffer = '\0';
+    return buffer;
+parse_failure:
+    return NULL;
+}
+static double __Pyx__PyBytes_AsDouble_inf_nan(const char* start, Py_ssize_t length) {
+    int matches = 1;
+    char sign = start[0];
+    int is_signed = (sign == '+') | (sign == '-');
+    start += is_signed;
+    length -= is_signed;
+    switch (start[0]) {
+        #ifdef Py_NAN
+        case 'n':
+        case 'N':
+            if (unlikely(length != 3)) goto parse_failure;
+            matches &= (start[1] == 'a' || start[1] == 'A');
+            matches &= (start[2] == 'n' || start[2] == 'N');
+            if (unlikely(!matches)) goto parse_failure;
+            return (sign == '-') ? -Py_NAN : Py_NAN;
+        #endif
+        case 'i':
+        case 'I':
+            if (unlikely(length < 3)) goto parse_failure;
+            matches &= (start[1] == 'n' || start[1] == 'N');
+            matches &= (start[2] == 'f' || start[2] == 'F');
+            if (likely(length == 3 && matches))
+                return (sign == '-') ? -Py_HUGE_VAL : Py_HUGE_VAL;
+            if (unlikely(length != 8)) goto parse_failure;
+            matches &= (start[3] == 'i' || start[3] == 'I');
+            matches &= (start[4] == 'n' || start[4] == 'N');
+            matches &= (start[5] == 'i' || start[5] == 'I');
+            matches &= (start[6] == 't' || start[6] == 'T');
+            matches &= (start[7] == 'y' || start[7] == 'Y');
+            if (unlikely(!matches)) goto parse_failure;
+            return (sign == '-') ? -Py_HUGE_VAL : Py_HUGE_VAL;
+        case '.': case '0': case '1': case '2': case '3': case '4': case '5': case '6': case '7': case '8': case '9':
+            break;
+        default:
+            goto parse_failure;
+    }
+    return 0.0;
+parse_failure:
+    return -1.0;
+}
+static CYTHON_INLINE int __Pyx__PyBytes_AsDouble_IsSpace(char ch) {
+    return (ch == 0x20) | !((ch < 0x9) | (ch > 0xd));
+}
+CYTHON_UNUSED static double __Pyx__PyBytes_AsDouble(PyObject *obj, const char* start, Py_ssize_t length) {
+    double value;
+    Py_ssize_t i, digits;
+    const char *last = start + length;
+    char *end;
+    while (__Pyx__PyBytes_AsDouble_IsSpace(*start))
+        start++;
+    while (start < last - 1 && __Pyx__PyBytes_AsDouble_IsSpace(last[-1]))
+        last--;
+    length = last - start;
+    if (unlikely(length <= 0)) goto fallback;
+    value = __Pyx__PyBytes_AsDouble_inf_nan(start, length);
+    if (unlikely(value == -1.0)) goto fallback;
+    if (value != 0.0) return value;
+    digits = 0;
+    for (i=0; i < length; digits += start[i++] != '_');
+    if (likely(digits == length)) {
+        value = PyOS_string_to_double(start, &end, NULL);
+    } else if (digits < 40) {
+        char number[40];
+        last = __Pyx__PyBytes_AsDouble_Copy(start, number, length);
+        if (unlikely(!last)) goto fallback;
+        value = PyOS_string_to_double(number, &end, NULL);
+    } else {
+        char *number = (char*) PyMem_Malloc((digits + 1) * sizeof(char));
+        if (unlikely(!number)) goto fallback;
+        last = __Pyx__PyBytes_AsDouble_Copy(start, number, length);
+        if (unlikely(!last)) {
+            PyMem_Free(number);
+            goto fallback;
+        }
+        value = PyOS_string_to_double(number, &end, NULL);
+        PyMem_Free(number);
+    }
+    if (likely(end == last) || (value == (double)-1 && PyErr_Occurred())) {
+        return value;
+    }
+fallback:
+    return __Pyx_SlowPyString_AsDouble(obj);
+}
+
 /* JoinPyUnicode */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      CYTHON_UNUSED Py_UCS4 max_char) {
+                                      Py_UCS4 max_char) {
 #if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     PyObject *result_uval;
-    int result_ukind;
+    int result_ukind, kind_shift;
     Py_ssize_t i, char_pos;
     void *result_udata;
+    CYTHON_MAYBE_UNUSED_VAR(max_char);
 #if CYTHON_PEP393_ENABLED
     result_uval = PyUnicode_New(result_ulength, max_char);
     if (unlikely(!result_uval)) return NULL;
     result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    kind_shift = (result_ukind == PyUnicode_4BYTE_KIND) ? 2 : result_ukind - 1;
     result_udata = PyUnicode_DATA(result_uval);
 #else
     result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
     if (unlikely(!result_uval)) return NULL;
     result_ukind = sizeof(Py_UNICODE);
+    kind_shift = (result_ukind == 4) ? 2 : result_ukind - 1;
     result_udata = PyUnicode_AS_UNICODE(result_uval);
 #endif
+    assert(kind_shift == 2 || kind_shift == 1 || kind_shift == 0);
     char_pos = 0;
     for (i=0; i < value_count; i++) {
         int ukind;
         Py_ssize_t ulength;
         void *udata;
         PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
         if (unlikely(__Pyx_PyUnicode_READY(uval)))
             goto bad;
         ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
         if (unlikely(!ulength))
             continue;
-        if (unlikely(char_pos + ulength < 0))
+        if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
-            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
+            memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
             #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
@@ -6651,22 +8594,26 @@
     return result_uval;
 overflow:
     PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
 bad:
     Py_DECREF(result_uval);
     return NULL;
 #else
-    result_ulength++;
-    value_count++;
+    CYTHON_UNUSED_VAR(max_char);
+    CYTHON_UNUSED_VAR(result_ulength);
+    CYTHON_UNUSED_VAR(value_count);
     return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
 }
 
 /* StopAsyncIteration */
 #if PY_VERSION_HEX < 0x030500B1
+#if CYTHON_USE_TYPE_SPECS
+#error Using async coroutines with type specs requires Python 3.5 or later.
+#else
 static PyTypeObject __Pyx__PyExc_StopAsyncIteration_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "StopAsyncIteration",
     sizeof(PyBaseExceptionObject),
     0,
     0,
     0,
@@ -6715,15 +8662,17 @@
     0,
 #endif
 #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
     0,
 #endif
 };
 #endif
-static int __pyx_StopAsyncIteration_init(void) {
+#endif
+static int __pyx_StopAsyncIteration_init(PyObject *module) {
+    CYTHON_UNUSED_VAR(module);
 #if PY_VERSION_HEX >= 0x030500B1
     __Pyx_PyExc_StopAsyncIteration = PyExc_StopAsyncIteration;
 #else
     PyObject *builtins = PyEval_GetBuiltins();
     if (likely(builtins)) {
         PyObject *exc = PyMapping_GetItemString(builtins, (char*) "StopAsyncIteration");
         if (exc) {
@@ -6735,107 +8684,1432 @@
     __Pyx__PyExc_StopAsyncIteration_type.tp_traverse = ((PyTypeObject*)PyExc_BaseException)->tp_traverse;
     __Pyx__PyExc_StopAsyncIteration_type.tp_clear = ((PyTypeObject*)PyExc_BaseException)->tp_clear;
     __Pyx__PyExc_StopAsyncIteration_type.tp_dictoffset = ((PyTypeObject*)PyExc_BaseException)->tp_dictoffset;
     __Pyx__PyExc_StopAsyncIteration_type.tp_base = (PyTypeObject*)PyExc_Exception;
     __Pyx_PyExc_StopAsyncIteration = (PyObject*) __Pyx_FetchCommonType(&__Pyx__PyExc_StopAsyncIteration_type);
     if (unlikely(!__Pyx_PyExc_StopAsyncIteration))
         return -1;
-    if (builtins && unlikely(PyMapping_SetItemString(builtins, (char*) "StopAsyncIteration", __Pyx_PyExc_StopAsyncIteration) < 0))
+    if (likely(builtins) && unlikely(PyMapping_SetItemString(builtins, (char*) "StopAsyncIteration", __Pyx_PyExc_StopAsyncIteration) < 0))
         return -1;
 #endif
     return 0;
 }
 
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* pep479 */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen) {
+    PyObject *exc, *val, *tb, *cur_exc;
+    __Pyx_PyThreadState_declare
+    #ifdef __Pyx_StopAsyncIteration_USED
+    int is_async_stopiteration = 0;
+    #endif
+    CYTHON_MAYBE_UNUSED_VAR(in_async_gen);
+    cur_exc = PyErr_Occurred();
+    if (likely(!__Pyx_PyErr_GivenExceptionMatches(cur_exc, PyExc_StopIteration))) {
+        #ifdef __Pyx_StopAsyncIteration_USED
+        if (in_async_gen && unlikely(__Pyx_PyErr_GivenExceptionMatches(cur_exc, __Pyx_PyExc_StopAsyncIteration))) {
+            is_async_stopiteration = 1;
+        } else
+        #endif
+            return;
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_GetException(&exc, &val, &tb);
+    Py_XDECREF(exc);
+    Py_XDECREF(val);
+    Py_XDECREF(tb);
+    PyErr_SetString(PyExc_RuntimeError,
+        #ifdef __Pyx_StopAsyncIteration_USED
+        is_async_stopiteration ? "async generator raised StopAsyncIteration" :
+        in_async_gen ? "async generator raised StopIteration" :
+        #endif
+        "generator raised StopIteration");
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    for (i = 1; i < n; i++)
+    {
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+    }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__5;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* PyVectorcallFastCallDict */
+#if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -6849,14 +10123,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -6927,25 +10202,36 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -6972,14 +10258,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -7034,14 +10321,15 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 /* UnicodeAsUCS4 */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
    Py_ssize_t length;
    #if CYTHON_PEP393_ENABLED
    length = PyUnicode_GET_LENGTH(x);
    if (likely(length == 1)) {
@@ -7125,14 +10413,29 @@
    ival = __Pyx_PyInt_As_long(x);
    if (unlikely(!__Pyx_is_valid_index(ival, 1114111 + 1))) {
        return __Pyx__PyObject_AsPy_UCS4_raise_error(ival);
    }
    return (Py_UCS4)ival;
 }
 
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__7));
+    }
+    return name;
+}
+#endif
+
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -7160,55 +10463,55 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (long) 0;
                 case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
                             return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
                             return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -7220,96 +10523,96 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (long) 0;
                 case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
                 case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
                             return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
                             return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
 #else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
@@ -7356,55 +10659,55 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (int) 0;
                 case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
                             return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
                             return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -7416,96 +10719,96 @@
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            const digit* digits = __Pyx_PyLong_Digits(x);
             switch (Py_SIZE(x)) {
                 case  0: return (int) 0;
                 case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
                 case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
                             return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
                             __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
                             return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
 #else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
@@ -7543,15 +10846,15 @@
     return (int) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -7564,14 +10867,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -7588,19 +10907,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -7677,15 +10996,15 @@
     return 0;
 }
 #endif
 
 /* ReturnWithStopIteration */
 static void __Pyx__ReturnWithStopIteration(PyObject* value) {
     PyObject *exc, *args;
-#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_PYSTON
+#if CYTHON_COMPILING_IN_CPYTHON
     __Pyx_PyThreadState_declare
     if ((PY_VERSION_HEX >= 0x03030000 && PY_VERSION_HEX < 0x030500B1)
             || unlikely(PyTuple_Check(value) || PyExceptionInstance_Check(value))) {
         args = PyTuple_New(1);
         if (unlikely(!args)) return;
         Py_INCREF(value);
         PyTuple_SET_ITEM(args, 0, value);
@@ -7695,15 +11014,15 @@
     } else {
         Py_INCREF(value);
         exc = value;
     }
     #if CYTHON_FAST_THREAD_STATE
     __Pyx_PyThreadState_assign
     #if CYTHON_USE_EXC_INFO_STACK
-    if (!__pyx_tstate->exc_info->exc_type)
+    if (!__pyx_tstate->exc_info->exc_value)
     #else
     if (!__pyx_tstate->exc_type)
     #endif
     {
         Py_INCREF(PyExc_StopIteration);
         __Pyx_ErrRestore(PyExc_StopIteration, exc, NULL);
         return;
@@ -7731,14 +11050,16 @@
 return next yielded value or raise StopIteration.");
 PyDoc_STRVAR(__Pyx_async_gen_await_doc,
 "__await__() -> return a representation that can be passed into the 'await' expression.");
 static PyObject *__Pyx_async_gen_asend_new(__pyx_PyAsyncGenObject *, PyObject *);
 static PyObject *__Pyx_async_gen_athrow_new(__pyx_PyAsyncGenObject *, PyObject *);
 static const char *__Pyx_NON_INIT_CORO_MSG = "can't send non-None value to a just-started coroutine";
 static const char *__Pyx_ASYNC_GEN_IGNORED_EXIT_MSG = "async generator ignored GeneratorExit";
+static const char *__Pyx_ASYNC_GEN_CANNOT_REUSE_SEND_MSG = "cannot reuse already awaited __anext__()/asend()";
+static const char *__Pyx_ASYNC_GEN_CANNOT_REUSE_CLOSE_MSG = "cannot reuse already awaited aclose()/athrow()";
 typedef enum {
     __PYX_AWAITABLE_STATE_INIT,
     __PYX_AWAITABLE_STATE_ITER,
     __PYX_AWAITABLE_STATE_CLOSED,
 } __pyx_AwaitableState;
 typedef struct {
     PyObject_HEAD
@@ -7760,15 +11081,15 @@
 #define _PyAsyncGen_MAXFREELIST 80
 #endif
 static __pyx__PyAsyncGenWrappedValue *__Pyx_ag_value_freelist[_PyAsyncGen_MAXFREELIST];
 static int __Pyx_ag_value_freelist_free = 0;
 static __pyx_PyAsyncGenASend *__Pyx_ag_asend_freelist[_PyAsyncGen_MAXFREELIST];
 static int __Pyx_ag_asend_freelist_free = 0;
 #define __pyx__PyAsyncGenWrappedValue_CheckExact(o)\
-                    (Py_TYPE(o) == __pyx__PyAsyncGenWrappedValueType)
+                    __Pyx_IS_TYPE(o, __pyx__PyAsyncGenWrappedValueType)
 static int
 __Pyx_async_gen_traverse(__pyx_PyAsyncGenObject *gen, visitproc visit, void *arg)
 {
     Py_VISIT(gen->ag_finalizer);
     return __Pyx_Coroutine_traverse((__pyx_CoroutineObject*)gen, visit, arg);
 }
 static PyObject *
@@ -7817,62 +11138,69 @@
     return 0;
 }
 #endif
 static PyObject *
 __Pyx_async_gen_anext(PyObject *g)
 {
     __pyx_PyAsyncGenObject *o = (__pyx_PyAsyncGenObject*) g;
-    if (__Pyx_async_gen_init_hooks(o)) {
+    if (unlikely(__Pyx_async_gen_init_hooks(o))) {
         return NULL;
     }
     return __Pyx_async_gen_asend_new(o, NULL);
 }
 static PyObject *
-__Pyx_async_gen_anext_method(PyObject *g, CYTHON_UNUSED PyObject *arg) {
+__Pyx_async_gen_anext_method(PyObject *g, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_async_gen_anext(g);
 }
 static PyObject *
 __Pyx_async_gen_asend(__pyx_PyAsyncGenObject *o, PyObject *arg)
 {
-    if (__Pyx_async_gen_init_hooks(o)) {
+    if (unlikely(__Pyx_async_gen_init_hooks(o))) {
         return NULL;
     }
     return __Pyx_async_gen_asend_new(o, arg);
 }
 static PyObject *
-__Pyx_async_gen_aclose(__pyx_PyAsyncGenObject *o, CYTHON_UNUSED PyObject *arg)
+__Pyx_async_gen_aclose(__pyx_PyAsyncGenObject *o, PyObject *arg)
 {
-    if (__Pyx_async_gen_init_hooks(o)) {
+    CYTHON_UNUSED_VAR(arg);
+    if (unlikely(__Pyx_async_gen_init_hooks(o))) {
         return NULL;
     }
     return __Pyx_async_gen_athrow_new(o, NULL);
 }
 static PyObject *
 __Pyx_async_gen_athrow(__pyx_PyAsyncGenObject *o, PyObject *args)
 {
-    if (__Pyx_async_gen_init_hooks(o)) {
+    if (unlikely(__Pyx_async_gen_init_hooks(o))) {
         return NULL;
     }
     return __Pyx_async_gen_athrow_new(o, args);
 }
 static PyObject *
-__Pyx_async_gen_self_method(PyObject *g, CYTHON_UNUSED PyObject *arg) {
+__Pyx_async_gen_self_method(PyObject *g, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_NewRef(g);
 }
 static PyGetSetDef __Pyx_async_gen_getsetlist[] = {
     {(char*) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the async generator"), 0},
     {(char*) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the async generator"), 0},
     {0, 0, 0, 0, 0}
 };
 static PyMemberDef __Pyx_async_gen_memberlist[] = {
-    {(char*) "ag_running", T_BOOL,   offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
+    {(char*) "ag_running", T_BOOL,   offsetof(__pyx_PyAsyncGenObject, ag_running_async), READONLY, NULL},
     {(char*) "ag_await", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
      (char*) PyDoc_STR("object being awaited on, or None")},
+    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 PyDoc_STRVAR(__Pyx_async_aclose_doc,
 "aclose() -> raise GeneratorExit inside generator.");
 PyDoc_STRVAR(__Pyx_async_asend_doc,
 "asend(v) -> send 'v' in generator.");
 PyDoc_STRVAR(__Pyx_async_athrow_doc,
@@ -7885,14 +11213,37 @@
     {"asend", (PyCFunction)__Pyx_async_gen_asend, METH_O, __Pyx_async_asend_doc},
     {"athrow",(PyCFunction)__Pyx_async_gen_athrow, METH_VARARGS, __Pyx_async_athrow_doc},
     {"aclose", (PyCFunction)__Pyx_async_gen_aclose, METH_NOARGS, __Pyx_async_aclose_doc},
     {"__aiter__", (PyCFunction)__Pyx_async_gen_self_method, METH_NOARGS, __Pyx_async_aiter_doc},
     {"__anext__", (PyCFunction)__Pyx_async_gen_anext_method, METH_NOARGS, __Pyx_async_anext_doc},
     {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_AsyncGenType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
+    {Py_am_aiter, (void *)PyObject_SelfIter},
+    {Py_am_anext, (void *)__Pyx_async_gen_anext},
+    {Py_tp_repr, (void *)__Pyx_async_gen_repr},
+    {Py_tp_traverse, (void *)__Pyx_async_gen_traverse},
+    {Py_tp_methods, (void *)__Pyx_async_gen_methods},
+    {Py_tp_members, (void *)__Pyx_async_gen_memberlist},
+    {Py_tp_getset, (void *)__Pyx_async_gen_getsetlist},
+#if CYTHON_USE_TP_FINALIZE
+    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
+#endif
+    {0, 0},
+};
+static PyType_Spec __pyx_AsyncGenType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "async_generator",
+    sizeof(__pyx_PyAsyncGenObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    __pyx_AsyncGenType_slots
+};
+#else
 #if CYTHON_USE_ASYNC_SLOTS
 static __Pyx_PyAsyncMethodsStruct __Pyx_async_gen_as_async = {
     0,
     PyObject_SelfIter,
     (unaryfunc)__Pyx_async_gen_anext,
 #if PY_VERSION_HEX >= 0x030A00A3
     0,
@@ -7967,33 +11318,37 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
+#endif
 static int
 __Pyx_PyAsyncGen_ClearFreeLists(void)
 {
     int ret = __Pyx_ag_value_freelist_free + __Pyx_ag_asend_freelist_free;
     while (__Pyx_ag_value_freelist_free) {
         __pyx__PyAsyncGenWrappedValue *o;
         o = __Pyx_ag_value_freelist[--__Pyx_ag_value_freelist_free];
         assert(__pyx__PyAsyncGenWrappedValue_CheckExact(o));
-        PyObject_GC_Del(o);
+        __Pyx_PyHeapTypeObject_GC_Del(o);
     }
     while (__Pyx_ag_asend_freelist_free) {
         __pyx_PyAsyncGenASend *o;
         o = __Pyx_ag_asend_freelist[--__Pyx_ag_asend_freelist_free];
-        assert(Py_TYPE(o) == __pyx__PyAsyncGenASendType);
-        PyObject_GC_Del(o);
+        assert(__Pyx_IS_TYPE(o, __pyx__PyAsyncGenASendType));
+        __Pyx_PyHeapTypeObject_GC_Del(o);
     }
     return ret;
 }
 static void
 __Pyx_PyAsyncGen_Fini(void)
 {
     __Pyx_PyAsyncGen_ClearFreeLists();
@@ -8005,34 +11360,36 @@
         PyObject *exc_type = PyErr_Occurred();
         if (!exc_type) {
             PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
             gen->ag_closed = 1;
         } else if (__Pyx_PyErr_GivenExceptionMatches2(exc_type, __Pyx_PyExc_StopAsyncIteration, PyExc_GeneratorExit)) {
             gen->ag_closed = 1;
         }
+        gen->ag_running_async = 0;
         return NULL;
     }
     if (__pyx__PyAsyncGenWrappedValue_CheckExact(result)) {
         __Pyx_ReturnWithStopIteration(((__pyx__PyAsyncGenWrappedValue*)result)->agw_val);
         Py_DECREF(result);
+        gen->ag_running_async = 0;
         return NULL;
     }
     return result;
 }
 static void
 __Pyx_async_gen_asend_dealloc(__pyx_PyAsyncGenASend *o)
 {
     PyObject_GC_UnTrack((PyObject *)o);
     Py_CLEAR(o->ags_gen);
     Py_CLEAR(o->ags_sendval);
-    if (__Pyx_ag_asend_freelist_free < _PyAsyncGen_MAXFREELIST) {
+    if (likely(__Pyx_ag_asend_freelist_free < _PyAsyncGen_MAXFREELIST)) {
         assert(__pyx_PyAsyncGenASend_CheckExact(o));
         __Pyx_ag_asend_freelist[__Pyx_ag_asend_freelist_free++] = o;
     } else {
-        PyObject_GC_Del(o);
+        __Pyx_PyHeapTypeObject_GC_Del(o);
     }
 }
 static int
 __Pyx_async_gen_asend_traverse(__pyx_PyAsyncGenASend *o, visitproc visit, void *arg)
 {
     Py_VISIT(o->ags_gen);
     Py_VISIT(o->ags_sendval);
@@ -8040,23 +11397,30 @@
 }
 static PyObject *
 __Pyx_async_gen_asend_send(PyObject *g, PyObject *arg)
 {
     __pyx_PyAsyncGenASend *o = (__pyx_PyAsyncGenASend*) g;
     PyObject *result;
     if (unlikely(o->ags_state == __PYX_AWAITABLE_STATE_CLOSED)) {
-        PyErr_SetNone(PyExc_StopIteration);
+        PyErr_SetString(PyExc_RuntimeError, __Pyx_ASYNC_GEN_CANNOT_REUSE_SEND_MSG);
         return NULL;
     }
     if (o->ags_state == __PYX_AWAITABLE_STATE_INIT) {
+        if (unlikely(o->ags_gen->ag_running_async)) {
+            PyErr_SetString(
+                PyExc_RuntimeError,
+                "anext(): asynchronous generator is already running");
+            return NULL;
+        }
         if (arg == NULL || arg == Py_None) {
             arg = o->ags_sendval ? o->ags_sendval : Py_None;
         }
         o->ags_state = __PYX_AWAITABLE_STATE_ITER;
     }
+    o->ags_gen->ag_running_async = 1;
     result = __Pyx_Coroutine_Send((PyObject*)o->ags_gen, arg);
     result = __Pyx_async_gen_unwrap_value(o->ags_gen, result);
     if (result == NULL) {
         o->ags_state = __PYX_AWAITABLE_STATE_CLOSED;
     }
     return result;
 }
@@ -8066,38 +11430,57 @@
     return __Pyx_async_gen_asend_send(o, Py_None);
 }
 static PyObject *
 __Pyx_async_gen_asend_throw(__pyx_PyAsyncGenASend *o, PyObject *args)
 {
     PyObject *result;
     if (unlikely(o->ags_state == __PYX_AWAITABLE_STATE_CLOSED)) {
-        PyErr_SetNone(PyExc_StopIteration);
+        PyErr_SetString(PyExc_RuntimeError, __Pyx_ASYNC_GEN_CANNOT_REUSE_SEND_MSG);
         return NULL;
     }
     result = __Pyx_Coroutine_Throw((PyObject*)o->ags_gen, args);
     result = __Pyx_async_gen_unwrap_value(o->ags_gen, result);
     if (result == NULL) {
         o->ags_state = __PYX_AWAITABLE_STATE_CLOSED;
     }
     return result;
 }
 static PyObject *
-__Pyx_async_gen_asend_close(PyObject *g, CYTHON_UNUSED PyObject *args)
+__Pyx_async_gen_asend_close(PyObject *g, PyObject *args)
 {
     __pyx_PyAsyncGenASend *o = (__pyx_PyAsyncGenASend*) g;
+    CYTHON_UNUSED_VAR(args);
     o->ags_state = __PYX_AWAITABLE_STATE_CLOSED;
     Py_RETURN_NONE;
 }
 static PyMethodDef __Pyx_async_gen_asend_methods[] = {
     {"send", (PyCFunction)__Pyx_async_gen_asend_send, METH_O, __Pyx_async_gen_send_doc},
     {"throw", (PyCFunction)__Pyx_async_gen_asend_throw, METH_VARARGS, __Pyx_async_gen_throw_doc},
     {"close", (PyCFunction)__Pyx_async_gen_asend_close, METH_NOARGS, __Pyx_async_gen_close_doc},
     {"__await__", (PyCFunction)__Pyx_async_gen_self_method, METH_NOARGS, __Pyx_async_gen_await_doc},
     {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx__PyAsyncGenASendType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_async_gen_asend_dealloc},
+    {Py_am_await, (void *)PyObject_SelfIter},
+    {Py_tp_traverse, (void *)__Pyx_async_gen_asend_traverse},
+    {Py_tp_methods, (void *)__Pyx_async_gen_asend_methods},
+    {Py_tp_iter, (void *)PyObject_SelfIter},
+    {Py_tp_iternext, (void *)__Pyx_async_gen_asend_iternext},
+    {0, 0},
+};
+static PyType_Spec __pyx__PyAsyncGenASendType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "async_generator_asend",
+    sizeof(__pyx_PyAsyncGenASend),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
+    __pyx__PyAsyncGenASendType_slots
+};
+#else
 #if CYTHON_USE_ASYNC_SLOTS
 static __Pyx_PyAsyncMethodsStruct __Pyx_async_gen_asend_as_async = {
     PyObject_SelfIter,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030A00A3
     0,
@@ -8165,29 +11548,33 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
+#endif
 static PyObject *
 __Pyx_async_gen_asend_new(__pyx_PyAsyncGenObject *gen, PyObject *sendval)
 {
     __pyx_PyAsyncGenASend *o;
-    if (__Pyx_ag_asend_freelist_free) {
+    if (likely(__Pyx_ag_asend_freelist_free)) {
         __Pyx_ag_asend_freelist_free--;
         o = __Pyx_ag_asend_freelist[__Pyx_ag_asend_freelist_free];
         _Py_NewReference((PyObject *)o);
     } else {
         o = PyObject_GC_New(__pyx_PyAsyncGenASend, __pyx__PyAsyncGenASendType);
-        if (o == NULL) {
+        if (unlikely(o == NULL)) {
             return NULL;
         }
     }
     Py_INCREF(gen);
     o->ags_gen = gen;
     Py_XINCREF(sendval);
     o->ags_sendval = sendval;
@@ -8196,28 +11583,42 @@
     return (PyObject*)o;
 }
 static void
 __Pyx_async_gen_wrapped_val_dealloc(__pyx__PyAsyncGenWrappedValue *o)
 {
     PyObject_GC_UnTrack((PyObject *)o);
     Py_CLEAR(o->agw_val);
-    if (__Pyx_ag_value_freelist_free < _PyAsyncGen_MAXFREELIST) {
+    if (likely(__Pyx_ag_value_freelist_free < _PyAsyncGen_MAXFREELIST)) {
         assert(__pyx__PyAsyncGenWrappedValue_CheckExact(o));
         __Pyx_ag_value_freelist[__Pyx_ag_value_freelist_free++] = o;
     } else {
-        PyObject_GC_Del(o);
+        __Pyx_PyHeapTypeObject_GC_Del(o);
     }
 }
 static int
 __Pyx_async_gen_wrapped_val_traverse(__pyx__PyAsyncGenWrappedValue *o,
                                      visitproc visit, void *arg)
 {
     Py_VISIT(o->agw_val);
     return 0;
 }
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx__PyAsyncGenWrappedValueType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_async_gen_wrapped_val_dealloc},
+    {Py_tp_traverse, (void *)__Pyx_async_gen_wrapped_val_traverse},
+    {0, 0},
+};
+static PyType_Spec __pyx__PyAsyncGenWrappedValueType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "async_generator_wrapped_value",
+    sizeof(__pyx__PyAsyncGenWrappedValue),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
+    __pyx__PyAsyncGenWrappedValueType_slots
+};
+#else
 static PyTypeObject __pyx__PyAsyncGenWrappedValueType_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "async_generator_wrapped_value",
     sizeof(__pyx__PyAsyncGenWrappedValue),
     0,
     (destructor)__Pyx_async_gen_wrapped_val_dealloc,
     0,
@@ -8267,24 +11668,28 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
+#endif
 static PyObject *
 __Pyx__PyAsyncGenValueWrapperNew(PyObject *val)
 {
     __pyx__PyAsyncGenWrappedValue *o;
     assert(val);
-    if (__Pyx_ag_value_freelist_free) {
+    if (likely(__Pyx_ag_value_freelist_free)) {
         __Pyx_ag_value_freelist_free--;
         o = __Pyx_ag_value_freelist[__Pyx_ag_value_freelist_free];
         assert(__pyx__PyAsyncGenWrappedValue_CheckExact(o));
         _Py_NewReference((PyObject*)o);
     } else {
         o = PyObject_GC_New(__pyx__PyAsyncGenWrappedValue, __pyx__PyAsyncGenWrappedValueType);
         if (unlikely(!o)) {
@@ -8298,149 +11703,189 @@
 }
 static void
 __Pyx_async_gen_athrow_dealloc(__pyx_PyAsyncGenAThrow *o)
 {
     PyObject_GC_UnTrack((PyObject *)o);
     Py_CLEAR(o->agt_gen);
     Py_CLEAR(o->agt_args);
-    PyObject_GC_Del(o);
+    __Pyx_PyHeapTypeObject_GC_Del(o);
 }
 static int
 __Pyx_async_gen_athrow_traverse(__pyx_PyAsyncGenAThrow *o, visitproc visit, void *arg)
 {
     Py_VISIT(o->agt_gen);
     Py_VISIT(o->agt_args);
     return 0;
 }
 static PyObject *
 __Pyx_async_gen_athrow_send(__pyx_PyAsyncGenAThrow *o, PyObject *arg)
 {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*)o->agt_gen;
-    PyObject *retval;
-    if (o->agt_state == __PYX_AWAITABLE_STATE_CLOSED) {
+    PyObject *retval, *exc_type;
+    if (unlikely(o->agt_state == __PYX_AWAITABLE_STATE_CLOSED)) {
+        PyErr_SetString(PyExc_RuntimeError, __Pyx_ASYNC_GEN_CANNOT_REUSE_CLOSE_MSG);
+        return NULL;
+    }
+    if (unlikely(gen->resume_label == -1)) {
+        o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
         PyErr_SetNone(PyExc_StopIteration);
         return NULL;
     }
     if (o->agt_state == __PYX_AWAITABLE_STATE_INIT) {
-        if (o->agt_gen->ag_closed) {
-            PyErr_SetNone(PyExc_StopIteration);
+        if (unlikely(o->agt_gen->ag_running_async)) {
+            o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
+            if (o->agt_args == NULL) {
+                PyErr_SetString(
+                    PyExc_RuntimeError,
+                    "aclose(): asynchronous generator is already running");
+            } else {
+                PyErr_SetString(
+                    PyExc_RuntimeError,
+                    "athrow(): asynchronous generator is already running");
+            }
+            return NULL;
+        }
+        if (unlikely(o->agt_gen->ag_closed)) {
+            o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
+            PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
             return NULL;
         }
-        if (arg != Py_None) {
+        if (unlikely(arg != Py_None)) {
             PyErr_SetString(PyExc_RuntimeError, __Pyx_NON_INIT_CORO_MSG);
             return NULL;
         }
         o->agt_state = __PYX_AWAITABLE_STATE_ITER;
+        o->agt_gen->ag_running_async = 1;
         if (o->agt_args == NULL) {
             o->agt_gen->ag_closed = 1;
             retval = __Pyx__Coroutine_Throw((PyObject*)gen,
-                                /* Do not close generator when
-                                   PyExc_GeneratorExit is passed */
-                                PyExc_GeneratorExit, NULL, NULL, NULL, 0);
+                PyExc_GeneratorExit, NULL, NULL, NULL, 0);
             if (retval && __pyx__PyAsyncGenWrappedValue_CheckExact(retval)) {
                 Py_DECREF(retval);
                 goto yield_close;
             }
         } else {
             PyObject *typ;
             PyObject *tb = NULL;
             PyObject *val = NULL;
-            if (!PyArg_UnpackTuple(o->agt_args, "athrow", 1, 3,
-                                   &typ, &val, &tb)) {
+            if (unlikely(!PyArg_UnpackTuple(o->agt_args, "athrow", 1, 3, &typ, &val, &tb))) {
                 return NULL;
             }
             retval = __Pyx__Coroutine_Throw((PyObject*)gen,
-                                typ, val, tb, o->agt_args, 0);
+                typ, val, tb, o->agt_args, 0);
             retval = __Pyx_async_gen_unwrap_value(o->agt_gen, retval);
         }
         if (retval == NULL) {
             goto check_error;
         }
         return retval;
     }
     assert (o->agt_state == __PYX_AWAITABLE_STATE_ITER);
     retval = __Pyx_Coroutine_Send((PyObject *)gen, arg);
     if (o->agt_args) {
         return __Pyx_async_gen_unwrap_value(o->agt_gen, retval);
     } else {
         if (retval) {
-            if (__pyx__PyAsyncGenWrappedValue_CheckExact(retval)) {
+            if (unlikely(__pyx__PyAsyncGenWrappedValue_CheckExact(retval))) {
                 Py_DECREF(retval);
                 goto yield_close;
             }
             else {
                 return retval;
             }
         }
         else {
             goto check_error;
         }
     }
 yield_close:
+    o->agt_gen->ag_running_async = 0;
+    o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
     PyErr_SetString(
         PyExc_RuntimeError, __Pyx_ASYNC_GEN_IGNORED_EXIT_MSG);
     return NULL;
 check_error:
-    if (PyErr_ExceptionMatches(__Pyx_PyExc_StopAsyncIteration)) {
-        o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
+    o->agt_gen->ag_running_async = 0;
+    o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
+    exc_type = PyErr_Occurred();
+    if (__Pyx_PyErr_GivenExceptionMatches2(exc_type, __Pyx_PyExc_StopAsyncIteration, PyExc_GeneratorExit)) {
         if (o->agt_args == NULL) {
             PyErr_Clear();
             PyErr_SetNone(PyExc_StopIteration);
         }
     }
-    else if (PyErr_ExceptionMatches(PyExc_GeneratorExit)) {
-        o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
-        PyErr_Clear();
-        PyErr_SetNone(PyExc_StopIteration);
-    }
     return NULL;
 }
 static PyObject *
 __Pyx_async_gen_athrow_throw(__pyx_PyAsyncGenAThrow *o, PyObject *args)
 {
     PyObject *retval;
-    if (o->agt_state == __PYX_AWAITABLE_STATE_INIT) {
-        PyErr_SetString(PyExc_RuntimeError, __Pyx_NON_INIT_CORO_MSG);
-        return NULL;
-    }
-    if (o->agt_state == __PYX_AWAITABLE_STATE_CLOSED) {
-        PyErr_SetNone(PyExc_StopIteration);
+    if (unlikely(o->agt_state == __PYX_AWAITABLE_STATE_CLOSED)) {
+        PyErr_SetString(PyExc_RuntimeError, __Pyx_ASYNC_GEN_CANNOT_REUSE_CLOSE_MSG);
         return NULL;
     }
     retval = __Pyx_Coroutine_Throw((PyObject*)o->agt_gen, args);
     if (o->agt_args) {
         return __Pyx_async_gen_unwrap_value(o->agt_gen, retval);
     } else {
-        if (retval && __pyx__PyAsyncGenWrappedValue_CheckExact(retval)) {
+        PyObject *exc_type;
+        if (unlikely(retval && __pyx__PyAsyncGenWrappedValue_CheckExact(retval))) {
+            o->agt_gen->ag_running_async = 0;
+            o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
             Py_DECREF(retval);
             PyErr_SetString(PyExc_RuntimeError, __Pyx_ASYNC_GEN_IGNORED_EXIT_MSG);
             return NULL;
         }
+        exc_type = PyErr_Occurred();
+        if (__Pyx_PyErr_GivenExceptionMatches2(exc_type, __Pyx_PyExc_StopAsyncIteration, PyExc_GeneratorExit)) {
+            PyErr_Clear();
+            PyErr_SetNone(PyExc_StopIteration);
+        }
         return retval;
     }
 }
 static PyObject *
 __Pyx_async_gen_athrow_iternext(__pyx_PyAsyncGenAThrow *o)
 {
     return __Pyx_async_gen_athrow_send(o, Py_None);
 }
 static PyObject *
-__Pyx_async_gen_athrow_close(PyObject *g, CYTHON_UNUSED PyObject *args)
+__Pyx_async_gen_athrow_close(PyObject *g, PyObject *args)
 {
     __pyx_PyAsyncGenAThrow *o = (__pyx_PyAsyncGenAThrow*) g;
+    CYTHON_UNUSED_VAR(args);
     o->agt_state = __PYX_AWAITABLE_STATE_CLOSED;
     Py_RETURN_NONE;
 }
 static PyMethodDef __Pyx_async_gen_athrow_methods[] = {
     {"send", (PyCFunction)__Pyx_async_gen_athrow_send, METH_O, __Pyx_async_gen_send_doc},
     {"throw", (PyCFunction)__Pyx_async_gen_athrow_throw, METH_VARARGS, __Pyx_async_gen_throw_doc},
     {"close", (PyCFunction)__Pyx_async_gen_athrow_close, METH_NOARGS, __Pyx_async_gen_close_doc},
     {"__await__", (PyCFunction)__Pyx_async_gen_self_method, METH_NOARGS, __Pyx_async_gen_await_doc},
     {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx__PyAsyncGenAThrowType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_async_gen_athrow_dealloc},
+    {Py_am_await, (void *)PyObject_SelfIter},
+    {Py_tp_traverse, (void *)__Pyx_async_gen_athrow_traverse},
+    {Py_tp_iter, (void *)PyObject_SelfIter},
+    {Py_tp_iternext, (void *)__Pyx_async_gen_athrow_iternext},
+    {Py_tp_methods, (void *)__Pyx_async_gen_athrow_methods},
+    {Py_tp_getattro, (void *)__Pyx_PyObject_GenericGetAttrNoDict},
+    {0, 0},
+};
+static PyType_Spec __pyx__PyAsyncGenAThrowType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "async_generator_athrow",
+    sizeof(__pyx_PyAsyncGenAThrow),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
+    __pyx__PyAsyncGenAThrowType_slots
+};
+#else
 #if CYTHON_USE_ASYNC_SLOTS
 static __Pyx_PyAsyncMethodsStruct __Pyx_async_gen_athrow_as_async = {
     PyObject_SelfIter,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030A00A3
     0,
@@ -8508,49 +11953,70 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
+#endif
 static PyObject *
 __Pyx_async_gen_athrow_new(__pyx_PyAsyncGenObject *gen, PyObject *args)
 {
     __pyx_PyAsyncGenAThrow *o;
     o = PyObject_GC_New(__pyx_PyAsyncGenAThrow, __pyx__PyAsyncGenAThrowType);
-    if (o == NULL) {
+    if (unlikely(o == NULL)) {
         return NULL;
     }
     o->agt_gen = gen;
     o->agt_args = args;
     o->agt_state = __PYX_AWAITABLE_STATE_INIT;
     Py_INCREF(gen);
     Py_XINCREF(args);
     PyObject_GC_Track((PyObject*)o);
     return (PyObject*)o;
 }
-static int __pyx_AsyncGen_init(void) {
+static int __pyx_AsyncGen_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_AsyncGenType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_AsyncGenType_spec, NULL);
+#else
+    CYTHON_MAYBE_UNUSED_VAR(module);
     __pyx_AsyncGenType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-    __pyx__PyAsyncGenWrappedValueType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-    __pyx__PyAsyncGenAThrowType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-    __pyx__PyAsyncGenASendType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_AsyncGenType = __Pyx_FetchCommonType(&__pyx_AsyncGenType_type);
+#endif
     if (unlikely(!__pyx_AsyncGenType))
         return -1;
+#if CYTHON_USE_TYPE_SPECS
+    __pyx__PyAsyncGenAThrowType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx__PyAsyncGenAThrowType_spec, NULL);
+#else
+    __pyx__PyAsyncGenAThrowType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx__PyAsyncGenAThrowType = __Pyx_FetchCommonType(&__pyx__PyAsyncGenAThrowType_type);
+#endif
     if (unlikely(!__pyx__PyAsyncGenAThrowType))
         return -1;
+#if CYTHON_USE_TYPE_SPECS
+    __pyx__PyAsyncGenWrappedValueType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx__PyAsyncGenWrappedValueType_spec, NULL);
+#else
+    __pyx__PyAsyncGenWrappedValueType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx__PyAsyncGenWrappedValueType = __Pyx_FetchCommonType(&__pyx__PyAsyncGenWrappedValueType_type);
+#endif
     if (unlikely(!__pyx__PyAsyncGenWrappedValueType))
         return -1;
+#if CYTHON_USE_TYPE_SPECS
+    __pyx__PyAsyncGenASendType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx__PyAsyncGenASendType_spec, NULL);
+#else
+    __pyx__PyAsyncGenASendType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx__PyAsyncGenASendType = __Pyx_FetchCommonType(&__pyx__PyAsyncGenASendType_type);
+#endif
     if (unlikely(!__pyx__PyAsyncGenASendType))
         return -1;
     return 0;
 }
 
 /* AsyncGen */
 
@@ -8581,50 +12047,60 @@
                 found_dot = 1;
             } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
                 break;
             }
             rtversion[i] = rt_from_call[i];
         }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
+#if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -8678,15 +12154,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -8707,30 +12183,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -8788,15 +12268,15 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
+    const digit* digits = __Pyx_PyLong_Digits(b);
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
         ival = likely(size) ? digits[0] : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
@@ -8862,8 +12342,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#if _MSV_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `aiocsv-1.2.3/aiocsv/_parser.pyx` & `aiocsv-1.2.4/aiocsv/_parser.pyx`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/aiocsv/parser.py` & `aiocsv-1.2.4/aiocsv/parser.py`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/aiocsv/readers.py` & `aiocsv-1.2.4/aiocsv/readers.py`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/aiocsv/writers.py` & `aiocsv-1.2.4/aiocsv/writers.py`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/aiocsv.egg-info/PKG-INFO` & `aiocsv-1.2.4/aiocsv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocsv
-Version: 1.2.3
+Version: 1.2.4
 Summary: Asynchronous CSV reading/writing
 Home-page: https://github.com/MKuranowski/aiocsv
 Author: Mikołaj Kuranowski
 Author-email: mkuranowski@gmail.com
 License: MIT
 Keywords: async asynchronous aiofiles csv tsv
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiocsv-1.2.3/license.md` & `aiocsv-1.2.4/license.md`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/readme.md` & `aiocsv-1.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `aiocsv-1.2.3/setup.py` & `aiocsv-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     name="aiocsv",
     py_modules=["aiocsv"],
     ext_modules=extensions,
     packages=find_packages(include=["aiocsv"]),
     package_data={"aiocsv": ["py.typed", "_parser.pyi"]},
     zip_safe=False,
     license="MIT",
-    version="1.2.3",
+    version="1.2.4",
     description="Asynchronous CSV reading/writing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Mikołaj Kuranowski",
     author_email="".join(chr(i) for i in [109, 107, 117, 114, 97, 110, 111, 119, 115, 107, 105,
                                           64, 103, 109, 97, 105, 108, 46, 99, 111, 109]),
     url="https://github.com/MKuranowski/aiocsv",
```

