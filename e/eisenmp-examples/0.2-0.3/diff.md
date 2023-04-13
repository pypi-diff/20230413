# Comparing `tmp/eisenmp_examples-0.2.tar.gz` & `tmp/eisenmp_examples-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.2.tar", last modified: Tue Apr  4 15:03:16 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.3.tar", last modified: Thu Apr 13 09:40:17 2023, max compression
```

## Comparing `eisenmp_examples-0.2.tar` & `eisenmp_examples-0.3.tar`

### file list

```diff
@@ -1,61 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.898672 eisenmp_examples-0.2/
--rw-rw-rw-   0        0        0     1525 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/LICENSE.rst
--rw-rw-rw-   0        0        0      197 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2023-04-04 15:03:16.899644 eisenmp_examples-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.818692 eisenmp_examples-0.2/eisenmp_examples/
--rw-rw-rw-   0        0        0      344 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.857708 eisenmp_examples-0.2/eisenmp_examples/__pycache__/
--rw-rw-rw-   0        0        0      552 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7019 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_bruteforce.cpython-310.pyc
--rw-rw-rw-   0        0        0     3008 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_double_q.cpython-310.pyc
--rw-rw-rw-   0        0        0     3728 2023-04-04 15:00:23.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_each_flask_orm_srv_one_cpu.cpython-310.pyc
--rw-rw-rw-   0        0        0     4234 2023-04-04 15:00:23.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_entry.cpython-310.pyc
--rw-rw-rw-   0        0        0     5667 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_http.cpython-310.pyc
--rw-rw-rw-   0        0        0     4317 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_multi_srv_each_cpu.cpython-310.pyc
--rw-rw-rw-   0        0        0     4817 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_prime.cpython-310.pyc
--rw-rw-rw-   0        0        0     4862 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/__pycache__/eisenmp_exa_web_csv.cpython-310.pyc
--rw-rw-rw-   0        0        0     2141 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0     8986 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     4740 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     5164 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     4920 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     7910 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     6211 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     6363 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     5741 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.864537 eisenmp_examples-0.2/eisenmp_examples/utils/
--rw-rw-rw-   0        0        0        0 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.873308 eisenmp_examples-0.2/eisenmp_examples/utils/__pycache__/
--rw-rw-rw-   0        0        0      175 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2189 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/utils/__pycache__/eisenmp_download.cpython-310.pyc
--rw-rw-rw-   0        0        0     4658 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/utils/__pycache__/eisenmp_search.cpython-310.pyc
--rw-rw-rw-   0        0        0     6965 2023-04-04 15:00:22.000000 eisenmp_examples-0.2/eisenmp_examples/utils/__pycache__/eisenmp_utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     1831 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_download.py
--rw-rw-rw-   0        0        0     4049 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_search.py
--rw-rw-rw-   0        0        0     6143 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.885993 eisenmp_examples-0.2/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0        0 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.896720 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/
--rw-rw-rw-   0        0        0     2953 2023-04-04 15:01:15.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_bf_bruteforce.cpython-310.pyc
--rw-rw-rw-   0        0        0     3812 2023-04-04 15:01:11.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_bf_reduce.cpython-310.pyc
--rw-rw-rw-   0        0        0     2678 2023-04-04 15:00:43.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_csv.cpython-310.pyc
--rw-rw-rw-   0        0        0     2330 2023-04-04 15:00:59.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_double.cpython-310.pyc
--rw-rw-rw-   0        0        0     2078 2023-04-04 15:00:43.000000 eisenmp_examples-0.2/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_watchdog.cpython-310.pyc
--rw-rw-rw-   0        0        0     3390 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     4717 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3202 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     2819 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     1571 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:03:16.839179 eisenmp_examples-0.2/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4328 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2470 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-04 15:03:16.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-04 14:59:47.000000 eisenmp_examples-0.2/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1062 2023-04-04 14:59:10.000000 eisenmp_examples-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-04 15:03:16.901597 eisenmp_examples-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/
+-rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/LICENSE.rst
+-rw-rw-rw-   0        0        0      230 2023-04-13 09:39:59.000000 eisenmp_examples-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4328 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3581 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.360058 eisenmp_examples-0.3/eisenmp_examples/
+-rw-rw-rw-   0        0        0      344 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    10119 2023-04-12 12:21:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6153 2023-04-12 23:19:46.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3330 2023-04-12 12:30:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6554 2023-04-12 16:14:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8751 2023-04-11 18:20:30.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4398 2023-04-12 14:44:17.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     7918 2023-04-12 22:39:31.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6673 2023-04-12 15:45:46.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.391310 eisenmp_examples-0.3/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/__init__.py
+-rw-rw-rw-   0        0        0     1826 2023-04-11 08:15:22.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4044 2023-04-11 08:15:22.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     6183 2023-04-11 20:23:47.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/__init__.py
+-rw-rw-rw-   0        0        0     3390 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     4717 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3391 2023-04-10 18:02:06.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     2802 2023-04-10 18:02:06.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     1984 2023-04-10 17:01:51.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.391310 eisenmp_examples-0.3/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4328 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1307 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 09:37:43.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1062 2023-04-12 22:56:11.000000 eisenmp_examples-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/setup.cfg
```

### Comparing `eisenmp_examples-0.2/LICENSE` & `eisenmp_examples-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/LICENSE.rst` & `eisenmp_examples-0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/PKG-INFO` & `eisenmp_examples-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.2
+Version: 0.3
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.2/README.md` & `eisenmp_examples-0.3/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples/cmd.py` & `eisenmp_examples-0.3/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples/database.db` & `eisenmp_examples-0.3/eisenmp_examples/database.db`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 """
 import os
 import io
 import time
 from zipfile import ZipFile
 
 import eisenmp
-from eisenmp_examples.utils.eisenmp_search import SearchStr
-from eisenmp_examples.utils.eisenmp_download import DownLoad
+import eisenmp.utils.eisenmp_utils as e_utils
+
+try:
+    from eisenmp.utils_exa.eisenmp_search import SearchStr
+    from eisenmp.utils_exa.eisenmp_download import DownLoad
+except ImportError:
+    import eisenmp_examples
+    from eisenmp_examples.utils_exa.eisenmp_search import SearchStr
+    from eisenmp_examples.utils_exa.eisenmp_download import DownLoad
 
 dir_name = os.path.dirname(__file__)  # absolute dir path
 
 
 class ModuleConfiguration:
     """
     - Loading the worker module has nothing to do with name resolution in 'this' module.
@@ -49,22 +56,27 @@
             'words.txt',
     }
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = []  # init for kwargs/toolbox, 'worker_module_set'
 
-        self.num_cores = None  # number of process we want, default is None; one proc/CPU core
-        self.num_rows = 500  # workload for each proc per cycle, can make the difference
-        self.store_result = True  # False: no result in lists or dicts as end result
-
-        # Worker part
-        self.multi_tool_get = None  # True: blocks Worker as long as no tool is in the mp_tools_q
-        self.multi_tool = None  # informational: toolbox.multi_tool can host the dict from mp_tools_q
-        self.info_td_max = None  # target value for info thread to calculate % and ETA if 'enable_info' set
+        # Multiprocess vars - override default
+        # self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
+        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
+        # self.NUM_ROWS = 2  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
+        self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
+        self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+
+        # Worker part - toolbox vars survive multiple worker calls
+        self.multi_tool_get = None  # custom var to allow only one download of MULTI_TOOL; init later in this example
+        self.MULTI_TOOL = None  # pre-defined toolbox.MULTI_TOOL can host the dict from mp_tools_q
+        self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
 
         # custom
         self.use_file_system = False  # False: download and unzip in mem        ------------ SWITCH --------------------
         self.result_lbl = None  # set by caller
         self.num_lists = 0  # add one for each list done, print out worker
         self.lowercase = True
         self.url = None  # 'use_file_system' False, URL of csv file
@@ -94,34 +106,34 @@
     - (B) len(String) >=  11, Reduce a dictionary len(str) condensed list and count characters.
     """
     pass
     modConf.str_permutation = searchStr.search_string
     if modConf.lowercase:
         modConf.str_permutation = modConf.str_permutation.lower()
     searchStr.create_key_word_val_none_shrink(lowercase=modConf.lowercase)  # dict, remove words != len(search str)
-    modConf.info_td_max = len(searchStr.words_dict)  # info thread calc rows done and len
+    modConf.INFO_THREAD_MAX = len(searchStr.words_dict)  # info thread calc rows done and len
 
     # ---------- selection of generator function reference ----------
     brute_force = True if len(modConf.str_permutation) <= 10 else False
-    function_ref = mp_brute_force if brute_force else mp_reduce
+    function_ref = mp_brute_force if brute_force else mp_reduce  # decide which function to call
     worker_module_set(function_ref)
 
     msg_b, msg_r = f'\n\t[BRUTE_FORCE]\t{modConf.str_permutation}', f'\n\t[LIST_REDUCTION]\t{modConf.str_permutation}'
     msg = msg_b if function_ref == mp_brute_force else msg_r
     print(msg)
 
     generator = function_ref(searchStr)
     words_dict = searchStr.words_dict if function_ref == mp_brute_force else None
 
     mP = eisenmp.Mp()
     mP.start(**modConf.__dict__)
     if brute_force:
         for _ in mP.proc_list:
             mP.mp_tools_q.put(words_dict)
-    mP.run_q_feeder(generator=generator)
+    mP.run_q_feeder(generator=generator, input_q=mP.mp_input_q)
 
 
 def worker_module_set(function_ref):
     """which worker module and function to load"""
     modConf.worker_modules = []  # del existing
 
     if function_ref == mp_brute_force:
@@ -202,15 +214,16 @@
 
 
 def wordlists_in_memory(downloader):
     """Open zip archive and load one file 'zipped_filename'
     Return as text.
     """
     archive = downloader.unzip_mem()
-    with io.TextIOWrapper(archive.open(modConf.zipped_filename, 'r')) as file:
+    # text files are all utf-8 encoded, py try open cp1252 on my windows
+    with io.TextIOWrapper(archive.open(modConf.zipped_filename, 'r'), encoding="UTF-8") as file:
         txt_lst = file.readlines()
     return txt_lst
 
 
 def wordlist_download(downloader):
     """Store response object in downloader instance.
     We could show dots during download, or open in binary, or csv, or ....
@@ -220,28 +233,35 @@
     print(downloader.url)
     downloader.load_url()
 
 
 def main():
     """
     """
-    str_list_alphabet_salad = ['EEEFFIKORRS', 'AMGNO', 'DIKKLOOR', 'BEEINNRST',
-                               'AACEFHKLMSS', 'CEEHNNRST', 'EEHINORST'
-                               'EEEFFIKORRS', 'CFHHILORRS'
-                               ]
+    str_list_alphabet_salad = [
+        'AMGNO',
+        'AACEFHKLMSS',
+        'DIKKLOOR', 'BEEINNRST',
+        'CEEHNNRST', 'EEHINORST',
+        'EEEFFIKORRS', 'CFHHILORRS'
+    ]
 
     start = time.perf_counter()
 
+    res_coll_dct = {}
     load_lang_word_dict()
-    for string in str_list_alphabet_salad:
+    for idx, string in enumerate(str_list_alphabet_salad):
         searchStr.search_string = string
         modConf.result_lbl = string
         modConf.lowercase = True
         mp_start_raid()
-
-        time.sleep(1)
+        msg_result = e_utils.Result.result_dict
+        res_coll_dct[idx] = msg_result
+        print(msg_result)
+        time.sleep(.5)
 
     print(f'BF Time in sec: {round((time.perf_counter() - start))}')
+    return res_coll_dct
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,308 +1,410 @@
 00000000: 2320 5079 7468 6f6e 2033 2073 6572 7665  # Python 3 serve
 00000010: 7220 6578 616d 706c 650d 0a23 2068 7474  r example..# htt
 00000020: 7073 3a2f 2f70 7974 686f 6e62 6173 6963  ps://pythonbasic
 00000030: 732e 6f72 672f 7765 6273 6572 7665 722f  s.org/webserver/
 00000040: 0d0a 2320 6d6f 6420 6279 2034 3478 7463  ..# mod by 44xtc
-00000050: 3434 0d0a 0d0a 696d 706f 7274 206a 736f  44....import jso
-00000060: 6e0d 0a69 6d70 6f72 7420 7469 6d65 0d0a  n..import time..
-00000070: 6672 6f6d 2068 7474 702e 7365 7276 6572  from http.server
-00000080: 2069 6d70 6f72 7420 4261 7365 4854 5450   import BaseHTTP
-00000090: 5265 7175 6573 7448 616e 646c 6572 2c20  RequestHandler, 
-000000a0: 4854 5450 5365 7276 6572 0d0a 0d0a 696d  HTTPServer....im
-000000b0: 706f 7274 2065 6973 656e 6d70 5f65 7861  port eisenmp_exa
-000000c0: 6d70 6c65 730d 0a0d 0a68 6f73 744e 616d  mples....hostNam
-000000d0: 6520 3d20 226c 6f63 616c 686f 7374 220d  e = "localhost".
-000000e0: 0a73 6572 7665 7250 6f72 7420 3d20 3132  .serverPort = 12
-000000f0: 5f33 3231 0d0a 0d0a 0d0a 636c 6173 7320  _321......class 
-00000100: 4d65 6e75 3a0d 0a0d 0a20 2020 2065 7861  Menu:....    exa
-00000110: 6d70 6c65 5f6d 656e 7520 3d20 5b0d 0a20  mple_menu = [.. 
-00000120: 2020 2020 2020 2027 5b73 696e 676c 6520         '[single 
-00000130: 7368 6f74 5d20 4d75 6c74 6970 6c65 2046  shot] Multiple F
-00000140: 6c61 736b 2073 6572 7665 7220 696e 2065  lask server in e
-00000150: 6163 6820 7072 6f63 6573 7365 7320 2d20  ach processes - 
-00000160: 7368 6172 6520 6120 4442 272c 0d0a 2020  share a DB',..  
-00000170: 2020 2020 2020 275b 7369 6e67 6c65 2073        '[single s
-00000180: 686f 745d 204f 6e65 2046 6c61 736b 2073  hot] One Flask s
-00000190: 6572 7665 7220 6f6e 2045 7665 7279 2070  erver on Every p
-000001a0: 726f 6365 7373 202d 2073 6861 7265 2061  rocess - share a
-000001b0: 2044 4227 2c0d 0a20 2020 2020 2020 2027   DB',..        '
-000001c0: 5072 696d 6520 4e75 6d62 6572 2063 616c  Prime Number cal
-000001d0: 6375 6c61 7469 6f6e 272c 0d0a 2020 2020  culation',..    
-000001e0: 2020 2020 2757 6562 2043 5356 206c 6172      'Web CSV lar
-000001f0: 6765 206c 6973 7420 6361 6c63 756c 6174  ge list calculat
-00000200: 696f 6e27 2c0d 0a20 2020 2020 2020 2027  ion',..        '
-00000210: 4f6e 6520 7369 6d70 6c65 2068 7474 7020  One simple http 
-00000220: 7365 7276 6572 2070 7265 7365 6e74 7320  server presents 
-00000230: 6120 7261 6469 6f20 6f6e 2065 7665 7279  a radio on every
-00000240: 2070 726f 6365 7373 272c 0d0a 2020 2020   process',..    
-00000250: 2020 2020 2754 776f 2051 7565 7565 7320      'Two Queues 
-00000260: 6665 6420 6174 206f 6e63 6527 2c0d 0a20  fed at once',.. 
-00000270: 2020 2020 2020 2027 4272 7574 6520 666f         'Brute fo
-00000280: 7263 6520 6174 7461 636b 2077 6974 6820  rce attack with 
-00000290: 6469 6374 696f 6e61 7279 2061 6e64 2069  dictionary and i
-000002a0: 7465 7274 6f6f 6c73 2067 656e 6572 6174  tertools generat
-000002b0: 6f72 272c 0d0a 2020 2020 5d0d 0a0d 0a20  or',..    ].... 
-000002c0: 2020 2065 7861 5f74 706c 5f6c 7374 203d     exa_tpl_lst =
-000002d0: 205b 0d0a 2020 2020 2020 2020 2830 2c20   [..        (0, 
-000002e0: 6578 616d 706c 655f 6d65 6e75 5b30 5d2c  example_menu[0],
-000002f0: 2065 6973 656e 6d70 5f65 7861 6d70 6c65   eisenmp_example
-00000300: 732e 6569 7365 6e6d 705f 6578 615f 6d75  s.eisenmp_exa_mu
-00000310: 6c74 695f 7372 765f 6561 6368 5f63 7075  lti_srv_each_cpu
-00000320: 2e6d 6169 6e29 2c0d 0a20 2020 2020 2020  .main),..       
-00000330: 2028 312c 2065 7861 6d70 6c65 5f6d 656e   (1, example_men
-00000340: 755b 315d 2c20 6569 7365 6e6d 705f 6578  u[1], eisenmp_ex
-00000350: 616d 706c 6573 2e65 6973 656e 6d70 5f65  amples.eisenmp_e
-00000360: 7861 5f65 6163 685f 666c 6173 6b5f 6f72  xa_each_flask_or
-00000370: 6d5f 7372 765f 6f6e 655f 6370 752e 6d61  m_srv_one_cpu.ma
-00000380: 696e 292c 0d0a 2020 2020 2020 2020 2832  in),..        (2
-00000390: 2c20 6578 616d 706c 655f 6d65 6e75 5b32  , example_menu[2
-000003a0: 5d2c 2065 6973 656e 6d70 5f65 7861 6d70  ], eisenmp_examp
-000003b0: 6c65 732e 6569 7365 6e6d 705f 6578 615f  les.eisenmp_exa_
-000003c0: 7072 696d 652e 6d61 696e 292c 0d0a 2020  prime.main),..  
-000003d0: 2020 2020 2020 2833 2c20 6578 616d 706c        (3, exampl
-000003e0: 655f 6d65 6e75 5b33 5d2c 2065 6973 656e  e_menu[3], eisen
-000003f0: 6d70 5f65 7861 6d70 6c65 732e 6569 7365  mp_examples.eise
-00000400: 6e6d 705f 6578 615f 7765 625f 6373 762e  nmp_exa_web_csv.
-00000410: 6d61 696e 292c 0d0a 2020 2020 2020 2020  main),..        
-00000420: 2834 2c20 6578 616d 706c 655f 6d65 6e75  (4, example_menu
-00000430: 5b34 5d2c 2065 6973 656e 6d70 5f65 7861  [4], eisenmp_exa
-00000440: 6d70 6c65 732e 6569 7365 6e6d 705f 6578  mples.eisenmp_ex
-00000450: 615f 6874 7470 2e6d 6169 6e29 2c0d 0a20  a_http.main),.. 
-00000460: 2020 2020 2020 2028 352c 2065 7861 6d70         (5, examp
-00000470: 6c65 5f6d 656e 755b 355d 2c20 6569 7365  le_menu[5], eise
-00000480: 6e6d 705f 6578 616d 706c 6573 2e65 6973  nmp_examples.eis
-00000490: 656e 6d70 5f65 7861 5f64 6f75 626c 655f  enmp_exa_double_
-000004a0: 712e 6d61 696e 292c 0d0a 2020 2020 2020  q.main),..      
-000004b0: 2020 2836 2c20 6578 616d 706c 655f 6d65    (6, example_me
-000004c0: 6e75 5b36 5d2c 2065 6973 656e 6d70 5f65  nu[6], eisenmp_e
-000004d0: 7861 6d70 6c65 732e 6569 7365 6e6d 705f  xamples.eisenmp_
-000004e0: 6578 615f 6272 7574 6566 6f72 6365 2e6d  exa_bruteforce.m
-000004f0: 6169 6e29 0d0a 2020 2020 5d0d 0a0d 0a0d  ain)..    ].....
-00000500: 0a64 6566 2072 756e 5f68 7474 7028 293a  .def run_http():
-00000510: 0d0a 2020 2020 2222 2242 6c6f 636b 6564  ..    """Blocked
-00000520: 2c20 6e6f 206c 6f6f 7020 6865 7265 0d0a  , no loop here..
-00000530: 2020 2020 2222 220d 0a20 2020 2067 6c6f      """..    glo
-00000540: 6261 6c20 7365 7276 6572 506f 7274 0d0a  bal serverPort..
-00000550: 0d0a 2020 2020 7765 6253 6572 7665 7220  ..    webServer 
-00000560: 3d20 4854 5450 5365 7276 6572 2828 686f  = HTTPServer((ho
-00000570: 7374 4e61 6d65 2c20 7365 7276 6572 506f  stName, serverPo
-00000580: 7274 292c 204d 7953 6572 7665 7229 0d0a  rt), MyServer)..
-00000590: 0d0a 2020 2020 7072 696e 7428 6622 4578  ..    print(f"Ex
-000005a0: 616d 706c 6573 2068 7474 703a 2f2f 2573  amples http://%s
-000005b0: 3a25 7322 2025 2028 686f 7374 4e61 6d65  :%s" % (hostName
-000005c0: 2c20 7365 7276 6572 506f 7274 2929 0d0a  , serverPort))..
-000005d0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000005e0: 2020 7765 6253 6572 7665 722e 7365 7276    webServer.serv
-000005f0: 655f 666f 7265 7665 7228 290d 0a20 2020  e_forever()..   
-00000600: 2065 7863 6570 7420 4b65 7962 6f61 7264   except Keyboard
-00000610: 496e 7465 7272 7570 743a 0d0a 2020 2020  Interrupt:..    
-00000620: 2020 2020 7061 7373 0d0a 2020 2020 7765      pass..    we
-00000630: 6253 6572 7665 722e 7365 7276 6572 5f63  bServer.server_c
-00000640: 6c6f 7365 2829 0d0a 2020 2020 7072 696e  lose()..    prin
-00000650: 7428 2253 6572 7665 7220 7374 6f70 7065  t("Server stoppe
-00000660: 642e 2229 0d0a 0d0a 0d0a 636c 6173 7320  d.")......class 
-00000670: 4d79 5365 7276 6572 2842 6173 6548 5454  MyServer(BaseHTT
-00000680: 5052 6571 7565 7374 4861 6e64 6c65 7229  PRequestHandler)
-00000690: 3a0d 0a0d 0a20 2020 2064 6566 2064 6f5f  :....    def do_
-000006a0: 504f 5354 2873 656c 6629 3a0d 0a20 2020  POST(self):..   
-000006b0: 2020 2020 2022 2222 2222 220d 0a20 2020       """"""..   
-000006c0: 2020 2020 2023 2070 7269 6e74 2873 656c       # print(sel
-000006d0: 662e 6865 6164 6572 7329 0d0a 2020 2020  f.headers)..    
-000006e0: 2020 2020 6c65 6e67 7468 203d 2069 6e74      length = int
-000006f0: 2873 656c 662e 6865 6164 6572 732e 6765  (self.headers.ge
-00000700: 745f 616c 6c28 2763 6f6e 7465 6e74 2d6c  t_all('content-l
-00000710: 656e 6774 6827 295b 305d 290d 0a20 2020  ength')[0])..   
-00000720: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
-00000730: 6865 6164 6572 732e 6765 745f 616c 6c28  headers.get_all(
-00000740: 2763 6f6e 7465 6e74 2d6c 656e 6774 6827  'content-length'
-00000750: 2929 0d0a 2020 2020 2020 2020 6461 7461  ))..        data
-00000760: 5f73 7472 696e 6720 3d20 7365 6c66 2e72  _string = self.r
-00000770: 6669 6c65 2e72 6561 6428 6c65 6e67 7468  file.read(length
-00000780: 290d 0a20 2020 2020 2020 2065 7861 6d70  )..        examp
-00000790: 6c65 5f66 756e 203d 204d 656e 752e 6578  le_fun = Menu.ex
-000007a0: 615f 7470 6c5f 6c73 745b 696e 7428 6461  a_tpl_lst[int(da
-000007b0: 7461 5f73 7472 696e 6729 5d5b 325d 0d0a  ta_string)][2]..
-000007c0: 2020 2020 2020 2020 6578 616d 706c 655f          example_
-000007d0: 6675 6e28 290d 0a20 2020 2020 2020 2070  fun()..        p
-000007e0: 7269 6e74 2864 6174 615f 7374 7269 6e67  rint(data_string
-000007f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000800: 7365 6e64 5f72 6573 706f 6e73 6528 3230  send_response(20
-00000810: 3029 0d0a 2020 2020 2020 2020 2320 7365  0)..        # se
-00000820: 6c66 2e73 656e 645f 6865 6164 6572 2822  lf.send_header("
-00000830: 436f 6e74 656e 742d 7479 7065 222c 2022  Content-type", "
-00000840: 7465 7874 2f70 6c61 696e 2229 0d0a 2020  text/plain")..  
-00000850: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00000860: 6865 6164 6572 2827 436f 6e74 656e 742d  header('Content-
-00000870: 5479 7065 272c 2027 6170 706c 6963 6174  Type', 'applicat
-00000880: 696f 6e2f 6a73 6f6e 2729 0d0a 2020 2020  ion/json')..    
-00000890: 2020 2020 7365 6c66 2e65 6e64 5f68 6561      self.end_hea
-000008a0: 6465 7273 2829 0d0a 2020 2020 2020 2020  ders()..        
-000008b0: 7365 6c66 2e66 6c75 7368 5f68 6561 6465  self.flush_heade
-000008c0: 7273 2829 0d0a 2020 2020 2020 2020 6a73  rs()..        js
-000008d0: 6f6e 5f73 7472 696e 6720 3d20 6a73 6f6e  on_string = json
-000008e0: 2e64 756d 7073 2873 7472 2864 6174 615f  .dumps(str(data_
-000008f0: 7374 7269 6e67 2929 2020 2320 6a75 7374  string))  # just
-00000900: 2066 6f72 2074 6865 2073 616b 6520 6f66   for the sake of
-00000910: 206d 7920 6172 740d 0a20 2020 2020 2020   my art..       
-00000920: 2073 656c 662e 7766 696c 652e 7772 6974   self.wfile.writ
-00000930: 6528 6279 7465 7328 6a73 6f6e 5f73 7472  e(bytes(json_str
-00000940: 696e 672c 2022 7574 662d 3822 2929 0d0a  ing, "utf-8"))..
-00000950: 0d0a 2020 2020 6465 6620 646f 5f47 4554  ..    def do_GET
-00000960: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000970: 2073 656c 662e 7365 6e64 5f72 6573 706f   self.send_respo
-00000980: 6e73 6528 3230 3029 0d0a 2020 2020 2020  nse(200)..      
-00000990: 2020 7365 6c66 2e73 656e 645f 6865 6164    self.send_head
-000009a0: 6572 2822 436f 6e74 656e 742d 7479 7065  er("Content-type
-000009b0: 222c 2022 7465 7874 2f68 746d 6c22 290d  ", "text/html").
-000009c0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-000009d0: 645f 6865 6164 6572 7328 290d 0a0d 0a20  d_headers().... 
-000009e0: 2020 2020 2020 2063 656e 7465 7220 3d20         center = 
-000009f0: 2274 6578 742d 616c 6967 6e3a 6365 6e74  "text-align:cent
-00000a00: 6572 3b22 0d0a 2020 2020 2020 2020 6272  er;"..        br
-00000a10: 6f77 6e20 3d20 2263 6f6c 6f72 3a62 726f  own = "color:bro
-00000a20: 776e 3b66 6f6e 742d 6661 6d69 6c79 3a52  wn;font-family:R
-00000a30: 6f62 6f74 6f3b 220d 0a20 2020 2020 2020  oboto;"..       
-00000a40: 2062 6c61 636b 203d 2022 636f 6c6f 723a   black = "color:
-00000a50: 626c 6163 6b3b 666f 6e74 2d66 616d 696c  black;font-famil
-00000a60: 793a 526f 626f 746f 3b66 6f6e 742d 7765  y:Roboto;font-we
-00000a70: 6967 6874 3a37 3030 3b22 0d0a 2020 2020  ight:700;"..    
-00000a80: 2020 2020 666c 6578 5f6f 7574 6572 203d      flex_outer =
-00000a90: 2022 6469 7370 6c61 793a 2066 6c65 783b   "display: flex;
-00000aa0: 636f 6c6f 723a 6272 6f77 6e3b 666f 6e74  color:brown;font
-00000ab0: 2d66 616d 696c 793a 526f 626f 746f 3b66  -family:Roboto;f
-00000ac0: 6f6e 742d 7765 6967 6874 3a36 3030 3b22  ont-weight:600;"
-00000ad0: 0d0a 2020 2020 2020 2020 666c 6578 5f6d  ..        flex_m
-00000ae0: 6964 203d 2022 6469 7370 6c61 793a 2066  id = "display: f
-00000af0: 6c65 783b 666c 6578 2d64 6972 6563 7469  lex;flex-directi
-00000b00: 6f6e 3a20 636f 6c75 6d6e 3b6d 6172 6769  on: column;margi
-00000b10: 6e3a 2061 7574 6f3b 220d 0a0d 0a20 2020  n: auto;"....   
-00000b20: 2020 2020 2064 615f 6874 6d6c 5f6c 7374       da_html_lst
-00000b30: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
-00000b40: 2020 223c 2164 6f63 7479 7065 2068 746d    "<!doctype htm
-00000b50: 6c3e 3c68 746d 6c3e 3c68 6561 643e 222c  l><html><head>",
-00000b60: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
-00000b70: 6d65 7461 2063 6861 7273 6574 3d27 7574  meta charset='ut
-00000b80: 662d 3827 3e22 2c0d 0a20 2020 2020 2020  f-8'>",..       
-00000b90: 2020 2020 2022 3c6d 6574 6120 6e61 6d65       "<meta name
-00000ba0: 3d27 7669 6577 706f 7274 2720 636f 6e74  ='viewport' cont
-00000bb0: 656e 743d 2777 6964 7468 3d64 6576 6963  ent='width=devic
-00000bc0: 652d 7769 6474 6820 696e 6974 6961 6c2d  e-width initial-
-00000bd0: 7363 616c 653d 312c 2073 6872 696e 6b2d  scale=1, shrink-
-00000be0: 746f 2d66 6974 3d6e 6f27 2f3e 222c 0d0a  to-fit=no'/>",..
-00000bf0: 2020 2020 2020 2020 2020 2020 2320 223c              # "<
-00000c00: 6c69 6e6b 2072 656c 3d73 7479 6c65 7368  link rel=stylesh
-00000c10: 6565 7420 6872 6566 3d68 7474 7073 3a2f  eet href=https:/
-00000c20: 2f66 6f6e 7473 2e67 6f6f 676c 6561 7069  /fonts.googleapi
-00000c30: 732e 636f 6d2f 6373 733f 6661 6d69 6c79  s.com/css?family
-00000c40: 3d52 6f62 6f74 6f2f 3e22 2c0d 0a20 2020  =Roboto/>",..   
-00000c50: 2020 2020 2020 2020 2066 223c 7469 746c           f"<titl
-00000c60: 653e 6874 7470 733a 2f2f 7079 7468 6f6e  e>https://python
-00000c70: 6261 7369 6373 2e6f 7267 3c2f 7469 746c  basics.org</titl
-00000c80: 653e 3c2f 6865 6164 3e22 2c0d 0a20 2020  e></head>",..   
-00000c90: 2020 2020 2020 2020 2022 3c62 6f64 793e           "<body>
-00000ca0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000cb0: 6622 3c68 3120 7374 796c 653d 7b63 656e  f"<h1 style={cen
-00000cc0: 7465 727d 7b62 726f 776e 7d27 3e20 5765  ter}{brown}'> We
-00000cd0: 6c63 6f6d 6520 746f 2065 6973 656e 6d70  lcome to eisenmp
-00000ce0: 5f65 7861 6d70 6c65 733c 2f68 313e 222c  _examples</h1>",
-00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 6622  ..            f"
-00000d00: 3c70 2073 7479 6c65 3d7b 6365 6e74 6572  <p style={center
-00000d10: 7d7b 626c 6163 6b7d 273e 2062 7574 746f  }{black}'> butto
-00000d20: 6e73 206d 6172 6b65 6420 5b73 696e 676c  ns marked [singl
-00000d30: 6520 7368 6f74 5d20 7275 6e20 616c 6f6e  e shot] run alon
-00000d40: 6520 2d20 656c 7365 2062 6c6f 636b 7320  e - else blocks 
-00000d50: 6f72 2063 7261 7368 203c 2f70 3e22 2c0d  or crash </p>",.
-00000d60: 0a20 2020 2020 2020 2020 2020 2066 223c  .            f"<
-00000d70: 6469 7620 636c 6173 733d 2763 6f6e 7461  div class='conta
-00000d80: 696e 6572 2720 7374 796c 653d 277b 666c  iner' style='{fl
-00000d90: 6578 5f6f 7574 6572 7d27 3e22 2c0d 0a20  ex_outer}'>",.. 
-00000da0: 2020 2020 2020 2020 2020 2066 223c 6469             f"<di
-00000db0: 7620 636c 6173 733d 276d 6964 646c 6527  v class='middle'
-00000dc0: 2073 7479 6c65 3d27 7b66 6c65 785f 6d69   style='{flex_mi
-00000dd0: 647d 273e 222c 0d0a 0d0a 2020 2020 2020  d}'>",....      
-00000de0: 2020 2020 2020 2765 7861 6d70 6c65 5f62        'example_b
-00000df0: 746e 272c 0d0a 0d0a 2020 2020 2020 2020  tn',....        
-00000e00: 2020 2020 223c 2f64 6976 3e3c 2f64 6976      "</div></div
-00000e10: 3e22 2c0d 0a20 2020 2020 2020 2020 2020  >",..           
-00000e20: 2022 5061 7468 3a20 3c70 2069 643d 7052   "Path: <p id=pR
-00000e30: 7370 5265 7475 726e 3e20 3c2f 703e 222c  spReturn> </p>",
-00000e40: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
-00000e50: 2f62 6f64 793e 3c2f 6874 6d6c 3e22 2c0d  /body></html>",.
-00000e60: 0a20 2020 2020 2020 2020 2020 2022 3c73  .            "<s
-00000e70: 6372 6970 743e 222c 0d0a 2020 2020 2020  cript>",..      
-00000e80: 2020 2020 2020 2266 756e 6374 696f 6e20        "function 
-00000e90: 6765 7445 7861 2872 6164 696f 5f62 746e  getExa(radio_btn
-00000ea0: 5f69 6429 207b 222c 0d0a 2020 2020 2020  _id) {",..      
-00000eb0: 2020 2020 2020 2263 6f6e 7374 2078 6872        "const xhr
-00000ec0: 203d 206e 6577 2058 4d4c 4874 7470 5265   = new XMLHttpRe
-00000ed0: 7175 6573 7428 293b 222c 0d0a 2020 2020  quest();",..    
-00000ee0: 2020 2020 2020 2020 2278 6872 2e6f 7065          "xhr.ope
-00000ef0: 6e28 2750 4f53 5427 2c20 272f 2729 3b22  n('POST', '/');"
-00000f00: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000f10: 7868 722e 6f6e 6c6f 6164 203d 2066 756e  xhr.onload = fun
-00000f20: 6374 696f 6e20 2829 207b 636f 6e73 6f6c  ction () {consol
-00000f30: 652e 6c6f 6728 2778 6872 2072 2027 2c20  e.log('xhr r ', 
-00000f40: 7868 722e 7265 7370 6f6e 7365 293b 7d3b  xhr.response);};
-00000f50: 2022 2c0d 0a20 2020 2020 2020 2020 2020   ",..           
-00000f60: 2022 7868 722e 7365 6e64 2872 6164 696f   "xhr.send(radio
-00000f70: 5f62 746e 5f69 6429 3b22 2c0d 0a20 2020  _btn_id);",..   
-00000f80: 2020 2020 2020 2020 2022 6c65 7420 7052           "let pR
-00000f90: 7370 5265 7475 726e 203d 2064 6f63 756d  spReturn = docum
-00000fa0: 656e 742e 6765 7445 6c65 6d65 6e74 4279  ent.getElementBy
-00000fb0: 4964 2827 7052 7370 5265 7475 726e 2729  Id('pRspReturn')
-00000fc0: 3b22 2c0d 0a20 2020 2020 2020 2020 2020  ;",..           
-00000fd0: 2022 7052 7370 5265 7475 726e 2e69 6e6e   "pRspReturn.inn
-00000fe0: 6572 5465 7874 3d72 6164 696f 5f62 746e  erText=radio_btn
-00000ff0: 5f69 643b 222c 0d0a 2020 2020 2020 2020  _id;",..        
-00001000: 2020 2020 227d 222c 0d0a 2020 2020 2020      "}",..      
-00001010: 2020 2020 2020 223c 2f73 6372 6970 743e        "</script>
-00001020: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001030: 223c 2f62 6f64 793e 3c2f 6874 6d6c 3e22  "</body></html>"
-00001040: 0d0a 2020 2020 2020 2020 5d0d 0a0d 0a20  ..        ].... 
-00001050: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
-00001060: 6461 5f68 746d 6c5f 6c73 743a 0d0a 2020  da_html_lst:..  
-00001070: 2020 2020 2020 2020 2020 6966 205f 203d            if _ =
-00001080: 3d20 2765 7861 6d70 6c65 5f62 746e 273a  = 'example_btn':
-00001090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000010a0: 2020 666f 7220 692c 205f 2069 6e20 656e    for i, _ in en
-000010b0: 756d 6572 6174 6528 4d65 6e75 2e65 7861  umerate(Menu.exa
-000010c0: 5f74 706c 5f6c 7374 293a 0d0a 2020 2020  _tpl_lst):..    
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 6964 7820 3d20 4d65 6e75 2e65 7861 5f74  idx = Menu.exa_t
-000010f0: 706c 5f6c 7374 5b69 5d5b 305d 0d0a 2020  pl_lst[i][0]..  
-00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 7368 6f77 203d 204d 656e 752e 6578    show = Menu.ex
-00001120: 615f 7470 6c5f 6c73 745b 695d 5b31 5d0d  a_tpl_lst[i][1].
-00001130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001140: 2020 2020 2065 7861 5f68 746d 6c5f 6c69       exa_html_li
-00001150: 6e65 203d 2066 223c 6469 763e 3c6c 6162  ne = f"<div><lab
-00001160: 656c 3e3c 696e 7075 7420 7479 7065 3d27  el><input type='
-00001170: 7261 6469 6f27 206e 616d 653d 2764 6127  radio' name='da'
-00001180: 2220 5c0d 0a20 2020 2020 2020 2020 2020  " \..           
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2020 2020 2020 2020 2066 2269 643d 277b           f"id='{
-000011b0: 6964 787d 2720 6f6e 636c 6963 6b3d 2767  idx}' onclick='g
-000011c0: 6574 4578 6128 6964 2927 3e7b 7368 6f77  etExa(id)'>{show
-000011d0: 7d3c 2f6c 6162 656c 3e3c 2f64 6976 3e22  }</label></div>"
-000011e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000011f0: 2020 2020 2020 7365 6c66 2e77 6669 6c65        self.wfile
-00001200: 2e77 7269 7465 2862 7974 6573 2865 7861  .write(bytes(exa
-00001210: 5f68 746d 6c5f 6c69 6e65 2c20 2275 7466  _html_line, "utf
-00001220: 2d38 2229 290d 0a20 2020 2020 2020 2020  -8"))..         
-00001230: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00001240: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001250: 662e 7766 696c 652e 7772 6974 6528 6279  f.wfile.write(by
-00001260: 7465 7328 5f2c 2022 7574 662d 3822 2929  tes(_, "utf-8"))
-00001270: 0d0a 0d0a 0d0a 6465 6620 6d61 696e 2829  ......def main()
-00001280: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00001290: 2222 220d 0a20 2020 2073 7461 7274 203d  """..    start =
-000012a0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
-000012b0: 6572 2829 0d0a 0d0a 2020 2020 7275 6e5f  er()....    run_
-000012c0: 6874 7470 2829 0d0a 0d0a 2020 2020 7072  http()....    pr
-000012d0: 696e 7428 2754 696d 6520 696e 2073 6563  int('Time in sec
-000012e0: 3a20 272c 2072 6f75 6e64 2828 7469 6d65  : ', round((time
-000012f0: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
-00001300: 2d20 7374 6172 7429 2929 0d0a 0d0a 0d0a  - start)))......
-00001310: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
-00001320: 5f5f 6d61 696e 5f5f 273a 0d0a 2020 2020  __main__':..    
-00001330: 6d61 696e 2829 0d0a                      main()..
+00000050: 3434 0d0a 696d 706f 7274 206f 730d 0a0d  44..import os...
+00000060: 0a69 6d70 6f72 7420 6a73 6f6e 0d0a 696d  .import json..im
+00000070: 706f 7274 2074 696d 650d 0a66 726f 6d20  port time..from 
+00000080: 6874 7470 2e73 6572 7665 7220 696d 706f  http.server impo
+00000090: 7274 2042 6173 6548 5454 5052 6571 7565  rt BaseHTTPReque
+000000a0: 7374 4861 6e64 6c65 722c 2048 5454 5053  stHandler, HTTPS
+000000b0: 6572 7665 720d 0a0d 0a74 7279 3a0d 0a20  erver....try:.. 
+000000c0: 2020 2069 6d70 6f72 7420 6569 7365 6e6d     import eisenm
+000000d0: 700d 0a20 2020 2069 6d70 6f72 7420 6569  p..    import ei
+000000e0: 7365 6e6d 702e 6569 7365 6e6d 705f 6578  senmp.eisenmp_ex
+000000f0: 615f 6d75 6c74 695f 7372 765f 6561 6368  a_multi_srv_each
+00000100: 5f63 7075 2061 7320 6d75 6c74 695f 6f6e  _cpu as multi_on
+00000110: 5f65 6163 685f 6370 750d 0a20 2020 2069  _each_cpu..    i
+00000120: 6d70 6f72 7420 6569 7365 6e6d 702e 6569  mport eisenmp.ei
+00000130: 7365 6e6d 705f 6578 615f 6561 6368 5f66  senmp_exa_each_f
+00000140: 6c61 736b 5f6f 726d 5f73 7276 5f6f 6e65  lask_orm_srv_one
+00000150: 5f63 7075 2061 7320 7369 6e67 6c65 5f6f  _cpu as single_o
+00000160: 6e5f 6561 6368 5f63 7075 0d0a 2020 2020  n_each_cpu..    
+00000170: 696d 706f 7274 2065 6973 656e 6d70 2e65  import eisenmp.e
+00000180: 6973 656e 6d70 5f65 7861 5f70 7269 6d65  isenmp_exa_prime
+00000190: 2061 7320 7072 696d 650d 0a20 2020 2069   as prime..    i
+000001a0: 6d70 6f72 7420 6569 7365 6e6d 702e 6569  mport eisenmp.ei
+000001b0: 7365 6e6d 705f 6578 615f 7765 625f 6373  senmp_exa_web_cs
+000001c0: 7620 6173 2077 6562 5f63 7376 0d0a 2020  v as web_csv..  
+000001d0: 2020 696d 706f 7274 2065 6973 656e 6d70    import eisenmp
+000001e0: 2e65 6973 656e 6d70 5f65 7861 5f68 7474  .eisenmp_exa_htt
+000001f0: 7020 6173 2068 7474 705f 7372 760d 0a20  p as http_srv.. 
+00000200: 2020 2069 6d70 6f72 7420 6569 7365 6e6d     import eisenm
+00000210: 702e 6569 7365 6e6d 705f 6578 615f 646f  p.eisenmp_exa_do
+00000220: 7562 6c65 5f71 2061 7320 646f 7562 6c65  uble_q as double
+00000230: 5f71 0d0a 2020 2020 696d 706f 7274 2065  _q..    import e
+00000240: 6973 656e 6d70 2e65 6973 656e 6d70 5f65  isenmp.eisenmp_e
+00000250: 7861 5f62 7275 7465 666f 7263 6520 6173  xa_bruteforce as
+00000260: 2062 7275 7465 666f 7263 650d 0a0d 0a65   bruteforce....e
+00000270: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+00000280: 723a 0d0a 2020 2020 696d 706f 7274 2065  r:..    import e
+00000290: 6973 656e 6d70 5f65 7861 6d70 6c65 732e  isenmp_examples.
+000002a0: 6569 7365 6e6d 705f 6578 615f 6d75 6c74  eisenmp_exa_mult
+000002b0: 695f 7372 765f 6561 6368 5f63 7075 2061  i_srv_each_cpu a
+000002c0: 7320 6d75 6c74 695f 6f6e 5f65 6163 685f  s multi_on_each_
+000002d0: 6370 750d 0a20 2020 2069 6d70 6f72 7420  cpu..    import 
+000002e0: 6569 7365 6e6d 705f 6578 616d 706c 6573  eisenmp_examples
+000002f0: 2e65 6973 656e 6d70 5f65 7861 5f65 6163  .eisenmp_exa_eac
+00000300: 685f 666c 6173 6b5f 6f72 6d5f 7372 765f  h_flask_orm_srv_
+00000310: 6f6e 655f 6370 7520 6173 2073 696e 676c  one_cpu as singl
+00000320: 655f 6f6e 5f65 6163 685f 6370 750d 0a20  e_on_each_cpu.. 
+00000330: 2020 2069 6d70 6f72 7420 6569 7365 6e6d     import eisenm
+00000340: 705f 6578 616d 706c 6573 2e65 6973 656e  p_examples.eisen
+00000350: 6d70 5f65 7861 5f70 7269 6d65 2061 7320  mp_exa_prime as 
+00000360: 7072 696d 650d 0a20 2020 2069 6d70 6f72  prime..    impor
+00000370: 7420 6569 7365 6e6d 705f 6578 616d 706c  t eisenmp_exampl
+00000380: 6573 2e65 6973 656e 6d70 5f65 7861 5f77  es.eisenmp_exa_w
+00000390: 6562 5f63 7376 2061 7320 7765 625f 6373  eb_csv as web_cs
+000003a0: 760d 0a20 2020 2069 6d70 6f72 7420 6569  v..    import ei
+000003b0: 7365 6e6d 705f 6578 616d 706c 6573 2e65  senmp_examples.e
+000003c0: 6973 656e 6d70 5f65 7861 5f68 7474 7020  isenmp_exa_http 
+000003d0: 6173 2068 7474 705f 7372 760d 0a20 2020  as http_srv..   
+000003e0: 2069 6d70 6f72 7420 6569 7365 6e6d 705f   import eisenmp_
+000003f0: 6578 616d 706c 6573 2e65 6973 656e 6d70  examples.eisenmp
+00000400: 5f65 7861 5f64 6f75 626c 655f 7120 6173  _exa_double_q as
+00000410: 2064 6f75 626c 655f 710d 0a20 2020 2069   double_q..    i
+00000420: 6d70 6f72 7420 6569 7365 6e6d 705f 6578  mport eisenmp_ex
+00000430: 616d 706c 6573 2e65 6973 656e 6d70 5f65  amples.eisenmp_e
+00000440: 7861 5f62 7275 7465 666f 7263 6520 6173  xa_bruteforce as
+00000450: 2062 7275 7465 666f 7263 650d 0a20 2020   bruteforce..   
+00000460: 2070 6173 730d 0a0d 0a68 6f73 744e 616d   pass....hostNam
+00000470: 6520 3d20 226c 6f63 616c 686f 7374 220d  e = "localhost".
+00000480: 0a73 6572 7665 7250 6f72 7420 3d20 3132  .serverPort = 12
+00000490: 5f33 3231 0d0a 6469 725f 6e61 6d65 203d  _321..dir_name =
+000004a0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+000004b0: 285f 5f66 696c 655f 5f29 0d0a 0d0a 0d0a  (__file__)......
+000004c0: 636c 6173 7320 4d65 6e75 3a0d 0a20 2020  class Menu:..   
+000004d0: 2065 7861 6d70 6c65 5f6d 656e 7520 3d20   example_menu = 
+000004e0: 5b0d 0a20 2020 2020 2020 2027 4d75 6c74  [..        'Mult
+000004f0: 6970 6c65 2073 6572 7665 7220 696e 2065  iple server in e
+00000500: 6163 6820 7072 6f63 6573 732f 4350 5520  ach process/CPU 
+00000510: 636f 7265 202d 2073 6861 7265 2061 2070  core - share a p
+00000520: 6f72 7420 7261 6e67 6520 2d20 7368 6172  ort range - shar
+00000530: 6520 6120 4442 2e20 576f 726b 6572 2047  e a DB. Worker G
+00000540: 7265 656e 2c20 5965 6c6c 6f77 2061 6e64  reen, Yellow and
+00000550: 2042 6c75 6527 2c0d 0a20 2020 2020 2020   Blue',..       
+00000560: 2027 5072 696d 6520 4e75 6d62 6572 2063   'Prime Number c
+00000570: 616c 6375 6c61 7469 6f6e 272c 0d0a 2020  alculation',..  
+00000580: 2020 2020 2020 2745 7665 7279 2046 6c61        'Every Fla
+00000590: 736b 2073 6572 7665 7220 696e 2061 2064  sk server in a d
+000005a0: 6966 6665 7265 6e74 2070 726f 6365 7373  ifferent process
+000005b0: 202d 2073 6861 7265 2061 2070 6f72 7420   - share a port 
+000005c0: 7261 6e67 6520 2d20 7368 6172 6520 6120  range - share a 
+000005d0: 4442 2e20 576f 726b 6572 2059 656c 6c6f  DB. Worker Yello
+000005e0: 7720 616e 6420 426c 7565 272c 0d0a 2020  w and Blue',..  
+000005f0: 2020 2020 2020 2757 6562 2043 5356 206c        'Web CSV l
+00000600: 6172 6765 206c 6973 742e 2041 7665 7261  arge list. Avera
+00000610: 6765 2066 6f72 2065 6163 6820 6368 756e  ge for each chun
+00000620: 6b20 6f66 2061 206c 6172 6765 206c 6973  k of a large lis
+00000630: 7420 636f 6c75 6d6e 2074 6f20 7369 6d70  t column to simp
+00000640: 6c79 2063 616c 6320 7468 6520 7265 7375  ly calc the resu
+00000650: 6c74 7320 6c61 7465 722e 272c 0d0a 2020  lts later.',..  
+00000660: 2020 2020 2020 274f 6e65 2073 696d 706c        'One simpl
+00000670: 6520 6874 7470 2073 6572 7665 7220 7072  e http server pr
+00000680: 6573 656e 7473 2061 2072 6164 696f 206f  esents a radio o
+00000690: 6e20 6576 6572 7920 7072 6f63 6573 732e  n every process.
+000006a0: 2022 556e 656d 706c 6f79 6564 2220 776f   "Unemployed" wo
+000006b0: 726b 6572 2065 7869 742e 272c 0d0a 2020  rker exit.',..  
+000006c0: 2020 2020 2020 2745 6163 6820 7072 6f63        'Each proc
+000006d0: 6573 7320 6861 7320 7477 6f20 5175 6575  ess has two Queu
+000006e0: 6573 2066 6565 6420 6175 6469 6f20 616e  es feed audio an
+000006f0: 6420 7669 6465 6f2e 204d 6572 6765 2069  d video. Merge i
+00000700: 6e20 6120 6661 6b65 2070 726f 6475 6374  n a fake product
+00000710: 696f 6e2e 272c 0d0a 2020 2020 2020 2020  ion.',..        
+00000720: 2742 7275 7465 2066 6f72 6365 2061 7474  'Brute force att
+00000730: 6163 6b20 7769 7468 2064 6963 7469 6f6e  ack with diction
+00000740: 6172 7920 616e 6420 6974 6572 746f 6f6c  ary and itertool
+00000750: 7320 6765 6e65 7261 746f 7227 0d0a 2020  s generator'..  
+00000760: 2020 5d0d 0a0d 0a20 2020 2065 7861 5f74    ]....    exa_t
+00000770: 706c 5f6c 7374 203d 205b 0d0a 2020 2020  pl_lst = [..    
+00000780: 2020 2020 2830 2c20 6578 616d 706c 655f      (0, example_
+00000790: 6d65 6e75 5b30 5d2c 206d 756c 7469 5f6f  menu[0], multi_o
+000007a0: 6e5f 6561 6368 5f63 7075 2e6d 6169 6e29  n_each_cpu.main)
+000007b0: 2c0d 0a20 2020 2020 2020 2028 312c 2065  ,..        (1, e
+000007c0: 7861 6d70 6c65 5f6d 656e 755b 315d 2c20  xample_menu[1], 
+000007d0: 7072 696d 652e 6d61 696e 292c 0d0a 2020  prime.main),..  
+000007e0: 2020 2020 2020 2832 2c20 6578 616d 706c        (2, exampl
+000007f0: 655f 6d65 6e75 5b32 5d2c 2073 696e 676c  e_menu[2], singl
+00000800: 655f 6f6e 5f65 6163 685f 6370 752e 6d61  e_on_each_cpu.ma
+00000810: 696e 292c 0d0a 2020 2020 2020 2020 2833  in),..        (3
+00000820: 2c20 6578 616d 706c 655f 6d65 6e75 5b33  , example_menu[3
+00000830: 5d2c 2077 6562 5f63 7376 2e6d 6169 6e29  ], web_csv.main)
+00000840: 2c0d 0a20 2020 2020 2020 2028 342c 2065  ,..        (4, e
+00000850: 7861 6d70 6c65 5f6d 656e 755b 345d 2c20  xample_menu[4], 
+00000860: 6874 7470 5f73 7276 2e6d 6169 6e29 2c0d  http_srv.main),.
+00000870: 0a20 2020 2020 2020 2028 352c 2065 7861  .        (5, exa
+00000880: 6d70 6c65 5f6d 656e 755b 355d 2c20 646f  mple_menu[5], do
+00000890: 7562 6c65 5f71 2e6d 6169 6e29 2c0d 0a20  uble_q.main),.. 
+000008a0: 2020 2020 2020 2028 362c 2065 7861 6d70         (6, examp
+000008b0: 6c65 5f6d 656e 755b 365d 2c20 6272 7574  le_menu[6], brut
+000008c0: 6566 6f72 6365 2e6d 6169 6e29 0d0a 2020  eforce.main)..  
+000008d0: 2020 5d0d 0a0d 0a0d 0a64 6566 2072 756e    ]......def run
+000008e0: 5f68 7474 7028 293a 0d0a 2020 2020 2222  _http():..    ""
+000008f0: 2242 6c6f 636b 6564 2c20 6e6f 206c 6f6f  "Blocked, no loo
+00000900: 7020 6865 7265 0d0a 2020 2020 2222 220d  p here..    """.
+00000910: 0a20 2020 2067 6c6f 6261 6c20 7365 7276  .    global serv
+00000920: 6572 506f 7274 0d0a 0d0a 2020 2020 7768  erPort....    wh
+00000930: 696c 6520 313a 0d0a 2020 2020 2020 2020  ile 1:..        
+00000940: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00000950: 2020 7765 6253 6572 7665 7220 3d20 4854    webServer = HT
+00000960: 5450 5365 7276 6572 2828 686f 7374 4e61  TPServer((hostNa
+00000970: 6d65 2c20 7365 7276 6572 506f 7274 292c  me, serverPort),
+00000980: 204d 7953 6572 7665 7229 0d0a 2020 2020   MyServer)..    
+00000990: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+000009a0: 2020 2020 2020 2065 7863 6570 7420 4f53         except OS
+000009b0: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+000009c0: 2020 2020 7072 696e 7428 6627 7365 7276      print(f'serv
+000009d0: 6572 506f 7274 2069 6e20 7573 6520 7b73  erPort in use {s
+000009e0: 6572 7665 7250 6f72 747d 5c6e 5c74 6164  erverPort}\n\tad
+000009f0: 6420 6f6e 6520 746f 2070 6f72 7420 6e75  d one to port nu
+00000a00: 6d62 6572 2729 0d0a 2020 2020 2020 2020  mber')..        
+00000a10: 2020 2020 7365 7276 6572 506f 7274 202b      serverPort +
+00000a20: 3d20 3120 2023 2070 6f72 7420 616c 7265  = 1  # port alre
+00000a30: 6164 7920 696e 2075 7365 0d0a 0d0a 2020  ady in use....  
+00000a40: 2020 7072 696e 7428 6622 4578 616d 706c    print(f"Exampl
+00000a50: 6573 2068 7474 703a 2f2f 2573 3a25 7322  es http://%s:%s"
+00000a60: 2025 2028 686f 7374 4e61 6d65 2c20 7365   % (hostName, se
+00000a70: 7276 6572 506f 7274 2929 0d0a 2020 2020  rverPort))..    
+00000a80: 7472 793a 0d0a 2020 2020 2020 2020 7765  try:..        we
+00000a90: 6253 6572 7665 722e 7365 7276 655f 666f  bServer.serve_fo
+00000aa0: 7265 7665 7228 290d 0a20 2020 2065 7863  rever()..    exc
+00000ab0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+00000ac0: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
+00000ad0: 7061 7373 0d0a 2020 2020 7765 6253 6572  pass..    webSer
+00000ae0: 7665 722e 7365 7276 6572 5f63 6c6f 7365  ver.server_close
+00000af0: 2829 0d0a 2020 2020 7072 696e 7428 2253  ()..    print("S
+00000b00: 6572 7665 7220 7374 6f70 7065 642e 2229  erver stopped.")
+00000b10: 0d0a 0d0a 0d0a 636c 6173 7320 4d79 5365  ......class MySe
+00000b20: 7276 6572 2842 6173 6548 5454 5052 6571  rver(BaseHTTPReq
+00000b30: 7565 7374 4861 6e64 6c65 7229 3a0d 0a0d  uestHandler):...
+00000b40: 0a20 2020 2064 6566 2064 6f5f 504f 5354  .    def do_POST
+00000b50: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000b60: 2022 2222 2222 220d 0a20 2020 2020 2020   """"""..       
+00000b70: 2023 2070 7269 6e74 2873 656c 662e 6865   # print(self.he
+00000b80: 6164 6572 7329 0d0a 2020 2020 2020 2020  aders)..        
+00000b90: 6c65 6e67 7468 203d 2069 6e74 2873 656c  length = int(sel
+00000ba0: 662e 6865 6164 6572 732e 6765 745f 616c  f.headers.get_al
+00000bb0: 6c28 2763 6f6e 7465 6e74 2d6c 656e 6774  l('content-lengt
+00000bc0: 6827 295b 305d 290d 0a20 2020 2020 2020  h')[0])..       
+00000bd0: 2070 7269 6e74 2873 656c 662e 6865 6164   print(self.head
+00000be0: 6572 732e 6765 745f 616c 6c28 2763 6f6e  ers.get_all('con
+00000bf0: 7465 6e74 2d6c 656e 6774 6827 2929 0d0a  tent-length'))..
+00000c00: 2020 2020 2020 2020 6461 7461 5f73 7472          data_str
+00000c10: 696e 6720 3d20 7365 6c66 2e72 6669 6c65  ing = self.rfile
+00000c20: 2e72 6561 6428 6c65 6e67 7468 290d 0a20  .read(length).. 
+00000c30: 2020 2020 2020 2065 7861 6d70 6c65 5f66         example_f
+00000c40: 756e 203d 204d 656e 752e 6578 615f 7470  un = Menu.exa_tp
+00000c50: 6c5f 6c73 745b 696e 7428 6461 7461 5f73  l_lst[int(data_s
+00000c60: 7472 696e 6729 5d5b 325d 0d0a 2020 2020  tring)][2]..    
+00000c70: 2020 2020 7265 745f 7661 6c20 3d20 6578      ret_val = ex
+00000c80: 616d 706c 655f 6675 6e28 290d 0a20 2020  ample_fun()..   
+00000c90: 2020 2020 2023 2070 7269 6e74 2864 6174       # print(dat
+00000ca0: 615f 7374 7269 6e67 290d 0a20 2020 2020  a_string)..     
+00000cb0: 2020 2073 656c 662e 7365 6e64 5f72 6573     self.send_res
+00000cc0: 706f 6e73 6528 3230 3029 0d0a 2020 2020  ponse(200)..    
+00000cd0: 2020 2020 2320 7365 6c66 2e73 656e 645f      # self.send_
+00000ce0: 6865 6164 6572 2822 436f 6e74 656e 742d  header("Content-
+00000cf0: 7479 7065 222c 2022 7465 7874 2f70 6c61  type", "text/pla
+00000d00: 696e 2229 0d0a 2020 2020 2020 2020 7365  in")..        se
+00000d10: 6c66 2e73 656e 645f 6865 6164 6572 2827  lf.send_header('
+00000d20: 436f 6e74 656e 742d 5479 7065 272c 2027  Content-Type', '
+00000d30: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00000d40: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
+00000d50: 2e65 6e64 5f68 6561 6465 7273 2829 0d0a  .end_headers()..
+00000d60: 2020 2020 2020 2020 7365 6c66 2e66 6c75          self.flu
+00000d70: 7368 5f68 6561 6465 7273 2829 0d0a 2020  sh_headers()..  
+00000d80: 2020 2020 2020 6a73 6f6e 5f73 7472 696e        json_strin
+00000d90: 6720 3d20 6a73 6f6e 2e64 756d 7073 2873  g = json.dumps(s
+00000da0: 7472 2872 6574 5f76 616c 2929 0d0a 2020  tr(ret_val))..  
+00000db0: 2020 2020 2020 7365 6c66 2e77 6669 6c65        self.wfile
+00000dc0: 2e77 7269 7465 2862 7974 6573 286a 736f  .write(bytes(jso
+00000dd0: 6e5f 7374 7269 6e67 2c20 2275 7466 2d38  n_string, "utf-8
+00000de0: 2229 290d 0a20 2020 2020 2020 2072 6574  "))..        ret
+00000df0: 7572 6e20 5472 7565 0d0a 0d0a 2020 2020  urn True....    
+00000e00: 6465 6620 646f 5f47 4554 2873 656c 6629  def do_GET(self)
+00000e10: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+00000e20: 7365 6e64 5f72 6573 706f 6e73 6528 3230  send_response(20
+00000e30: 3029 0d0a 2020 2020 2020 2020 7365 6c66  0)..        self
+00000e40: 2e73 656e 645f 6865 6164 6572 2822 436f  .send_header("Co
+00000e50: 6e74 656e 742d 7479 7065 222c 2022 7465  ntent-type", "te
+00000e60: 7874 2f68 746d 6c22 290d 0a20 2020 2020  xt/html")..     
+00000e70: 2020 2073 656c 662e 656e 645f 6865 6164     self.end_head
+00000e80: 6572 7328 290d 0a0d 0a20 2020 2020 2020  ers()....       
+00000e90: 2064 615f 6874 6d6c 5f6c 7374 203d 205b   da_html_lst = [
+00000ea0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000eb0: 223c 2164 6f63 7479 7065 2068 746d 6c3e  "<!doctype html>
+00000ec0: 3c68 746d 6c3e 3c68 746d 6c20 6c61 6e67  <html><html lang
+00000ed0: 3d27 656e 273e 222c 0d0a 2020 2020 2020  ='en'>",..      
+00000ee0: 2020 2020 2020 223c 6865 6164 3e22 2c0d        "<head>",.
+00000ef0: 0a20 2020 2020 2020 2020 2020 2022 3c6d  .            "<m
+00000f00: 6574 6120 6368 6172 7365 743d 2755 5446  eta charset='UTF
+00000f10: 2d38 273e 222c 0d0a 2020 2020 2020 2020  -8'>",..        
+00000f20: 2020 2020 223c 6d65 7461 2058 2d43 6f6e      "<meta X-Con
+00000f30: 7465 6e74 2d54 7970 652d 4f70 7469 6f6e  tent-Type-Option
+00000f40: 733d 276e 6f73 6e69 6666 273e 222c 0d0a  s='nosniff'>",..
+00000f50: 2020 2020 2020 2020 2020 2020 223c 6d65              "<me
+00000f60: 7461 206e 616d 653d 2776 6965 7770 6f72  ta name='viewpor
+00000f70: 7427 2063 6f6e 7465 6e74 3d27 7769 6474  t' content='widt
+00000f80: 683d 6465 7669 6365 2d77 6964 7468 2c20  h=device-width, 
+00000f90: 696e 6974 6961 6c2d 7363 616c 653d 312e  initial-scale=1.
+00000fa0: 3027 3e22 2c0d 0a20 2020 2020 2020 2020  0'>",..         
+00000fb0: 2020 2022 3c73 7479 6c65 3e22 2c0d 0a20     "<style>",.. 
+00000fc0: 2020 2020 2020 2020 2020 2022 4066 6f6e             "@fon
+00000fd0: 742d 6661 6365 207b 666f 6e74 2d66 616d  t-face {font-fam
+00000fe0: 696c 793a 2027 5054 2053 616e 7327 3b66  ily: 'PT Sans';f
+00000ff0: 6f6e 742d 7374 796c 653a 206e 6f72 6d61  ont-style: norma
+00001000: 6c3b 666f 6e74 2d77 6569 6768 743a 206e  l;font-weight: n
+00001010: 6f72 6d61 6c3b 222c 0d0a 2020 2020 2020  ormal;",..      
+00001020: 2020 2020 2020 2273 7263 3a20 6c6f 6361        "src: loca
+00001030: 6c28 2750 5420 5361 6e73 2729 2c20 6c6f  l('PT Sans'), lo
+00001040: 6361 6c28 2750 5453 616e 732d 5265 6775  cal('PTSans-Regu
+00001050: 6c61 7227 292c 222c 0d0a 2020 2020 2020  lar'),",..      
+00001060: 2020 2020 2020 2275 726c 2864 6174 613a        "url(data:
+00001070: 6170 706c 6963 6174 696f 6e2f 666f 6e74  application/font
+00001080: 2d77 6f66 6632 3b63 6861 7273 6574 3d75  -woff2;charset=u
+00001090: 7466 2d38 3b62 6173 6536 342c 6430 3947  tf-8;base64,d09G
+000010a0: 5267 4142 4141 4141 4148 6f77 4142 4d41  RgABAAAAAHowABMA
+000010b0: 4141 4141 2b4f 4141 2920 666f 726d 6174  AAAA+OAA) format
+000010c0: 2827 776f 6666 3227 293b 7d22 2c0d 0a0d  ('woff2');}",...
+000010d0: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
+000010e0: 6479 7b66 6f6e 742d 6661 6d69 6c79 3a50  dy{font-family:P
+000010f0: 5420 5361 6e73 2c20 6172 6961 6c3b 2063  T Sans, arial; c
+00001100: 6f6c 6f72 3a62 6c61 636b 3b62 6163 6b67  olor:black;backg
+00001110: 726f 756e 642d 636f 6c6f 723a 2363 6363  round-color:#ccc
+00001120: 3b7d 222c 0d0a 2020 2020 2020 2020 2020  ;}",..          
+00001130: 2020 2268 3120 7b63 6f6c 6f72 3a62 726f    "h1 {color:bro
+00001140: 776e 3b74 6578 742d 616c 6967 6e3a 6365  wn;text-align:ce
+00001150: 6e74 6572 3b7d 222c 0d0a 2020 2020 2020  nter;}",..      
+00001160: 2020 2020 2020 222e 636f 6e74 6169 6e65        ".containe
+00001170: 7220 7b64 6973 706c 6179 3a20 666c 6578  r {display: flex
+00001180: 3b7d 222c 0d0a 2020 2020 2020 2020 2020  ;}",..          
+00001190: 2020 222e 6d69 6464 6c65 207b 6469 7370    ".middle {disp
+000011a0: 6c61 793a 2066 6c65 783b 666c 6578 2d64  lay: flex;flex-d
+000011b0: 6972 6563 7469 6f6e 3a20 636f 6c75 6d6e  irection: column
+000011c0: 3b6d 6172 6769 6e3a 2061 7574 6f3b 636f  ;margin: auto;co
+000011d0: 6c6f 723a 6272 6f77 6e3b 7d22 2c0d 0a20  lor:brown;}",.. 
+000011e0: 2020 2020 2020 2020 2020 2022 2e70 4d69             ".pMi
+000011f0: 6420 7b63 6f6c 6f72 3a20 626c 6163 6b3b  d {color: black;
+00001200: 2074 6578 742d 616c 6967 6e3a 6365 6e74   text-align:cent
+00001210: 6572 3b7d 222c 0d0a 2020 2020 2020 2020  er;}",..        
+00001220: 2020 2020 223c 2f73 7479 6c65 3e22 2c0d      "</style>",.
+00001230: 0a20 2020 2020 2020 2020 2020 2066 223c  .            f"<
+00001240: 7469 746c 653e 4578 616d 706c 6573 3c2f  title>Examples</
+00001250: 7469 746c 653e 222c 0d0a 2020 2020 2020  title>",..      
+00001260: 2020 2020 2020 223c 2f68 6561 643e 222c        "</head>",
+00001270: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001280: 223c 626f 6479 3e22 2c0d 0a20 2020 2020  "<body>",..     
+00001290: 2020 2020 2020 2066 223c 6831 3e20 5765         f"<h1> We
+000012a0: 6c63 6f6d 6520 746f 2065 6973 656e 6d70  lcome to eisenmp
+000012b0: 5f65 7861 6d70 6c65 733c 2f68 313e 222c  _examples</h1>",
+000012c0: 0d0a 2020 2020 2020 2020 2020 2020 6622  ..            f"
+000012d0: 3c70 2063 6c61 7373 3d70 4d69 643e 2045  <p class=pMid> E
+000012e0: 7861 6d70 6c65 7320 7275 6e20 696e 2074  xamples run in t
+000012f0: 6865 2074 6572 6d69 6e61 6c20 7769 6e64  he terminal wind
+00001300: 6f77 2e20 3c2f 703e 222c 0d0a 2020 2020  ow. </p>",..    
+00001310: 2020 2020 2020 2020 6622 3c64 6976 2063          f"<div c
+00001320: 6c61 7373 3d27 636f 6e74 6169 6e65 7227  lass='container'
+00001330: 3e22 2c0d 0a20 2020 2020 2020 2020 2020  >",..           
+00001340: 2066 223c 6469 7620 636c 6173 733d 276d   f"<div class='m
+00001350: 6964 646c 6527 3e22 2c0d 0a20 2020 2020  iddle'>",..     
+00001360: 2020 2020 2020 2027 5f6f 5f5f 6578 616d         '_o__exam
+00001370: 706c 655f 6275 7474 6f6e 735f 5f5f 5f27  ple_buttons____'
+00001380: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001390: 3c2f 6469 763e 3c2f 6469 763e 222c 0d0a  </div></div>",..
+000013a0: 2020 2020 2020 2020 2020 2020 2273 656e              "sen
+000013b0: 643a 203c 7020 6964 3d70 5273 7052 6574  d: <p id=pRspRet
+000013c0: 7572 6e20 636c 6173 733d 7049 6e4f 7574  urn class=pInOut
+000013d0: 3e20 3c2f 703e 222c 0d0a 2020 2020 2020  > </p>",..      
+000013e0: 2020 2020 2020 6622 7265 7370 3a20 3c70        f"resp: <p
+000013f0: 2069 643d 704d 7367 2063 6c61 7373 3d70   id=pMsg class=p
+00001400: 496e 4f75 743e 203c 2f70 3e22 2c0d 0a20  InOut> </p>",.. 
+00001410: 2020 2020 2020 2020 2020 2022 3c2f 626f             "</bo
+00001420: 6479 3e3c 2f68 746d 6c3e 222c 0d0a 0d0a  dy></html>",....
+00001430: 2020 2020 2020 2020 2020 2020 223c 7363              "<sc
+00001440: 7269 7074 3e22 2c0d 0a20 2020 2020 2020  ript>",..       
+00001450: 2020 2020 2022 6675 6e63 7469 6f6e 2067       "function g
+00001460: 6574 4578 6128 7261 6469 6f5f 6274 6e5f  etExa(radio_btn_
+00001470: 6964 2920 7b22 2c0d 0a20 2020 2020 2020  id) {",..       
+00001480: 2020 2020 2022 646f 6375 6d65 6e74 2e67       "document.g
+00001490: 6574 456c 656d 656e 7442 7949 6428 2770  etElementById('p
+000014a0: 4d73 6727 292e 696e 6e65 7248 544d 4c3d  Msg').innerHTML=
+000014b0: 2727 3b22 2c0d 0a20 2020 2020 2020 2020  '';",..         
+000014c0: 2020 2022 636f 6e73 7420 7868 7220 3d20     "const xhr = 
+000014d0: 6e65 7720 584d 4c48 7474 7052 6571 7565  new XMLHttpReque
+000014e0: 7374 2829 3b22 2c0d 0a20 2020 2020 2020  st();",..       
+000014f0: 2020 2020 2022 7868 722e 6f70 656e 2827       "xhr.open('
+00001500: 504f 5354 272c 2027 2f27 293b 222c 0d0a  POST', '/');",..
+00001510: 2020 2020 2020 2020 2020 2020 2278 6872              "xhr
+00001520: 2e6f 6e6c 6f61 6420 3d20 6675 6e63 7469  .onload = functi
+00001530: 6f6e 2028 2920 7b63 6f6e 736f 6c65 2e6c  on () {console.l
+00001540: 6f67 2827 7868 7220 7220 272c 2078 6872  og('xhr r ', xhr
+00001550: 2e72 6573 706f 6e73 6529 3b20 222c 0d0a  .response); ",..
+00001560: 2020 2020 2020 2020 2020 2020 2264 6f63              "doc
+00001570: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+00001580: 4279 4964 2827 704d 7367 2729 2e69 6e6e  ById('pMsg').inn
+00001590: 6572 4854 4d4c 3d78 6872 2e72 6573 706f  erHTML=xhr.respo
+000015a0: 6e73 653b 7d3b 2022 2c0d 0a20 2020 2020  nse;}; ",..     
+000015b0: 2020 2020 2020 2022 7868 722e 7365 6e64         "xhr.send
+000015c0: 2872 6164 696f 5f62 746e 5f69 6429 3b22  (radio_btn_id);"
+000015d0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000015e0: 6c65 7420 7052 7370 5265 7475 726e 203d  let pRspReturn =
+000015f0: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
+00001600: 6d65 6e74 4279 4964 2827 7052 7370 5265  mentById('pRspRe
+00001610: 7475 726e 2729 3b22 2c0d 0a20 2020 2020  turn');",..     
+00001620: 2020 2020 2020 2022 7052 7370 5265 7475         "pRspRetu
+00001630: 726e 2e69 6e6e 6572 5465 7874 3d72 6164  rn.innerText=rad
+00001640: 696f 5f62 746e 5f69 643b 222c 0d0a 2020  io_btn_id;",..  
+00001650: 2020 2020 2020 2020 2020 227d 222c 0d0a            "}",..
+00001660: 2020 2020 2020 2020 2020 2020 223c 2f73              "</s
+00001670: 6372 6970 743e 222c 0d0a 2020 2020 2020  cript>",..      
+00001680: 2020 2020 2020 223c 2f62 6f64 793e 3c2f        "</body></
+00001690: 6874 6d6c 3e22 0d0a 2020 2020 2020 2020  html>"..        
+000016a0: 5d0d 0a0d 0a20 2020 2020 2020 2066 6f72  ]....        for
+000016b0: 205f 2069 6e20 6461 5f68 746d 6c5f 6c73   _ in da_html_ls
+000016c0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+000016d0: 6966 205f 203d 3d20 275f 6f5f 5f65 7861  if _ == '_o__exa
+000016e0: 6d70 6c65 5f62 7574 746f 6e73 5f5f 5f5f  mple_buttons____
+000016f0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+00001700: 2020 2020 666f 7220 692c 205f 2069 6e20      for i, _ in 
+00001710: 656e 756d 6572 6174 6528 4d65 6e75 2e65  enumerate(Menu.e
+00001720: 7861 5f74 706c 5f6c 7374 293a 0d0a 2020  xa_tpl_lst):..  
+00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001740: 2020 6964 7820 3d20 4d65 6e75 2e65 7861    idx = Menu.exa
+00001750: 5f74 706c 5f6c 7374 5b69 5d5b 305d 0d0a  _tpl_lst[i][0]..
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 2020 7368 6f77 203d 204d 656e 752e      show = Menu.
+00001780: 6578 615f 7470 6c5f 6c73 745b 695d 5b31  exa_tpl_lst[i][1
+00001790: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000017a0: 2020 2020 2020 2065 7861 5f68 746d 6c5f         exa_html_
+000017b0: 6c69 6e65 203d 2066 223c 6469 763e 3c6c  line = f"<div><l
+000017c0: 6162 656c 3e3c 696e 7075 7420 7479 7065  abel><input type
+000017d0: 3d27 7261 6469 6f27 206e 616d 653d 2764  ='radio' name='d
+000017e0: 6127 2220 5c0d 0a20 2020 2020 2020 2020  a'" \..         
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 2020 2020 2066 2269 643d             f"id=
+00001810: 277b 6964 787d 2720 6f6e 636c 6963 6b3d  '{idx}' onclick=
+00001820: 2767 6574 4578 6128 6964 2927 3e7b 7368  'getExa(id)'>{sh
+00001830: 6f77 7d3c 2f6c 6162 656c 3e3c 2f64 6976  ow}</label></div
+00001840: 3e22 0d0a 2020 2020 2020 2020 2020 2020  >"..            
+00001850: 2020 2020 2020 2020 7365 6c66 2e77 6669          self.wfi
+00001860: 6c65 2e77 7269 7465 2862 7974 6573 2865  le.write(bytes(e
+00001870: 7861 5f68 746d 6c5f 6c69 6e65 2c20 2275  xa_html_line, "u
+00001880: 7466 2d38 2229 290d 0a20 2020 2020 2020  tf-8"))..       
+00001890: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000018a0: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+000018b0: 656c 662e 7766 696c 652e 7772 6974 6528  elf.wfile.write(
+000018c0: 6279 7465 7328 5f2c 2022 7574 662d 3822  bytes(_, "utf-8"
+000018d0: 2929 0d0a 0d0a 0d0a 6465 6620 6d61 696e  ))......def main
+000018e0: 2829 3a0d 0a20 2020 2022 2222 0d0a 2020  ():..    """..  
+000018f0: 2020 2222 220d 0a20 2020 2073 7461 7274    """..    start
+00001900: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+00001910: 6e74 6572 2829 0d0a 0d0a 2020 2020 7275  nter()....    ru
+00001920: 6e5f 6874 7470 2829 0d0a 0d0a 2020 2020  n_http()....    
+00001930: 7072 696e 7428 2754 696d 6520 696e 2073  print('Time in s
+00001940: 6563 3a20 272c 2072 6f75 6e64 2828 7469  ec: ', round((ti
+00001950: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+00001960: 2920 2d20 7374 6172 7429 2929 0d0a 0d0a  ) - start)))....
+00001970: 0d0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00001980: 2027 5f5f 6d61 696e 5f5f 273a 0d0a 2020   '__main__':..  
+00001990: 2020 6d61 696e 2829 0d0a                   main()..
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_http.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,17 +52,26 @@
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = [
             self.first_module,  # second module must be threaded, else we hang
             # self.watchdog_module,  # enable for threaded module start live example
         ]
-        # not enough work example, useless worker auto shutdown, the modules return False
-        self.num_cores = 16  # [option] number of process we want, default is None: one proc/CPU core
-        self.num_rows = 1  # micro workload, every process want to get a piece of generator; default None: 10_000 rows
+
+        # Multiprocess vars - override default
+        self.NUM_PROCS = 16  # your process count, default is None: one proc/CPU core
+        self.NUM_ROWS = 1  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
+        self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
+        self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
+        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
+        self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+
+        # 'not enough work example', useless worker auto shutdown, the modules return False
         self.radio_name = None  # define to get it as key in 'modConf' dictionary and worker use 'toolbox.radio_name'
         self.radio_url = None
         self.sleep_time = 60  # if watchdog enabled, toolbox.sleep_time = 60
 
 
 modConf = ModuleConfiguration()  # Accessible in the module.
 
@@ -86,27 +95,27 @@
 
     Blocked, no loop here
     toolbox is the all-in-one box for vars and queues. incl. ModuleConfiguration
     We have num_procs, we have ports to add, we need worker in groups to serve ports
     """
     global serverPort
 
-    worker_id = toolbox.worker_id
-    serverPort = serverPort + worker_id
+    WORKER_ID = toolbox.WORKER_ID
+    serverPort = serverPort + WORKER_ID
     while 1:
         toolbox.next_lst = toolbox.mp_input_q.get()
         break
-    if toolbox.stop_msg in toolbox.next_lst[1]:  # eisenmp.iterator_loop() informs (single list) stop, no more lists
+    if toolbox.STOP_MSG in toolbox.next_lst[1]:  # eisenmp.iterator_loop() informs (single list) stop, no more lists
         return False  # eisenmp_worker_loader will re-send the shutdown msg to the next worker - generator is empty
 
     toolbox.radio_name, toolbox.radio_url = toolbox.next_lst[1]  # list of tuples, [0] iterator list header
     MyServer.toolbox = toolbox
     webServer = HTTPServer((hostName, serverPort), MyServer)
 
-    toolbox.mp_print_q.put(f"Server {worker_id} started http://%s:%s" % (hostName, serverPort))
+    toolbox.mp_print_q.put(f"Server {WORKER_ID} started http://%s:%s" % (hostName, serverPort))
     try:
         webServer.serve_forever()
     except KeyboardInterrupt:
         pass
     webServer.server_close()
     print("Server stopped.")
 
@@ -146,22 +155,25 @@
         self.wfile.write(bytes("(function() {", "utf-8"))
         self.wfile.write(bytes("const audio = document.getElementById('audioR');audio.volume=0.5;", "utf-8"))
         self.wfile.write(bytes("})();", "utf-8"))
         self.wfile.write(bytes("</script>", "utf-8"))
         self.wfile.write(bytes("</body></html>", "utf-8"))
         self.wfile.write(bytes("", "utf-8"))
 
-        self.toolbox.mp_print_q.put(f'proc name: {self.toolbox.worker_name} pid: {self.toolbox.worker_pid}')
+        self.toolbox.mp_print_q.put(f'proc name: {self.toolbox.WORKER_NAME} pid: {self.toolbox.WORKER_PID}')
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
     manager_http_srv()
 
     print('Time in sec: ', round((time.perf_counter() - start)))
+    msg_time = 'HTTP Server, Time in sec: ', round((time.perf_counter() - start))
+    print(msg_time)
+    return msg_time
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,174 +1,171 @@
-"""Multiprocessor Prime number finder (worker) and number Generator.
+"""Green CSV generator / Worker in folder /worker
 
-Example for a ``two in one module``. Generator and worker. 'generator_prime'/'worker_prime'
+We download a NZ government report and calculate the average of split lists.
+See URL. Try your own URL. They have a lot.
 """
+
 import os
+import csv
 import time
-from math import isqrt
+from io import TextIOWrapper
+from zipfile import ZipFile
 
 import eisenmp
+try:
+    import eisenmp.utils.eisenmp_utils as e_utils
+    from eisenmp.utils_exa.eisenmp_download import DownLoad
+except ImportError:
+    import eisenmp_examples.utils.eisenmp_utils as e_utils
+    from eisenmp_examples.utils_exa.eisenmp_download import DownLoad
+
 dir_name = os.path.dirname(__file__)
 
 
 class ModuleConfiguration:
-    """
+    """Fill the existing attributes.
     You can use the class to have your variables available in the module.
-
-    'worker_prime()' is executed by all processes on a CPU somewhere.
-    Each 'worker_prime()' gets (one by one) a list chunk from eisenmp.mp_input_q.
     You have full access to all queues and methods. mp = eisenmp.Mp()
+
     """
-    # path to worker module and entry function reference, worker module import in [isolated] process environment
-    # -------------------- MANDATORY WORKER STRINGS --------------------
+    # path to worker module and entry function reference, worker module import in
+    # [isolated, dead references to data structures, [list, dict, instance], offset addr. unreachable] process env
+    # -------------------- MANDATORY WORKER STRINGS (large worker live in /worker) --------------------
     first_module = {
-        'WORKER_PATH': os.path.join(dir_name, 'eisenmp_exa_prime.py'),
-        'WORKER_REF': 'worker_prime',  # Warning: loader runs all f(toolbox) as single argument; pull args from toolbox
+        'worker_path': os.path.join(dir_name, 'worker', 'eisenmp_exa_wrk_csv.py'),
+        'worker_ref': 'worker_entrance',
+    }
+    watchdog_module = {
+        'WORKER_PATH': os.path.join(dir_name, 'worker', 'eisenmp_exa_wrk_watchdog.py'),
+        'WORKER_REF': 'mp_start_show_threads',
     }
-    foo = {'WORKER_PATH': 'bar', 'WORKER_REF': 'baz'}
+    dl_url = 'https://www.stats.govt.nz/assets/Uploads/International-trade/' \
+             'International-trade-December-2022-quarter/Download-data/international-trade-december-2022-quarter.zip'
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = [
-            self.first_module,   # second module must be threaded, else we hang
-            # foo
+            self.first_module,  # second module must be started by a thread, else we hang
+            self.watchdog_module,
         ]
-        # manager
-        self.num_cores = 6  # number of process we want, default is None: one proc/CPU core
-        self.num_rows = 42  # spread workload, list rows to calc in one loop, default is None: 10_000
-        self.store_result = True  # keep in dictionary, can crash the system if working with network chunks
-
-        # custom part, write your own Attributes
-        self.range_num = 1_000  # we got a target/max value and num_rows for each proc, can calc ETA est. time arrival
-        self.info_td_max = self.range_num  # target value for info thread to calculate % and ETA
-        self.n = 10 ** 7  # 10_000_000_000_000_000 .....
-        self.result_lbl = 'Large PRIME numbers '
-        self.say_hello = 'Hello'  # just to show that worker can [read] all attributes of instance, in 'worker_prime()'
-
 
-modConf = ModuleConfiguration()  # Accessible in the module.
-
-
-def generator_prime():
-    """Manager
-
-    - Generator - One time execution.
+        # Multiprocess vars - override default
+        self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
+        self.NUM_ROWS = 50_000  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
+        self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
+        self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
+        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
+        self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+
+        # CSV part
+        self.use_file_system = False  # False: download and unzip in mem; True must exist on fs ------------- SWITCH ---
+        self.url = self.dl_url  # False 'use_file_system', URL of csv file
+        self.zipped_filename = 'revised.csv'  # name of the uncompressed file in zip archive
+        self.csv_col_name = 'value'  # CSV table column header
+        self.sleep_time = 45  # watchdog module in 'worker_modules' list
+
+
+modConf = ModuleConfiguration()  # accessible in module
+
+
+def generator_calc_csv():
+    """
+    - Manager -
+
+    Generator part of calc CSV. Worker module in /worker folder.
+
+    :params: result_lbl: find result in a list; sum findings, mandatory
+    :params: use_file_system: True 'use_file_system'; False: in mem unzip
+    :params: url: dl_url, if not 'use_file_system', URL of csv file
+    :params: zipped_filename: 'revised.csv',  name of the uncompressed file in zip archive
+    :params: csv_col_name: 'value',  # table column header name, mandatory
+    :params: 'num_rows': num list rows to calc in one loop for each process
+    :params: 'num_proc': procs to start, can be more or less than system CPU core count
     """
-    # auto
     mP = eisenmp.Mp()
+    mP.start(**modConf.__dict__)  # thread & processes start, attributes avail. for worker and feeder loop
+    mP.mp_print_q.put('\tDownload large list')
+    mP.mp_print_q.put(modConf.dl_url)
 
-    generator = number_generator()
-    mP.start(**modConf.__dict__)  # instance attributes available for worker and feeder loop
-    mP.run_q_feeder(generator=generator)  # also 'header_msg' modConf   header_msg='MAXIMUS_PRIME'
+    report_file = os.path.join(dir_name, 'download', 'report.zip')
+    downloader = download_report_zip_archive(mP, report_file)  # and prn msg
+    generator = g_use_fs_csv(report_file) if modConf.use_file_system else g_in_mem_csv(downloader)  # CSV generator
+    mP.run_q_feeder(generator=generator)
 
+    return mP
 
-def number_generator():
-    """Generates numbers from start count.
-    Has an end value, range.
-    """
-    range_num = modConf.range_num
-    n = modConf.n  # start with a large number to see some work in progress
-    for _ in range(range_num):
-        yield n
-        n += 1
 
-
-def worker_prime(toolbox):
+def g_in_mem_csv(downloader):
     """
-    - WORKER -      Called in a loop until returns False.
-
-    Start, Entry, Exit of this 'single' process worker.
-    We return True to get next list chunk, whatever object is in the rows.
-    Fed from mp_input_q to our toolbox. toolbox is our work instance with queues,
-    messages, list chunk, and work tools like language dictionary or hash list.
-
-    toolbox.foo, gives also access to all attributes and values
-    of the 'modConf.foo' instance, you have created
     """
-    # toolbox.mp_print_q.put(toolbox.say_hello)
-    busy = workload_get(toolbox)
-    calc_prime(toolbox)  # start worker function
-    if not busy:
-        return False
-    send_eta_data(toolbox)  # send data list, first row is header, info thread can find it in eisenmp.output_q_box
-    return True
+    archive = downloader.unzip_mem()
+    in_file = archive.open(modConf.zipped_filename, 'r')
+    dict_reader = csv.DictReader(TextIOWrapper(in_file, 'utf-8'))
+    generator = (column[modConf.csv_col_name] for column in dict_reader)
+    return generator
 
 
-def workload_get(toolbox):
-    """"""
-    while 1:
-        if not toolbox.mp_input_q.empty():
-            toolbox.next_lst = toolbox.mp_input_q.get()
-            break
-    if toolbox.stop_msg in toolbox.next_lst:  # eisenmp.iterator_loop() informs stop, no more lists
-        return False  # loop worker sends shutdown msg to next worker - generator is empty
-    return True
-
-
-def calc_prime(toolbox):
-    """Calc prime num.
+def g_use_fs_csv(report_file):
     """
-    remove_header(toolbox)
-
-    # calc
-    lst = toolbox.next_lst  # next_lst is default var for the new list in mp_input_q
-    stop_msg = toolbox.stop_msg  # string 'STOP'
-    prime_lst = [str(num) for num in lst if num is not stop_msg and type(num) is int and is_prime(num)]
-
-    # output result
-    result_lst = [toolbox.result_header_proc,  # result list, stored in 'eisenmp.output_q_box' dictionary
-                  prime_lst]
-    toolbox.mp_output_q.put(result_lst)  # result thread reads the header, if ok store result in a list
-
-    # print message
-    primes = ''.join(str(prime_lst)) if len(prime_lst) else ''
-    output_msg = f' ... Result {toolbox.worker_name} ... Prime {primes}'
-    toolbox.mp_print_q.put(output_msg) if len(prime_lst) else None  # blocks the whole mp
+    """
+    file_path = os.path.join(os.path.dirname(report_file), modConf.zipped_filename)
+    filename = open(file_path, 'r')
+    dict_reader = csv.DictReader(filename)
+    
+    generator = (column[modConf.csv_col_name] for column in dict_reader)
+    return generator
 
 
-def is_prime(n: int) -> bool:
-    """https://en.wikipedia.org/wiki/Primality_test
+def unzip_on_file_system(downloader, report_f):
     """
-    if n <= 3:
-        return n > 1
-    if n % 2 == 0 or n % 3 == 0:
-        return False
-    limit = isqrt(n)
-    for i in range(5, limit + 1, 6):
-        if n % i == 0 or n % (i + 2) == 0:
-            return False
-    return True
+    """
+    downloader.save(report_f)
+    with ZipFile(report_f, 'r') as un_zip:
+        un_zip.extractall(os.path.dirname(report_f))
 
 
-def send_eta_data(toolbox):
-    """list of [perf_header_eta, perf_current_eta] to ProcInfo, to calc arrival time ETA
+def download_report_zip_archive(mP, report_file):
     """
-    toolbox.perf_current_eta = len(toolbox.next_lst)
-    perf_lst = [toolbox.perf_header_eta + toolbox.worker_name,  # binary head
-                toolbox.perf_current_eta]
-    # disable info q will block all
-    toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from info_q, of all proc lists
-
+    """
+    mP.mp_print_q.put(origin_msg_create())
+    downloader = DownLoad()
+    downloader.url = modConf.url
+    downloader.zipped_filename = modConf.zipped_filename
+    downloader.load_url()  # now decide to read csv from mem or file
+    if modConf.use_file_system:
+        unzip_on_file_system(downloader, report_file)  # comment no dl
+    return downloader
 
-def remove_header(toolbox):
-    """Transport ticket with consecutive number.
-    Remove if no recreation of order is necessary.
-    Can reuse list for result, if rebuild order.
 
-    Use self.header_msg attribute to overwrite default header string
+def origin_msg_create():
+    """
     """
-    # toolbox.mp_print_q.put(toolbox.next_lst[0])
-    del toolbox.next_lst[0]  # remove header str
+    str_fs = 'WRITE_FILE_SYSTEM'
+    str_dl = 'LOAD_URL_UNZIP_READ_IN_MEM'
+    origin = str_fs if modConf.use_file_system else str_dl
+    origin_msg = f'\n\t{origin} [{modConf.zipped_filename}] [{modConf.csv_col_name}]' \
+                 f'\n\t~~~~~~~~~~~~~~~~\n'
+    return origin_msg
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
-    generator_prime()
+    mP = generator_calc_csv()
+    while 1:
+        # running threads, wait
+        if mP.begin_proc_shutdown:
+            break
+        time.sleep(1)
+
+    print(f'Time in sec: {round((time.perf_counter() - start))}')
 
-    print('Time in sec: ', round((time.perf_counter() - start)))
+    msg_result = e_utils.Result.result_dict
+    return msg_result
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_download.py` & `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import zipfile
 from io import BytesIO
 
-import eisenmp_examples.utils.eisenmp_utils as g_utils
+import eisenmp.utils_exa.eisenmp_utils as g_utils
 
 
 class DownLoad:
     """If we have the response, we can read it at once or as a stream.
 
     """
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_search.py` & `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 
-import eisenmp_examples.utils.eisenmp_utils as g_utils
+import eisenmp.utils_exa.eisenmp_utils as g_utils
 
 
 class SearchStr:
     """Hosts the dict to compare,
     and a 'search string shaker' generator.
 
     el cheapo goes brute force, but it shows the basics
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/utils/eisenmp_utils.py` & `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,18 @@
 
     :params: args: tuple of OS paths word list(s)
     :params: lower: True is all lowercase
     """
     word_list = []
     for arg in list(*list_paths):
         print(f' .. read wordlist {arg}')
-        with open(arg, 'r') as reader:
+        with open(arg, 'r', encoding="UTF-8") as reader:
             if lowercase:
                 stripped = [line.lower().rstrip() for line in reader.readlines()]  # remove \n
+                pass
             else:
                 stripped = [line.rstrip() for line in reader.readlines()]
             word_list.extend(stripped)
     return word_list
 
 
 def unzip(file_path):
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,17 +62,19 @@
     tbl_flt = [float(num) for num in lst if str(num) and 'nan' not in str(num) and num != stop_msg]
 
     average = 0
     if len(tbl_flt):  # calc with float type to get comma values
         average = sum([num for num in tbl_flt]) / len(tbl_flt)
     average = average if average else 0
 
-    result_lst = [toolbox.result_header_proc,  # result list for mp_output_q, collected in mp_output_q_box dictionary
+    # output result; result_header (to distinguish) header_msg (result dict name) worker_name (Process-1, name of proc)
+    header = toolbox.result_header
+    result_lst = [header,  # result list, stored in 'eisenmp.output_q_box' dictionary
                   average]
-    toolbox.mp_output_q.put(result_lst)
+    toolbox.mp_output_q.put(result_lst)  # result thread reads the header, if ok store result in a list
 
     output_msg = f' ... {toolbox.worker_name} ... [ average |{average}| ] of {len(toolbox.next_lst)} rows'
     toolbox.mp_print_q.put(output_msg)
 
     return busy
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_double.py` & `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_double.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,18 +51,21 @@
     toolbox.perf_current_eta = len(lst)
     perf_lst = [toolbox.perf_header_eta + toolbox.worker_name,  # binary head
                 toolbox.perf_current_eta]
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from mp_info_q, of all proc lists
 
 
 def send_result_msg(toolbox, *res_lst):
-    """"""
+    """
+    :params: toolbox:
+    :params: res_lst: list, res_lst = [row_aud, row_aud]
+    """
+    result_lst = [toolbox.result_header]
     for msg in res_lst:
-        result_lst = [toolbox.result_header_proc,  # result list, stored in 'eisenmp.output_q_box' dictionary
-                      msg]  # will crash the system mem, binaries
+        result_lst.append(msg)
         toolbox.mp_output_q.put(result_lst)
 
 
 def template_worker(toolbox, audio_chunk_lst, video_chunk_lst):
     """
     """
     busy = True
```

### Comparing `eisenmp_examples-0.2/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.2/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.3/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.2
+Version: 0.3
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.2/pyproject.toml` & `eisenmp_examples-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.2"
+version = "0.3"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "eisenmp multiprocess(or) example collection for server and mobiles"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
 requires-python = ">=3.7"
```

