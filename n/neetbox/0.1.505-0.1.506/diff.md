# Comparing `tmp/neetbox-0.1.505.tar.gz` & `tmp/neetbox-0.1.506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.505.tar", max compression
+gzip compressed data, was "neetbox-0.1.506.tar", max compression
```

## Comparing `neetbox-0.1.505.tar` & `neetbox-0.1.506.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-04-12 12:16:59.917266 neetbox-0.1.505/LICENSE
--rw-r--r--   0        0        0      397 2023-04-12 12:16:59.917266 neetbox-0.1.505/README.md
--rw-r--r--   0        0        0     2138 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2594 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/cli/parse.py
--rw-r--r--   0        0        0      549 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/config/__init__.py
--rw-r--r--   0        0        0      907 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/config/_config.py
--rw-r--r--   0        0        0       19 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/core/core.py
--rw-r--r--   0        0        0      418 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     6754 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      301 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/_default.py
--rw-r--r--   0        0        0    12181 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18657 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      171 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5485 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2018 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1245 2023-04-12 12:16:59.925266 neetbox-0.1.505/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.505/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 15:25:13.784400 neetbox-0.1.506/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-13 15:25:13.784400 neetbox-0.1.506/README.md
+-rw-r--r--   0        0        0     2824 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/config/_config.py
+-rw-r--r--   0        0        0     1094 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      499 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     1850 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     2989 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0      409 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     7527 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18647 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5594 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2165 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1332 2023-04-13 15:25:13.792400 neetbox-0.1.506/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.506/PKG-INFO
```

### Comparing `neetbox-0.1.505/LICENSE` & `neetbox-0.1.506/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/cli/parse.py` & `neetbox-0.1.506/neetbox/cli/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import argparse
 import os
+import json
 import neetbox
 from neetbox.logging.logger import Logger
+from neetbox.logging.formatting import LogStyle
+from neetbox.daemon._apis import get_status_of
 
-logger = Logger("NEETBOX")  # builtin standalone logger
+_log_style = LogStyle()
+_log_style.with_datetime = False
+logger = Logger("NEETBOX", style=_log_style)  # builtin standalone logger
 
 
 def handle_status(args):
-    logger.err(
-        "This feature is not availiable. CLI Features are still under construction."
-    )
-    pass
+    _stat_json = None
+    try:
+        _stat_json = get_status_of()
+        print(json.dumps(_stat_json))
+    except Exception as e:
+        logger.log("Could not fetch data. Is there any project with NEETBOX running?")
 
 
 def handle_init(args):
-    path = vars(args)["pathspec"]
-    path = None if not len(path) else path[0]
+    name = vars(args)["name"]
     try:
-        neetbox.init()
-        logger.skip_lines(2)
-        logger.banner("neetbox", font="ansishadow")
-        logger.log("Welcome to NEETBOX")
+        if neetbox.init(name=name):
+            logger.skip_lines(2)
+            logger.banner("neetbox", font="ansishadow")
+            logger.log("Welcome to NEETBOX")
     except Exception as e:
-        logger.err(f"Failed to init {path}: {e}")
+        logger.err(f"Failed to init here: {e}")
 
 
 def handle_archive(args):
     logger.err(
         "This feature is not availiable. CLI Features are still under construction."
     )
     pass
@@ -61,15 +67,22 @@
 status_parser = subparsers.add_parser("status", help="Show the working tree status")
 status_parser.set_defaults(handle=handle_status)
 
 init_parser = subparsers.add_parser(
     "init",
     help="initialize current folder as workspace and generate the config file from defaults",
 )
