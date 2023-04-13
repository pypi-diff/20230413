# Comparing `tmp/eisenmp_examples-0.3.1.tar.gz` & `tmp/eisenmp_examples-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.3.1.tar", last modified: Thu Apr 13 11:12:10 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.4.tar", last modified: Thu Apr 13 16:32:09 2023, max compression
```

## Comparing `eisenmp_examples-0.3.1.tar` & `eisenmp_examples-0.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.085816 eisenmp_examples-0.3.1/
--rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/LICENSE.rst
--rw-rw-rw-   0        0        0      230 2023-04-13 09:39:59.000000 eisenmp_examples-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4330 2023-04-13 11:12:10.085816 eisenmp_examples-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.038999 eisenmp_examples-0.3.1/eisenmp_examples/
--rw-rw-rw-   0        0        0      344 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/__init__.py
--rw-rw-rw-   0        0        0     2141 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0    10119 2023-04-12 12:21:58.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     6153 2023-04-12 23:19:46.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     3330 2023-04-12 12:30:58.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     6573 2023-04-13 10:28:16.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     8751 2023-04-11 18:20:30.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     4398 2023-04-13 10:19:31.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     7918 2023-04-12 22:39:31.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     6609 2023-04-13 10:08:43.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.069235 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/
--rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/__init__.py
--rw-rw-rw-   0        0        0     1835 2023-04-13 10:10:13.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_download.py
--rw-rw-rw-   0        0        0     4053 2023-04-13 10:11:12.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_search.py
--rw-rw-rw-   0        0        0     6183 2023-04-11 20:23:47.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.083868 eisenmp_examples-0.3.1/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0     3812 2023-04-12 08:03:45.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     5300 2023-04-12 15:48:27.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3621 2023-04-12 12:10:17.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     4412 2023-04-12 09:45:05.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     1920 2023-04-12 12:31:59.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     2382 2023-04-12 12:29:05.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     1571 2023-04-11 07:55:37.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.061435 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4330 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1333 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 11:09:00.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1064 2023-04-13 11:06:28.000000 eisenmp_examples-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-13 11:12:10.089717 eisenmp_examples-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.618106 eisenmp_examples-0.4/
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/LICENSE.rst
+-rw-rw-rw-   0        0        0      230 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4328 2023-04-13 16:32:09.618106 eisenmp_examples-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3581 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.469852 eisenmp_examples-0.4/eisenmp_examples/
+-rw-rw-rw-   0        0        0      344 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    10180 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6212 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3389 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6573 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4457 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     8104 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6670 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.537151 eisenmp_examples-0.4/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4139 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     6183 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.616156 eisenmp_examples-0.4/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/__init__.py
+-rw-rw-rw-   0        0        0     3812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     5300 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3621 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     4412 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     1920 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     2382 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.509845 eisenmp_examples-0.4/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4328 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 16:32:08.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1064 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-13 16:32:09.621035 eisenmp_examples-0.4/setup.cfg
```

### Comparing `eisenmp_examples-0.3.1/LICENSE` & `eisenmp_examples-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/LICENSE.rst` & `eisenmp_examples-0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/PKG-INFO` & `eisenmp_examples-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.3.1
+Version: 0.4
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.3.1/README.md` & `eisenmp_examples-0.4/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/cmd.py` & `eisenmp_examples-0.4/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/database.db` & `eisenmp_examples-0.4/eisenmp_examples/database.db`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 - worker must have the 'toolbox' as arg in entry function (arg count 1)
 - path to worker module and the entry function reference, all are str
 
 """
 import os
 import io
 import time
+import platform
 from zipfile import ZipFile
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 try:
     from eisenmp.utils_exa.eisenmp_search import SearchStr
@@ -63,15 +64,16 @@
         # Multiprocess vars - override default
         # self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
         # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         # self.NUM_ROWS = 2  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # Worker part - toolbox vars survive multiple worker calls
         self.multi_tool_get = None  # custom var to allow only one download of MULTI_TOOL; init later in this example
         self.MULTI_TOOL = None  # pre-defined toolbox.MULTI_TOOL can host the dict from mp_tools_q
         self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
 
         # custom
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_double_q.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_double_q.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - fake production of audio and video coding, is loop through to result dict
 - two processors work on different streams (src is same here, so what)
 
 """
 import os
 import threading
 import time
-
+import platform
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 dir_name = os.path.dirname(__file__)
 
 
 chunks_0 = [
@@ -87,15 +87,16 @@
         # Multiprocess vars - override default
         self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 3  # arbitrary num here
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULT_LABEL = 'fake production of audio and video coding for WHO studios'
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # work to do
         self.sleep_time = 20  # watchdog
         self.num_of_lists = 0  # worker lists done counter
 
         # vars lived before in worker module classes
         self.header_aud = None  # pre-defined, use in whole worker mod, save input list header to mark output header
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """See some examples,
 it's always the same process,
 you extend or switch off defaults
 
 """
 import os
 import time
-
+import platform
 import eisenmp
 
 
 class ModuleConfiguration:
     """
     You can use the class to have your variables available in the module.
 
@@ -30,15 +30,16 @@
         # Multiprocess vars - override default
         self.NUM_PROCS = 6  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULT_LABEL = 'No result, server blocks'  # pretty print as result header for RESULTS_PRINT
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
 
 modConf = ModuleConfiguration()  # Accessible in the module.
 
 
 def manager():
     """
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Python 3 server example
 # https://pythonbasics.org/webserver/
 # mod by 44xtc44
 
 import os
 import time
+import platform
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
 import eisenmp
 
 hostName = "localhost"
 serverPort = 12_000
 
@@ -61,15 +62,16 @@
         self.NUM_PROCS = 16  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
         # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # 'not enough work example', useless worker auto shutdown, the modules return False
         self.radio_name = None  # define to get it as key in 'modConf' dictionary and worker use 'toolbox.radio_name'
         self.radio_url = None
         self.sleep_time = 60  # if watchdog enabled, toolbox.sleep_time = 60
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 Multiple server on each CPU core, if server has that many cores.
 needs Flask_SQLAlchemy_Project_Template >=1.3
 """
 import os
 import time
-
+import platform
 import eisenmp
 
 
 class ModuleConfiguration:
     """
     You can use the class to have your variables available in the module.
 
@@ -39,15 +39,16 @@
 
         # Multiprocess vars - override default
         self.NUM_PROCS = 3  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         self.STOP_MSG_DISABLE = True  # module_loader leaves worker loop and waits for stop msg in mp_process_q
 
         # worker port groups, nailed on one cpu
         self.blue_lst = [0]  # one CPU core for blue list, if toolbox.kwargs['START_SEQUENCE_NUM'] in worker_blue_lst,
         self.yellow_lst = [1]  # one CPU core for yellow, process spawn num 1; (class ProcEnv 'run_proc -> core')
         self.green_lst = [2]
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_prime.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 This is NOT ADVISABLE and only to show the mechanics.
 Use a separate worker module to not import your 'Generator' imports twice.
 That is what the loader is for.
 """
 import os
 import time
-from math import isqrt
+import math
+import platform
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 dir_name = os.path.dirname(__file__)
 
 
@@ -42,15 +43,16 @@
         # Multiprocess vars - override default
         self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
         # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.NUM_ROWS = 42  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # custom part, write your own Attributes
         self.range_num = 10 ** 4  # got a target/max value and NUM_ROWS for each proc, can calc ETA est. time arrival
         self.INFO_THREAD_MAX = self.range_num  # target value for info thread to calculate % and ETA
         # self.INFO_ENABLE = True  # [baustelle]
         self.n = 10 ** 12  # ten with zero count, 10_000_000_000_000_000
         self.say_hello = 'Hello'  # just to show that worker can [read] all attributes of instance, in 'worker_prime()'
@@ -134,20 +136,22 @@
     primes = ''.join(str(prime_lst)) if len(prime_lst) else ''
     output_msg = f' ... Result {toolbox.WORKER_NAME} ... Prime {primes}'
     toolbox.mp_print_q.put(output_msg) if len(prime_lst) else None  # blocks the whole mp
 
 
 def is_prime(n: int) -> bool:
     """https://en.wikipedia.org/wiki/Primality_test
+
+    mod by 44xtc44, limit = int(math.sqrt(n)) , isqrt(n) is Python 3.8, package shall run 3.7
     """
     if n <= 3:
         return n > 1
     if n % 2 == 0 or n % 3 == 0:
         return False
-    limit = isqrt(n)
+    limit = int(math.sqrt(n))  # python 3.8 isqrt(n) humbug
     for i in range(5, limit + 1, 6):
         if n % i == 0 or n % (i + 2) == 0:
             return False
     return True
 
 
 def send_output(toolbox, prime_lst):
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_web_csv.py` & `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 We download a NZ government report and calculate the average of split lists.
 See URL. Try your own URL. They have a lot.
 """
 
 import os
 import csv
 import time
+import platform
 from io import TextIOWrapper
 from zipfile import ZipFile
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 try:
     from eisenmp.utils_exa.eisenmp_download import DownLoad
@@ -51,15 +52,16 @@
         self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 50_000  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
-        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        if platform.system() == 'Linux':
+            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # CSV part
         self.use_file_system = False  # False: download and unzip in mem; True must exist on fs ------------- SWITCH ---
         self.url = self.dl_url  # False 'use_file_system', URL of csv file
         self.zipped_filename = 'revised.csv'  # name of the uncompressed file in zip archive
         self.csv_col_name = 'value'  # CSV table column header
         self.sleep_time = 45  # watchdog module in 'worker_modules' list
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_download.py` & `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import io
 import zipfile
 from io import BytesIO
 
-import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
+try:
+    import eisenmp.utils_exa.eisenmp_utils as e_utils
+except ImportError:
+    import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
 
 
 class DownLoad:
     """If we have the response, we can read it at once or as a stream.
 
     """
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_search.py` & `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import itertools
 
-import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
+try:
+    import eisenmp.utils_exa.eisenmp_utils as e_utils
+except ImportError:
+    import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
 
 
 class SearchStr:
     """Hosts the dict to compare,
     and a 'search string shaker' generator.
 
     el cheapo goes brute force, but it shows the basics
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_utils.py` & `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_double.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.4/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.3.1
+Version: 0.4
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.3.1/eisenmp_examples.egg-info/SOURCES.txt` & `eisenmp_examples-0.4/eisenmp_examples.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 eisenmp_examples.egg-info/requires.txt
 eisenmp_examples.egg-info/top_level.txt
 eisenmp_examples.egg-info/zip-safe
 eisenmp_examples/utils_exa/__init__.py
 eisenmp_examples/utils_exa/eisenmp_download.py
 eisenmp_examples/utils_exa/eisenmp_search.py
 eisenmp_examples/utils_exa/eisenmp_utils.py
+eisenmp_examples/worker/__init__.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
 eisenmp_examples/worker/eisenmp_exa_wrk_double.py
 eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
 eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
 eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
```

### Comparing `eisenmp_examples-0.3.1/pyproject.toml` & `eisenmp_examples-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.3.1"
+version = "0.4"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "eisenmp multiprocess(or) example collection for server and mobiles"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
 requires-python = ">=3.7"
 
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable"
 ]
 dependencies = [
     "eisenmp",
```

