# Comparing `tmp/rucio-consistency-1.0.3.tar.gz` & `tmp/rucio-consistency-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.3.tar", last modified: Thu Apr 13 14:13:09 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.4.tar", last modified: Thu Apr 13 14:43:39 2023, max compression
```

## Comparing `rucio-consistency-1.0.3.tar` & `rucio-consistency-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:13:09.698893 rucio-consistency-1.0.3/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.3/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:13:09.698653 rucio-consistency-1.0.3/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.3/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:13:09.692596 rucio-consistency-1.0.3/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:13:09.697454 rucio-consistency-1.0.3/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9447 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/db_dump.py
--rw-r--r--   0 ivm        (501) staff       (20)     2276 2023-04-13 14:10:11.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/diffs.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.3/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.3/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 14:11:30.000000 rucio-consistency-1.0.3/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:13:09.698167 rucio-consistency-1.0.3/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.3/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.3/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:13:09.694622 rucio-consistency-1.0.3/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      885 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      437 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 14:13:09.000000 rucio-consistency-1.0.3/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 14:13:09.698953 rucio-consistency-1.0.3/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1455 2023-04-13 13:49:07.000000 rucio-consistency-1.0.3/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.337809 rucio-consistency-1.0.4/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.4/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:43:39.337569 rucio-consistency-1.0.4/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.4/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.332318 rucio-consistency-1.0.4/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.336215 rucio-consistency-1.0.4/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.4/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.4/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 14:43:23.000000 rucio-consistency-1.0.4/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.337092 rucio-consistency-1.0.4/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 14:43:39.334194 rucio-consistency-1.0.4/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 14:43:39.000000 rucio-consistency-1.0.4/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 14:43:39.337880 rucio-consistency-1.0.4/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.4/setup.py
```

### Comparing `rucio-consistency-1.0.3/LICENSE` & `rucio-consistency-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/cmplib.py` & `rucio-consistency-1.0.4/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/config.py` & `rucio-consistency-1.0.4/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/part.py` & `rucio-consistency-1.0.4/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/db_dump.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import getopt, os, time, re, gzip, json, traceback
 import sys, uuid
 
-from rucio_consistency import PartitionedList, DBConfig, CEConfiguration, Stats
-
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, Integer, String
 from sqlalchemy.orm import sessionmaker
 
 from sqlalchemy.dialects.postgresql import UUID, JSONB
 from sqlalchemy.dialects.oracle import RAW, CLOB
 from sqlalchemy.dialects.mysql import BINARY
 from sqlalchemy.types import TypeDecorator, CHAR, String
 from sqlalchemy.exc import ArgumentError
 
-Version = "1.2"
-
-t0 = time.time()
+from rucio_consistency import PartitionedList, DBConfig, CEConfiguration, Stats
 
-#from sqlalchemy import schema
+Version = "2.0"
 
 Usage = """
-%s [options] -c <config.yaml> <rse_name>
+python db_dump.py [options] -c <config.yaml> <rse_name>
     -c <config file> -- required
     -d <db config file> -- required - uses rucio.cfg format. Must contain "default" and "schema" under [databse]
     -v -- verbose
     -n <nparts>
     -f <state>:<prefix> -- filter files with given state to the files set with prefix
         state can be either combination of capital letters or "*" 
         can be repeated  ( -f A:/path1 -f CD:/path2 )
         use "*" for state to send all the files to the output set ( -f *:/path )
     -l -- include more columns, otherwise physical path only, automatically on if -a is used
     -z -- produce gzipped output
     -s <stats file> -- write stats into JSON file
        -S <key> -- add dump stats to stats under the key
+    -r <file>   -- file counts per root and store in the file as JSON structure with file counts
     -m <N files> -- stop after N files
 """
 
+t0 = time.time()
+
 class DBDumpConfiguration(CEConfiguration):
 
     def __init__(self, rse, *params, **agrs):
         CEConfiguration.__init__(self, rse, *params, **agrs)
         self.DBDumpPathRoot = self.dbdump_param(rse, "path_root", "/")
 
     def __getitem__(self, name):
         return self.dbdump_param(self.RSE, name, required=True)
 
