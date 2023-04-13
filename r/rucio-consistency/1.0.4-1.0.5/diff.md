# Comparing `tmp/rucio-consistency-1.0.4.tar.gz` & `tmp/rucio-consistency-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.4.tar", last modified: Thu Apr 13 14:43:39 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.5.tar", last modified: Thu Apr 13 15:29:24 2023, max compression
```

## Comparing `rucio-consistency-1.0.4.tar` & `rucio-consistency-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.337809 rucio-consistency-1.0.4/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.4/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:43:39.337569 rucio-consistency-1.0.4/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.4/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.332318 rucio-consistency-1.0.4/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.336215 rucio-consistency-1.0.4/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.4/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 14:43:23.000000 rucio-consistency-1.0.4/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.337092 rucio-consistency-1.0.4/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.334194 rucio-consistency-1.0.4/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 14:43:39.337880 rucio-consistency-1.0.4/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.4/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.188287 rucio-consistency-1.0.5/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.5/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 15:29:24.187967 rucio-consistency-1.0.5/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.5/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.181750 rucio-consistency-1.0.5/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.5/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.186215 rucio-consistency-1.0.5/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.5/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 15:29:19.000000 rucio-consistency-1.0.5/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.187377 rucio-consistency-1.0.5/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.183665 rucio-consistency-1.0.5/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 15:29:24.188368 rucio-consistency-1.0.5/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.5/setup.py
```

### Comparing `rucio-consistency-1.0.4/LICENSE` & `rucio-consistency-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/cmplib.py` & `rucio-consistency-1.0.5/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/config.py` & `rucio-consistency-1.0.5/rucio_consistency/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
             backend = ConfigRucioBackend(**args)
         else:
             backend = ConfigYAMLBackend(source)
         self.Backend = backend
         self.RSE = rse
         self.NPartitions = int(backend.rse_param(rse, "npartitions", 10))
         self.IgnoreList = self.rse_param(rse, "ignore_list", [])
+        self.RootList = self.root_list(rse)
         
     def __contains__(self, name):
         try:    _ = self[name]
         except KeyError:    return False
         else:   return True
 
     def __getattr__(self, name):
@@ -278,19 +279,18 @@
 
 class ScannerConfiguration(CEConfiguration):
     
     def __init__(self, rse, source, **source_agrs):
         CEConfiguration.__init__(self, rse, source, **source_agrs)
 
         self.Server = self.scanner_param(rse, "server", None, required=True)
-        self.ServerRoot = self.scanner_param(rse, "server_root", "/store")
+        self.ServerRoot = self.scanner_param(rse, "server_root", "/")           # prefix up to, but not including /store/
         self.ScannerTimeout = int(self.scanner_param(rse, "timeout", 300))
-        self.RootList = self.root_list(rse)
-        self.RemovePrefix = self.scanner_param(rse, "remove_prefix", "/")
-        self.AddPrefix = self.scanner_param(rse, "add_prefix", "/store/")
+        self.RemovePrefix = self.scanner_param(rse, "remove_prefix", "")        # to be applied after site root is removed
+        self.AddPrefix = self.scanner_param(rse, "add_prefix", "")              # to be applied after site root is removed
         self.NWorkers = int(self.scanner_param(rse, "nworkers", 8))
         self.IncludeSizes = self.scanner_param(rse, "include_sizes", "yes") == "yes"
         self.RecursionThreshold = int(self.scanner_param(rse, "recursion", 1))
         self.ServerIsRedirector = self.scanner_param(rse, "is_redirector", True)
 
     def ignore_subdirs(self, root):
         return self.root_param(self.RSE, root, "ignore", [])
```

### Comparing `rucio-consistency-1.0.4/rucio_consistency/part.py` & `rucio-consistency-1.0.5/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.0.5/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/stats.py` & `rucio-consistency-1.0.5/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.5/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.4/setup.py` & `rucio-consistency-1.0.5/setup.py`

 * *Files identical despite different names*

