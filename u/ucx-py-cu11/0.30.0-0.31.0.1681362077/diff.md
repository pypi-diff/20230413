# Comparing `tmp/ucx_py_cu11-0.30.0.tar.gz` & `tmp/ucx_py_cu11-0.31.0.1681362077.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucx_py_cu11-0.30.0.tar", last modified: Fri Feb 10 17:20:40 2023, max compression
+gzip compressed data, was "ucx_py_cu11-0.31.0.1681362077.tar", last modified: Thu Apr 13 19:15:14 2023, max compression
```

## Comparing `ucx_py_cu11-0.30.0.tar` & `ucx_py_cu11-0.31.0.1681362077.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:20:40.243762 ucx_py_cu11-0.30.0/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-02-09 04:23:22.000000 ucx_py_cu11-0.30.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-02-10 17:20:40.243762 ucx_py_cu11-0.30.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-02-10 17:20:40.000000 ucx_py_cu11-0.30.0/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-02-10 17:20:40.243762 ucx_py_cu11-0.30.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-02-09 04:23:22.000000 ucx_py_cu11-0.30.0/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:20:40.243762 ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1592 2023-02-10 17:20:40.000000 ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      170 2023-02-10 17:20:40.000000 ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:20:40.000000 ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:20:40.000000 ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:15:14.004041 ucx_py_cu11-0.31.0.1681362077/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      443 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:15:03.000000 ucx_py_cu11-0.31.0.1681362077/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1603 2023-04-13 19:15:14.002041 ucx_py_cu11-0.31.0.1681362077/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      238 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:15:14.004041 ucx_py_cu11-0.31.0.1681362077/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:15:03.000000 ucx_py_cu11-0.31.0.1681362077/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:15:14.002041 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1603 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:15:13.000000 ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/top_level.txt
```

### Comparing `ucx_py_cu11-0.30.0/LICENSE.md` & `ucx_py_cu11-0.31.0.1681362077/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.30.0/PKG-INFO` & `ucx_py_cu11-0.31.0.1681362077/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucx_py_cu11
-Version: 0.30.0
+Version: 0.31.0.1681362077
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `ucx_py_cu11-0.30.0/setup.py` & `ucx_py_cu11-0.31.0.1681362077/setup.py`

 * *Files identical despite different names*

### Comparing `ucx_py_cu11-0.30.0/ucx_py_cu11.egg-info/PKG-INFO` & `ucx_py_cu11-0.31.0.1681362077/ucx_py_cu11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucx-py-cu11
-Version: 0.30.0
+Version: 0.31.0.1681362077
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

