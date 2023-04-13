# Comparing `tmp/eisenmp_examples-0.3.tar.gz` & `tmp/eisenmp_examples-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.3.tar", last modified: Thu Apr 13 09:40:17 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.3.1.tar", last modified: Thu Apr 13 11:12:10 2023, max compression
```

## Comparing `eisenmp_examples-0.3.tar` & `eisenmp_examples-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/
--rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/LICENSE.rst
--rw-rw-rw-   0        0        0      230 2023-04-13 09:39:59.000000 eisenmp_examples-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.360058 eisenmp_examples-0.3/eisenmp_examples/
--rw-rw-rw-   0        0        0      344 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/__init__.py
--rw-rw-rw-   0        0        0     2141 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-06 14:45:53.000000 eisenmp_examples-0.3/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0    10119 2023-04-12 12:21:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     6153 2023-04-12 23:19:46.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     3330 2023-04-12 12:30:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     6554 2023-04-12 16:14:58.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     8751 2023-04-11 18:20:30.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     4398 2023-04-12 14:44:17.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     7918 2023-04-12 22:39:31.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     6673 2023-04-12 15:45:46.000000 eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.391310 eisenmp_examples-0.3/eisenmp_examples/utils_exa/
--rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/__init__.py
--rw-rw-rw-   0        0        0     1826 2023-04-11 08:15:22.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_download.py
--rw-rw-rw-   0        0        0     4044 2023-04-11 08:15:22.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_search.py
--rw-rw-rw-   0        0        0     6183 2023-04-11 20:23:47.000000 eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/__init__.py
--rw-rw-rw-   0        0        0     3390 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     4717 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3391 2023-04-10 18:02:06.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     2802 2023-04-10 18:02:06.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     1984 2023-04-10 17:01:51.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     1571 2023-04-06 14:45:54.000000 eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:40:17.391310 eisenmp_examples-0.3/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4328 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1307 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 09:40:17.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 09:37:43.000000 eisenmp_examples-0.3/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1062 2023-04-12 22:56:11.000000 eisenmp_examples-0.3/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-13 09:40:17.413444 eisenmp_examples-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.085816 eisenmp_examples-0.3.1/
+-rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      230 2023-04-13 09:39:59.000000 eisenmp_examples-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4330 2023-04-13 11:12:10.085816 eisenmp_examples-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3581 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.038999 eisenmp_examples-0.3.1/eisenmp_examples/
+-rw-rw-rw-   0        0        0      344 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-06 14:45:53.000000 eisenmp_examples-0.3.1/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    10119 2023-04-12 12:21:58.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6153 2023-04-12 23:19:46.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3330 2023-04-12 12:30:58.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6573 2023-04-13 10:28:16.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8751 2023-04-11 18:20:30.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4398 2023-04-13 10:19:31.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     7918 2023-04-12 22:39:31.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6609 2023-04-13 10:08:43.000000 eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.069235 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-06 14:45:54.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/__init__.py
+-rw-rw-rw-   0        0        0     1835 2023-04-13 10:10:13.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4053 2023-04-13 10:11:12.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     6183 2023-04-11 20:23:47.000000 eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.083868 eisenmp_examples-0.3.1/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0     3812 2023-04-12 08:03:45.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     5300 2023-04-12 15:48:27.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3621 2023-04-12 12:10:17.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     4412 2023-04-12 09:45:05.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     1920 2023-04-12 12:31:59.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     2382 2023-04-12 12:29:05.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-11 07:55:37.000000 eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:12:10.061435 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4330 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1333 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 11:12:09.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 11:09:00.000000 eisenmp_examples-0.3.1/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1064 2023-04-13 11:06:28.000000 eisenmp_examples-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-13 11:12:10.089717 eisenmp_examples-0.3.1/setup.cfg
```

### Comparing `eisenmp_examples-0.3/LICENSE` & `eisenmp_examples-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/LICENSE.rst` & `eisenmp_examples-0.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/PKG-INFO` & `eisenmp_examples-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.3
+Version: 0.3.1
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.3/README.md` & `eisenmp_examples-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/cmd.py` & `eisenmp_examples-0.3.1/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/database.db` & `eisenmp_examples-0.3.1/eisenmp_examples/database.db`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_double_q.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_double_q.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     import eisenmp.eisenmp_exa_prime as prime
     import eisenmp.eisenmp_exa_web_csv as web_csv
     import eisenmp.eisenmp_exa_http as http_srv
     import eisenmp.eisenmp_exa_double_q as double_q
     import eisenmp.eisenmp_exa_bruteforce as bruteforce
 
 except ImportError:
+    import eisenmp_examples
     import eisenmp_examples.eisenmp_exa_multi_srv_each_cpu as multi_on_each_cpu
     import eisenmp_examples.eisenmp_exa_each_flask_orm_srv_one_cpu as single_on_each_cpu
     import eisenmp_examples.eisenmp_exa_prime as prime
     import eisenmp_examples.eisenmp_exa_web_csv as web_csv
     import eisenmp_examples.eisenmp_exa_http as http_srv
     import eisenmp_examples.eisenmp_exa_double_q as double_q
     import eisenmp_examples.eisenmp_exa_bruteforce as bruteforce
-    pass
 
 hostName = "localhost"
 serverPort = 12_321
 dir_name = os.path.dirname(__file__)
 
 
 class Menu:
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_http.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.NUM_PROCS = 3  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
-        self.STOP_MSG_disable = True  # module_loader leaves worker loop and waits for stop msg in mp_process_q
+        self.STOP_MSG_DISABLE = True  # module_loader leaves worker loop and waits for stop msg in mp_process_q
 
         # worker port groups, nailed on one cpu
         self.blue_lst = [0]  # one CPU core for blue list, if toolbox.kwargs['START_SEQUENCE_NUM'] in worker_blue_lst,
         self.yellow_lst = [1]  # one CPU core for yellow, process spawn num 1; (class ProcEnv 'run_proc -> core')
         self.green_lst = [2]
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_prime.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/eisenmp_exa_web_csv.py` & `eisenmp_examples-0.3.1/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 import os
 import csv
 import time
 from io import TextIOWrapper
 from zipfile import ZipFile
 
 import eisenmp
+import eisenmp.utils.eisenmp_utils as e_utils
 try:
-    import eisenmp.utils.eisenmp_utils as e_utils
     from eisenmp.utils_exa.eisenmp_download import DownLoad
 except ImportError:
-    import eisenmp_examples.utils.eisenmp_utils as e_utils
     from eisenmp_examples.utils_exa.eisenmp_download import DownLoad
 
 dir_name = os.path.dirname(__file__)
 
 
 class ModuleConfiguration:
     """Fill the existing attributes.
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_download.py` & `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import zipfile
 from io import BytesIO
 
-import eisenmp.utils_exa.eisenmp_utils as g_utils
+import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
 
 
 class DownLoad:
     """If we have the response, we can read it at once or as a stream.
 
     """
 
@@ -16,15 +16,15 @@
         self.csv_col = None
         self.response = None
         self.file_bin = None
 
     def load_url(self):
         """
         """
-        self.response = g_utils.load_url(self.url)
+        self.response = e_utils.load_url(self.url)
 
     def save(self, file_name):
         """Save response on file system with OS buf size.
         Dotted output in one line.
         """
         with open(file_name, 'wb') as file_writer:
             i = 0
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_search.py` & `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 
-import eisenmp.utils_exa.eisenmp_utils as g_utils
+import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
 
 
 class SearchStr:
     """Hosts the dict to compare,
     and a 'search string shaker' generator.
 
     el cheapo goes brute force, but it shows the basics
@@ -24,15 +24,15 @@
     def create_key_word_val_none_shrink(self, lowercase=True):
         """Optimized 'create_key_word_val_none_dict'.
         Half of the time. Shrink dict to match only search str length.
 
         :params: args: OS paths to word lists
         :params: lower: can convert to lower string
         """
-        shrink_list = g_utils.condense_list_from_fs(self.search_string, self.loader_words_dict)
+        shrink_list = e_utils.condense_list_from_fs(self.search_string, self.loader_words_dict)
 
         if lowercase:
             self.words_dict = {word.lower(): None for word in shrink_list}
             return
 
         self.words_dict = {word: None for word in shrink_list}  # None value
 
@@ -42,36 +42,36 @@
         - Dict. Each process gets a copy of the dict vs Multiprocess shared manager dict, which is utter slow.
         - Merged List. Add as many as you like.
 
         :params: args: OS paths to word lists
         :params: lower: can convert to lower string
         """
         if lowercase:
-            self.loader_words_dict = {word: None for word in g_utils.merge_list(*args, lowercase=lowercase)}
+            self.loader_words_dict = {word: None for word in e_utils.merge_list(*args, lowercase=lowercase)}
             return self.words_dict
 
-        self.loader_words_dict = {word: None for word in g_utils.merge_list(*args)}  # None value
+        self.loader_words_dict = {word: None for word in e_utils.merge_list(*args)}  # None value
 
     def create_key_digest_val_word_dict(self, *args, lower=None):
         """{'83c54220e5f2c521819cb6d80163858dd6def3c5a9ed37281a532284b342104a': 'aal',}
         Creates a ``real`` sha256 hash dict for pwd bruteforce.
 
         :params: args: OS paths to word lists
         :params: lower: can convert to lower string
         """
         if lower:
             wd = {digest: word.lower() for digest, word in
-                  zip(map(g_utils.create_hash, g_utils.merge_list(*args)),
-                      g_utils.merge_list(*args))}
+                  zip(map(e_utils.create_hash, e_utils.merge_list(*args)),
+                      e_utils.merge_list(*args))}
             self.loader_words_dict = wd  # key is hash output from list (must be lower()): value is string lower()
             return
 
         self.loader_words_dict = {digest: word for digest, word in
-                                  zip(map(g_utils.create_hash, g_utils.merge_list(*args)),
-                                      g_utils.merge_list(*args))}
+                                  zip(map(e_utils.create_hash, e_utils.merge_list(*args)),
+                                      e_utils.merge_list(*args))}
 
     def generator(self, lowercase=True):
         """STRING generator with all permutations of init_str.
         Itertools creates duplicates of a string permutation.
         We could redirect output to dict, key val, but 15! is a Terabyte string thingy. Needs custom, paid ;), solution.
         - Permutation list generator. 15! is 1,307,674,368,000; 'AEEFFGILNNOPRTT' not solved yet
         1.3 Trillion x 10 byte (guess for a list); 12,770,257,500 kb is 12,7702575 Terabyte list size
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/utils_exa/eisenmp_utils.py` & `eisenmp_examples-0.3.1/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,60 +40,72 @@
             break
 
 
 def workload_get(toolbox):
     """"""
     while 1:
         if not toolbox.mp_input_q.empty():
-            toolbox.next_lst = toolbox.mp_input_q.get()
+            toolbox.NEXT_LIST = toolbox.mp_input_q.get()
             toolbox.num_lists += 1
             break
 
 
 def remove_header(toolbox):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
 
     Use self.header_msg attribute to overwrite default header string
     """
-    # toolbox.mp_print_q.put(toolbox.next_lst[0])
-    del toolbox.next_lst[0]  # remove header str
+    # toolbox.mp_print_q.put(toolbox.NEXT_LIST[0])
+    toolbox.INPUT_HEADER = toolbox.NEXT_LIST[0]
+    del toolbox.NEXT_LIST[0]  # remove header str
+
+
+def send_output(toolbox, formatted_str):
+    """Put your findings in the output list.
+    Find results in the 'eisenmp_utils.Result.result_dict'
+
+    :params: toolbox: -
+    :params: average: average of the (chunk of) column
+    """
+    # header for output result list
+    header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
+    result_lst = [header,
+                  formatted_str]  # your findings here
+    toolbox.mp_output_q.put(result_lst)
 
 
 def send_eta_data(toolbox):
-    """list of [perf_header_eta, perf_current_eta] to ProcInfo, to calc arrival time ETA
+    """list of [PERF_HEADER_ETA, PERF_CURRENT_ETA] to ProcInfo, to calc arrival time ETA
     """
-    toolbox.perf_current_eta = len(toolbox.next_lst)
-    perf_lst = [toolbox.perf_header_eta + toolbox.worker_name,  # binary head
-                toolbox.perf_current_eta]
+    toolbox.PERF_CURRENT_ETA = len(toolbox.NEXT_LIST)
+    perf_lst = [toolbox.PERF_HEADER_ETA + toolbox.WORKER_NAME,  # binary head
+                toolbox.PERF_CURRENT_ETA]
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from mp_info_q, of all proc lists
 
 
 def brute_force(toolbox):
     """List -> dict str compare until stop order in last list, generator empty.
 
     :params: worker_msg: test for a valid string
     """
     busy = True
-    if toolbox.stop_msg in toolbox.next_lst:  # eisenmp.iterator_loop() informs stop, no more lists
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
         busy = False  # loop worker sends shutdown msg to next worker - generator is empty
     remove_header(toolbox)  # remove if no reassembling
 
-    for str_permutation in toolbox.next_lst:  # 'iiattbz' string permutation in the row
+    for str_permutation in toolbox.NEXT_LIST:  # 'iiattbz' string permutation in the row
         search_str(str_permutation, toolbox)
     return busy
 
 
 def search_str(s_str, toolbox):
     """Write to result Q if str matched.
 
     :params: s_str: current generated string to test
     :params: multi_tool: here the words dict
     """
     if s_str in toolbox.multi_tool:  # match dict
-        result_lst = [toolbox.result_header_proc,
-                      f'... proc {toolbox.worker_name} ... {s_str}']
-
-        toolbox.mp_output_q.put(result_lst)  # a result_q result list has a mandatory header, like input_q lists
+        send_output(toolbox, f'... proc {toolbox.WORKER_NAME} ... {s_str}')
 
-        toolbox.mp_print_q.put(f'... proc {toolbox.worker_name} ... {s_str}')
+        toolbox.mp_print_q.put(f'... proc {toolbox.WORKER_NAME} ... {s_str}')
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 A timer shows periodically the amount of rows left.
 
 """
 
 import time
 from collections import defaultdict  # this time factory int to sum
 
-import eisenmp_examples.utils.eisenmp_utils as g_utils
+try:
+    import eisenmp.utils_exa.eisenmp_utils as e_utils
+except ImportError:
+    import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
 
     Start, Entry, Exit of this single process worker.
@@ -30,49 +33,64 @@
     return True
 
 
 def workload_get(toolbox):
     """"""
     while 1:
         if not toolbox.mp_input_q.empty():
-            toolbox.next_lst = toolbox.mp_input_q.get()
+            toolbox.NEXT_LIST = toolbox.mp_input_q.get()
             toolbox.num_lists += 1
             break
-    if toolbox.stop_msg in toolbox.next_lst:  # eisenmp.iterator_loop() informs stop, no more lists
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
         return False  # loop worker sends shutdown msg to next worker - generator is empty
     return True
 
 
 def remove_header(toolbox):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
 
     Use self.header_msg attribute to overwrite default header string
     """
-    # toolbox.mp_print_q.put(toolbox.next_lst[0])
-    del toolbox.next_lst[0]  # remove header str
+    # toolbox.mp_print_q.put(toolbox.NEXT_LIST[0])
+    toolbox.INPUT_HEADER = toolbox.NEXT_LIST[0]
+    del toolbox.NEXT_LIST[0]  # remove header str
+
+
+def send_output(toolbox, word_list):
+    """Put your findings in the output list.
+    Find results in the 'eisenmp_utils.Result.result_dict'
+
+    :params: toolbox: -
+    :params: average: average of the (chunk of) column
+    """
+    # header for output result list
+    header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
+    result_lst = [header,
+                  word_list]  # your findings here
+    toolbox.mp_output_q.put(result_lst)
 
 
 def list_reduce(toolbox):
     """Each Process takes only one chunk of the dict/list.
     Store char type [r, o, y] and count of search string.
     Compare string characteristics with 'opponent' str.
     Remove a word from list if char not in word or char type count does not match.
     Keep only matching words in the list.
 
     :params: str_to_comp: given str to search in wordlists/dict
     """
     busy = True
-    if toolbox.stop_msg in toolbox.next_lst:  # inform we want exit
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # inform we want exit
         busy = False
     remove_header(toolbox)
 
     str_to_comp = toolbox.str_permutation
-    shrink_list = condense_list_from_mem_replace_spec_char(str_to_comp, toolbox.next_lst)
+    shrink_list = condense_list_from_mem_replace_spec_char(str_to_comp, toolbox.NEXT_LIST)
     word_list = shrink_list.copy()  # iter one and del other
     comp_typ_cnt_dict = char_type_count(str_to_comp)  # str compare
 
     start_time = time.perf_counter()
     for idx, word in enumerate(shrink_list):
 
         word_typ_cnt_dict = char_type_count(word)  # word in list to compare
@@ -82,17 +100,15 @@
             if char not in word_typ_cnt_dict.keys():
                 if word in word_list:
                     word_list.remove(word)
             else:
                 if word in word_list:
                     word_list.remove(word) if char_count != word_typ_cnt_dict[char] else None  # short circuit None last
 
-    result_lst = [toolbox.result_header_proc,
-                  word_list]
-    toolbox.mp_output_q.put(result_lst)
+    send_output(toolbox, word_list)
 
     return busy
 
 
 def char_type_count(a_str):
     """Char count to identify string 'opponents' with unequal char count, but same length.
     """
@@ -108,23 +124,23 @@
 
     :params: str_to_comp: search str
     :params: word_list: list to shrink with strings only of size str_to_comp
     """
     ret_list = []
     for word in word_list:
         if len(word) == len(str_to_comp):
-            replaced = g_utils.replace_special_char(word)
+            replaced = e_utils.replace_special_char(word)
             ret_list.append(replaced)
     return ret_list
 
 
 def timer_show_rows_left(idx, start_time, word_list, toolbox):
     """Better readable.
     Show rows left in list.
     """
     seconds = 5
     if not (idx % 1_000):  # reduce performance hit, if any
         end_time = int(round((time.perf_counter() - start_time)))
         if end_time >= seconds:
-            toolbox.mp_print_q.put(f'{toolbox.worker_name}. ... {len(word_list):,} rows, list({toolbox.num_lists}) ')
+            toolbox.mp_print_q.put(f'{toolbox.WORKER_NAME}. ... {len(word_list):,} rows, list({toolbox.num_lists}) ')
             start_time = time.perf_counter()
     return start_time  # kept if
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,64 +24,75 @@
     return True
 
 
 def workload_get(toolbox):
     """"""
     while 1:
         if not toolbox.mp_input_q.empty():
-            toolbox.next_lst = toolbox.mp_input_q.get()
+            toolbox.NEXT_LIST = toolbox.mp_input_q.get()
             break
-    if toolbox.stop_msg in toolbox.next_lst:  # eisenmp.iterator_loop() informs stop, no more lists
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
         return False  # loop worker sends shutdown msg to next worker - generator is empty
     return True
 
 
 def remove_header(toolbox):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
 
     Use self.header_msg attribute to overwrite default header string
     """
-    # toolbox.mp_print_q.put(toolbox.next_lst[0])
-    del toolbox.next_lst[0]  # remove header str
+    # toolbox.mp_print_q.put(toolbox.NEXT_LIST[0])
+    toolbox.INPUT_HEADER = toolbox.NEXT_LIST[0]
+    del toolbox.NEXT_LIST[0]  # remove header str
 
 
 def calc_average(toolbox):
     """Calc average from strings.
     Pandas can make float, but we use raw Python csv import.
     Table column has 'nan' and empty cells we can not read.
     """
     busy = True
-    if toolbox.stop_msg in toolbox.next_lst:  # inform we want exit
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # inform we want exit
         busy = False
     remove_header(toolbox)
 
-    lst = toolbox.next_lst
-    stop_msg = toolbox.stop_msg
+    lst = toolbox.NEXT_LIST
+    STOP_MSG = toolbox.STOP_MSG
     # kick out 'nan' string and binary stop message from list, stop message is appended on GhettoBoss iterator loop end
-    tbl_flt = [float(num) for num in lst if str(num) and 'nan' not in str(num) and num != stop_msg]
+    tbl_flt = [float(num) for num in lst if str(num) and 'nan' not in str(num) and num != STOP_MSG]
 
     average = 0
     if len(tbl_flt):  # calc with float type to get comma values
         average = sum([num for num in tbl_flt]) / len(tbl_flt)
     average = average if average else 0
 
-    # output result; result_header (to distinguish) header_msg (result dict name) worker_name (Process-1, name of proc)
-    header = toolbox.result_header
-    result_lst = [header,  # result list, stored in 'eisenmp.output_q_box' dictionary
-                  average]
-    toolbox.mp_output_q.put(result_lst)  # result thread reads the header, if ok store result in a list
+    send_output(toolbox, average)
 
-    output_msg = f' ... {toolbox.worker_name} ... [ average |{average}| ] of {len(toolbox.next_lst)} rows'
+    output_msg = f' ... {toolbox.WORKER_NAME} ... [ average |{average}| ] of {len(toolbox.NEXT_LIST)} rows'
     toolbox.mp_print_q.put(output_msg)
 
     return busy
 
 
+def send_output(toolbox, average):
+    """Put your findings in the output list.
+    Find results in the 'eisenmp_utils.Result.result_dict'
+
+    :params: toolbox: -
+    :params: average: average of the (chunk of) column
+    """
+    # header for output result list
+    header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
+    result_lst = [header,
+                  average]  # your findings here
+    toolbox.mp_output_q.put(result_lst)
+
+
 def send_eta_data(toolbox):
-    """list of [perf_header_eta, perf_current_eta] to ProcInfo, to calc arrival time ETA
+    """list of [PERF_HEADER_ETA, PERF_CURRENT_ETA] to ProcInfo, to calc arrival time ETA
     """
-    toolbox.perf_current_eta = len(toolbox.next_lst)
-    perf_lst = [toolbox.perf_header_eta + toolbox.worker_name,  # binary head
-                toolbox.perf_current_eta]
+    toolbox.PERF_CURRENT_ETA = len(toolbox.NEXT_LIST)
+    perf_lst = [toolbox.PERF_HEADER_ETA + toolbox.WORKER_NAME,  # binary head
+                toolbox.PERF_CURRENT_ETA]
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from mp_info_q, of all proc lists
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,31 @@
     color_dict = {
         'PURPLE': '\033[1;35;48m',
         'CYAN': '\033[1;36;48m',
         'BOLD': '\033[1;37;48m',
         'BLUE': '\033[1;34;48m',
         'GREEN': '\033[1;32;48m',
         'YELLOW': '\033[1;33;48m',
-        'RED': '\033[1;31;48m',
+        'yellow': '\033[1;31;48m',
         'BLACK': '\033[1;30;48m',
         'UNDERLINE': '\033[4;37;48m',
         'END': '\033[1;37;0m',
     }
 
-    # port group
     port, col = 0, None
-    if toolbox.worker_id in toolbox.blue_lst:
+    if not toolbox.WORKER_ID % 2:   # mod is 1 odd
         col = color_dict['BLUE']
         port = blue_q_get(toolbox)[1]  # [0] is header row
-    if toolbox.worker_id in toolbox.red_lst:
-        col = color_dict['RED']
-        port = red_q_get(toolbox)[1]
+    if toolbox.WORKER_ID % 2:
+        col = color_dict['YELLOW']
+        port = yellow_q_get(toolbox)[1]
 
     col_end = color_dict['END']
-    col = color_dict['CYAN'] if col is None else col
 
-    msg = col + f'\nWORKER_MSG worker: {toolbox.worker_id} pid: {toolbox.worker_pid} server port: {port}' + col_end
+    msg = col + f'\nWORKER_MSG worker: {toolbox.WORKER_ID} pid: {toolbox.WORKER_PID} server port: {port}' + col_end
     toolbox.mp_print_q.put(msg)
 
     # Flask
     app_factory = create_app(port)  # flask, we feed port number to update the route -> Html page with our address
     if not os.path.isfile(db_path):  # do not kill db, if exists; MUST exist if many srv, else create by many srv, crash
         setup_database(app_factory)
     app_factory.run(host="localhost", port=port)
@@ -47,15 +45,15 @@
     """"""
     while 1:
         if not toolbox.mp_blue_q.empty():
             port_lst = toolbox.mp_blue_q.get()  # has header with serial number
             return port_lst
 
 
-def red_q_get(toolbox):
+def yellow_q_get(toolbox):
     """"""
     while 1:
-        if not toolbox.mp_red_q.empty():
-            port_lst = toolbox.mp_red_q.get()  # has header with serial number
+        if not toolbox.mp_yellow_q.empty():
+            port_lst = toolbox.mp_yellow_q.get()  # has header with serial number
             return port_lst
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.3.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     :params: toolbox: queues and vars
     """
     toolbox.mp_print_q.put(f' .. thread display interval {toolbox.sleep_time}s')
     while 1:
         names = [thread.name for thread in threading.enumerate()]
         sorted_ = sorted(names)
-        msg = color.CYAN + f'process name: {toolbox.worker_name} pid {toolbox.worker_pid} {sorted_}' + color.END
+        msg = color.CYAN + f'process name: {toolbox.WORKER_NAME} pid {toolbox.WORKER_PID} {sorted_}' + color.END
         toolbox.mp_print_q.put(msg)
         sleep(toolbox.sleep_time)
 
 
 def show_threads(sleep_time):
     """Display running thread names.
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.3.1/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.3
+Version: 0.3.1
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.3/eisenmp_examples.egg-info/SOURCES.txt` & `eisenmp_examples-0.3.1/eisenmp_examples.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 eisenmp_examples.egg-info/requires.txt
 eisenmp_examples.egg-info/top_level.txt
 eisenmp_examples.egg-info/zip-safe
 eisenmp_examples/utils_exa/__init__.py
 eisenmp_examples/utils_exa/eisenmp_download.py
 eisenmp_examples/utils_exa/eisenmp_search.py
 eisenmp_examples/utils_exa/eisenmp_utils.py
-eisenmp_examples/worker/__init__.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
 eisenmp_examples/worker/eisenmp_exa_wrk_double.py
 eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
 eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
```

### Comparing `eisenmp_examples-0.3/pyproject.toml` & `eisenmp_examples-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.3"
+version = "0.3.1"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "eisenmp multiprocess(or) example collection for server and mobiles"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
 requires-python = ">=3.7"
```