-init_parser.add_argument("pathspec", help="Files to add content from", nargs="*")
+init_parser.add_argument(
+    "--name",
+    "-n",
+    help="set project name",
+    metavar="name",
+    required=False,
+    default=None,
+)
 init_parser.set_defaults(handle=handle_init)
 
 commit_parser = subparsers.add_parser(
     "archive", help="Record changes to the repository"
 )
 commit_parser.add_argument(
     "--message",
```

### Comparing `neetbox-0.1.505/neetbox/integrations/engine.py` & `neetbox-0.1.506/neetbox/integrations/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# -*- coding: utf-8 -*-
+#
+# Author: GavinGong aka VisualDust
+# URL:    https://gong.host
+# Date:   20230413
+
 from enum import Enum
 from neetbox.logging import logger
 import importlib
 from typing import List,Optional
 
 class Engine(Enum):
     Torch = "torch"
```

### Comparing `neetbox-0.1.505/neetbox/integrations/environment.py` & `neetbox-0.1.506/neetbox/integrations/environment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+# -*- coding: utf-8 -*-
+#
+# Author: GavinGong aka VisualDust
+# URL:    https://gong.host
+# Date:   20230413
+
 import asyncio
 import getpass
 import importlib
 import locale
 import platform
 import re, os
 import subprocess
 import time
 from threading import Thread
 import pip
 import GPUtil
 import psutil
-from GPUtil import GPU as GPU
+from GPUtil import GPU
 from neetbox.logging import logger
 from typing import Union
 from neetbox.utils.framing import get_caller_identity_traceback
 from neetbox.utils.utils import Singleton
+from neetbox.daemon import watch
 
 
 class Package(metaclass=Singleton):
     def __init__(self) -> None:
         self.installed_packages = None
 
     @logger.catch
@@ -66,65 +73,83 @@
             importlib.import_module(package)
             self.installed_packages.append(package)
             return True
         except:
             package_name_install = (
                 package if type(try_install_if_not) is bool else try_install_if_not
             )
-            logger.warn(f"{caller_name} requires '{package_name_install}' which is not installed.")
+            logger.warn(
+                f"{caller_name} requires '{package_name_install}' which is not installed."
+            )
             if try_install_if_not:
-                return self.install(package=package_name_install,terminate=True)
+                return self.install(package=package_name_install, terminate=True)
             return False
 
 
 # singleton
 Package = Package()
 
 
-class _CPU_STAT:
+class _CPU_STAT(dict):
     def __init__(self, id=-1, percent=0.0, freq=0.0) -> None:
-        self.id = id
-        self.percent = percent
-        self.freq = freq
+        self["id"] = id
+        self["percent"] = percent
+        self["freq"] = freq
 
     def __str__(self) -> str:
-        return f"CPU{self.id}, {self.percent}%, {self.freq}Mhz"
+        return f"CPU{self['id']}, {(self['percent'])}%, {(self['freq'])}Mhz"
+
 
+class _GPU_STAT(dict):
+    def __init__(self, id=-1, name="GPU"):
+        self["id"] = id
+        self["name"] = name
+
+    @classmethod
+    def parse(cls, gpu: GPU):
+        _instance = _GPU_STAT()
+        _instance["id"] = gpu.id
+        _instance["name"] = gpu.name
+        _instance["memoryUtil"] = gpu.memoryUtil
+        _instance["memoryTotal"] = gpu.memoryTotal
+        _instance["memoryFree"] = gpu.memoryFree
+        _instance["memoryUsed"] = gpu.memoryUsed
+        _instance["temperature"] = gpu.temperature
+        _instance["driver"] = gpu.driver
+        return _instance
 
-class Environment(metaclass=Singleton):
+
+class Environment(dict, metaclass=Singleton):
     _update_interval = 1.0
     """
     The watcher may interacts with external libraries or devices
     a thread may be more suitable because it can provide a separate execution
     context with its own stack and memory space, which can simplify the design
     and debugging of the code.
     """
     _watcher: Thread = None
     _do_watch: bool = True
     _update_interval: float = 1.0
-    gpus: list = []
-    cpus: list = []
-    platform_info: dict = {}
 
     def __init__(self) -> None:
         # system
-        self.platform_info["username"] = getpass.getuser()
-        self.platform_info["machine"] = platform.machine()
-        self.platform_info["processor"] = (
+        self["username"] = getpass.getuser()
+        self["machine"] = platform.machine()
+        self["processor"] = (
             "unknown" if len(platform.processor()) == 0 else platform.processor()
         )
-        self.platform_info["os name"] = platform.system()
-        self.platform_info["os release"] = platform.version()
-        self.platform_info["architecture"] = platform.architecture()
-        self.platform_info["python version"] = platform.python_version()
-        self.platform_info["python build"] = platform.python_build()
+        self["os_name"] = platform.system()
+        self["os_release"] = platform.version()
+        self["architecture"] = platform.architecture()
+        self["python_version"] = platform.python_version()
+        self["python_build"] = platform.python_build()
         # device
-        self.cpus = [_CPU_STAT() for _ in range(psutil.cpu_count(logical=True))]
-        self.gpus = GPUtil.getGPUs()
-        self._with_gpu = False if len(self.gpus) == 0 else True
+        self["cpus"] = [_CPU_STAT() for _ in range(psutil.cpu_count(logical=True))]
+        self["gpus"] = [_GPU_STAT.parse(_gpu) for _gpu in GPUtil.getGPUs()]
+        self._with_gpu = False if len(self["gpus"]) == 0 else True
 
         # the environment shoube be imported in the __init__.py of the outer module. And the watcher thread should be auto started
         self.set_update_intervel()
 
     def set_update_intervel(self, intervel=1.0) -> None:
         if intervel < 1.0:
             self._do_watch = False
@@ -136,32 +161,32 @@
             def watcher_fun(env_instance: Environment, do_update_gpus: bool):
                 while env_instance._do_watch:
                     cpu_percent = psutil.cpu_percent(percpu=True)
                     cpu_freq = psutil.cpu_freq(percpu=True)
                     if len(cpu_freq) == 1:
                         cpu_freq = cpu_freq * len(cpu_percent)
                     for index in range(len(cpu_percent)):
-                        env_instance.cpus[index] = _CPU_STAT(
+                        env_instance["cpus"][index] = _CPU_STAT(
                             id=index,
                             percent=cpu_percent[index],
                             freq=cpu_freq[index],
                         )
                     if do_update_gpus:
-                        env_instance.gpus = GPUtil.getGPUs()
-                    env_instance.cpu_stats = psutil.cpu_stats()
+                        env_instance["gpus"] = [_GPU_STAT.parse(_gpu) for _gpu in GPUtil.getGPUs()]
+                    env_instance[""] = psutil.cpu_stats()
                     time.sleep(env_instance._update_interval)
 
             self._watcher = Thread(
                 target=watcher_fun, args=(self, self._with_gpu), daemon=True
             )
             self._watcher.start()
 
-    def _run(self, command):
+    def exec(self, command):
         """
-        Running a command like a terminal.
+        Run a terminal command.
 
         Args:
             command (str): The command need to run.
 
         Returns:
             int: The command return code.
             str: The command running results.
@@ -180,7 +205,13 @@
         err = raw_err.decode(enc)
 
         return rc, output.strip(), err.strip()
 
 
 # singleton
 Environment = Environment()
+
+
+# watch updates in daemon
+@watch(name="env")
+def update_env_stat():
+    return dict(Environment)
```

### Comparing `neetbox-0.1.505/neetbox/integrations/resource.py` & `neetbox-0.1.506/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/_colorama.py` & `neetbox-0.1.506/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.506/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.506/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.506/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.506/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.506/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/formatting.py` & `neetbox-0.1.506/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/logging/logger.py` & `neetbox-0.1.506/neetbox/logging/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
 import os
 import io
-import re
 from datetime import date, datetime
 from enum import Enum
 from neetbox.utils.framing import *
 from pyfiglet import Figlet, FigletFont
 from neetbox.utils import utils
 from neetbox.logging.formatting import *
 from inspect import isclass, iscoroutinefunction, isgeneratorfunction
```

### Comparing `neetbox-0.1.505/neetbox/pipeline/registry.py` & `neetbox-0.1.506/neetbox/pipeline/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# -*- coding: utf-8 -*-
+#
+# Author: GavinGong aka VisualDust
+# URL:    https://gong.host
+# Date:   20230413
+
 from neetbox.logging import logger
 from neetbox.utils.utils import *
 from typing import Optional, Union, Sequence
 import inspect
 import json
 import functools
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
```

### Comparing `neetbox-0.1.505/neetbox/plotting/plot.py` & `neetbox-0.1.506/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/arch/canny.py` & `neetbox-0.1.506/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/arch/cnn.py` & `neetbox-0.1.506/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/arch/kernels.py` & `neetbox-0.1.506/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.506/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/nlp.py` & `neetbox-0.1.506/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/torch/profile.py` & `neetbox-0.1.506/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/utils/framing.py` & `neetbox-0.1.506/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.505/neetbox/utils/utils.py` & `neetbox-0.1.506/neetbox/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230319
 
 import re
 import platform
 import functools
+import json
 
 
 def is_pure_ansi(text: str) -> bool:
     if not re.compile(r"^[A-Za-z0-9_-]+$").match(text):
         return False
     return True
 
@@ -35,14 +36,20 @@
     """
     if platform.system().lower() == "windows":
         rstr = r"[\/\\\:\*\?\"\<\>\|]"  # '/ \ : * ? " < > |'
         new_title = re.sub(rstr, "_", text)  # replace with '_'
         return new_title
     return text
 
+def is_jsonable(x):
+    try:
+        x = json.dumps(x)
+        return True
+    except (TypeError, OverflowError):
+        return False
 
 def singleton(class_):
     class class_w(class_):
         _instance = None
 
         def __new__(class_, *args, **kwargs):
             if class_w._instance is None:
```

### Comparing `neetbox-0.1.505/pyproject.toml` & `neetbox-0.1.506/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.505"
+version = "0.1.506"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
@@ -28,26 +28,30 @@
 
 # [[tool.poetry.source]]
 # name = "pypi"
 # url = "https://pypi.org/simple"
 # default = true
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4"
 numpy = ">=1"
 pillow = ">=8"
 pandas = ">=1"
 tqdm = ">=4"
 colorama = ">=0.3"
 toml = ">0.10"
 pytest = "*"
 gputil = ">=1.4"
 psutil = ">=5.0"
 injector = ">=0.20"
 pyfiglet = ">=0.8"
+python-daemon = "^3.0.1"
+flask = "^2.2.3"
+setproctitle = "^1.3.2"
+requests = "^2.28.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
-neetbox = 'neetbox.cli.parse:parse'
+neet = 'neetbox.cli.parse:parse'
```

### Comparing `neetbox-0.1.505/PKG-INFO` & `neetbox-0.1.506/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.505
+Version: 0.1.506
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
 Maintainer-email: gavin@gong.host
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -21,22 +21,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.3)
+Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: gputil (>=1.4)
 Requires-Dist: injector (>=0.20)
 Requires-Dist: numpy (>=1)
 Requires-Dist: pandas (>=1)
 Requires-Dist: pillow (>=8)
 Requires-Dist: psutil (>=5.0)
 Requires-Dist: pyfiglet (>=0.8)
 Requires-Dist: pytest
+Requires-Dist: python-daemon (>=3.0.1,<4.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: setproctitle (>=1.3.2,<2.0.0)
 Requires-Dist: toml (>0.10)
 Requires-Dist: tqdm (>=4)
 Project-URL: Repository, https://github.com/visualDust/neetbox
 Description-Content-Type: text/markdown
 
 # NEETBox contains use~~ful~~less tiny deeplearning code snippets
```

