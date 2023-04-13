# Comparing `tmp/ftd2xx-1.3.1.tar.gz` & `tmp/ftd2xx-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftd2xx-1.3.1.tar", last modified: Tue Apr 12 15:23:49 2022, max compression
+gzip compressed data, was "ftd2xx-1.3.2.tar", last modified: Thu Apr 13 10:20:53 2023, max compression
```

## Comparing `ftd2xx-1.3.1.tar` & `ftd2xx-1.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:49.159242 ftd2xx-1.3.1/ftd2xx/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34987 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/_ftd2xx.py
--rw-r--r--   0 runner    (1001) docker     (121)    95375 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/_ftd2xx_darwin.py
--rw-r--r--   0 runner    (1001) docker     (121)    37524 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/_ftd2xx_linux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/ftd2xx/aio/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/aio/aio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/defines.py
--rw-r--r--   0 runner    (1001) docker     (121)    19927 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/ftd2xx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/ftd2xx/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/tests/t_aio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4361 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/ftd2xx/tests/t_ftd2xx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/ftd2xx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-12 15:23:49.000000 ftd2xx-1.3.1/ftd2xx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/myversion.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-04-12 15:23:49.163242 ftd2xx-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-04-12 15:23:42.000000 ftd2xx-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34987 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95427 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx_darwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37524 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/_ftd2xx_linux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/aio/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19978 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/ftd2xx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/t_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/ftd2xx/tests/t_ftd2xx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/ftd2xx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 10:20:53.000000 ftd2xx-1.3.2/ftd2xx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/myversion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 10:20:53.941053 ftd2xx-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 10:20:43.000000 ftd2xx-1.3.2/setup.py
```

### Comparing `ftd2xx-1.3.1/LICENSE` & `ftd2xx-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/PKG-INFO` & `ftd2xx-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ftd2xx
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python interface to ftd2xx.dll from FTDI using ctypesbased on d2xx by Pablo Bleyer
 Home-page: https://github.com/snmishra/ftd2xx
 Author: Satya Mishra
 Author-email: satya.devel@gmail.com
 License: MIT
 Keywords: ftd2xx d2xx ftdi
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 Provides-Extra: aio
 License-File: LICENSE
 
@@ -48,9 +47,7 @@
 .. |python|
     image:: https://img.shields.io/pypi/pyversions/ftd2xx.svg
         :target: https://pypi.org/project/ftd2xx/
 .. |package|
     image:: https://github.com/snmishra/ftd2xx/workflows/Python%20package/badge.svg
 .. |lint|
     image:: https://github.com/snmishra/ftd2xx/workflows/Lint/badge.svg
-
-
```

### Comparing `ftd2xx-1.3.1/README.rst` & `ftd2xx-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/__init__.py` & `ftd2xx-1.3.2/ftd2xx/__init__.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/_ftd2xx.py` & `ftd2xx-1.3.2/ftd2xx/_ftd2xx.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/_ftd2xx_darwin.py` & `ftd2xx-1.3.2/ftd2xx/_ftd2xx_darwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 __int32_t = c_int
 __uint32_t = c_uint
 __int64_t = c_longlong
 __uint64_t = c_ulonglong
 __darwin_intptr_t = c_long
 __darwin_natural_t = c_uint
 __darwin_ct_rune_t = c_int
+
+
 # /usr/include/i386/_types.h 79
 class __mbstate_t(Union):
     pass
 
 
 __darwin_mbstate_t = __mbstate_t
 __darwin_ptrdiff_t = c_int
@@ -59,72 +61,90 @@
 __darwin_wchar_t = c_int
 __darwin_rune_t = __darwin_wchar_t
 __darwin_wint_t = c_int
 __darwin_clock_t = c_ulong
 __darwin_socklen_t = __uint32_t
 __darwin_ssize_t = c_long
 __darwin_time_t = c_long
+
+
 # /usr/include/sys/_types.h 64
 class _opaque_pthread_attr_t(Structure):
     pass
 
 
 __darwin_pthread_attr_t = _opaque_pthread_attr_t
 pthread_attr_t = __darwin_pthread_attr_t
