# Comparing `tmp/rmm_cu11-23.2.0.tar.gz` & `tmp/rmm_cu11-23.4.0.1681362075.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmm_cu11-23.2.0.tar", last modified: Fri Feb 10 15:59:15 2023, max compression
+gzip compressed data, was "rmm_cu11-23.4.0.1681362075.tar", last modified: Thu Apr 13 18:22:41 2023, max compression
```

## Comparing `rmm_cu11-23.2.0.tar` & `rmm_cu11-23.4.0.1681362075.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 15:59:15.477558 rmm_cu11-23.2.0/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-02-09 03:02:43.000000 rmm_cu11-23.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1580 2023-02-10 15:59:15.477558 rmm_cu11-23.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      229 2023-02-10 15:59:15.000000 rmm_cu11-23.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 15:59:15.477558 rmm_cu11-23.2.0/rmm_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1580 2023-02-10 15:59:15.000000 rmm_cu11-23.2.0/rmm_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      158 2023-02-10 15:59:15.000000 rmm_cu11-23.2.0/rmm_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 15:59:15.000000 rmm_cu11-23.2.0/rmm_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 15:59:15.000000 rmm_cu11-23.2.0/rmm_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-02-10 15:59:15.477558 rmm_cu11-23.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-02-09 03:02:43.000000 rmm_cu11-23.2.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:22:41.054240 rmm_cu11-23.4.0.1681362075/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      440 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 02:54:55.000000 rmm_cu11-23.4.0.1681362075/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        8 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1591 2023-04-13 18:22:41.054240 rmm_cu11-23.4.0.1681362075/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      229 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:22:41.054240 rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1591 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      181 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:22:41.000000 rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 18:22:41.054240 rmm_cu11-23.4.0.1681362075/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 02:54:55.000000 rmm_cu11-23.4.0.1681362075/setup.py
```

### Comparing `rmm_cu11-23.2.0/LICENSE.md` & `rmm_cu11-23.4.0.1681362075/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rmm_cu11-23.2.0/PKG-INFO` & `rmm_cu11-23.4.0.1681362075/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmm_cu11
-Version: 23.2.0
+Version: 23.4.0.1681362075
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `rmm_cu11-23.2.0/rmm_cu11.egg-info/PKG-INFO` & `rmm_cu11-23.4.0.1681362075/rmm_cu11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmm-cu11
-Version: 23.2.0
+Version: 23.4.0.1681362075
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `rmm_cu11-23.2.0/setup.py` & `rmm_cu11-23.4.0.1681362075/setup.py`

 * *Files identical despite different names*

