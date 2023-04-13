# Comparing `tmp/optscale_arcee-0.1.26.tar.gz` & `tmp/optscale_arcee-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.26.tar", last modified: Thu Mar  9 13:29:47 2023, max compression
+gzip compressed data, was "optscale_arcee-0.1.30.tar", last modified: Thu Apr 13 11:07:46 2023, max compression
```

## Comparing `optscale_arcee-0.1.26.tar` & `optscale_arcee-0.1.30.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    11304 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1494 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1173 2023-02-10 11:41:12.000000 optscale_arcee-0.1.26/README.rst
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       95 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3490 2023-02-10 11:41:12.000000 optscale_arcee-0.1.26/optscale_arcee/arcee.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee/hw_stat_collector/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/hw_stat_collector/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3959 2023-03-09 13:14:41.000000 optscale_arcee-0.1.26/optscale_arcee/hw_stat_collector/collector.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee/module_collector/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/module_collector/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2615 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/module_collector/collector.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     6757 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/name_generator.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     9821 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/platform.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee/platforms_meta/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/platforms_meta/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2469 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/platforms_meta/azure.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee/sender/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/optscale_arcee/sender/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4063 2023-02-10 11:41:12.000000 optscale_arcee-0.1.26/optscale_arcee/sender/sender.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/optscale_arcee.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1494 2023-03-09 13:29:47.000000 optscale_arcee-0.1.26/optscale_arcee.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1190 2023-03-09 13:29:47.000000 optscale_arcee-0.1.26/optscale_arcee.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-09 13:29:47.000000 optscale_arcee-0.1.26/optscale_arcee.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       60 2023-03-09 13:29:47.000000 optscale_arcee-0.1.26/optscale_arcee.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       15 2023-03-09 13:29:47.000000 optscale_arcee-0.1.26/optscale_arcee.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      524 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       69 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/setup.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-09 13:29:47.099647 optscale_arcee-0.1.26/tests/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/tests/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4593 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/tests/test_data.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3870 2023-02-08 17:23:40.000000 optscale_arcee-0.1.26/tests/test_platform.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/
+-rw-rw-r--   0 am        (1000) am        (1000)    11304 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/LICENSE.txt
+-rw-rw-r--   0 am        (1000) am        (1000)     2241 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)     1423 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/README.rst
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.407026 optscale_arcee-0.1.30/optscale_arcee/
+-rw-rw-r--   0 am        (1000) am        (1000)       95 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3751 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/arcee.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4098 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/collector.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/module_collector/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/module_collector/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2633 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/module_collector/collector.py
+-rw-rw-r--   0 am        (1000) am        (1000)     6757 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/name_generator.py
+-rw-rw-r--   0 am        (1000) am        (1000)     9821 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platform.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2469 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/azure.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/sender/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/sender/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4064 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/sender/sender.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee.egg-info/
+-rw-rw-r--   0 am        (1000) am        (1000)     2241 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)      734 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/SOURCES.txt
+-rw-rw-r--   0 am        (1000) am        (1000)        1 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/dependency_links.txt
+-rw-rw-r--   0 am        (1000) am        (1000)       60 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/requires.txt
+-rw-rw-r--   0 am        (1000) am        (1000)       15 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/top_level.txt
+-rw-rw-r--   0 am        (1000) am        (1000)      524 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/setup.cfg
+-rw-rw-r--   0 am        (1000) am        (1000)       69 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/setup.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/tests/
+-rw-rw-r--   0 am        (1000) am        (1000)     4593 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/tests/test_data.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3850 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/tests/test_platform.py
```

### Comparing `optscale_arcee-0.1.26/LICENSE.txt` & `optscale_arcee-0.1.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.26/README.rst` & `optscale_arcee-0.1.30/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 # Arcee
-## _The OptScale ML profiling tool by Hystax_
-
+## *The OptScale ML profiling tool by Hystax*
 
 Arcee is a tool that hepls you to integrate ML tasks with [OptScale](https://my.optscale.com/).
 This tool can automatically collect executor metadata from cloud and process stats.
- 
+
 ## Installation
-Arcee requires python 3.7+ to run. 
+Arcee requires python 3.7+ to run.
 ```sh
 pip install optscale-arcee
 ```
-## Usage
 
+## Usage
 First of all you need to import and init arcee in your code:
 ```sh
 import optscale_arcee as arcee
 ```
 
 ```sh
-# init arcee
-arcee.init('token', 'application_key')
+# init arcee using context manager syntax
+with arcee.init('token', 'application_key'):
+    # some code
 ```
 
 To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
 ```sh
-arcee.init('token', 'application_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False)
+with arcee.init('token', 'application_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+    # some code
+```
+
+Alternatively arcee can be initialized via function call. However manual finish is required:
+```sh
+arcee.init('token', 'application_key')
+# some code
+arcee.finish()
+```
+
+Or in error case:
+```sh
+arcee.init('token', 'application_key')
+# some code
+arcee.error()
 ```
 
 To send stats:
 ```sh
 arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
 ```
 (key should be string, value - int or float, multiple values can be sent)
 
 To add tags to application run (key, value):
 ```sh
 arcee.tag("project", "torchvision demo")
 ```
+
 To add milestones:
 ```sh
 arcee.milestone("Download test data")
 ```
+
 To add stages:
 ```sh
 arcee.stage("calculation")
 ```
-To finish model:
-```sh
-arcee.finish()
-```
-or for failed task:
-```sh
-arcee.error()
-```
```

### Comparing `optscale_arcee-0.1.26/optscale_arcee/arcee.py` & `optscale_arcee-0.1.30/optscale_arcee/arcee.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import datetime
 import time
 import threading
 from optscale_arcee.sender.sender import Sender
 from optscale_arcee.name_generator import NameGenerator
 
 
 def single(class_):
@@ -73,23 +72,34 @@
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
         self._name = value
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is None:
+            finish()
+        else:
+            error()
+        return exc_type is None
+
 
 def init(token, application_key, run_name=None, endpoint_url=None, ssl=True, period=1):
     arcee = Arcee(token, application_key, endpoint_url, ssl)
     name = run_name if run_name is not None else NameGenerator.get_random_name()
     run_id = asyncio.run(arcee.sender.get_run_id(application_key, token, name))["id"]
     arcee.run = run_id
     arcee.name = name
     arcee.hb = Job(meth_args=(arcee.sender, run_id, token), sleep=period)
     arcee.hb.start()
+    return arcee
 
 
 def tag(key, value):
     arcee = Arcee()
     arcee.tags = (key, value)
     asyncio.run(arcee.sender.add_tags(arcee.run, arcee.token, arcee.tags))
 
@@ -102,38 +112,42 @@
 def stage(name):
     arcee = Arcee()
     asyncio.run(arcee.sender.create_stage(arcee.run, arcee.token, name))
 
 
 def finish():
     arcee = Arcee()
-    asyncio.run(
-        arcee.sender.change_state(
-            arcee.run,
-            arcee.token,
-            2,
-            int(datetime.datetime.utcnow().timestamp()),
+    try:
+        asyncio.run(
+            arcee.sender.change_state(
+                arcee.run,
+                arcee.token,
+                2,
+                True,
+            )
         )
-    )
-    arcee.hb.shutdown_flag.set()
-    arcee.hb.join()
+    finally:
+        arcee.hb.shutdown_flag.set()
+        arcee.hb.join()
 
 
 def error():
     arcee = Arcee()
-    asyncio.run(
-        arcee.sender.change_state(
-            arcee.run,
-            arcee.token,
-            3,
-            int(datetime.datetime.utcnow().timestamp()),
+    try:
+        asyncio.run(
+            arcee.sender.change_state(
+                arcee.run,
+                arcee.token,
+                3,
+                True,
+            )
         )
-    )
-    arcee.hb.shutdown_flag.set()
-    arcee.hb.join()
+    finally:
+        arcee.hb.shutdown_flag.set()
+        arcee.hb.join()
 
 
 def info():
     arcee = Arcee()
     return arcee.__dict__
```

### Comparing `optscale_arcee-0.1.26/optscale_arcee/hw_stat_collector/collector.py` & `optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import math
 import os
 import concurrent.futures
 from functools import partial, reduce
 
 import GPUtil
 import psutil
 
@@ -37,20 +38,23 @@
         ) / len(gpus)
         avg_gpu_memory_total = reduce(
             lambda x, y: x + y, map(lambda z: z.memoryTotal, gpus)
         ) / len(gpus)
         avg_gpu_memory_used = reduce(
             lambda x, y: x + y, map(lambda z: z.memoryUsed, gpus)
         ) / len(gpus)
-        return {
-            "avg_gpu_load": avg_gpu_load,
+        stats = {
             "avg_gpu_memory_free": avg_gpu_memory_free,
             "avg_gpu_memory_total": avg_gpu_memory_total,
             "avg_gpu_memory_used": avg_gpu_memory_used,
         }
+        # get rid of devices with limited support
+        if not math.isnan(avg_gpu_load):
+            stats["avg_gpu_load"] = avg_gpu_load * 100,
+        return stats
 
     @staticmethod
     def _ps_stats(cpu_interval=0.5, proc_interval=0.5):
         load1, load5, load15 = psutil.getloadavg()
         cpu_load = psutil.cpu_percent(interval=cpu_interval, percpu=True)
         cpu_percent = round(sum(cpu_load) / psutil.cpu_count(), 2)
         # get proc pid
```

### Comparing `optscale_arcee-0.1.26/optscale_arcee/module_collector/collector.py` & `optscale_arcee-0.1.30/optscale_arcee/module_collector/collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 file = __main__.__file__
             else:
                 file = await cls.get_cfp()
         try:
             finder = ModuleFinder()
             await cls.run_async(finder.run_script, file)
             m = finder.modules.keys()
-        except AttributeError:
+        except (AttributeError, RecursionError):
             # try to bypass 40350/84530 ns mod issue
             # pls see following for details
 
             # https://bugs.python.org/issue40350
             # https://github.com/python/cpython/issues/84530
             # https://github.com/python/cpython/pull/19917
             # https://github.com/python/cpython/pull/29196
```

### Comparing `optscale_arcee-0.1.26/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.30/optscale_arcee/name_generator.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.26/optscale_arcee/platform.py` & `optscale_arcee-0.1.30/optscale_arcee/platform.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.26/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.30/optscale_arcee/platforms_meta/azure.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.26/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.30/optscale_arcee/sender/sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         return await self.send_post_request(uri, headers, {"milestone": value})
 
     async def add_tags(self, run_id, token, tags):
         uri = "%s/run/%s" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_patch_request(uri, headers, {"tags": tags})
 
-    async def change_state(self, run_id, token, state, finish=None):
+    async def change_state(self, run_id, token, state, finish=False):
         uri = "%s/run/%s" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_patch_request(
             uri, headers, {"state": state, "finish": finish}
         )
 
     async def create_stage(self, run_id, token, name):
```

### Comparing `optscale_arcee-0.1.26/setup.cfg` & `optscale_arcee-0.1.30/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.26
+version = 0.1.30
 author = Hystax
 description = ML profiling tool for OptScale
 long_description = file: README.rst
 long_description_content_type = text/markdown
 url = https://my.optscale.com/
 keywords = arcee, ml, optscale, finops, mlops
 
 [options]
 python_requires = >=3.7, <4
 install_requires = 
-	aiohttp==3.8.1
+	aiohttp==3.8.4
 	aiofiles==22.1.0
 	GPUtil==1.4.0
 	psutil==5.9.2
 packages = find:
 package_dir = 
 	=.
 test =
```

### Comparing `optscale_arcee-0.1.26/tests/test_data.py` & `optscale_arcee-0.1.30/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.26/tests/test_platform.py` & `optscale_arcee-0.1.30/tests/test_platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from unittest.mock import patch
-from unittest import IsolatedAsyncioTestCase
+import aiounittest
 
 from optscale_arcee.platform import (
     Platform,
     AzureCollector,
     CollectorFactory,
     PlatformType,
     AwsCollector,
     PlatformMeta,
     InstanceLifeCycle,
 )
 from tests.test_data import TestDataAzure
 
 
-class TestPlatform(IsolatedAsyncioTestCase):
+class TestPlatform(aiounittest.AsyncTestCase):
     def test_platform_is_static(self):
         self.assertRaises(TypeError, Platform())
 
     @patch("optscale_arcee.platform.Platform.sys_vendor")
     async def test_platform_factory(self, mock_sys_vendor):
         mock_sys_vendor.return_value = PlatformType.aws
         self.assertEqual(await CollectorFactory.get(), AwsCollector)
 
 
-class TestAzureCollector(IsolatedAsyncioTestCase):
+class TestAzureCollector(aiounittest.AsyncTestCase):
     @patch("optscale_arcee.platform.AzureCollector.collect")
     async def test_azure_base_collector(self, mocked_collect):
         mocked_collect.return_value = TestDataAzure.get_test_data()
         platform_meta = await AzureCollector().get_platform_meta()
         self.assertTrue(isinstance(platform_meta, PlatformMeta))
         self.assertTrue(platform_meta.platform_type, PlatformType.azure)
         self.assertTrue(platform_meta.local_ip)
@@ -51,15 +51,15 @@
         platform_meta = await AzureCollector().get_platform_meta()
         self.assertTrue(isinstance(platform_meta, PlatformMeta))
         self.assertTrue(platform_meta.platform_type, PlatformType.azure)
         self.assertTrue(platform_meta.instance_lc, InstanceLifeCycle.Unknown)
         self.assertTrue(platform_meta.to_dict())
 
 
-class TestAwsCollector(IsolatedAsyncioTestCase):
+class TestAwsCollector(aiounittest.AsyncTestCase):
     @patch("optscale_arcee.platform.AwsCollector.get_instance_type")
     @patch("optscale_arcee.platform.AwsCollector.get_region")
     @patch("optscale_arcee.platform.AwsCollector.get_az")
     @patch("optscale_arcee.platform.AwsCollector.get_life_cycle")
     @patch("optscale_arcee.platform.AwsCollector.get_public_ip")
     @patch("optscale_arcee.platform.AwsCollector.get_local_ip")
     @patch("optscale_arcee.platform.AwsCollector.get_account_id")
```

