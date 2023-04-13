# Comparing `tmp/eisenmp-0.9.3.tar.gz` & `tmp/eisenmp-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp-0.9.3.tar", last modified: Sun Apr  2 22:14:48 2023, max compression
+gzip compressed data, was "eisenmp-0.9.5.tar", last modified: Thu Apr 13 09:03:18 2023, max compression
```

## Comparing `eisenmp-0.9.3.tar` & `eisenmp-0.9.5.tar`

### file list

```diff
@@ -1,25 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 22:14:48.443666 eisenmp-0.9.3/
--rw-rw-rw-   0        0        0     1525 2023-04-02 21:34:17.000000 eisenmp-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-02 21:34:17.000000 eisenmp-0.9.3/LICENSE.rst
--rw-rw-rw-   0        0        0      187 2023-04-02 21:34:17.000000 eisenmp-0.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9549 2023-04-02 22:14:48.443666 eisenmp-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     7021 2023-04-02 21:34:17.000000 eisenmp-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 22:14:48.401320 eisenmp-0.9.3/eisenmp/
--rw-rw-rw-   0        0        0     3896 2023-04-02 21:52:23.000000 eisenmp-0.9.3/eisenmp/__init__.py
--rw-rw-rw-   0        0        0     6260 2023-04-02 21:34:17.000000 eisenmp-0.9.3/eisenmp/eisenmp_procenv.py
--rw-rw-rw-   0        0        0     8639 2023-04-02 21:52:23.000000 eisenmp-0.9.3/eisenmp/eisenmp_q_coll.py
--rw-rw-rw-   0        0        0     5048 2023-04-02 21:52:23.000000 eisenmp-0.9.3/eisenmp/eisenmp_worker_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-02 22:14:48.441712 eisenmp-0.9.3/eisenmp/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 21:34:17.000000 eisenmp-0.9.3/eisenmp/utils/__init__.py
--rw-rw-rw-   0        0        0      464 2023-04-02 22:08:55.000000 eisenmp-0.9.3/eisenmp/utils/eisenmp_constants.py
--rw-rw-rw-   0        0        0     3898 2023-04-02 21:34:17.000000 eisenmp-0.9.3/eisenmp/utils/eisenmp_info.py
--rw-rw-rw-   0        0        0     1377 2023-04-02 21:34:17.000000 eisenmp-0.9.3/eisenmp/utils/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-02 22:14:48.435860 eisenmp-0.9.3/eisenmp.egg-info/
--rw-rw-rw-   0        0        0     9549 2023-04-02 22:14:48.000000 eisenmp-0.9.3/eisenmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-02 22:14:48.000000 eisenmp-0.9.3/eisenmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 22:14:48.000000 eisenmp-0.9.3/eisenmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-02 22:14:48.000000 eisenmp-0.9.3/eisenmp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-02 22:14:48.000000 eisenmp-0.9.3/eisenmp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-02 22:14:47.000000 eisenmp-0.9.3/eisenmp.egg-info/zip-safe
--rw-rw-rw-   0        0        0      921 2023-04-02 21:59:43.000000 eisenmp-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0      392 2023-04-02 22:14:48.451465 eisenmp-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.427952 eisenmp-0.9.5/
+-rw-rw-rw-   0        0        0     1525 2023-04-06 10:49:51.000000 eisenmp-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-06 10:49:51.000000 eisenmp-0.9.5/LICENSE.rst
+-rw-rw-rw-   0        0        0      187 2023-04-06 10:49:51.000000 eisenmp-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9965 2023-04-13 09:03:18.427952 eisenmp-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7437 2023-04-13 00:15:44.000000 eisenmp-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.265143 eisenmp-0.9.5/docs/
+-rw-rw-rw-   0        0        0      756 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.349815 eisenmp-0.9.5/docs/source/
+-rw-rw-rw-   0        0        0     6979 2023-04-12 21:34:45.000000 eisenmp-0.9.5/docs/source/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.349815 eisenmp-0.9.5/docs/source/_static/
+-rw-rw-rw-   0        0        0      458 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/source/_static/css-style.css
+-rw-rw-rw-   0        0        0     3283 2023-04-12 21:37:25.000000 eisenmp-0.9.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2504 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.rst
+-rw-rw-rw-   0        0        0      747 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.utils.rst
+-rw-rw-rw-   0        0        0      806 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.utils_exa.rst
+-rw-rw-rw-   0        0        0    27208 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/source/eisenmp_logo.png
+-rw-rw-rw-   0        0        0      237 2023-04-12 20:26:08.000000 eisenmp-0.9.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0       65 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.381082 eisenmp-0.9.5/eisenmp/
+-rw-rw-rw-   0        0        0     4471 2023-04-12 16:40:53.000000 eisenmp-0.9.5/eisenmp/__init__.py
+-rw-rw-rw-   0        0        0     7399 2023-04-12 19:09:27.000000 eisenmp-0.9.5/eisenmp/eisenmp_procenv.py
+-rw-rw-rw-   0        0        0    10522 2023-04-11 18:12:16.000000 eisenmp-0.9.5/eisenmp/eisenmp_q_coll.py
+-rw-rw-rw-   0        0        0     5401 2023-04-12 09:25:01.000000 eisenmp-0.9.5/eisenmp/eisenmp_worker_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.427952 eisenmp-0.9.5/eisenmp/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:49:51.000000 eisenmp-0.9.5/eisenmp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-10 16:30:06.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_constants.py
+-rw-rw-rw-   0        0        0     3918 2023-04-10 10:29:05.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_info.py
+-rw-rw-rw-   0        0        0     1434 2023-04-11 11:41:34.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.412341 eisenmp-0.9.5/eisenmp.egg-info/
+-rw-rw-rw-   0        0        0     9965 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 09:03:17.000000 eisenmp-0.9.5/eisenmp.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      921 2023-04-12 20:36:14.000000 eisenmp-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0      392 2023-04-13 09:03:18.443591 eisenmp-0.9.5/setup.cfg
```

### Comparing `eisenmp-0.9.3/LICENSE` & `eisenmp-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.3/LICENSE.rst` & `eisenmp-0.9.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.3/PKG-INFO` & `eisenmp-0.9.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.3
+Version: 0.9.5
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
         
