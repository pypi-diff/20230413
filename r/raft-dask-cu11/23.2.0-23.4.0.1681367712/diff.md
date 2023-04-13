# Comparing `tmp/raft_dask_cu11-23.2.0.tar.gz` & `tmp/raft_dask_cu11-23.4.0.1681367712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raft_dask_cu11-23.2.0.tar", last modified: Fri Feb 10 16:30:53 2023, max compression
+gzip compressed data, was "raft_dask_cu11-23.4.0.1681367712.tar", last modified: Thu Apr 13 18:15:08 2023, max compression
```

## Comparing `raft_dask_cu11-23.2.0.tar` & `raft_dask_cu11-23.4.0.1681367712.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 16:30:53.212726 raft_dask_cu11-23.2.0/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-02-09 04:19:24.000000 raft_dask_cu11-23.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-02-10 16:30:53.212726 raft_dask_cu11-23.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-02-10 16:30:53.000000 raft_dask_cu11-23.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-02-10 16:30:53.212726 raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-02-10 16:30:53.000000 raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      182 2023-02-10 16:30:53.000000 raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 16:30:53.000000 raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-02-10 16:30:53.000000 raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-02-10 16:30:53.212726 raft_dask_cu11-23.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-02-09 04:19:24.000000 raft_dask_cu11-23.2.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:15:08.794447 raft_dask_cu11-23.4.0.1681367712/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-12 18:02:21.000000 raft_dask_cu11-23.4.0.1681367712/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 18:15:08.794447 raft_dask_cu11-23.4.0.1681367712/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 18:15:08.794447 raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 18:15:08.000000 raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 18:15:08.794447 raft_dask_cu11-23.4.0.1681367712/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-12 18:02:21.000000 raft_dask_cu11-23.4.0.1681367712/setup.py
```

### Comparing `raft_dask_cu11-23.2.0/LICENSE.md` & `raft_dask_cu11-23.4.0.1681367712/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raft_dask_cu11-23.2.0/PKG-INFO` & `raft_dask_cu11-23.4.0.1681367712/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raft_dask_cu11
-Version: 23.2.0
+Version: 23.4.0.1681367712
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `raft_dask_cu11-23.2.0/raft_dask_cu11.egg-info/PKG-INFO` & `raft_dask_cu11-23.4.0.1681367712/raft_dask_cu11.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raft-dask-cu11
-Version: 23.2.0
+Version: 23.4.0.1681367712
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `raft_dask_cu11-23.2.0/setup.py` & `raft_dask_cu11-23.4.0.1681367712/setup.py`

 * *Files identical despite different names*

