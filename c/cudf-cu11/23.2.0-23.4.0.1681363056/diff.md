# Comparing `tmp/cudf_cu11-23.2.0.tar.gz` & `tmp/cudf_cu11-23.4.0.1681363056.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudf_cu11-23.2.0.tar", last modified: Fri Feb 10 17:30:12 2023, max compression
+gzip compressed data, was "cudf_cu11-23.4.0.1681363056.tar", last modified: Thu Apr 13 19:10:44 2023, max compression
```

## Comparing `cudf_cu11-23.2.0.tar` & `cudf_cu11-23.4.0.1681363056.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:30:12.166524 cudf_cu11-23.2.0/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-02-09 03:02:43.000000 cudf_cu11-23.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-02-10 17:30:12.166524 cudf_cu11-23.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-02-10 17:30:12.000000 cudf_cu11-23.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:30:12.166524 cudf_cu11-23.2.0/cudf_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-02-10 17:30:12.000000 cudf_cu11-23.2.0/cudf_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      162 2023-02-10 17:30:12.000000 cudf_cu11-23.2.0/cudf_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:30:12.000000 cudf_cu11-23.2.0/cudf_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:30:12.000000 cudf_cu11-23.2.0/cudf_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-02-10 17:30:12.166524 cudf_cu11-23.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-02-09 03:02:43.000000 cudf_cu11-23.2.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 14:11:27.000000 cudf_cu11-23.4.0.1681363056/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:10:44.000000 cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:10:44.883822 cudf_cu11-23.4.0.1681363056/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 14:11:27.000000 cudf_cu11-23.4.0.1681363056/setup.py
```

### Comparing `cudf_cu11-23.2.0/LICENSE.md` & `cudf_cu11-23.4.0.1681363056/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cudf_cu11-23.2.0/PKG-INFO` & `cudf_cu11-23.4.0.1681363056/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf_cu11
-Version: 23.2.0
+Version: 23.4.0.1681363056
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf_cu11-23.2.0/cudf_cu11.egg-info/PKG-INFO` & `cudf_cu11-23.4.0.1681363056/cudf_cu11.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf-cu11
-Version: 23.2.0
+Version: 23.4.0.1681363056
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf_cu11-23.2.0/setup.py` & `cudf_cu11-23.4.0.1681363056/setup.py`

 * *Files identical despite different names*

