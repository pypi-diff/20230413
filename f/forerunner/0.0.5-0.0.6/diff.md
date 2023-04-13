# Comparing `tmp/forerunner-0.0.5.tar.gz` & `tmp/forerunner-0.0.6.tar.gz`

## Comparing `forerunner-0.0.5.tar` & `forerunner-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 forerunner-0.0.5/Makefile
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/__init__.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/app.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/cli.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/console.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/module.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/utils.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/dependency/depends.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/dependency/utils.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/job/__init__.py
--rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/job/base.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/job/cron.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/job/sub.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/queue/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.5/src/forerunner/queue/queue.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.5/.gitignore
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 forerunner-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 forerunner-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 forerunner-0.0.6/Makefile
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 forerunner-0.0.6/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/__init__.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/app.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/cli.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/console.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/module.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/utils.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/dependency/depends.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/dependency/utils.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/__init__.py
+-rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/base.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/cron.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/sub.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/queue/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/queue/queue.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.6/.gitignore
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 forerunner-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 forerunner-0.0.6/PKG-INFO
```

### Comparing `forerunner-0.0.5/src/forerunner/app.py` & `forerunner-0.0.6/src/forerunner/app.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.5/src/forerunner/module.py` & `forerunner-0.0.6/src/forerunner/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import Callable, List, Literal
 
-from ipdb import set_trace
 
 from .job import Cron, Sub
 from .queue import BaseQueue
 
 
 class Module:
     def __init__(
```

### Comparing `forerunner-0.0.5/src/forerunner/utils.py` & `forerunner-0.0.6/src/forerunner/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import importlib
 from typing import Any, Callable, List
 
-from ipdb import set_trace
 
 from .app import Module
 
 
 def init_module_jobs(
     *,
     app_name: str,
```

### Comparing `forerunner-0.0.5/src/forerunner/dependency/depends.py` & `forerunner-0.0.6/src/forerunner/dependency/depends.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.5/src/forerunner/dependency/utils.py` & `forerunner-0.0.6/src/forerunner/dependency/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import asyncio
 import inspect
 from contextlib import AsyncExitStack, asynccontextmanager, contextmanager
 from typing import Any, Callable, ContextManager, Dict
 
-from ipdb import set_trace
-
 
 @asynccontextmanager
 async def contextmanager_in_threadpool(
     *, cm: ContextManager, loop: asyncio.AbstractEventLoop
 ):
     try:
         yield await loop.run_in_executor(None, cm.__enter__)
```

### Comparing `forerunner-0.0.5/src/forerunner/job/base.py` & `forerunner-0.0.6/src/forerunner/job/base.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.5/src/forerunner/job/cron.py` & `forerunner-0.0.6/src/forerunner/job/cron.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import asyncio
-from contextlib import AsyncExitStack
 from datetime import datetime
 
 from croniter import croniter
-from ipdb import set_trace
 
-from forerunner.dependency.utils import resolve_dependencies
 
 from .base import Job
 
 
 class Cron(Job):
     def __init__(self, *, expr: str, eager: bool, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `forerunner-0.0.5/src/forerunner/job/sub.py` & `forerunner-0.0.6/src/forerunner/job/sub.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from contextlib import AsyncExitStack
 
-from forerunner.dependency.utils import resolve_dependencies
 from forerunner.queue.queue import BaseQueue
 
 from .base import Job
 
 
 class Sub(Job):
     def __init__(self, *, queue: BaseQueue, **kwargs):
```

### Comparing `forerunner-0.0.5/src/forerunner/queue/queue.py` & `forerunner-0.0.6/src/forerunner/queue/queue.py`

 * *Files identical despite different names*