+
+
 # /usr/include/sys/_types.h 65
 class _opaque_pthread_cond_t(Structure):
     pass
 
 
 __darwin_pthread_cond_t = _opaque_pthread_cond_t
 pthread_cond_t = __darwin_pthread_cond_t
+
+
 # /usr/include/sys/_types.h 66
 class _opaque_pthread_condattr_t(Structure):
     pass
 
 
 __darwin_pthread_condattr_t = _opaque_pthread_condattr_t
 pthread_condattr_t = __darwin_pthread_condattr_t
 __darwin_pthread_key_t = c_ulong
 pthread_key_t = __darwin_pthread_key_t
+
+
 # /usr/include/sys/_types.h 67
 class _opaque_pthread_mutex_t(Structure):
     pass
 
 
 __darwin_pthread_mutex_t = _opaque_pthread_mutex_t
 pthread_mutex_t = __darwin_pthread_mutex_t
+
+
 # /usr/include/sys/_types.h 68
 class _opaque_pthread_mutexattr_t(Structure):
     pass
 
 
 __darwin_pthread_mutexattr_t = _opaque_pthread_mutexattr_t
 pthread_mutexattr_t = __darwin_pthread_mutexattr_t
+
+
 # /usr/include/sys/_types.h 69
 class _opaque_pthread_once_t(Structure):
     pass
 
 
 __darwin_pthread_once_t = _opaque_pthread_once_t
 pthread_once_t = __darwin_pthread_once_t
+
+
 # /usr/include/sys/_types.h 70
 class _opaque_pthread_rwlock_t(Structure):
     pass
 
 
 __darwin_pthread_rwlock_t = _opaque_pthread_rwlock_t
 pthread_rwlock_t = __darwin_pthread_rwlock_t
+
+
 # /usr/include/sys/_types.h 71
 class _opaque_pthread_rwlockattr_t(Structure):
     pass
 
 
 __darwin_pthread_rwlockattr_t = _opaque_pthread_rwlockattr_t
 pthread_rwlockattr_t = __darwin_pthread_rwlockattr_t
+
+
 # /usr/include/sys/_types.h 72
 class _opaque_pthread_t(Structure):
     pass
 
 
 __darwin_pthread_t = POINTER(_opaque_pthread_t)
 pthread_t = __darwin_pthread_t
@@ -171,14 +191,16 @@
     "/usr/local/lib/libftd2xx.dylib"
 ].pthread_attr_getinheritsched
 pthread_attr_getinheritsched.restype = c_int
 # pthread_attr_getinheritsched(p1, p2)
 pthread_attr_getinheritsched.argtypes = [POINTER(pthread_attr_t), POINTER(c_int)]
 pthread_attr_getinheritsched.__doc__ = """int pthread_attr_getinheritsched(unknown * p1, int * p2)
 /usr/include/pthread.h:252"""
+
+
 # /usr/include/sched.h 35
 class sched_param(Structure):
     pass
 
 
 # /usr/include/pthread.h 254
 pthread_attr_getschedparam = _libraries[
@@ -364,14 +386,16 @@
 # /usr/include/pthread.h 286
 pthread_cond_signal = _libraries["/usr/local/lib/libftd2xx.dylib"].pthread_cond_signal
 pthread_cond_signal.restype = c_int
 # pthread_cond_signal(p1)
 pthread_cond_signal.argtypes = [POINTER(pthread_cond_t)]
 pthread_cond_signal.__doc__ = """int pthread_cond_signal(pthread_cond_t * p1)
 /usr/include/pthread.h:286"""
+
+
 # /usr/include/sys/_structs.h 89
 class timespec(Structure):
     pass
 
 
 timespec._fields_ = [
     # /usr/include/sys/_structs.h 89
@@ -961,14 +985,16 @@
     "/usr/local/lib/libftd2xx.dylib"
 ].sched_get_priority_max
 sched_get_priority_max.restype = c_int
 # sched_get_priority_max(p1)
 sched_get_priority_max.argtypes = [c_int]
 sched_get_priority_max.__doc__ = """int sched_get_priority_max(int p1)
 /usr/include/sched.h:40"""
+
+
 # /usr/include/sys/_structs.h 184
 class fd_set(Structure):
     pass
 
 
 # /usr/include/sys/_structs.h 101
 class timeval(Structure):
@@ -994,14 +1020,16 @@
     ("tv_sec", __darwin_time_t),
     ("tv_usec", __darwin_suseconds_t),
 ]
 fd_set._fields_ = [
     # /usr/include/sys/_structs.h 184
     ("fds_bits", __int32_t * 32),
 ]
