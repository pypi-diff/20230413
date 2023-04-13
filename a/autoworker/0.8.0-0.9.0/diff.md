# Comparing `tmp/autoworker-0.8.0.tar.gz` & `tmp/autoworker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoworker-0.8.0.tar", last modified: Mon May  4 14:00:50 2020, max compression
+gzip compressed data, was "dist/autoworker-0.9.0.tar", last modified: Thu Apr 13 07:46:20 2023, max compression
```

## Comparing `autoworker-0.8.0.tar` & `autoworker-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 14:00:50.000000 autoworker-0.8.0/
--rw-r--r--   0 afita     (1000) afita     (1000)      396 2020-05-04 14:00:50.000000 autoworker-0.8.0/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)       38 2020-05-04 14:00:50.000000 autoworker-0.8.0/setup.cfg
--rw-r--r--   0 afita     (1000) afita     (1000)      579 2020-05-04 13:59:35.000000 autoworker-0.8.0/setup.py
-drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker/
--rw-r--r--   0 afita     (1000) afita     (1000)     4079 2020-05-04 13:59:05.000000 autoworker-0.8.0/autoworker/__init__.py
--rw-r--r--   0 afita     (1000) afita     (1000)      542 2020-05-04 13:59:05.000000 autoworker-0.8.0/README.rst
-drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)       11 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      211 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      396 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)       18 2020-05-04 14:00:50.000000 autoworker-0.8.0/autoworker.egg-info/requires.txt
+drwxr-xr-x   0 psala     (1000) psala     (1000)        0 2023-04-13 07:46:20.000000 autoworker-0.9.0/
+-rw-r--r--   0 psala     (1000) psala     (1000)       38 2023-04-13 07:46:20.000000 autoworker-0.9.0/setup.cfg
+drwxr-xr-x   0 psala     (1000) psala     (1000)        0 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker/
+-rw-r--r--   0 psala     (1000) psala     (1000)     3957 2023-04-13 07:46:13.000000 autoworker-0.9.0/autoworker/__init__.py
+-rw-r--r--   0 psala     (1000) psala     (1000)      542 2023-04-13 07:46:13.000000 autoworker-0.9.0/README.rst
+-rw-r--r--   0 psala     (1000) psala     (1000)      396 2023-04-13 07:46:20.000000 autoworker-0.9.0/PKG-INFO
+-rw-r--r--   0 psala     (1000) psala     (1000)      579 2023-04-13 07:46:13.000000 autoworker-0.9.0/setup.py
+drwxr-xr-x   0 psala     (1000) psala     (1000)        0 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/
+-rw-r--r--   0 psala     (1000) psala     (1000)        1 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 psala     (1000) psala     (1000)       18 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/requires.txt
+-rw-r--r--   0 psala     (1000) psala     (1000)       11 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/top_level.txt
+-rw-r--r--   0 psala     (1000) psala     (1000)      396 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/PKG-INFO
+-rw-r--r--   0 psala     (1000) psala     (1000)      211 2023-04-13 07:46:20.000000 autoworker-0.9.0/autoworker.egg-info/SOURCES.txt
```

### Comparing `autoworker-0.8.0/setup.py` & `autoworker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 INSTALL_REQUIRES = ['rq>=0.10.0', 'osconf']
 
 setup(
     name='autoworker',
-    version='0.8.0',
+    version='0.9.0',
     packages=find_packages(exclude=['spec']),
     url='https://github.com/gisce/autoworker',
     license='MIT',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     install_requires=INSTALL_REQUIRES,
     description='Start Python RQ Workers automatically',
```

### Comparing `autoworker-0.8.0/autoworker/__init__.py` & `autoworker-0.9.0/autoworker/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 from __future__ import unicode_literals
 import os
 import multiprocessing as mp
 from uuid import uuid4
+import subprocess
 
 from redis import Redis
 from rq.defaults import DEFAULT_RESULT_TTL
 from rq.contrib.legacy import cleanup_ghosts
 from rq.queue import Queue
 from rq.worker import Worker, WorkerStatus
 from rq.utils import import_attribute
@@ -82,41 +83,38 @@
         return len([
             w for w in Worker.all(queue=self.queue) if w.state in (
                 WorkerStatus.STARTED, WorkerStatus.SUSPENDED, WorkerStatus.BUSY,
                 WorkerStatus.IDLE
             )
         ])
 
-    def worker(self):
+    @property
+    def worker_command(self):
         """Internal target to use in multiprocessing
         """
-        cleanup_ghosts(self.connection)
-        worker_class = import_attribute(self.config['worker_class'])
-        if self.skip_failed:
-            exception_handlers = []
-        else:
-            exception_handlers = None
 
-        name = '{}-auto'.format(uuid4().hex)
-        worker = worker_class(
-            [self.queue], name=name, connection=self.connection,
-            exception_handlers=exception_handlers,
-            default_result_ttl=self.default_result_ttl
-        )
-        worker.work(burst=True)
+        rq_params = {
+            '-b': '',
+            '-w': self.config['worker_class'],
+            '-n': '{}-auto'.format(uuid4().hex),
+            '-u': self.config['redis_url'],
+            '--results-ttl': self.default_result_ttl
+
+        }
+        if self.skip_failed:
+            rq_params['--disable-default-exception-handler'] = ''
 
-    def _create_worker(self):
-        child_pid = os.fork()
-        if child_pid == 0:
-            self.worker()
+        command = ['rq', 'worker']
+        for k, v in rq_params.items():
+            command.append(str(k))
+            if v:
+                command.append(str(v))
+        command.append(self.queue.name)
+        return command
 
     def work(self):
         """Spawn the multiple workers using multiprocessing and `self.worker`_
         targget
         """
         max_procs = self.max_procs - self.num_connected_workers()
-        self.processes = [
-            mp.Process(target=self._create_worker) for _ in range(0, max_procs)
-        ]
-        for proc in self.processes:
-            proc.daemon = False
-            proc.start()
+        for _ in range(0, max_procs):
+            subprocess.Popen(self.worker_command, close_fds=True)
```

### Comparing `autoworker-0.8.0/README.rst` & `autoworker-0.9.0/README.rst`

 * *Files identical despite different names*

