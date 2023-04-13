# Comparing `tmp/dr-buster-1.0.6.tar.gz` & `tmp/dr-buster-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kelj0/github/dr_buster/dist/tmpnw3eb3mj/dr-buster-1.0.6.tar", last modified: Tue Feb 23 22:12:36 2021, max compression
+gzip compressed data, was "dr-buster-1.0.7.tar", last modified: Thu Apr 13 14:04:27 2023, max compression
```

## Comparing `dr-buster-1.0.6.tar` & `dr-buster-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 kelj0     (1000) kelj0     (1000)        0 2021-02-23 22:12:36.000000 dr-buster-1.0.6/
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)     3002 2021-02-23 22:12:36.000000 dr-buster-1.0.6/PKG-INFO
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)     1880 2021-02-23 22:11:43.000000 dr-buster-1.0.6/README.md
-drwxr-xr-x   0 kelj0     (1000) kelj0     (1000)        0 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster/
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)        0 2021-02-23 21:11:06.000000 dr-buster-1.0.6/dr_buster/__init__.py
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)      367 2021-02-23 21:57:22.000000 dr-buster-1.0.6/dr_buster/__main__.py
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)     5335 2021-02-23 21:57:15.000000 dr-buster-1.0.6/dr_buster/core.py
-drwxr-xr-x   0 kelj0     (1000) kelj0     (1000)        0 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster.egg-info/
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)     3002 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster.egg-info/PKG-INFO
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)      237 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster.egg-info/SOURCES.txt
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)        1 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster.egg-info/dependency_links.txt
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)       10 2021-02-23 22:12:36.000000 dr-buster-1.0.6/dr_buster.egg-info/top_level.txt
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)      105 2021-02-23 21:10:07.000000 dr-buster-1.0.6/pyproject.toml
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)      602 2021-02-23 22:12:36.000000 dr-buster-1.0.6/setup.cfg
--rw-r--r--   0 kelj0     (1000) kelj0     (1000)       38 2021-02-23 21:14:30.000000 dr-buster-1.0.6/setup.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1062 2023-04-13 14:02:32.000000 dr-buster-1.0.7/LICENSE
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-13 14:04:27.883455 dr-buster-1.0.7/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1880 2023-04-13 14:02:32.000000 dr-buster-1.0.7/README.md
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/dr_buster/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/__init__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      367 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/__main__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     5962 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/core.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/dr_buster.egg-info/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      265 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/SOURCES.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        1 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/dependency_links.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       10 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/top_level.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      105 2023-04-13 14:02:32.000000 dr-buster-1.0.7/pyproject.toml
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      602 2023-04-13 14:04:27.883455 dr-buster-1.0.7/setup.cfg
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       38 2023-04-13 14:02:32.000000 dr-buster-1.0.7/setup.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/tests/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1643 2023-04-13 14:02:32.000000 dr-buster-1.0.7/tests/testserver.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dr-buster-1.0.6/PKG-INFO` & `dr-buster-1.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
-Description: # dr.buster
-        Simple, yet effective web path finder implemented with multiprocessing in Python
-        
-        ### Install
-        ```
-        pip3 install dr_buster
-        ```
-        
-        ### Module usage
-        ```py
-        from dr_buster.core import start_scan
-        
-        start_scan(url, wordlist_path)
-        ```
-        You will have a report generated after program finishes and you can parse it easy cause url and code is in `url [code]` format
-        
-        ### CLI usage
-        ```
-        $ python3 -m dr_buster https://example.com /home/user/wordlist.txt
-        
-        starts scan on example.com with wordlist wordlist.txt
-        and generates report dr.buster.report.$datetime$
-        ```
-        
-        ##### Example output when started with words.txt on testserver
-        ![alt text](res/usage.png)
-        
-        ##### Sample report
-        ```
-        user@hostname:~/dr.buster$ cat dr.buster.report.09-08-2020_10-54-28 
-        http://localhost:5000/900 [200]
-        http://localhost:5000/623 [200]
-        http://localhost:5000/500 [200]
-        http://localhost:5000/130 [200]
-        http://localhost:5000/904 [200]
-        http://localhost:5000/100 [200]
-        http://localhost:5000/504 [200]
-        http://localhost:5000/102 [200]
-        http://localhost:5000/103 [200]
-        http://localhost:5000/104 [200]
-        http://localhost:5000/600 [200]
-        http://localhost:5000/105 [200]
-        http://localhost:5000/200 [200]
-        http://localhost:5000/604 [200]
-        http://localhost:5000/700 [200]
-        http://localhost:5000/300 [200]
-        http://localhost:5000/703 [200]
-        http://localhost:5000/303 [200]
-        http://localhost:5000/800 [200]
-        http://localhost:5000/120 [200]
-        http://localhost:5000/770 [200]
-        http://localhost:5000/400 [200]
-        ```
-        
-        ### Test it out on testserver
-        ```
-        $ pip3 install flask
-        $ export FLASK_APP=testserver.py
-        $ python3 -m flask run
-        
-        and run dr.buster in another terminal
-        ```
-        
-        ## TODO:
-        * [x] - add argsparse
-        * [x] - add support for dirbusting on specific path
-        * [x] - create C++ version of dr.buster -> https://github.com/kelj0/dr.faster
-        
-        ##### DISCLAMER: I AM NOT RESPONSIBLE FOR ANY ACTIONS DONE WITH THIS SCRIPT, USE IT ONLY IF YOU HAVE PERMISSION
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dr.buster
+Simple, yet effective web path finder implemented with multiprocessing in Python
+
+### Install
+```
+pip3 install dr_buster
+```
+
+### Module usage
+```py
+from dr_buster.core import start_scan
+
+start_scan(url, wordlist_path)
+```
+You will have a report generated after program finishes and you can parse it easy cause url and code is in `url [code]` format
+
+### CLI usage
+```
+$ python3 -m dr_buster https://example.com /home/user/wordlist.txt
+
+starts scan on example.com with wordlist wordlist.txt
+and generates report dr.buster.report.$datetime$
+```
+
+##### Example output when started with words.txt on testserver
+![alt text](res/usage.png)
+
+##### Sample report
+```
+user@hostname:~/dr.buster$ cat dr.buster.report.09-08-2020_10-54-28 
+http://localhost:5000/900 [200]
+http://localhost:5000/623 [200]
+http://localhost:5000/500 [200]
+http://localhost:5000/130 [200]
+http://localhost:5000/904 [200]
+http://localhost:5000/100 [200]
+http://localhost:5000/504 [200]
+http://localhost:5000/102 [200]
+http://localhost:5000/103 [200]
+http://localhost:5000/104 [200]
+http://localhost:5000/600 [200]
+http://localhost:5000/105 [200]
+http://localhost:5000/200 [200]
+http://localhost:5000/604 [200]
+http://localhost:5000/700 [200]
+http://localhost:5000/300 [200]
+http://localhost:5000/703 [200]
+http://localhost:5000/303 [200]
+http://localhost:5000/800 [200]
+http://localhost:5000/120 [200]
+http://localhost:5000/770 [200]
+http://localhost:5000/400 [200]
+```
+
+### Test it out on testserver
+```
+$ pip3 install flask
+$ export FLASK_APP=testserver.py
+$ python3 -m flask run
+
+and run dr.buster in another terminal
+```
+
+## TODO:
+* [x] - add argsparse
+* [x] - add support for dirbusting on specific path
+* [x] - create C++ version of dr.buster -> https://github.com/kelj0/dr.faster
+
+##### DISCLAMER: I AM NOT RESPONSIBLE FOR ANY ACTIONS DONE WITH THIS SCRIPT, USE IT ONLY IF YOU HAVE PERMISSION
+
```

### Comparing `dr-buster-1.0.6/README.md` & `dr-buster-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dr-buster-1.0.6/dr_buster/core.py` & `dr-buster-1.0.7/dr_buster/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import itertools
 from socket import socket, gaierror, AF_INET, SOCK_STREAM
 from ssl import wrap_socket, SSLError, PROTOCOL_TLSv1_2
 from time import time
 from datetime import datetime
 from sys import exit
