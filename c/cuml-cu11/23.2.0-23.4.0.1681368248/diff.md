# Comparing `tmp/cuml_cu11-23.2.0.tar.gz` & `tmp/cuml_cu11-23.4.0.1681368248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuml_cu11-23.2.0.tar", last modified: Fri Feb 10 17:22:01 2023, max compression
+gzip compressed data, was "cuml_cu11-23.4.0.1681368248.tar", last modified: Thu Apr 13 19:13:51 2023, max compression
```

## Comparing `cuml_cu11-23.2.0.tar` & `cuml_cu11-23.4.0.1681368248.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:22:01.198511 cuml_cu11-23.2.0/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-02-09 07:49:17.000000 cuml_cu11-23.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-02-10 17:22:01.198511 cuml_cu11-23.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-02-10 17:22:01.000000 cuml_cu11-23.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 17:22:01.197510 cuml_cu11-23.2.0/cuml_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-02-10 17:22:01.000000 cuml_cu11-23.2.0/cuml_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      162 2023-02-10 17:22:01.000000 cuml_cu11-23.2.0/cuml_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:22:01.000000 cuml_cu11-23.2.0/cuml_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 17:22:01.000000 cuml_cu11-23.2.0/cuml_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-02-10 17:22:01.198511 cuml_cu11-23.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-02-09 07:49:17.000000 cuml_cu11-23.2.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:13:51.096128 cuml_cu11-23.4.0.1681368248/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-04-13 19:13:50.000000 cuml_cu11-23.4.0.1681368248/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:15:03.000000 cuml_cu11-23.4.0.1681368248/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-04-13 19:13:50.000000 cuml_cu11-23.4.0.1681368248/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:13:51.095128 cuml_cu11-23.4.0.1681368248/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-04-13 19:13:50.000000 cuml_cu11-23.4.0.1681368248/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:13:51.094128 cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1595 2023-04-13 19:13:51.000000 cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-04-13 19:13:51.000000 cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:13:51.000000 cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:13:51.000000 cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:13:51.096128 cuml_cu11-23.4.0.1681368248/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:15:03.000000 cuml_cu11-23.4.0.1681368248/setup.py
```

### Comparing `cuml_cu11-23.2.0/LICENSE.md` & `cuml_cu11-23.4.0.1681368248/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cuml_cu11-23.2.0/PKG-INFO` & `cuml_cu11-23.4.0.1681368248/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuml_cu11
-Version: 23.2.0
+Version: 23.4.0.1681368248
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cuml_cu11-23.2.0/cuml_cu11.egg-info/PKG-INFO` & `cuml_cu11-23.4.0.1681368248/cuml_cu11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuml-cu11
-Version: 23.2.0
+Version: 23.4.0.1681368248
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cuml_cu11-23.2.0/setup.py` & `cuml_cu11-23.4.0.1681368248/setup.py`

 * *Files identical despite different names*