@@ -44,90 +44,118 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: LICENSE.rst
 
 # eisenmp
  
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
+Python 3.7 
+[Multiprocessor](https://en.wikipedia.org/wiki/Multiprocessing)
 [Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
 
+Forget about pools, swim in the sea.
+
 Features:
 
-* Load modules from Network or FS. Load **multi, independent and before a worker** into ➜ Process
-* Run every Python generator on _every_ CPU core, enable auto collect results
-* Load a fixed number of servers into each process
-* Build port groups with CPU cores and network adapters
-* Create **categories of Queues**, read them with **all custom vars** in a **ToolBox** dictionary, used by the worker
+* Create **uniform** multiprocess programs for your projects
+* Calculate your Python generator output on _every_ CPU core
+* Worker **module_loader** decouples your Worker imports from Main()
+* **auto Exit** of worker and process
+* Start methods, **spawn**, **fork** and **forkserver**
+* Create VM_ware like **port groups** on CPU cores and stream with (tcp/http) maximum speed via selected NIC adapters
+* Process **START_SEQUENCE_NUM** Worker on a CPU core can grab a specific queue 0=red_q, 1=blue_q,2=yellow_q
+* **Categories of Queues**, read them with **all custom vars** in a worker **ToolBox** dictionary
 * no libraries, light weight; (Linux, Windows)
-* [Examples](https://github.com/44xtc44/eisenmp_examples) 
-flask_orm_user_db, web_csv_large-list, brute_force_attack, double_queue_feeding, multi_srv_ ...
-* All scenarios follow the **Template style** and have descriptions
-
-Workplace:
-* Server or mobile device
-
-Note:
-Generator prod. 1, 2, 3, 4, 5  ➜ we make Worker chunks, [los](https://de.wikipedia.org/wiki/Los_(Produktion))
-[1,2] [3,4] [5] lists. Each process worker gets one.
 
+Visit the features above in the
+[Examples gitHub repository](https://github.com/44xtc44/eisenmp_examples), 
+or get the [Examples PyPi package](https://pypi.org/project/eisenmp-examples/),
+run 
+
+    eisenmp_url 
+    or 
+    eisenmp_menu
+simpleHTTP Ajax server, or terminal menu
 
-### min. ToDo
+All scenarios run on **reusable Template Modules**. Enjoy the descriptions and discover.
 
-Generator - iterator chunks on every CPU core:
-- (A) Mngr(): **Every generator** yield, or generator expression
-- (B) Wkr(): The **worker** wants a loop. Return True, get the next chunk or False for **auto exit worker and process**.
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (D) Mngr(): default call: **iterator** ...raid.run_q_feeder(generator=your generator), runs also on ➜ assigned queues
+## How it works
+You write two functions and two modules.
+Let's call 'em **Generator.py** and **Worker.py**.
 
-One Server (or more) on every CPU core:
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (C.1) Wkr(): The **worker module** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
-- (C.2) Wkr(): The **worker module** starts **MANY** server. All server starts must be threads **stop_msg_disable=True**
-- Server reads queues: Needs (A) Mngr and (D) Mngr
-- **Port groups** (applications, server): map **toolbox.worker_id**
-'s ➜ to server ports on CPU cores ➜ to an IP address
+1. Generator.py starts a new process, _but_ the target is **module_loader.py** (loader).
+2. loader imports your (independent) Worker.py module from file system. 
+This makes sure that only imports of the worker.py module are loaded, without side effects.
+3. loader sits in a loop and calls your Worker.py entry function endless. Until there is no more work in the queues.
+This loop keeps the process alive.
+4. **q_feeder** iterator sends a STOP Worker message with the last chunk. Your Worker reads STOP, return False and exit. 
+5. The **module loader** then puts a STOP Worker message in all other input queues.
+Loader runs idle and awaits the internal STOP Process message. **Next** Worker reads STOP, exit ...
 
-## How it works
-Needs one **Caller (Mngr)** and one **Worker** fun() in the module for simple tasks.
-- ModuleConfiguration class collects data variables as default and custom variables in a **modConf** instance
-- Mngr fun() updates eisenmp with the **modConf** instance dictionary
-- create **custom Queue**s, either single named in a dict or as dict with category names for easy deployment
-- eisenmp threaded method **run_q_feeder** can be called multiple times to fill the worker Queues with generator output
-
-The loader imports **arbitrary** modules. Iterator loop threads (option) put work chunks in queues.
-The **first registered module function**, the worker, is called in an **endless loop**, as long as it exits after 
-each own cycle. Microcontroller style. It is the **last loaded module**.
-
-Following modules in the register list (LIFO) execute a thread start function to not block the Worker module. 
-They may control the worker and have access to its started instances references (offset address). 
-main(), Parent Process has no access in Child Processes. 
-It needs any help it can get. We use 'spawn' multiprocessing.
-See also the watchdog threaded module in the [Examples](https://github.com/44xtc44/eisenmp_examples) , please.
+Default ``six Queues``
+- ``Input`` worker lists, ``Output`` result and stop lists, ``Process`` shutdown
+- ``Tools``, ``Print``, ``Info``
 
-Use Server only, set **stop_msg_disable=True**. This allows to use threaded modules only.
+### In detail:
 
-Generator output can be any data type (int, str, response stream chunks, floats) as long as it is delivered by a 
-[generator function (yield)](https://docs.python.org/3/reference/expressions.html#yieldexpr)
+Generator - iterator chunks on every CPU core:
+- [Generator yield](https://docs.python.org/3/reference/expressions.html#yieldexpr)
 or 
-[(generator expression)](https://peps.python.org/pep-0289/)
+[(expression)](https://peps.python.org/pep-0289/)
+output 1, 2, 3, 4, 5 ➜ eisenmp iterator list [ [1,2] [3,4] [5] ] ➜ **NUM_ROWS** chunks for your Worker
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker in (also) a list. 
+- (B) Mngr(): Assign Worker load and process count.
+- (C) Mngr(): Call **iterator** run_q_feeder(generator=Mngr generator)
+- (D) Wkr(): Loop over **NUM_ROWS** list chunks. Return False to **auto exit worker and process**, or get next chunk 
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
 
+One Server (or more) on every CPU core:
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
+- (D.1) Wkr(): The **worker** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
+- (D.2) Wkr(): The **worker** starts **MANY** server. Server start call must be threaded, set **STOP_MSG_DISABLE=True**
+- Server read queues: Follow the Generator todo
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
+
+Port groups:
+- Map **START_SEQUENCE_NUM**'s ➜ to multiple (server) ports on CPU cores ➜ to an IP address, 
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
 
-Default ``six Queues``
-- ``Input`` serial number header, ``Output`` result and stop lists w. header, ``Process`` shutdown
-- ``Tools``, ``Print``, ``Info``
 
-Default means **ready to use**:
-- **mp_input_q** lists have a header with a **serial number** to be able to recreate the original order of chunks
+### ready to use:
+- **run_q_feeder()** iterator lists get a **serial number** header to recreate the original order of chunks
 - **mp_tools_q** for big tools stuff delivery to every single Worker proc module;
 It may be a 27GB rainbow table; See the bruteforce (small) example, please
-- Output **can** be stored if **store_result** is set in config
+- Output **can** be stored if **RESULTS_STORE** is set in config
+
+
+## Issues
+eisenmp can run on Python 3.6 (Ubuntu test), but not the samples.
 
 ## How to run the examples?
-Clone the repo [Examples](https://github.com/44xtc44/eisenmp_examples) and ``run an eisenmp_exa_...``.
+Most easy is PyPi package mentioned above. **eisenmp** will be installed also.
+
+Clone both repos.
+[eisenmp](https://github.com/44xtc44/eisenmp) and
+[eisenmp_examples](https://github.com/44xtc44/eisenmp_examples)
+
+Install in editable pip mode.
+
+    cd eisenmp 
+    pip3 install -e .  # uninstall (linux pip3) with: pip3 uninstall eisenmp
+
+    cd eisenmp_examples
+    pip3 install -e .  # uninstall with: pip3 uninstall eisenmp_examples
+Run the examples.
+ 
+    eisenmp_url
+    # or
+    eisenmp_menu
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
 
 	[BRUTE_FORCE]	cfhhilorrs
```

### Comparing `eisenmp-0.9.3/README.md` & `eisenmp-0.9.5/docs/source/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,90 @@
 # eisenmp
+#########
  
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
-[Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
+Python 3.7
+
+`Multiprocessor <https://en.wikipedia.org/wiki/Multiprocessing>`_
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for Server and Mobiles
+
+Forget about pools, swim in the sea.
 
 Features:
 
-* Load modules from Network or FS. Load **multi, independent and before a worker** into ➜ Process
-* Run every Python generator on _every_ CPU core, enable auto collect results
-* Load a fixed number of servers into each process
-* Build port groups with CPU cores and network adapters
-* Create **categories of Queues**, read them with **all custom vars** in a **ToolBox** dictionary, used by the worker
+* Create **uniform** multiprocess programs for your projects
+* Calculate your Python generator output on _every_ CPU core
+* Worker **module_loader** decouples your Worker imports from Main()
+* **auto Exit** of worker and process
+* Start methods, **spawn**, **fork** and **forkserver**
+* Create **port groups** on CPU cores and connect network adapters
+* Process **START_SEQUENCE_NUM** Worker on a CPU core can grab a specific queue 0=red_q, 1=blue_q, 2=yellow_q
+* **Categories of Queues**, read them with **all custom vars** in a worker **ToolBox** dictionary
+* Visit the features above in the
+`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
+or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_,
+run **eisenmp_url** simpleHTTP Ajax server
+* All scenarios run on **reusable Template Modules**. Enjoy the descriptions and discover.
 * no libraries, light weight; (Linux, Windows)
-* [Examples](https://github.com/44xtc44/eisenmp_examples) 
-flask_orm_user_db, web_csv_large-list, brute_force_attack, double_queue_feeding, multi_srv_ ...
-* All scenarios follow the **Template style** and have descriptions
 
-Workplace:
-* Server or mobile device
+## How it works
+You write two functions and two modules.
+Let's call 'em **Generator.py** and **Worker.py**.
 
-Note:
-Generator prod. 1, 2, 3, 4, 5  ➜ we make Worker chunks, [los](https://de.wikipedia.org/wiki/Los_(Produktion))
-[1,2] [3,4] [5] lists. Each process worker gets one.
+1. Generator.py starts a new process, _but_ the target is **module_loader.py** (loader).
+2. loader imports your (independent) Worker.py module from file system. 
+This makes sure that only imports of the worker.py module are loaded, without side effects.
+3. loader sits in a loop and calls your Worker.py entry function endless. Until there is no more work in the queues.
+This loop keeps the process alive.
+4. **q_feeder** iterator sends a STOP Worker message with the last chunk. Your Worker reads STOP, return False and exit. 
+5. The **module loader** then puts a STOP Worker message in all other input queues.
+Loader runs idle and awaits the internal STOP Process message. **Next** Worker reads STOP, exit ...
 
+Default ``six Queues``
+- ``Input`` worker lists, ``Output`` result and stop lists, ``Process`` shutdown
+- ``Tools``, ``Print``, ``Info``
 
-### min. ToDo
+### In detail:
 
 Generator - iterator chunks on every CPU core:
-- (A) Mngr(): **Every generator** yield, or generator expression
-- (B) Wkr(): The **worker** wants a loop. Return True, get the next chunk or False for **auto exit worker and process**.
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (D) Mngr(): default call: **iterator** ...raid.run_q_feeder(generator=your generator), runs also on ➜ assigned queues
-
-One Server (or more) on every CPU core:
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (C.1) Wkr(): The **worker module** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
-- (C.2) Wkr(): The **worker module** starts **MANY** server. All server starts must be threads **stop_msg_disable=True**
-- Server reads queues: Needs (A) Mngr and (D) Mngr
-- **Port groups** (applications, server): map **toolbox.worker_id**
-'s ➜ to server ports on CPU cores ➜ to an IP address
-
-## How it works
-Needs one **Caller (Mngr)** and one **Worker** fun() in the module for simple tasks.
-- ModuleConfiguration class collects data variables as default and custom variables in a **modConf** instance
-- Mngr fun() updates eisenmp with the **modConf** instance dictionary
-- create **custom Queue**s, either single named in a dict or as dict with category names for easy deployment
-- eisenmp threaded method **run_q_feeder** can be called multiple times to fill the worker Queues with generator output
-
-The loader imports **arbitrary** modules. Iterator loop threads (option) put work chunks in queues.
-The **first registered module function**, the worker, is called in an **endless loop**, as long as it exits after 
-each own cycle. Microcontroller style. It is the **last loaded module**.
-
-Following modules in the register list (LIFO) execute a thread start function to not block the Worker module. 
-They may control the worker and have access to its started instances references (offset address). 
-main(), Parent Process has no access in Child Processes. 
-It needs any help it can get. We use 'spawn' multiprocessing.
-See also the watchdog threaded module in the [Examples](https://github.com/44xtc44/eisenmp_examples) , please.
-
-Use Server only, set **stop_msg_disable=True**. This allows to use threaded modules only.
-
-Generator output can be any data type (int, str, response stream chunks, floats) as long as it is delivered by a 
-[generator function (yield)](https://docs.python.org/3/reference/expressions.html#yieldexpr)
+- `Generator yield <https://docs.python.org/3/reference/expressions.html#yieldexpr>`_
 or 
-[(generator expression)](https://peps.python.org/pep-0289/)
+[(expression)](https://peps.python.org/pep-0289/)
+output 1, 2, 3, 4, 5 ➜ eisenmp iterator list [ [1,2] [3,4] [5] ] ➜ **NUM_ROWS** chunks for your Worker
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker in (also) a list. 
+- (B) Mngr(): Assign Worker load and process count.
+- (C) Mngr(): Call **iterator** run_q_feeder(generator=Mngr generator)
+- (D) Wkr(): Loop over **NUM_ROWS** list chunks. Return False to **auto exit worker and process**, or get next chunk 
+`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
+or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
 
+One Server (or more) on every CPU core:
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
+- (D.1) Wkr(): The **worker** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
+- (D.2) Wkr(): The **worker** starts **MANY** server. Server start call must be threaded, set **STOP_MSG_DISABLE=True**
+- Server read queues: Follow the Generator todo
+`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
+or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
+
+Port groups:
+- Map **toolbox.WORKER_ID**'s ➜ to server ports on CPU cores ➜ to an IP address, 
+`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
+or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
 
-Default ``six Queues``
-- ``Input`` serial number header, ``Output`` result and stop lists w. header, ``Process`` shutdown
-- ``Tools``, ``Print``, ``Info``
-
-Default means **ready to use**:
-- **mp_input_q** lists have a header with a **serial number** to be able to recreate the original order of chunks
+### ready to use:
+- **run_q_feeder()** iterator lists get a **serial number** header to recreate the original order of chunks
 - **mp_tools_q** for big tools stuff delivery to every single Worker proc module;
 It may be a 27GB rainbow table; See the bruteforce (small) example, please
-- Output **can** be stored if **store_result** is set in config
+- Output **can** be stored if **RESULTS_STORE** is set in config
+
+
+## Issues
+eisenmp can run on Python 3.6 (Ubuntu test), but not the samples.
 
 ## How to run the examples?
-Clone the repo [Examples](https://github.com/44xtc44/eisenmp_examples) and ``run an eisenmp_exa_...``.
+Clone the repo [Examples gitHub](https://github.com/44xtc44/eisenmp_examples) and ``run an eisenmp_exa_...``.
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
 
 	[BRUTE_FORCE]	cfhhilorrs
@@ -131,15 +136,15 @@
     Inbuild example, assert a scrambled string. Use brute force or condensing.
     We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
     (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
         Permutation lists grow very fast, reaching Terabyte size.
     (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
 
 `eisenmp` uses Pythons permutation generator
- [itertools](https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations)
+ `itertools <https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations>`_
 for the brute force attack example.
 
     Another example downloads a large list and calculates average for one column.
     Python CSV extracts the column and we calculate the average with the assigned number
     of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
```

### Comparing `eisenmp-0.9.3/eisenmp/__init__.py` & `eisenmp-0.9.5/eisenmp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A Python ``multiprocess, multi CPU`` module.
 An example function cracks a game quest.
 
     ::
 
     Inheritance - proc: ProcEnv -> QueueCollect -> Mp
-        Create Queue/Process -> Collect messages in boxes -> Manage, feed
+        Create Queue/Process -> Collect messages in boxes -> Manage, feed queues
 
     Thread names are in ProcEnv:
         QueueCollect [print_q, output_q, input_q, tools_q, info_q],
         GhettoGang [view_output_q_box, tools_q feeder],
         [ProcInfo]
 
 """
@@ -32,65 +32,85 @@
     def __init__(self):
         super().__init__()
         self.kwargs = None
 
     def start(self, **kwargs):
         """enable Processes and eisenmp worker threads.
         """
-        self.all_threads_stop = False  # frequent calls without exit, see bruteforce
+        self.reset()
         self.kwargs = kwargs
         self.run_proc(**kwargs)
 
         self.enable_q_box_threads()  # [Baustelle] some q are collected in boxes, 'output', 'print' for later review
-        self.enable_view_output_q_box()  # search worker stop msg and collect result if 'store_result' is set
 
         self.enable_info_q()  # never disable, else sender blocks, nobody consumes from q
-        if 'enable_info' in kwargs and kwargs['enable_info']:
+        if 'INFO_ENABLE' in kwargs and kwargs['INFO_ENABLE']:
             self.enable_info_thread()  # collect worker send nums from info box and shows % and ETA
         return
 
+    def reset(self):
+        """"""
+        self.all_threads_stop = False  # frequent calls without exit, see bruteforce
+        self.begin_proc_shutdown = False  # frequent calls without exit, see bruteforce
+        if len(e_utils.Result.result_dict):
+            e_utils.Result.result_dict = {}
+
     def run_q_feeder(self, **kwargs):
         """Threaded instance, run multiple q_feeder, called by manager of worker
         """
         self.kwargs.update(kwargs)  # upd boss kwargs with generator, queues and header_msg
         threading.Thread(name='eisenmp_q_feeder',  # better than class thread here, no overlap, interesting.
-                         target=self.q_feeder(),
+                         target=self.q_feeder,
                          ).start()
 
     def q_feeder(self):
         """Chunk list producer of generator input.
 
-        - We need a generator to make chunks of whatever. Put chunks in list rows for transport. Numbers, str, dicts ...
-        - A ticket is attached as header, to identify the workload (list chunks).
-        - We stamp the lists with a serial number to rebuild the modified results in the right order, if needed.
+        - A ticket is attached as header to identify the workload (list chunks)
+        - Serial number to rebuild the modified results in the right order
         """
         kw = self.kwargs
-        generator = kw['generator']  # no generator, crash for sure
-        num_rows = kw['num_rows'] if 'num_rows' in kw and kw['num_rows'] else const.NUM_ROWS
-        header_msg = kw['header_msg'] if 'header_msg' in kw and kw['header_msg'] else const.HEADER_MSG
-        feeder_input_q = kw['feeder_input_q'] if 'feeder_input_q' in kw else self.mp_input_q
+        generator = kw['generator']  # no generator for run_q_feeder, crash for sure
+        num_rows = kw['NUM_ROWS'] if 'NUM_ROWS' in kw and kw['NUM_ROWS'] else const.NUM_ROWS  # processor workload
+        feeder_input_q = kw['input_q'] if 'input_q' in kw else self.mp_input_q  # use default if not specified
+
+        result_key = ''  # key name where Queue is stored as value, need a name to distinguish results in result dict
+        for tup in self.q_name_id_lst:
+            name, q_id, _ = tup  # name id q_ref
+            if q_id == id(feeder_input_q):  # unique Python id for objects
+                result_key = name
+                break
 
         start = time.perf_counter()
         num_gen = e_utils.consecutive_number()
         while 1:
             if self.all_threads_stop:
                 break
-            chunk_lst = create_transport_ticket(num_gen, header_msg)
+            chunk_lst = create_transport_ticket(num_gen, result_key)
             for _ in range(num_rows):
                 try:
                     chunk_lst.append(next(generator))
                 except StopIteration:
                     chunk_lst.append(const.STOP_MSG)  # signal stop to one worker module, worker module 'loader' to many
                     self.mp_print_q.put(f'\n\tgenerator empty, '
                                         f'run time iterator {round((time.perf_counter() - start))} seconds\n')
-                    feeder_input_q.put(chunk_lst)
+                    self.q_input_put(feeder_input_q, chunk_lst)
                     return
 
-            feeder_input_q.put(chunk_lst)
+            self.q_input_put(feeder_input_q, chunk_lst)
+
+    def q_input_put(self, feeder_input_q, chunk_lst):
+        while 1:
+            if self.all_threads_stop:
+                break
+            if feeder_input_q.empty():
+                feeder_input_q.put(chunk_lst)
+                break
 
 
-def create_transport_ticket(num_gen, header_msg=None):
+def create_transport_ticket(num_gen, result_key):
     """Semicolon to split easy.
     """
-    header_msg = header_msg if header_msg else const.HEADER_MSG
-    serial_num = f';_ID_;{str(next(num_gen))}'
-    return [header_msg + serial_num]
+    if not result_key:
+        result_key = 'mp_input_q'
+    serial_num = ';' + const.TICKET_ID_PREFIX + f'{str(next(num_gen))};'  # ';_TID_1;'
+    return [result_key + serial_num]
```

### Comparing `eisenmp-0.9.3/eisenmp/eisenmp_procenv.py` & `eisenmp-0.9.5/eisenmp/eisenmp_procenv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+"""ProcEnv
+
+"""
 import time
-import multiprocessing
+import multiprocessing as mp
 from multiprocessing import Queue
 
 import eisenmp.eisenmp_worker_loader as loader
 import eisenmp.utils.eisenmp_utils as e_utils
 import eisenmp.utils.eisenmp_constants as const
 
-multiprocessing.set_start_method('spawn', force=True)
-
 
 class ProcEnv:
-    """Create an environment for worker processes on CPUs.
+    """Create the environment for worker processes on CPUs.
     All queues shared among processes.
     'maxsize=1' can be altered, should be tested and documented.
 
+    - **Queues ONLY** in this version
+    - custom Queue builder with a queue in a dict to show a name
+    - another Queue builder can add a category name, dict in dict
+
     """
 
     def __init__(self):
         # CPU - process
-        self.num_cores = self.core_count_get()
+        self.NUM_PROCS = self.core_count_get()  # user override in mod
         self.proc_list = []  # join processes at the end
         # Queues
         self.q_max_size = 1
         self.mp_info_q = Queue(maxsize=self.q_max_size)  # fake news and performance data
         self.mp_tools_q = Queue(maxsize=self.q_max_size)  # feeder is thread
         self.mp_print_q = Queue(maxsize=self.q_max_size)  # [!mp blocking!] OMG use sparse, formatted output
         self.mp_input_q = Queue(maxsize=self.q_max_size)  # order lists
@@ -33,14 +38,15 @@
                                'mp_print_q': self.mp_print_q,
                                'mp_input_q': self.mp_input_q,
                                'mp_output_q': self.mp_output_q,
                                'mp_process_q': self.mp_process_q}
         self.queue_cust_dict_std = {}  # std dict, val is a q
         self.queue_cust_dict_cat = {}  # custom category, dict in dict
         self.q_lst = []  # all queues in a list, clean up; 'queue_lst_get'
+        self.q_name_id_lst = [('mp_input_q (default)', id(self.mp_input_q), self.mp_info_q)]  # tuple (name, id, q_ref)
 
         # Threads - Collect queue grabber
         self.thread_list = []
         self.info_q_thread_name = 'eisenmp_info_q_thread'
         self.input_q_thread_name = 'eisenmp_input_q_thread'
         self.output_q_thread_name = 'eisenmp_output_q_thread'
         self.print_q_thread_name = 'eisenmp_print_q_thread'
@@ -59,78 +65,91 @@
         - Two queue creator functions. All use tuple to ease unpacking.
 
         'queue_cust_dict_std_create' - > 'queue_cust_dict_std'
         'queue_cust_dict_category_create' - > 'queue_cust_dict_cat'
         """
         for name, maxsize in queue_name_maxsize:
             self.queue_cust_dict_std[name] = Queue(maxsize=maxsize)
+            self.q_name_id_lst.append((name, id(self.queue_cust_dict_std[name]), self.queue_cust_dict_std[name]))
+            pass
 
     def queue_cust_dict_category_create(self, *queue_cat_name_maxsize: tuple):
-        """('category_1', 'input_q_3', 10)"""
+        """('category_1', 'input_q_3', 10)
+        """
         for cat, name, maxsize in queue_cat_name_maxsize:
             new_dct = {name: Queue(maxsize=maxsize)}
             if cat not in self.queue_cust_dict_cat:
                 self.queue_cust_dict_cat[cat] = {}
             self.queue_cust_dict_cat[cat].update(new_dct)
+            self.q_name_id_lst.append((cat + '|' + name, id(new_dct[name]), new_dct[name]))
+            pass
 
     def queue_lst_get(self):
         """List of qs for shut down msg put in, of ...worker_loader.py
         """
-        q_lst = []  # dbg
-        for name, q in self.queue_std_dict.items():
-            if name == 'mp_print_q':  # else mass prn shutdown messages
-                continue
-            q_lst.append(q)
+        q_lst = [self.mp_input_q]
 
         for q in self.queue_cust_dict_std.values():  # custom, std dict
             self.q_lst.append(q)
         for cat_dct in self.queue_cust_dict_cat.values():  # custom, category dict
             for q in cat_dct.values():
                 q_lst.append(q)
 
         self.q_lst.extend(q_lst)
         return self.q_lst
 
     @staticmethod
     def core_count_get():
         """"""
-        num = 1 if not multiprocessing.cpu_count() else multiprocessing.cpu_count() / 2  # hyper thread
+        num = 1 if not mp.cpu_count() else mp.cpu_count() / 2  # hyper thread
         return int(num)
 
     def kwargs_env_update_custom(self, **kwargs):
-        """override default num_cores,
+        """override default NUM_PROCS,
         'queue_lst_get' for worker loader stop msg in all qs
         """
-        self.num_cores = kwargs['num_cores'] if 'num_cores' in kwargs and kwargs['num_cores'] else self.core_count_get()
+        self.NUM_PROCS = kwargs['NUM_PROCS'] if 'NUM_PROCS' in kwargs and kwargs['NUM_PROCS'] else self.core_count_get()
         kwargs.update(self.queue_std_dict)
         kwargs.update(self.queue_cust_dict_std)
         kwargs.update(self.queue_cust_dict_cat)
-        all_qs_dict = {'all_qs_lst_dct': self.queue_lst_get()}
+        all_qs_dict = {const.ALL_QUEUES_LIST: self.queue_lst_get()}  # view q name,id,ref in debugger: 'q_name_id_lst'
         kwargs.update(all_qs_dict)
         return kwargs
 
-    def run_proc(self, **kwargs):  # test with args from caller
+    def run_proc(self, **kwargs):
         """Create a Process for each CPU core, if `num_proc` None set or not set.
-        kwargs dict is updated for worker 'toolbox', reveals all vars and dead ref. avail.
+        - kwargs dict is updated for worker 'toolbox', reveals all vars and dead references (spawn) available
+
+        :params: kwargs: -
+        :params: start_method: selection spawn, fork
+        :params: START_SEQUENCE_NUM: useful if eisenmp instance is called often, process numbers rise, but start from 0
+        :params: target=loader: the worker_loader module is loaded and keeps the process alive
         """
         kwargs = self.kwargs_env_update_custom(**kwargs)
-        self.kwargs_env.update(kwargs)
+        self.kwargs_env.update(kwargs)  # eat kwargs
+
+        start_method = 'spawn' if 'START_METHOD' not in kwargs else kwargs['START_METHOD']
+        mp.set_start_method(start_method, force=True)
 
-        print(f'\nCreate {self.num_cores} processes.')
-        for core in range(self.num_cores):
+        print(f'\nCreate {self.NUM_PROCS} processes.')
+        for core in range(self.NUM_PROCS):
             print(core, end=" ")
-            proc = multiprocessing.Process(target=loader.mp_worker_entry,
-                                           kwargs=kwargs)
+            # start_sequence_num always starts zero and is independent of sub-process spawn number
+            start_sequence_num = {'START_SEQUENCE_NUM': core}  # worker in proc can grab a specific queue 0=red,1=blue
+            kwargs.update(start_sequence_num)
+
+            proc = mp.Process(target=loader.mp_worker_entry,
+                              kwargs=kwargs)
             proc.start()
 
             self.proc_list.append(proc)
         self.mp_print_q.put('\n')
 
     def stop_proc(self):
-        """"""
+        """All worker must have confirmed shutdown msg."""
         for proc in range(len(self.proc_list)):
             self.mp_process_q.put(['Simon Says:', const.STOP_PROCESS])
 
         for process in self.proc_list:
             while process.is_alive():
                 time.sleep(.1)
```

### Comparing `eisenmp-0.9.3/eisenmp/eisenmp_q_coll.py` & `eisenmp-0.9.5/eisenmp/eisenmp_q_coll.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 import threading
 import contextlib
 import multiprocessing
 
 import eisenmp.utils.eisenmp_utils as e_utils
 import eisenmp.utils.eisenmp_constants as const
 from eisenmp.eisenmp_procenv import ProcEnv
@@ -43,20 +42,22 @@
     """
 
     def __init__(self):
         super().__init__()
         # collect box
         self.info_q_box = {}
         self.print_q_box = []
-        self.output_q_box = {}  # dict multi thread access, Gang and ProcInfo
+        self.output_q_box = {}  # dict multi thread access
         # internal lists
-        self.stop_list = []  # proc stop answered, names collector
-        self.result_lst_gang = []  # collected findings from procs for this run
+        self.stop_list = []  # proc stop answered, worker names collector
+        self.result_lst = []  # collected findings from procs for this run
         # collect results [baustelle]
-        self.e_utilsResult = e_utils.Result()  # interim result calc for long-running tasks, exec(foo), or (bar)
+        self.e_utilsResult = e_utils.Result()  # interim result calc for long-running task
+
+        self.begin_proc_shutdown = False
 
     def enable_q_box_threads(self):
         """Collect Q messages and put em in a box for review, if enabled
         """
         self.enable_print_q()
         self.enable_output_q()
 
@@ -68,29 +69,29 @@
 
     def enable_info_thread(self):
         """Shows % done, time left, if fed with an end value"""
         args_inf = [self.info_proc_info_thread,
                     self.mp_print_q,
                     self.info_q_box]
         self.pi = ProcInfo(*args_inf, **self.kwargs_env)  # ProcInfo sits on a subclassed thread
-        self.pi.start()  # we cancel() the thread in 'thread_end_join'
+        self.pi.start()  # cancel() the thread in 'thread_end_join'
 
     def enable_print_q(self):
         """Thread for loop."""
         printQThread = FunThread('eisenmp_PrintQThread', self.print_q_loop)
         printQThread.start()
         self.thread_list.append(printQThread)
 
     def enable_output_q(self):
         """Start a thread loop to not block the show.
         Want collect stop confirm worker msg and results, all lists
         """
         outputQThread = FunThread('eisenmp_OutputQThread', self.output_q_loop)
         outputQThread.start()
-        self.thread_list.append(outputQThread)
+        # self.thread_list.append(outputQThread)
 
     def print_q_loop(self):
         """Use a Print Q and a thread for formatted printing.
 
         Use it only sparingly. BLOCKS the whole multiprocessing.
         """
         while 1:
@@ -102,29 +103,14 @@
                         msg = self.mp_print_q.get()
                         self.print_q_box.append(msg)
                         print(msg)
             except Exception as e:
                 with contextlib.redirect_stdout(None):
                     print(e)
 
-    def output_q_loop(self):
-        """Collect list header strings.
-        Stop signal strings used to init loops exit.
-        Standard dict with num generator for unique keys.
-        """
-        generator = e_utils.consecutive_number()
-        while 1:
-            if self.all_threads_stop:
-                break
-            if not self.mp_output_q.empty():
-                msg = self.mp_output_q.get()
-                num = next(generator)
-                self.output_q_box[num] = msg
-                pass
-
     def info_q_loop(self):
         """Print info or collect statistics from boxed messages.
         Box is a standard dict with num generator for unique keys.
         """
         while 1:
             if self.all_threads_stop:
                 break
@@ -132,95 +118,147 @@
             while not self.all_threads_stop:
                 if not self.mp_info_q.empty():
                     msg = self.mp_info_q.get()
                     num = next(generator)
                     self.info_q_box[num] = msg
                     pass
 
-    def enable_view_output_q_box(self):
-        """ """
-        viewOutputBoxThread = FunThread('eisenmp_viewOutputBoxThread', self.view_output_q_box)
-        viewOutputBoxThread.start()
-        # can not join() current thread msg
-
-    def view_output_q_box(self):
-        """Only lists with header accepted.
-        Box is a dictionary.
+    def output_q_loop(self):
+        """Grab output from Queue and put it in a box.
+        Use consecutive_number to create unique keys.
+
+        Note: Multiple threads can loop over the box (dict).
         """
-        outbox = self.output_q_box
+        generator = e_utils.consecutive_number()
         while 1:
             if self.all_threads_stop:
                 break
+            if not self.mp_output_q.empty():
+                worker_output = self.mp_output_q.get()
+                serial_num = next(generator)
+                self.output_q_box[serial_num] = worker_output
+                is_STOP_MSG = self.output_q_search_stop_confirm(serial_num)
+                self.output_q_box_view_results(serial_num) if not is_STOP_MSG else None
+
+    def output_q_search_stop_confirm(self, serial_num):
+        """Search stop msg of workers and put 'em in a list.
+        Stop processes and threads, if list is full.
+        {1: ['RESULT_HEADER;PRIME_NUM;_TID_1;Process-1', ['10000079']], 24: ['PROC_STOP;Process-5']}
 
-            for idx in range(len(outbox)):
-                if type(outbox[idx]) is list:
-                    outbox_list = outbox[idx]
-                    if const.GOT_RESULT_OUTPUT_Q in outbox_list:  # red list already
-                        continue
-
-                    list_header = outbox_list[0]
-                    if list_header[:len(const.STOP_CONFIRM)] == const.STOP_CONFIRM:
-                        if self.worker_mods_down_ask(list_header):
-                            self.print_findings()
-                            self.stop_proc()
-                            self.end_proc()
-                            self.stop_thread()
-                            self.end_thread()
-                            return
-
-                    if list_header[:len(const.RESULT_HEADER_PROC)] == const.RESULT_HEADER_PROC:
-                        result_lst = outbox_list
-                        p_result_row = outbox_list[1]
-                        if 'store_result' in self.kwargs_env and self.kwargs_env['store_result']:
-                            self.e_utilsResult.result_dict_update(list_header, result_lst)
-                            self.proc_result_list_findings(p_result_row)
+        :params: serial_num: serial number of `output_q_loop`
+        """
+        outbox = self.output_q_box
+        if type(outbox[serial_num]) is list:
+            outbox_list = outbox[serial_num]
+
+            list_header = outbox_list[0]
+            if list_header[:len(const.STOP_CONFIRM)] == const.STOP_CONFIRM:
+                if self.worker_mods_down_ask(list_header):
+                    self.print_findings()
+
+                    self.begin_proc_shutdown = True
+                    self.all_threads_stop = True
+
+                    self.stop_proc()
+                    self.end_proc()
+                    self.stop_thread()
+                    self.end_thread()
+
+                return True
+
+    def output_q_box_view_results(self, serial_num):
+        """Only `lists` with header accepted.
+        Box is a dictionary. {key: val} 'output_q_loop()' -> output_q_box[num]: payload or stop msg
+
+        {1: ['RESULT_HEADER;PRIME_NUM;_TID_1;Process-1', ['10000079']], 24: ['PROC_STOP;Process-5']}
 
-                    outbox_list.append(const.GOT_RESULT_OUTPUT_Q)
-            time.sleep(1)  # this thread can slow down bruteforce if too short, [Baustelle] need a trigger here
+        Result header: RESULT_HEADER
+        Delivery header: PRIME_NUM;_TID_;0  ['header_msg' and eisenmp, custom iterator, loop ticket id, split(;)]
+
+        Add your custom header_msg, taken from double Q Example:
+        - mP.run_q_feeder(generator=generator_aud, feeder_input_q=audio_q_b1, header_msg='BATCH_1_A')  # custom head
+        - mP.run_q_feeder(generator=generator_vid, feeder_input_q=video_q_b1, header_msg='BATCH_1_V')
+
+        :params: serial_num: serial number of `output_q_loop`
+        """
+        outbox = self.output_q_box
+        if type(outbox[serial_num]) is list:
+            outbox_list = outbox[serial_num]  # value of consecutive_number key is the list with results or stop msg
+
+            list_header = outbox_list[0]
+            if list_header[:len(const.OUTPUT_HEADER)] == const.OUTPUT_HEADER:
+                result_row = outbox_list[1]
+
+                if 'RESULTS_STORE' in self.kwargs_env and self.kwargs_env['RESULTS_STORE']:  # store results switch
+                    queue_header_msg, queue_ticket_id = self.proc_result_store(list_header)
+                    if not queue_ticket_id:
+                        return
+
+                    res_val = (queue_ticket_id, result_row)  # tuple
+                    self.e_utilsResult.result_dict_update(queue_header_msg, res_val)  # result_dict['PRIME_NUM']=res_val
+
+                if 'RESULTS_PRINT' in self.kwargs_env and self.kwargs_env['RESULTS_PRINT']:
+                    self.proc_result_list_findings(result_row)
+
+    @staticmethod
+    def proc_result_store(list_header):
+        """"""
+        queue_head = list_header[len(const.OUTPUT_HEADER):]  # remove 'RESULT_HEADER'
+        queue_head_lst = queue_head.split(';')  # search ticket number
+        queue_header_msg = queue_head_lst[0]  # 'PRIME_NUM', use as key for result dict
+        queue_ticket_id = None
+        for str_section in queue_head_lst:
+            if str_section[:len(const.TICKET_ID_PREFIX)] == const.TICKET_ID_PREFIX:
+                queue_ticket_id = str_section
+                break
+        return queue_header_msg, queue_ticket_id
 
     def proc_result_list_findings(self, p_result_row):
         """RESULT DICT in utils, collect all results
         Append to result list for print out at finish.
         Add to a dict to monitor results via additional thread during runtime. [baustelle]
 
         STOP msg was also appended!
 
         :params: p_result_row: process loop result list row, can be a list in this row
         """
         if const.STOP_MSG in str(p_result_row):
             return
 
         if type(p_result_row) is list:
-            [self.result_lst_gang.append(str(row) + '\n') for row in p_result_row if str(row)]  # internal list
+            [self.result_lst.append(str(row) + '\n') for row in p_result_row if str(row)]  # internal list
         else:
-            self.result_lst_gang.append(str(p_result_row) + '\n')
+            self.result_lst.append(str(p_result_row) + '\n')
 
     def worker_mods_down_ask(self, list_header):
         """All worker MODULES confirm shutdown.
 
         Worker is using the original name of its process in shut down msg.
         Process IS still running. Worker module entry function returned False.
 
         :params: list_header: answer of WORKER MODULE to stop request; string with proc id at end
         :returns: None; True if done
         """
-        worker_name = list_header[len(const.STOP_CONFIRM):]
-        self.stop_list.append(worker_name)
+        WORKER_NAME = list_header[len(const.STOP_CONFIRM):]
+        self.stop_list.append(WORKER_NAME)
         pending = any([True for proc in self.proc_list if proc.name not in self.stop_list])
         if not pending:
             return True
 
     def print_findings(self):
         """Condensed result list for this run.
         A thread can sum the results in 'Result' class.
         """
         c_lst = []
-        condensed_gen = (line.split('...') for line in list(set(self.result_lst_gang)))
+        generator = (line.split('...') for line in list(set(self.result_lst)))
         try:
-            c_lst = list(set([tup[2] for tup in condensed_gen]))
+            c_lst = list(set([tup[2] for tup in generator]))
         except IndexError:
-            c_lst.extend(self.result_lst_gang)
+            c_lst.extend(self.result_lst)
 
-        lbl = self.kwargs_env['result_lbl'] if 'result_lbl' in self.kwargs_env else 'add a "result_lbl" var'
+        lbl = self.kwargs_env['RESULT_LABEL'] if 'RESULT_LABEL' in self.kwargs_env else const.RESULT_LABEL
         c_lst.insert(0, f'\n--- Result for [{lbl}]---\n')
         c_lst.append('    --- END ---\n')
         print('\n'.join(c_lst))  # procs down
+
+        if 'RESULTS_DICT_PRINT' in self.kwargs_env and self.kwargs_env['RESULTS_DICT_PRINT']:
+            print(e_utils.Result.result_dict)
```

### Comparing `eisenmp-0.9.3/eisenmp/eisenmp_worker_loader.py` & `eisenmp-0.9.5/eisenmp/eisenmp_worker_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 import multiprocessing as mp
 
 import eisenmp.utils.eisenmp_constants as const
 
 
 class ToolBox:
     """Storage box for a Single Worker Process.
+    Switch as much data fields to constant like shape. Used in worker.
+    User can distinguish between custom and (automatic) in-build variables or constants.
 
     """
     def __init__(self):
+        # default queues names from procenv
         self.mp_info_q = None  # performance data, or other
         self.mp_tools_q = None  # data too big to send with every list to worker
         self.mp_print_q = None  # formatted screen output with multiprocessor lock(), use sparse
         self.mp_input_q = None
         self.mp_output_q = None
         self.mp_process_q = None  # proc shutdown msg's
-        self.next_lst = None  # input_q, next list from your generator -> Ghetto is iterator, list creator
-        self.worker_id = None  # name id from Process name
-        self.worker_pid = None  # process pid
-        self.worker_name = None  # stop confirmations collected by GhettoGang and send shutdown signal to program
-        self.header_msg = None  # list header, attached for every list
-        self.multi_tool = None  # tools_q, can be any prerequisite object for a module
-        self.stop_msg = None  # all q, not mp_print_q, if Boss StopIteration is raised, or this wrk informs other worker
-        self.stop_confirm = ''  # output_q, GhettoGang collects msg to send shutdown signal to program
-        self.result_header_proc = ''  # identify proc result in output_q_box
-        self.perf_header_eta = None  # 'PROC_PERF_ETA_'
-        self.perf_current_eta = None  # list rows done or other count
+        # reserved names
+        self.NEXT_LIST = None  # input_q, next list from your generator -> Ghetto is iterator, list creator
+        self.WORKER_ID = None  # name id from Process name
+        self.WORKER_PID = None  # process pid
+        self.WORKER_NAME = None  # stop confirmations collected by GhettoGang and send shutdown signal to program
+        self.MULTI_TOOL = None  # tools_q, can be any prerequisite object for a module
+        self.STOP_MSG = None  # all q, not mp_print_q, if Boss StopIteration is raised, or this wrk informs other worker
+        self.STOP_CONFIRM = ''  # output_q, GhettoGang collects msg to send shutdown signal to program
+        self.OUTPUT_HEADER = ''  # identify proc result in output_q_box
+        self.INPUT_HEADER = ''
+        self.PERF_HEADER_ETA = None  # 'PROC_PERF_ETA_'
+        self.PERF_CURRENT_ETA = None  # list rows done or other count
         self.kwargs = None
 
 
 def module_path_load(file_path):
     """Imports the module from path and returns it in the env.
     """
     path, f_name = os.path.split(file_path)
@@ -45,27 +49,27 @@
     if path not in sys.path:
         sys.path.insert(0, path)
     return __import__(modulename)
 
 
 def all_worker_exit_msg(toolbox):
     """
-    Warning: Signal stop event to [ALL] -----> WORKER modules, not process.
+    Warning: Signal stop event to [ALL] -----> worker MODULES, not to PROCESS.
 
     :params: toolbox: tools and Queues for processes
     """
-    stop_token_lst = [const.RESULT_HEADER_PROC,
+    stop_token_lst = [const.OUTPUT_HEADER,
                       const.STOP_MSG]  # 'STOP' was sent if last list was produced; now we inform other worker
 
-    for q in toolbox.all_qs_lst_dct:  # next worker on any q reads 'stop_token_lst', except 'mp_print_q'
+    for q in toolbox.ALL_QUEUES_LIST:  # next worker on any q reads 'stop_token_lst', except 'mp_print_q'
         if q.empty():
             q.put(stop_token_lst)
 
-    toolbox.mp_output_q.put([toolbox.stop_confirm])  # essential msg for caller, count stop to exit
-    toolbox.mp_print_q.put(f'\texit WORKER {toolbox.worker_id}')
+    toolbox.mp_output_q.put([toolbox.STOP_CONFIRM])  # essential msg for caller, count stop to exit
+    toolbox.mp_print_q.put(f'\texit WORKER {toolbox.WORKER_ID}')
     pass
 
 
 def mp_worker_entry(**kwargs):
     """Entry.
     We are 'disconnected' from parent process now.
     Only Queue communication. Threads can exec() 'string' commands.
@@ -74,22 +78,22 @@
     worker = None
     # assembled vars and names
     name = mp.process.current_process().name
     proc_id = name.split('-')
     tool_box = {name: ToolBox()}
     tool_box[name].__dict__.update(kwargs)  # ToolBox class, add user defined attributes of ModuleConfiguration inst
     # defaults
-    tool_box[name].worker_id = int(proc_id[1])
-    tool_box[name].worker_pid = int(os.getpid())
-    tool_box[name].worker_name = name
-    tool_box[name].stop_msg = const.STOP_MSG
-    tool_box[name].stop_confirm = const.STOP_CONFIRM + name
-    tool_box[name].result_header_proc = const.RESULT_HEADER_PROC
-    tool_box[name].perf_header_eta = const.PERF_HEADER_ETA  # performance list header for ProcInfo
-    tool_box[name].perf_current_eta = None
+    tool_box[name].WORKER_ID = int(proc_id[1])
+    tool_box[name].WORKER_PID = int(os.getpid())
+    tool_box[name].WORKER_NAME = name
+    tool_box[name].STOP_MSG = const.STOP_MSG
+    tool_box[name].STOP_CONFIRM = const.STOP_CONFIRM + name
+    tool_box[name].OUTPUT_HEADER = const.OUTPUT_HEADER
+    tool_box[name].PERF_HEADER_ETA = const.PERF_HEADER_ETA  # performance list header for ProcInfo
+    tool_box[name].PERF_CURRENT_ETA = None
     tool_box[name].kwargs = kwargs
 
     toolbox = tool_box[name]  # use normal instance like
 
     # Module Loader
     mod_fun_lst = []
     for row in kwargs['worker_modules']:
@@ -111,16 +115,20 @@
                 mate_fun(toolbox)
         worker = mod_fun_lst.pop()  # last but not least
 
     while 1:
 
         busy = worker(toolbox)  # until worker reads the iterator STOP msg
         if not busy:
-            if 'stop_msg_disable' not in toolbox.kwargs or not toolbox.kwargs['stop_msg_disable']:
+            if 'STOP_MSG_DISABLE' not in toolbox.kwargs or not toolbox.kwargs['STOP_MSG_DISABLE']:
                 all_worker_exit_msg(toolbox)  # stop msg in all queues, if not all loaded worker are threads
             break
 
     while 1:
 
         msg_lst = toolbox.mp_process_q.get()  # loader keeps proc alive and awaits, 'stop_proc'
         if const.STOP_PROCESS in msg_lst:
+
+            for q in toolbox.ALL_QUEUES_LIST:  # multiple qs feeder may stick if first sent the worker stop
+                if not q.empty():
+                    q.get()
             break
```

### Comparing `eisenmp-0.9.3/eisenmp/utils/eisenmp_info.py` & `eisenmp-0.9.5/eisenmp/utils/eisenmp_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.daemon = True
         self.cancelled = False
         # info
         self.perf_dict_eta = {}
         self.info_shutdown = False
         self.print_q = print_q
         self.info_q_box = info_q_box  # dict
-        self.info_td_max = kwargs['info_td_max'] if 'info_td_max' in kwargs else None
+        self.INFO_THREAD_MAX = kwargs['INFO_THREAD_MAX'] if 'INFO_THREAD_MAX' in kwargs else None
         self.info_td_exec = kwargs['info_td_exec'] if 'info_td_exec' in kwargs else None
 
     def run(self):
         """feed init args instead of method args"""
         self.performance_coll()
 
     def cancel(self):
@@ -62,16 +62,16 @@
         for idx in range(len(info_box)):
             if idx in info_box.keys():
                 if type(info_box[idx]) is list:
 
                     list_header = info_box[idx][0]
                     if list_header[:14] == constants.PERF_HEADER_ETA:
                         a_num = int(info_box[idx][1])
-                        if self.info_td_max:
-                            self.perf_dict_eta['target'] = self.info_td_max
+                        if self.INFO_THREAD_MAX:
+                            self.perf_dict_eta['target'] = self.INFO_THREAD_MAX
                             if self.info_td_exec:
                                 exec(self.info_td_exec)
                             else:
                                 self.perf_dict_eta['rows_done'] += a_num  # ETA
                         info_box[idx] = None
 
     def perf_count_print_eta(self):
```

### Comparing `eisenmp-0.9.3/eisenmp/utils/eisenmp_utils.py` & `eisenmp-0.9.5/eisenmp/utils/eisenmp_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 import time
 import threading
-from collections import defaultdict
 
 
 class Result:
     """Finest results only here.
-    Can save number stuff, not response chunks, or we crash
 
     """
+    result_dict = {}
 
-    def __init__(self):
-        self._result_dict = defaultdict(list)  # threads can read/write dict
-
-    @property
-    def result_dict(self):
-        return self._result_dict
-
-    @result_dict.setter
-    def result_dict(self, update):
-        self._result_dict = update
-
-    @result_dict.deleter
-    def result_dict(self):
-        del self._result_dict
-
-    def result_dict_update(self, key, value):
-        self._result_dict[key].append(value)
+    def result_dict_update(self, key: str, id_result: tuple) -> None:
+        """Sort results yourself.
+        If something is wrong, you see one TID is not there.
+
+        Tuple for simple extraction: id, result = result_dict['PRIME_NUM']
+        {'PRIME_NUM': [(ticket_id, result_lst), (ticket_id, result_lst)]}
+
+        :params: key: str name of the queue feeder 'header_msg' argument
+        :params: result_value_t: tuple(_TID_0, result)
+        """
+        if key not in self.result_dict:
+            self.result_dict[key] = []
+        self.result_dict[key].append(id_result)
 
 
 def consecutive_number():
     """Want a stamp on each list header.
     Used for Queue messages get() and put in box_dict[num] = msg
     Can rebuild original order if worker puts result in a list
     with same num as order list.
```

### Comparing `eisenmp-0.9.3/eisenmp.egg-info/PKG-INFO` & `eisenmp-0.9.5/eisenmp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.3
+Version: 0.9.5
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
         
@@ -44,90 +44,118 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: LICENSE.rst
 
 # eisenmp
  
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
+Python 3.7 
+[Multiprocessor](https://en.wikipedia.org/wiki/Multiprocessing)
 [Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
 
+Forget about pools, swim in the sea.
+
 Features:
 
-* Load modules from Network or FS. Load **multi, independent and before a worker** into ➜ Process
-* Run every Python generator on _every_ CPU core, enable auto collect results
-* Load a fixed number of servers into each process
-* Build port groups with CPU cores and network adapters
-* Create **categories of Queues**, read them with **all custom vars** in a **ToolBox** dictionary, used by the worker
+* Create **uniform** multiprocess programs for your projects
+* Calculate your Python generator output on _every_ CPU core
+* Worker **module_loader** decouples your Worker imports from Main()
+* **auto Exit** of worker and process
+* Start methods, **spawn**, **fork** and **forkserver**
+* Create VM_ware like **port groups** on CPU cores and stream with (tcp/http) maximum speed via selected NIC adapters
+* Process **START_SEQUENCE_NUM** Worker on a CPU core can grab a specific queue 0=red_q, 1=blue_q,2=yellow_q
+* **Categories of Queues**, read them with **all custom vars** in a worker **ToolBox** dictionary
 * no libraries, light weight; (Linux, Windows)
-* [Examples](https://github.com/44xtc44/eisenmp_examples) 
-flask_orm_user_db, web_csv_large-list, brute_force_attack, double_queue_feeding, multi_srv_ ...
-* All scenarios follow the **Template style** and have descriptions
-
-Workplace:
-* Server or mobile device
-
-Note:
-Generator prod. 1, 2, 3, 4, 5  ➜ we make Worker chunks, [los](https://de.wikipedia.org/wiki/Los_(Produktion))
-[1,2] [3,4] [5] lists. Each process worker gets one.
 
+Visit the features above in the
+[Examples gitHub repository](https://github.com/44xtc44/eisenmp_examples), 
+or get the [Examples PyPi package](https://pypi.org/project/eisenmp-examples/),
+run 
+
+    eisenmp_url 
+    or 
+    eisenmp_menu
+simpleHTTP Ajax server, or terminal menu
 
-### min. ToDo
+All scenarios run on **reusable Template Modules**. Enjoy the descriptions and discover.
 
-Generator - iterator chunks on every CPU core:
-- (A) Mngr(): **Every generator** yield, or generator expression
-- (B) Wkr(): The **worker** wants a loop. Return True, get the next chunk or False for **auto exit worker and process**.
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (D) Mngr(): default call: **iterator** ...raid.run_q_feeder(generator=your generator), runs also on ➜ assigned queues
+## How it works
+You write two functions and two modules.
+Let's call 'em **Generator.py** and **Worker.py**.
 
-One Server (or more) on every CPU core:
-- (C) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (C.1) Wkr(): The **worker module** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
-- (C.2) Wkr(): The **worker module** starts **MANY** server. All server starts must be threads **stop_msg_disable=True**
-- Server reads queues: Needs (A) Mngr and (D) Mngr
-- **Port groups** (applications, server): map **toolbox.worker_id**
-'s ➜ to server ports on CPU cores ➜ to an IP address
+1. Generator.py starts a new process, _but_ the target is **module_loader.py** (loader).
+2. loader imports your (independent) Worker.py module from file system. 
+This makes sure that only imports of the worker.py module are loaded, without side effects.
+3. loader sits in a loop and calls your Worker.py entry function endless. Until there is no more work in the queues.
+This loop keeps the process alive.
+4. **q_feeder** iterator sends a STOP Worker message with the last chunk. Your Worker reads STOP, return False and exit. 
+5. The **module loader** then puts a STOP Worker message in all other input queues.
+Loader runs idle and awaits the internal STOP Process message. **Next** Worker reads STOP, exit ...
 
-## How it works
-Needs one **Caller (Mngr)** and one **Worker** fun() in the module for simple tasks.
-- ModuleConfiguration class collects data variables as default and custom variables in a **modConf** instance
-- Mngr fun() updates eisenmp with the **modConf** instance dictionary
-- create **custom Queue**s, either single named in a dict or as dict with category names for easy deployment
-- eisenmp threaded method **run_q_feeder** can be called multiple times to fill the worker Queues with generator output
-
-The loader imports **arbitrary** modules. Iterator loop threads (option) put work chunks in queues.
-The **first registered module function**, the worker, is called in an **endless loop**, as long as it exits after 
-each own cycle. Microcontroller style. It is the **last loaded module**.
-
-Following modules in the register list (LIFO) execute a thread start function to not block the Worker module. 
-They may control the worker and have access to its started instances references (offset address). 
-main(), Parent Process has no access in Child Processes. 
-It needs any help it can get. We use 'spawn' multiprocessing.
-See also the watchdog threaded module in the [Examples](https://github.com/44xtc44/eisenmp_examples) , please.
+Default ``six Queues``
+- ``Input`` worker lists, ``Output`` result and stop lists, ``Process`` shutdown
+- ``Tools``, ``Print``, ``Info``
 
-Use Server only, set **stop_msg_disable=True**. This allows to use threaded modules only.
+### In detail:
 
-Generator output can be any data type (int, str, response stream chunks, floats) as long as it is delivered by a 
-[generator function (yield)](https://docs.python.org/3/reference/expressions.html#yieldexpr)
+Generator - iterator chunks on every CPU core:
+- [Generator yield](https://docs.python.org/3/reference/expressions.html#yieldexpr)
 or 
-[(generator expression)](https://peps.python.org/pep-0289/)
+[(expression)](https://peps.python.org/pep-0289/)
+output 1, 2, 3, 4, 5 ➜ eisenmp iterator list [ [1,2] [3,4] [5] ] ➜ **NUM_ROWS** chunks for your Worker
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker in (also) a list. 
+- (B) Mngr(): Assign Worker load and process count.
+- (C) Mngr(): Call **iterator** run_q_feeder(generator=Mngr generator)
+- (D) Wkr(): Loop over **NUM_ROWS** list chunks. Return False to **auto exit worker and process**, or get next chunk 
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
 
+One Server (or more) on every CPU core:
+- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
+- (D.1) Wkr(): The **worker** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
+- (D.2) Wkr(): The **worker** starts **MANY** server. Server start call must be threaded, set **STOP_MSG_DISABLE=True**
+- Server read queues: Follow the Generator todo
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
+
+Port groups:
+- Map **START_SEQUENCE_NUM**'s ➜ to multiple (server) ports on CPU cores ➜ to an IP address, 
+[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
+or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
 
-Default ``six Queues``
-- ``Input`` serial number header, ``Output`` result and stop lists w. header, ``Process`` shutdown
-- ``Tools``, ``Print``, ``Info``
 
-Default means **ready to use**:
-- **mp_input_q** lists have a header with a **serial number** to be able to recreate the original order of chunks
+### ready to use:
+- **run_q_feeder()** iterator lists get a **serial number** header to recreate the original order of chunks
 - **mp_tools_q** for big tools stuff delivery to every single Worker proc module;
 It may be a 27GB rainbow table; See the bruteforce (small) example, please
-- Output **can** be stored if **store_result** is set in config
+- Output **can** be stored if **RESULTS_STORE** is set in config
+
+
+## Issues
+eisenmp can run on Python 3.6 (Ubuntu test), but not the samples.
 
 ## How to run the examples?
-Clone the repo [Examples](https://github.com/44xtc44/eisenmp_examples) and ``run an eisenmp_exa_...``.
+Most easy is PyPi package mentioned above. **eisenmp** will be installed also.
+
+Clone both repos.
+[eisenmp](https://github.com/44xtc44/eisenmp) and
+[eisenmp_examples](https://github.com/44xtc44/eisenmp_examples)
+
+Install in editable pip mode.
+
+    cd eisenmp 
+    pip3 install -e .  # uninstall (linux pip3) with: pip3 uninstall eisenmp
+
+    cd eisenmp_examples
+    pip3 install -e .  # uninstall with: pip3 uninstall eisenmp_examples
+Run the examples.
+ 
+    eisenmp_url
+    # or
+    eisenmp_menu
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
 
 	[BRUTE_FORCE]	cfhhilorrs
```

### Comparing `eisenmp-0.9.3/pyproject.toml` & `eisenmp-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp"
-version = "0.9.3"
+version = "0.9.5"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,"
 keywords = ['multiprocess framework', 'python multiprocessor framework']
 license = {file = "LICENSE.rst"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