+import os
 from os.path import exists
 from multiprocessing import cpu_count, Process
 
 PROCESSES_COUNT = 32 if cpu_count() <= 4 else 64
 WORD_LISTS = []
 WORDLIST_PATH = ""
 URL = ""
 SSL_SUPPORTED = True
-TIME = datetime.now().strftime("%d-%m-%Y_%H-%M-%S")
 NOT_FOUND_CODE = 404
 
 def get_code(host, port, path):
     global SSL_SUPPORTED
     s = socket(AF_INET, SOCK_STREAM)
     response = None
     if path.startswith("/"):
@@ -115,49 +115,63 @@
     for p in range(PROCESSES_COUNT):
         if p == PROCESSES_COUNT - 1:
             WORD_LISTS.append(lines[start:])
         else:
             WORD_LISTS.append(lines[start:start+words_per_process])
         start+=words_per_process
 
-def scan_host(host, port, wordlist, process_id=None, path=""):
+def scan_host(host, port, wordlist, runtime, process_id=None, path=""):
     for word in wordlist:
         try:
             code = get_code(host, port, path+word)
         except Exception:
             print(host,port,path,word)
             exit(1)
         if code != NOT_FOUND_CODE and code != 400:
             print("%s:%s/%s%s returned [%s]!                \r" 
                     % ("http://"+host if not SSL_SUPPORTED else "https://"+host, port, path, word, code))
             finding = ("%s:%s/%s%s [%s]\n"
                     % ("http://"+host if not SSL_SUPPORTED else "https://"+host, port, path, word, code))
