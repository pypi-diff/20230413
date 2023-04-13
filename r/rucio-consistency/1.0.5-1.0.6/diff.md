# Comparing `tmp/rucio-consistency-1.0.5.tar.gz` & `tmp/rucio-consistency-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.5.tar", last modified: Thu Apr 13 15:29:24 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.6.tar", last modified: Thu Apr 13 18:56:25 2023, max compression
```

## Comparing `rucio-consistency-1.0.5.tar` & `rucio-consistency-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.188287 rucio-consistency-1.0.5/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.5/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 15:29:24.187967 rucio-consistency-1.0.5/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.5/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.181750 rucio-consistency-1.0.5/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.5/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.186215 rucio-consistency-1.0.5/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.5/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.5/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 15:29:19.000000 rucio-consistency-1.0.5/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.187377 rucio-consistency-1.0.5/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 15:29:24.183665 rucio-consistency-1.0.5/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 15:29:24.000000 rucio-consistency-1.0.5/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 15:29:24.188368 rucio-consistency-1.0.5/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.5/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 18:56:25.004105 rucio-consistency-1.0.6/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.6/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 18:56:25.003870 rucio-consistency-1.0.6/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.6/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 18:56:24.998542 rucio-consistency-1.0.6/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.6/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 18:56:25.002727 rucio-consistency-1.0.6/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.6/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.6/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 18:56:21.000000 rucio-consistency-1.0.6/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 18:56:25.003528 rucio-consistency-1.0.6/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.6/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.6/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27384 2023-04-13 18:56:05.000000 rucio-consistency-1.0.6/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 18:56:25.000389 rucio-consistency-1.0.6/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 18:56:24.000000 rucio-consistency-1.0.6/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 18:56:25.004166 rucio-consistency-1.0.6/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.6/setup.py
```

### Comparing `rucio-consistency-1.0.5/LICENSE` & `rucio-consistency-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/cmplib.py` & `rucio-consistency-1.0.6/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/config.py` & `rucio-consistency-1.0.6/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/part.py` & `rucio-consistency-1.0.6/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.0.6/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/stats.py` & `rucio-consistency-1.0.6/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.0.6/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.0.6/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pythreader import TaskQueue, Task, DEQueue, PyThread, synchronized, ShellCommand, Primitive
-import re, json, os, os.path, traceback
+import re, json, os, os.path, traceback, sys
 import subprocess, time, random, gzip
 
-from rucio_ce import to_str, Stats, PartitionedList, ScannerConfiguration
+from rucio_consistency import to_str, Stats, PartitionedList, ScannerConfiguration
 from .xrootd_client import XRootDClient
 
 Version = "3.1"
 
 GB = 1024*1024*1024
 
 try:
@@ -437,23 +437,22 @@
         if not rewrite_path.search(lfn):
             sys.stderr.write(f"Path rewrite pattern for root {root} did not find a match in path {lfn}\n")
             sys.exit(1)
         lfn = rewrite_path.sub(rewrite_out, lfn)   
     return lfn
 
 def scan_root(rse, config, client, root, root_expected, my_stats, stats, stats_key,
-            recursive_threshold, max_scanners, file_list, dir_list, empty_dirs_file,
+            recursive_threshold, max_scanners, timeout,
+            file_list, dir_list, empty_dirs_file,
             ignore_failed_directories, include_sizes):
 
     failed = root_failed = False
     
-    timeout = override_timeout or config.ScannerTimeout
     server = config.Server
     server_root = config.ServerRoot
-    max_scanners = override_max_scanners or config.NWorkers
     ignore_subdirs = config.ignore_subdirs(root)
     is_redirector = config.ServerIsRedirector
     ignore_list = config.IgnoreList
 
     t0 = time.time()
     root_stats = {
        "root": root,
@@ -580,17 +579,19 @@
         sys.exit(2)
 
     rse = args[0]
     config = ScannerConfiguration(rse, opts["-c"])
 
     quiet = "-q" in opts
     display_progress = not quiet and "-v" in opts
-    override_recursive_threshold = int(opts.get("-R", 0))
-    override_timeout = int(opts.get("-t", 0))
-    override_max_scanners = int(opts.get("-m", 0))
+
+    recursive_threshold = int(opts.get("-R", config.RecursionThreshold))
+    max_scanners = int(opts.get("-m", config.NWorkers))
+    timeout = int(opts.get("-t", config.ScannerTimeout))
+    
     max_files = opts.get("-M")
     if max_files is not None: max_files = int(max_files)
     stats_file = opts.get("-s")
     stats_key = opts.get("-S", "scanner")
     ignore_directory_scan_errors = "-k" in opts
     root_file_counts = opts.get("-r")
     if root_file_counts:
@@ -652,16 +653,14 @@
         "dirs_output_prefix":           dir_output,
         "empty_dirs_output_file":       empty_dir_output
     }
     
     if stats is not None:
         stats[stats_key] = my_stats
     
-    max_scanners = override_max_scanners or config.NWorkers
-    recursive_threshold = override_recursive_threshold or config.RecursionThreshold
     root_paths = [canonic_path(root if root.startswith("/") else server_root + "/" + root) for root in config.RootList]
     
     t0 = time.time()
     good_roots, failed_roots = Prescanner(server, server_root, config.ServerIsRedirector, config.RootList, config.ScannerTimeout, max_scanners).run()
     t1 = time.time()
 
     failed = False
@@ -684,16 +683,17 @@
 
     if not failed:
         all_roots_failed = not good_roots
         for client, root in good_roots:
             try:
                 print(f"Scanning root {root} ...", file=sys.stderr)
                 expected = root_file_counts.get(root, 0) > 0
-                failed = scan_root(rse, config, client, root, expected, my_stats, stats, stats_key, recursive_threshold, 
-                        max_scanners, out_list, dir_list, empty_dirs_file,
+                failed = scan_root(rse, config, client, root, expected, my_stats, stats, stats_key, 
+                        recursive_threshold, max_scanners, timeout,
+                        out_list, dir_list, empty_dirs_file,
                         ignore_directory_scan_errors, include_sizes)
             except:
                 exc = traceback.format_exc()
                 print(exc)
                 lines = exc.split("\n")
                 scanning = my_stats.setdefault("scanning", {"root":client.Root})
                 scanning["exception"] = lines
```

### Comparing `rucio-consistency-1.0.5/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.6/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.5/setup.py` & `rucio-consistency-1.0.6/setup.py`

 * *Files identical despite different names*