+#from sqlalchemy import schema
+
 class GUID(TypeDecorator):
     """
     Platform-independent GUID type.
 
     Uses PostgreSQL's UUID type,
     uses Oracle's RAW type,
     uses MySQL's BINARY type,
@@ -92,40 +93,40 @@
             return str(uuid.UUID(bytes=value)).replace('-', '').lower()
         elif dialect.name == 'mysql':
             return str(uuid.UUID(bytes=value)).replace('-', '').lower()
         else:
             return str(uuid.UUID(value)).replace('-', '').lower()
 
 def main():
-    opts, args = getopt.getopt(sys.argv[1:], "f:c:ln:vd:s:S:zm:")
+    opts, args = getopt.getopt(sys.argv[1:], "f:c:ln:vd:s:S:zm:r:")
 
     filters = {}
     all_states = set()
     for opt, val in opts:
         if opt == '-f':
             states, prefix = val.split(':')
             filters[states] = prefix
             all_states |= set(states)
 
     opts = dict(opts)
 
     if not args or (not "-c" in opts and not "-d" in opts):
-        cmd = sys.argv[0].rsplit("/", 1)[-1]
-        if cmd.endswith(".py"):
-            cmd = "python " + cmd
-        print(Usage % (cmd,))
-        sys.exit(2)
+            print (Usage)
+            sys.exit(2)
 
     verbose = "-v" in opts
     long_output = "-l" in opts
     out_prefix = opts.get("-o")
     zout = "-z" in opts
     stats_file = opts.get("-s")
     stats_key = opts.get("-S", "db_dump")
     stop_after = int(opts.get("-m", 0)) or None
+    root_file_counts_out = opts.get("-r")
+    if root_file_counts_out:
+        root_file_counts_out = open(root_file_counts_out, "w")
 
     rse_name = args[0]
 
     if "-d" in opts:
         dbconfig = DBConfig.from_cfg(opts["-d"])
     else:
         dbconfig = DBConfig.from_yaml(opts["-c"])
@@ -216,29 +217,36 @@
                 replicas = replicas.filter(Replica.state.in_(list(all_states)))
         dirs = set()
         n = 0
         filter_re = None    #config.dbdump_param(rse, "filter")
         ignored_files = 0
         if filter_re:
             filter_re = re.compile(filter_re)
+        root_file_counts = {root: 0 for root in config.RootList}
         for r in replicas:
             path = r.name
             state = r.state
 
             if not path.startswith(subdir):
                     continue
 
             if filter_re is not None:
                 if not filter_re.search(path):
                     continue
             
             if any(path.startswith(ignore_prefix) for ignore_prefix in ignore_list):
                 ignored_files += 1
                 continue
-            
+
+            for r, n in list(root_file_counts.items()):
+                prefix = r + '/' if not r.endswith('/') else r
+                if path.startswith(prefix):
+                    root_file_counts[r] = n + 1
+                    break
+
             words = path.rsplit("/", 1)
             if len(words) == 1:
                     dirp = "/"
             else:
                     dirp = words[0]
             dirs.add(dirp)
 
@@ -280,10 +288,13 @@
                 "end_time":t1,
                 "files":n,
                 "ignored_files":ignored_files,
                 "elapsed":t1-t0,
                 "directories":len(dirs),
                 "ignore_list":ignore_list
             })
+        if root_file_counts_out is not None:
+            root_file_counts_out.write(json.dumps(root_file_counts, indent=4, sort_keys=True))
+            root_file_counts_out.close()
             
 if __name__ == "__main__":
-        main()
+    main()
```

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.0.4/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/stats.py` & `rucio-consistency-1.0.4/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.0.4/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.3/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.4/rucio_consistency.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,13 +15,12 @@
 rucio_consistency.egg-info/not-zip-safe
 rucio_consistency.egg-info/requires.txt
 rucio_consistency.egg-info/top_level.txt
 rucio_consistency/scripts/cmp2.py
 rucio_consistency/scripts/cmp3.py
 rucio_consistency/scripts/cmp5.py
 rucio_consistency/scripts/db_dump.py
-rucio_consistency/scripts/diffs.py
 rucio_consistency/scripts/partition.py
 rucio_consistency/scripts/update_stats.py
 rucio_consistency/xrootd/__init__.py
 rucio_consistency/xrootd/xrootd_client.py
 rucio_consistency/xrootd/xrootd_scanner.py
```

### Comparing `rucio-consistency-1.0.3/setup.py` & `rucio-consistency-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     packages=['rucio_consistency', "rucio_consistency.scripts", "rucio_consistency.xrootd"],
     long_description="Common modules and scripts for Rucio consistency enforcement", #read('README'),
     zip_safe = False,
     install_requires=["sqlalchemy", "pythreader"],
     entry_points = {
         "console_scripts": [
             "rce_update_stats = rucio_consistency.scripts.update_stats:main",
-            "rce_diffs = rucio_consistency.scripts.diffs:main",
             "rce_partition = rucio_consistency.scripts.partition:main",
             "rce_db_dump = rucio_consistency.scripts.db_dump:main",
             "rce_cmp5 = rucio_consistency.scripts.cmp5:main",
             "rce_cmp3 = rucio_consistency.scripts.cmp3:main",
             "rce_cmp2 = rucio_consistency.scripts.cmp2:main",
             "rce_scan = rucio_consistency.xrootd.xrootd_scanner:main"
         ]
```