-            write_to_report(finding)
+            write_to_report(finding, runtime)
 
-def start_scan(url, wordlist_path):
+def start_scan(url, wordlist_path, runtime):
     global WORD_LISTS
     print("Starting scan on %s.." % (url,))
     host, port, path = parse_url(url)
     prepare_wordlists(wordlist_path)
     procs = []
     for n, wordlist in enumerate(WORD_LISTS):
-        procs.append(Process(target=scan_host, args=(host, port, wordlist, n+1, path)))
+        procs.append(Process(target=scan_host, args=(host, port, wordlist, runtime, n+1, path)))
     for p in procs:
         p.start()
     for p in procs:
         p.join()
 
-def write_to_report(finding):
-    fname = "./dr.buster.report."+TIME
+def write_to_report(finding, runtime):
+    fname = "./dr.buster.report."+runtime
     with open(fname, "a") as f:
         f.write(finding)
 
-def main(url, wordlist_path):
+def main(url, wordlist_path, cli_run=True):
+    '''
+        returns a path to the result of a scan
+        @url: url that you want to scan, it can be ip or an url to root, or to some specific path
+        @wordlist_path: provide a path to a wordlist that you want to use to scan that path
+        @cli_run: boolean, if True dr buster prints out results and findings, if False, runs silently 
+    '''
+    
     URL = url
     WORDLIST_PATH = wordlist_path
-    print("Starting Dr.buster..\nURL: %s \nWORDLIST: %s" % (URL, WORDLIST_PATH))
+    runtime = datetime.now().strftime("%d-%m-%Y_%H-%M-%S")
+    if cli_run:
+        print("Starting Dr.buster..\nURL: %s \nWORDLIST: %s" % (URL, WORDLIST_PATH))
     start_time = time()
-    start_scan(URL, WORDLIST_PATH)
+    start_scan(URL, WORDLIST_PATH, runtime)
     end_time = time()
