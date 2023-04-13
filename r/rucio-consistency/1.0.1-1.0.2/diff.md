# Comparing `tmp/rucio-consistency-1.0.1.tar.gz` & `tmp/rucio-consistency-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.1.tar", last modified: Wed Apr 12 14:58:27 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.2.tar", last modified: Thu Apr 13 14:06:08 2023, max compression
```

## Comparing `rucio-consistency-1.0.1.tar` & `rucio-consistency-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.487654 rucio-consistency-1.0.1/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.1/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-12 14:58:27.487347 rucio-consistency-1.0.1/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.1/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.481781 rucio-consistency-1.0.1/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.485429 rucio-consistency-1.0.1/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9447 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3500 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-12 14:57:22.000000 rucio-consistency-1.0.1/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.486825 rucio-consistency-1.0.1/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9440 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.483859 rucio-consistency-1.0.1/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      808 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      325 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-12 14:58:27.487736 rucio-consistency-1.0.1/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1313 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:06:08.652639 rucio-consistency-1.0.2/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.2/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:06:08.652404 rucio-consistency-1.0.2/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.2/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:06:08.645638 rucio-consistency-1.0.2/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:06:08.650613 rucio-consistency-1.0.2/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9447 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/db_dump.py
+-rw-r--r--   0 ivm        (501) staff       (20)     2264 2023-04-13 13:43:20.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/diffs.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.2/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.2/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 14:06:04.000000 rucio-consistency-1.0.2/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:06:08.651980 rucio-consistency-1.0.2/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9440 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.2/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:06:08.647164 rucio-consistency-1.0.2/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      885 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      437 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 14:06:08.000000 rucio-consistency-1.0.2/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 14:06:08.652699 rucio-consistency-1.0.2/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1455 2023-04-13 13:49:07.000000 rucio-consistency-1.0.2/setup.py
```

### Comparing `rucio-consistency-1.0.1/LICENSE` & `rucio-consistency-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/cmplib.py` & `rucio-consistency-1.0.2/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/config.py` & `rucio-consistency-1.0.2/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/part.py` & `rucio-consistency-1.0.2/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.0.2/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.0.2/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.0.2/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.0.2/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.0.2/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/stats.py` & `rucio-consistency-1.0.2/rucio_consistency/stats.py`

 * *Files 23% similar despite different names*

```diff
@@ -77,45 +77,8 @@
                 stats = json.loads(f.read())
         if stats_key:
             stats[stats_key] = my_stats
         else:
             stats.update(my_stats)
         open(stats_file, "w").write(json.dumps(stats))
 
-Usage = """
-python [-k <key>] [-u <update JSON file>] [-j "<inline JSON expression>"] [-t] <stats JSON file to update>
-"""
-
-if __name__ == "__main__":
-    import sys, getopt
-    
-    opts, args = getopt.getopt(sys.argv[1:], "k:u:j:t")
-    opts = dict(opts)
-    
-    if not args:
-        print(Usage)
-        sys.exit(2)
-    stats_file = args[0]
-    key = opts.get("-k")
-    if "-u" in opts:
-        update = json.loads(open(opts["-u"], "r").read())
-    elif "-j" in opts:
-        update = json.loads(opts["-j"])
-    elif "-t" in opts:
-        update = sys.stdin.read()           # treat the input as text value
-    else:
-        update = json.loads(sys.stdin.read())
-
-    s = Stats(stats_file)
-    if key:
-        path = key.split("/")
-        path, last = path[:-1], path[-1]
-        d = s
-        for p in path:
-            d = d.setdefault(p, {})            
-            print(p, d, s.Data)
-        d[last] = update
-        s.save()
-    else:
-        s.update(update)
-    
-    
+
```

### Comparing `rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.0.2/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.0.2/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.1/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.2/rucio_consistency.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 rucio_consistency.egg-info/not-zip-safe
 rucio_consistency.egg-info/requires.txt
 rucio_consistency.egg-info/top_level.txt
 rucio_consistency/scripts/cmp2.py
 rucio_consistency/scripts/cmp3.py
 rucio_consistency/scripts/cmp5.py
 rucio_consistency/scripts/db_dump.py
+rucio_consistency/scripts/diffs.py
 rucio_consistency/scripts/partition.py
+rucio_consistency/scripts/update_stats.py
 rucio_consistency/xrootd/__init__.py
 rucio_consistency/xrootd/xrootd_client.py
 rucio_consistency/xrootd/xrootd_scanner.py
```

### Comparing `rucio-consistency-1.0.1/setup.py` & `rucio-consistency-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     url = "https://github.com/rucio/consistency-enforcement",
     packages=['rucio_consistency', "rucio_consistency.scripts", "rucio_consistency.xrootd"],
     long_description="Common modules and scripts for Rucio consistency enforcement", #read('README'),
     zip_safe = False,
     install_requires=["sqlalchemy", "pythreader"],
     entry_points = {
         "console_scripts": [
+            "rce_update_stats = rucio_consistency.scripts.update_stats:main",
+            "rce_diffs = rucio_consistency.scripts.diffs:main",
             "rce_partition = rucio_consistency.scripts.partition:main",
             "rce_db_dump = rucio_consistency.scripts.db_dump:main",
             "rce_cmp5 = rucio_consistency.scripts.cmp5:main",
             "rce_cmp3 = rucio_consistency.scripts.cmp3:main",
             "rce_cmp2 = rucio_consistency.scripts.cmp2:main",
             "rce_scan = rucio_consistency.xrootd.xrootd_scanner:main"
         ]
```