+
+
 # /usr/include/sys/_types.h 59
 class __darwin_pthread_handler_rec(Structure):
     pass
 
 
 __darwin_pthread_handler_rec._fields_ = [
     # /usr/include/sys/_types.h 59
@@ -1067,34 +1095,40 @@
 __darwin_mode_t = __uint16_t
 __darwin_off_t = __int64_t
 __darwin_pid_t = __int32_t
 __darwin_uid_t = __uint32_t
 __darwin_useconds_t = __uint32_t
 __darwin_uuid_t = c_ubyte * 16
 suseconds_t = __darwin_suseconds_t
+
+
 # /usr/include/sys/time.h 93
 class itimerval(Structure):
     pass
 
 
 itimerval._fields_ = [
     # /usr/include/sys/time.h 93
     ("it_interval", timeval),
     ("it_value", timeval),
 ]
+
+
 # /usr/include/sys/time.h 144
 class timezone(Structure):
     pass
 
 
 timezone._fields_ = [
     # /usr/include/sys/time.h 144
     ("tz_minuteswest", c_int),
     ("tz_dsttime", c_int),
 ]
+
+
 # /usr/include/sys/time.h 187
 class clockinfo(Structure):
     pass
 
 
 clockinfo._fields_ = [
     # /usr/include/sys/time.h 187
@@ -1158,14 +1192,16 @@
 utimes.restype = c_int
 # utimes(p1, p2)
 utimes.argtypes = [STRING, POINTER(timeval)]
 utimes.__doc__ = """int utimes(unknown * p1, unknown * p2)
 /usr/include/sys/time.h:217"""
 clock_t = __darwin_clock_t
 time_t = __darwin_time_t
+
+
 # /usr/include/time.h 90
 class tm(Structure):
     pass
 
 
 tm._fields_ = [
     # /usr/include/time.h 90
@@ -1359,14 +1395,16 @@
 LPTSTR = STRING
 LPDWORD = POINTER(DWORD)
 LPWORD = POINTER(WORD)
 PULONG = POINTER(ULONG)
 LPVOID = PVOID
 VOID = None
 ULONGLONG = c_ulonglong
+
+
 # /usr/local/include/WinTypes.h 36
 class _OVERLAPPED(Structure):
     pass
 
 
 _OVERLAPPED._fields_ = [
     # /usr/local/include/WinTypes.h 36
@@ -1374,14 +1412,16 @@
     ("InternalHigh", DWORD),
     ("Offset", DWORD),
     ("OffsetHigh", DWORD),
     ("hEvent", HANDLE),
 ]
 LPOVERLAPPED = POINTER(_OVERLAPPED)
 OVERLAPPED = _OVERLAPPED
+
+
 # /usr/local/include/WinTypes.h 44
 class _SECURITY_ATTRIBUTES(Structure):
     pass
 
 
 _SECURITY_ATTRIBUTES._fields_ = [
     # /usr/local/include/WinTypes.h 44
@@ -1389,14 +1429,16 @@
     ("lpSecurityDescriptor", LPVOID),
     ("bInheritHandle", BOOL),
 ]
 LPSECURITY_ATTRIBUTES = POINTER(_SECURITY_ATTRIBUTES)
 SECURITY_ATTRIBUTES = _SECURITY_ATTRIBUTES
 SYSTEMTIME = timeval
 FILETIME = timeval
+
+
 # /usr/local/include/ftd2xx.h 64
 class _EVENT_HANDLE(Structure):
     pass
 
 
 _EVENT_HANDLE._fields_ = [
     # /usr/local/include/ftd2xx.h 64
@@ -1653,14 +1695,16 @@
 # /usr/local/include/ftd2xx.h 431
 FT_EraseEE = _libraries["/usr/local/lib/libftd2xx.dylib"].FT_EraseEE
 FT_EraseEE.restype = FT_STATUS
 # FT_EraseEE(ftHandle)
 FT_EraseEE.argtypes = [FT_HANDLE]
 FT_EraseEE.__doc__ = """FT_STATUS FT_EraseEE(FT_HANDLE ftHandle)
 /usr/local/include/ftd2xx.h:431"""
+
+
 # /usr/local/include/ftd2xx.h 436
 class ft_program_data(Structure):
     pass
 
 
 ft_program_data._fields_ = [
     # /usr/local/include/ftd2xx.h 436
@@ -1908,14 +1952,16 @@
 # /usr/local/include/ftd2xx.h 688
 FT_W32_CancelIo = _libraries["/usr/local/lib/libftd2xx.dylib"].FT_W32_CancelIo
 FT_W32_CancelIo.restype = BOOL
 # FT_W32_CancelIo(ftHandle)
 FT_W32_CancelIo.argtypes = [FT_HANDLE]
 FT_W32_CancelIo.__doc__ = """BOOL FT_W32_CancelIo(FT_HANDLE ftHandle)
 /usr/local/include/ftd2xx.h:688"""
+
+
 # /usr/local/include/ftd2xx.h 694
 class _FTCOMSTAT(Structure):
     pass
 
 
 _FTCOMSTAT._fields_ = [
     # /usr/local/include/ftd2xx.h 694
@@ -1928,14 +1974,16 @@
     ("fTxim", DWORD, 1),
     ("fReserved", DWORD, 25),
     ("cbInQue", DWORD),
     ("cbOutQue", DWORD),
 ]
 LPFTCOMSTAT = POINTER(_FTCOMSTAT)
 FTCOMSTAT = _FTCOMSTAT
+
+
 # /usr/local/include/ftd2xx.h 707
 class _FTDCB(Structure):
     pass
 
 
 _FTDCB._fields_ = [
     # /usr/local/include/ftd2xx.h 707
@@ -1966,14 +2014,16 @@
     ("ErrorChar", c_char),
     ("EofChar", c_char),
     ("EvtChar", c_char),
     ("wReserved1", WORD),
 ]
 FTDCB = _FTDCB
 LPFTDCB = POINTER(_FTDCB)
+
+
 # /usr/local/include/ftd2xx.h 738
 class _FTTIMEOUTS(Structure):
     pass
 
 
 _FTTIMEOUTS._fields_ = [
     # /usr/local/include/ftd2xx.h 738
@@ -2084,14 +2134,16 @@
 # /usr/local/include/ftd2xx.h 824
 FT_W32_WaitCommEvent = _libraries["/usr/local/lib/libftd2xx.dylib"].FT_W32_WaitCommEvent
 FT_W32_WaitCommEvent.restype = BOOL
 # FT_W32_WaitCommEvent(ftHandle, pulEvent, lpOverlapped)
 FT_W32_WaitCommEvent.argtypes = [FT_HANDLE, PULONG, LPOVERLAPPED]
 FT_W32_WaitCommEvent.__doc__ = """BOOL FT_W32_WaitCommEvent(FT_HANDLE ftHandle, PULONG pulEvent, LPOVERLAPPED lpOverlapped)
 /usr/local/include/ftd2xx.h:824"""
+
+
 # /usr/local/include/ftd2xx.h 830
 class _ft_device_list_info_node(Structure):
     pass
 
 
 _ft_device_list_info_node._fields_ = [
     # /usr/local/include/ftd2xx.h 830
```

### Comparing `ftd2xx-1.3.1/ftd2xx/_ftd2xx_linux.py` & `ftd2xx-1.3.2/ftd2xx/_ftd2xx_linux.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/aio/aio.py` & `ftd2xx-1.3.2/ftd2xx/aio/aio.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/defines.py` & `ftd2xx-1.3.2/ftd2xx/defines.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/ftd2xx.py` & `ftd2xx-1.3.2/ftd2xx/ftd2xx.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,15 +448,15 @@
         call_ft(_ft.FT_SetLatencyTimer, self.handle, _ft.UCHAR(latency))
 
     def getLatencyTimer(self) -> int:
         latency = _ft.UCHAR()
         call_ft(_ft.FT_GetLatencyTimer, self.handle, c.byref(latency))
         return latency.value
 
-    def setBitMode(self, mask: int, enable: bool):
+    def setBitMode(self, mask: int, enable: int):
         call_ft(_ft.FT_SetBitMode, self.handle, _ft.UCHAR(mask), _ft.UCHAR(enable))
 
     def getBitMode(self) -> int:
         mask = _ft.UCHAR()
         call_ft(_ft.FT_GetBitMode, self.handle, c.byref(mask))
         return mask.value
 
@@ -550,34 +550,34 @@
         Description = c.create_string_buffer(defines.MAX_DESCRIPTION_SIZE)
         SerialNumber = c.create_string_buffer(defines.MAX_DESCRIPTION_SIZE)
         progdata = ft_program_data(
             **ProgramData(
                 Signature1=0,
                 Signature2=0xFFFFFFFF,
                 Version=2,
-                Manufacturer=c.addressof(Manufacturer),
-                ManufacturerId=c.addressof(ManufacturerId),
-                Description=c.addressof(Description),
-                SerialNumber=c.addressof(SerialNumber),
+                Manufacturer=c.cast(Manufacturer, c.c_char_p),
+                ManufacturerId=c.cast(ManufacturerId, c.c_char_p),
+                Description=c.cast(Description, c.c_char_p),
+                SerialNumber=c.cast(SerialNumber, c.c_char_p),
             )
         )
 
         call_ft(_ft.FT_EE_Read, self.handle, c.byref(progdata))
         return progdata
 
     def eeUASize(self) -> int:
         """Get the EEPROM user area size"""
         uasize = _ft.DWORD()
         call_ft(_ft.FT_EE_UASize, self.handle, c.byref(uasize))
         return uasize.value
 
     def eeUAWrite(self, data: bytes) -> None:
-        """Write data to the EEPROM user area. data must be a string with
+        """Write data to the EEPROM user area. data must be a bytes object with
         appropriate byte values"""
-        buf = c.create_string_buffer(data)
+        buf = (c.c_ubyte * len(data)).from_buffer_copy(data)
         call_ft(_ft.FT_EE_UAWrite, self.handle, buf, len(data))
 
     def eeUARead(self, b_to_read: int) -> bytes:
         """Read b_to_read bytes from the EEPROM user area"""
         b_read = _ft.DWORD()
         # buf = c.create_string_buffer(b_to_read)
         buf = (c.c_ubyte * (b_to_read + 1))()
```

### Comparing `ftd2xx-1.3.1/ftd2xx/tests/t_aio.py` & `ftd2xx-1.3.2/ftd2xx/tests/t_aio.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx/tests/t_ftd2xx.py` & `ftd2xx-1.3.2/ftd2xx/tests/t_ftd2xx.py`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/ftd2xx.egg-info/PKG-INFO` & `ftd2xx-1.3.2/ftd2xx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ftd2xx
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python interface to ftd2xx.dll from FTDI using ctypesbased on d2xx by Pablo Bleyer
 Home-page: https://github.com/snmishra/ftd2xx
 Author: Satya Mishra
 Author-email: satya.devel@gmail.com
 License: MIT
 Keywords: ftd2xx d2xx ftdi
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 Provides-Extra: aio
 License-File: LICENSE
 
@@ -48,9 +47,7 @@
 .. |python|
     image:: https://img.shields.io/pypi/pyversions/ftd2xx.svg
         :target: https://pypi.org/project/ftd2xx/
 .. |package|
     image:: https://github.com/snmishra/ftd2xx/workflows/Python%20package/badge.svg
 .. |lint|
     image:: https://github.com/snmishra/ftd2xx/workflows/Lint/badge.svg
-
-
```

### Comparing `ftd2xx-1.3.1/ftd2xx.egg-info/SOURCES.txt` & `ftd2xx-1.3.2/ftd2xx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/setup.cfg` & `ftd2xx-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ftd2xx-1.3.1/setup.py` & `ftd2xx-1.3.2/setup.py`

 * *Files identical despite different names*