-    print()
-    print("\nScanned %s paths in %s s." % (len(list(itertools.chain.from_iterable(WORD_LISTS))), end_time-start_time))
+    if cli_run:
+        print()
+        print("\nScanned %s paths in %s s." % (len(list(itertools.chain.from_iterable(WORD_LISTS))), end_time-start_time))
+    
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    
+    return os.path.join(dir_path, f"dr.buster.report.{runtime}")
```

### Comparing `dr-buster-1.0.6/dr_buster.egg-info/PKG-INFO` & `dr-buster-1.0.7/dr_buster.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
-Description: # dr.buster
-        Simple, yet effective web path finder implemented with multiprocessing in Python
-        
-        ### Install
-        ```
-        pip3 install dr_buster
-        ```
-        
-        ### Module usage
-        ```py
-        from dr_buster.core import start_scan
-        
-        start_scan(url, wordlist_path)
-        ```
-        You will have a report generated after program finishes and you can parse it easy cause url and code is in `url [code]` format
-        
-        ### CLI usage
-        ```
-        $ python3 -m dr_buster https://example.com /home/user/wordlist.txt
-        
-        starts scan on example.com with wordlist wordlist.txt
-        and generates report dr.buster.report.$datetime$
-        ```
-        
-        ##### Example output when started with words.txt on testserver
-        ![alt text](res/usage.png)
-        
-        ##### Sample report
-        ```
-        user@hostname:~/dr.buster$ cat dr.buster.report.09-08-2020_10-54-28 
-        http://localhost:5000/900 [200]
-        http://localhost:5000/623 [200]
-        http://localhost:5000/500 [200]
-        http://localhost:5000/130 [200]
-        http://localhost:5000/904 [200]
-        http://localhost:5000/100 [200]
-        http://localhost:5000/504 [200]
-        http://localhost:5000/102 [200]
-        http://localhost:5000/103 [200]
-        http://localhost:5000/104 [200]
-        http://localhost:5000/600 [200]
-        http://localhost:5000/105 [200]
-        http://localhost:5000/200 [200]
-        http://localhost:5000/604 [200]
-        http://localhost:5000/700 [200]
-        http://localhost:5000/300 [200]
-        http://localhost:5000/703 [200]
-        http://localhost:5000/303 [200]
-        http://localhost:5000/800 [200]
-        http://localhost:5000/120 [200]
-        http://localhost:5000/770 [200]
-        http://localhost:5000/400 [200]
-        ```
-        
-        ### Test it out on testserver
-        ```
-        $ pip3 install flask
-        $ export FLASK_APP=testserver.py
-        $ python3 -m flask run
-        
-        and run dr.buster in another terminal
-        ```
-        
-        ## TODO:
-        * [x] - add argsparse
-        * [x] - add support for dirbusting on specific path
-        * [x] - create C++ version of dr.buster -> https://github.com/kelj0/dr.faster
-        
-        ##### DISCLAMER: I AM NOT RESPONSIBLE FOR ANY ACTIONS DONE WITH THIS SCRIPT, USE IT ONLY IF YOU HAVE PERMISSION
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dr.buster
+Simple, yet effective web path finder implemented with multiprocessing in Python
+
+### Install
+```
+pip3 install dr_buster
+```
+
+### Module usage
+```py
+from dr_buster.core import start_scan
+
+start_scan(url, wordlist_path)
+```
+You will have a report generated after program finishes and you can parse it easy cause url and code is in `url [code]` format
+
+### CLI usage
+```
+$ python3 -m dr_buster https://example.com /home/user/wordlist.txt
+
+starts scan on example.com with wordlist wordlist.txt
+and generates report dr.buster.report.$datetime$
+```
+
+##### Example output when started with words.txt on testserver
+![alt text](res/usage.png)
+
+##### Sample report
+```
+user@hostname:~/dr.buster$ cat dr.buster.report.09-08-2020_10-54-28 
+http://localhost:5000/900 [200]
+http://localhost:5000/623 [200]
+http://localhost:5000/500 [200]
+http://localhost:5000/130 [200]
+http://localhost:5000/904 [200]
+http://localhost:5000/100 [200]
+http://localhost:5000/504 [200]
+http://localhost:5000/102 [200]
+http://localhost:5000/103 [200]
+http://localhost:5000/104 [200]
+http://localhost:5000/600 [200]
+http://localhost:5000/105 [200]
+http://localhost:5000/200 [200]
+http://localhost:5000/604 [200]
+http://localhost:5000/700 [200]
+http://localhost:5000/300 [200]
+http://localhost:5000/703 [200]
+http://localhost:5000/303 [200]
+http://localhost:5000/800 [200]
+http://localhost:5000/120 [200]
+http://localhost:5000/770 [200]
+http://localhost:5000/400 [200]
+```
+
+### Test it out on testserver
+```
+$ pip3 install flask
+$ export FLASK_APP=testserver.py
+$ python3 -m flask run
+
+and run dr.buster in another terminal
+```
+
+## TODO:
+* [x] - add argsparse
+* [x] - add support for dirbusting on specific path
+* [x] - create C++ version of dr.buster -> https://github.com/kelj0/dr.faster
+
+##### DISCLAMER: I AM NOT RESPONSIBLE FOR ANY ACTIONS DONE WITH THIS SCRIPT, USE IT ONLY IF YOU HAVE PERMISSION
+
```

### Comparing `dr-buster-1.0.6/setup.cfg` & `dr-buster-1.0.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dr-buster
-version = 1.0.6
+version = 1.0.7
 author = kelj0
 author_email = kelj0@protonmail.com
 description = Simple, yet effective web path finder implemented with multiprocessing in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kelj0/dr_buster
 project_urls =
```

