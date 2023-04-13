# Comparing `tmp/xqute-0.1.5.tar.gz` & `tmp/xqute-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xqute-0.1.5.tar", max compression
+gzip compressed data, was "xqute-0.2.0.tar", max compression
```

## Comparing `xqute-0.1.5.tar` & `xqute-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-03-14 04:57:26.990411 xqute-0.1.5/LICENSE
--rw-r--r--   0        0        0     3985 2023-03-14 04:57:26.994411 xqute-0.1.5/README.md
--rw-r--r--   0        0        0     1020 2023-03-14 04:57:26.994411 xqute-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      246 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/__init__.py
--rw-r--r--   0        0        0     3344 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/defaults.py
--rw-r--r--   0        0        0     8552 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/job.py
--rw-r--r--   0        0        0     3001 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/plugin.py
--rw-r--r--   0        0        0     8081 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/scheduler.py
--rw-r--r--   0        0        0      609 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/schedulers/__init__.py
--rw-r--r--   0        0        0     3071 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/schedulers/local_scheduler.py
--rw-r--r--   0        0        0     3962 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/schedulers/sge_scheduler.py
--rw-r--r--   0        0        0     1855 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/utils.py
--rw-r--r--   0        0        0     9308 2023-03-14 04:57:26.994411 xqute-0.1.5/xqute/xqute.py
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 xqute-0.1.5/setup.py
--rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 xqute-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 04:44:12.633953 xqute-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4795 2023-04-13 04:44:12.633953 xqute-0.2.0/README.md
+-rw-r--r--   0        0        0     1173 2023-04-13 04:44:12.637953 xqute-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/defaults.py
+-rw-r--r--   0        0        0     8595 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/job.py
+-rw-r--r--   0        0        0     3017 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/plugin.py
+-rw-r--r--   0        0        0     8109 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/scheduler.py
+-rw-r--r--   0        0        0      633 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/__init__.py
+-rw-r--r--   0        0        0     2361 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/local_scheduler.py
+-rw-r--r--   0        0        0     4225 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/sge_scheduler.py
+-rw-r--r--   0        0        0     7155 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/slurm_scheduler.py
+-rw-r--r--   0        0        0       44 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/__init__.py
+-rw-r--r--   0        0        0     3547 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/client.py
+-rw-r--r--   0        0        0     2548 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/scheduler.py
+-rw-r--r--   0        0        0      691 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/submitter.py
+-rw-r--r--   0        0        0     2176 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/utils.py
+-rw-r--r--   0        0        0     9511 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/xqute.py
+-rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 xqute-0.2.0/setup.py
+-rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 xqute-0.2.0/PKG-INFO
```

### Comparing `xqute-0.1.5/LICENSE` & `xqute-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xqute-0.1.5/README.md` & `xqute-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 An xqute is initialized by:
 ```python
 xqute = Xqute(...)
 ```
 Available arguments are:
 
+- loglevel: The log level (Default: `INFO`)
 - scheduler: The scheduler class or name
 - plugins: The plugins to enable/disable for this session
 - job_metadir: The job meta directory (Default: `./.xqute/`)
 - job_error_strategy: The strategy when there is error happened
 - job_num_retries: Max number of retries when job_error_strategy is retry
 - job_submission_batch: The number of consumers to submit jobs
 - scheduler_forks: Max number of job forks
@@ -61,33 +62,76 @@
 To push a job into the queue:
 ```python
 await xqute.put(['echo', 1])
 ```
 
 ### Using SGE scheduler
 ```python
-xqute = Xqute('sge',
-              scheduler_forks=100,
-              qsub='path to qsub',
-              qdel='path to qdel',
-              qstat='path to qstat',
-              sge_q='1-day',
-              ...)
+xqute = Xqute(
+    'sge',
+    scheduler_forks=100,
+    qsub='path to qsub',
+    qdel='path to qdel',
+    qstat='path to qstat',
+    sge_q='1-day',  # or qsub_q='1-day'
+    ...
+)
 ```
 Keyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:
 `sge_l=['h_vmem=2G', 'gpu=1']` will be expanded in wrapped script like this:
 ```shell
 # ...
 
 #$ -l h_vmem=2G
 #$ -l gpu=1
 
 # ...
 ```
 
+
+### Using Slurm scheduler
+
+```python
+xqute = Xqute(
+    'slurm',
+    scheduler_forks=100,
+    sbatch='path to sbatch',
+    scancel='path to scancel',
+    squeue='path to squeue',
+    sbatch_partition='1-day',  # or slurm_partition='1-day'
+    sbatch_time='01:00:00',
+    ...
+)
+```
+
+### Using ssh scheduler
+
+```python
+xqute = Xqute(
+    'ssh',
+    scheduler_forks=100,
+    ssh='path to ssh',
+    ssh_servers={
+        "server1": {
+            "user": ...,
+            "port": 22,
+            "keyfile": ...,
+            # How long to keep the ssh connection alive
+            "ctrl_persist": 600,
+            # Where to store the control socket
+            "ctrl_dir": "/tmp",
+        },
+        ...
+    }
+    ...
+)
+```
+
+SSH servers must share the same filesystem and using keyfile authentication.
+
 ### Plugins
 
 To write a plugin for `xqute`, you will need to implement the following hooks:
 
 - `on_init(scheduler)`: Right after scheduler object is initialized
 - `on_shutdown(scheduler, sig)`: When scheduler is shutting down
 - `on_job_init(scheduler, job)`: When the job is initialized
```

### Comparing `xqute-0.1.5/xqute/defaults.py` & `xqute-0.2.0/xqute/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,18 @@
     DEFAULT_JOB_NUM_RETRIES: Default number of retries when
         DEFAULT_JOB_ERROR_STRATEGY is retry
     DEFAULT_JOB_CMD_WRAPPER_SHELL: The default shell for job wrapper
     DEFAULT_JOB_CMD_WRAPPER_TEMPLATE: The template for job cmd wrapping
     DEFAULT_SCHEDULER_FORKS: Default number of job forks for scheduler
     DEFAULT_JOB_SUBMISSION_BATCH: Default consumer workers
 """
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Tuple, Union
+from typing import Tuple
 import uvloop
 
 uvloop.install()
 
 
 class JobErrorStrategy:
     """The strategy when error happen from jobs
@@ -57,15 +59,15 @@
     SUBMITTED: int = 3
     RUNNING: int = 4
     KILLING: int = 5
     FINISHED: int = 6
     FAILED: int = 7
 
     @classmethod
-    def get_name(cls, *statuses: Tuple[int]) -> Union[Tuple[str], str]:
+    def get_name(cls, *statuses: int) -> Tuple[str, ...] | str:
         """Get the name of the status
 
         Args:
             *statuses: The status values
 
         Returns:
             The name of the status if a single status is passed, otherwise
@@ -77,15 +79,14 @@
                 ret_dict[value] = name
         ret_tuple = tuple(ret_dict[status] for status in statuses)
         if len(ret_tuple) > 1:
             return ret_tuple
         return ret_tuple[0]  # pragma: no cover
 
 
-DEBUG = True
 LOGGER_NAME = 'XQUTE'
 
 DEFAULT_JOB_METADIR: Path = Path('./.xqute')
 DEFAULT_JOB_ERROR_STRATEGY: str = JobErrorStrategy.IGNORE
 DEFAULT_JOB_NUM_RETRIES: int = 3
 DEFAULT_JOB_SUBMISSION_BATCH: int = 8
 DEFAULT_JOB_CMD_WRAPPER_SHELL: str = '/bin/bash'
```

### Comparing `xqute-0.1.5/xqute/job.py` & `xqute-0.2.0/xqute/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from __future__ import annotations
 
 import shlex
 import shutil
 from abc import ABC, abstractmethod
 from os import PathLike, unlink
 from pathlib import Path
-from typing import TYPE_CHECKING, ClassVar, List, Optional, Union
+from typing import TYPE_CHECKING, ClassVar, List, Optional
 
-from aiopath import AsyncPath
+from aiopath import AsyncPath  # type: ignore
 
 from .defaults import (
     DEFAULT_JOB_METADIR,
     DEFAULT_JOB_CMD_WRAPPER_TEMPLATE,
     DEFAULT_JOB_CMD_WRAPPER_SHELL,
     JobStatus,
 )
@@ -70,30 +70,30 @@
 
     CMD_WRAPPER_TEMPLATE: ClassVar[str] = DEFAULT_JOB_CMD_WRAPPER_TEMPLATE
     CMD_WRAPPER_SHELL: ClassVar[str] = DEFAULT_JOB_CMD_WRAPPER_SHELL
 
     def __init__(
         self,
         index: int,
-        cmd: Union[str, List[str]],
+        cmd: str | List[str],
         metadir: PathLike = DEFAULT_JOB_METADIR,
         error_retry: Optional[bool] = None,
         num_retries: Optional[int] = None,
     ):
         """Construct"""
         self.cmd = cmd
         self.index = index
         self.metadir = Path(metadir) / str(self.index)
         self.metadir.mkdir(exist_ok=True, parents=True)
 
         # The name of the job, should be the unique id from the scheduler
         self.trial_count = 0
         self.prev_status = JobStatus.INIT
 
-        self._jid = None
+        self._jid: int | str | None = None
         self._status = JobStatus.INIT
         self._rc = -1
         self._error_retry = error_retry
         self._num_retries = num_retries
 
     def __repr__(self) -> str:
         """repr of the job"""
@@ -101,25 +101,25 @@
             return f"<{self.__class__.__name__}-{self.index}: ({self.cmd})>"
         return (
             f"<{self.__class__.__name__}-{self.index}({self.jid}): "
             f"({self.cmd})>"
         )
 
     @property
-    def jid(self) -> str:
+    def jid(self) -> int | str | None:
         """Get the jid of the job in scheduler system"""
         if self._jid is None and not self.jid_file.is_file():
             return None
         if self._jid is not None:
             return self._jid
         self._jid = self.jid_file.read_text()
         return self._jid
 
     @jid.setter
-    def jid(self, uniqid: Union[int, str]):
+    def jid(self, uniqid: int | str):
         self._jid = uniqid
         self.jid_file.write_text(str(uniqid))
 
     @property
     def stdout_file(self) -> Path:
         """The stdout file of the job"""
         return self.metadir / "job.stdout"
@@ -170,15 +170,15 @@
                 TypeError,
             ):  # pragma: no cover
                 pass
 
         if (
             self._status == JobStatus.FAILED
             and self._error_retry
-            and self.trial_count < self._num_retries
+            and self.trial_count < self._num_retries  # type: ignore
         ):
             self._status = JobStatus.RETRYING
 
         if self.prev_status != self._status and (
             self._status == JobStatus.RETRYING
             or self._status >= JobStatus.KILLING
         ):
@@ -264,13 +264,13 @@
             not await AsyncPath(wrapt_script).is_file()
             or await a_read_text(wrapt_script) != wrapt_cmd
         ):
             await a_write_text(wrapt_script, self.wrap_cmd(scheduler))
         return wrapt_script
 
     @abstractmethod
-    def wrap_cmd(self, scheduler: Scheduler) -> None:
+    def wrap_cmd(self, scheduler: Scheduler) -> str:
         """Wrap the command for the scheduler to submit and run
 
         Args:
             scheduler: The scheduler
         """
```

### Comparing `xqute-0.1.5/xqute/plugin.py` & `xqute-0.2.0/xqute/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Hook specifications for scheduler plugins"""
 from __future__ import annotations
 
 import signal
 from typing import TYPE_CHECKING
-from simplug import Simplug, SimplugResult
+from simplug import Simplug, SimplugResult  # type: ignore
 
 if TYPE_CHECKING:  # pragma: no cover
     from .xqute import Xqute
     from .job import Job
     from .scheduler import Scheduler
```

### Comparing `xqute-0.1.5/xqute/scheduler.py` & `xqute-0.2.0/xqute/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """The scheduler to schedule jobs"""
+from __future__ import annotations
+
 import os
 import signal
 from abc import ABC, abstractmethod
-from typing import ClassVar, List, Type, Union
+from typing import List, Type
 
-from diot import Diot
+from diot import Diot  # type: ignore
 
 from .defaults import JobStatus
 from .utils import logger, asyncify, a_write_text
 from .job import Job
 from .plugin import plugin
 
 
@@ -23,16 +25,16 @@
         prescript: The script to run before the command
         postscript: The script to run after the command
         **kwargs: Other arguments for the scheduler
     """
 
     __slots__ = ("config",)
 
-    name: ClassVar[str]
-    job_class: ClassVar[Type[Job]]
+    name: str
+    job_class: Type[Job]
 
     def __init__(
         self, forks: int, prescript: str = "", postscript: str = "", **kwargs
     ):
         """Construct"""
         self.config = Diot(
             forks=forks, prescript=prescript, postscript=postscript, **kwargs
@@ -57,28 +59,28 @@
                 "/Scheduler-%s Skip submitting, "
                 "job %r is already submitted or running.",
                 self.name,
                 job,
             )
             return
 
-        exception = None
+        exception: Exception | None = None
         try:
             if await plugin.hooks.on_job_submitting(self, job) is False:
                 return
             await job.clean()
 
             try:
                 # raise the exception immediately
                 # it somehow cannot be catched immediately
                 job.jid = await self.submit_job(job)
             except Exception as exc:
                 exception = RuntimeError(
                     "Failed to submit job: "
-                    f"[{type(exc).__name__}]{exc}"
+                    f"[{type(exc).__name__}] {exc}"
                 )
                 exception.__traceback__ = exc.__traceback__
             else:
                 logger.info(
                     "/Scheduler-%s Job %s submitted (jid: %s, wrapped: %s)",
                     self.name,
                     job.index,
@@ -226,15 +228,15 @@
         if job.jid_file.is_file():
             if await self.job_is_running(job):
                 job.status = JobStatus.SUBMITTED
                 return True
         return False
 
     @abstractmethod
-    async def submit_job(self, job: Job) -> Union[int, str]:
+    async def submit_job(self, job: Job) -> int | str:
         """Submit a job
 
         Args:
             job: The job
 
         Returns:
             The unique id in the scheduler system
```

### Comparing `xqute-0.1.5/xqute/schedulers/__init__.py` & `xqute-0.2.0/xqute/schedulers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Builtin schedulers"""
+from __future__ import annotations
+
 from importlib import import_module
-from typing import Type, Union
+from typing import Type
+
 from ..scheduler import Scheduler
 
 
-def get_scheduler(scheduler: Union[str, Type[Scheduler]]) -> Type[Scheduler]:
+def get_scheduler(scheduler: str | Type[Scheduler]) -> Type[Scheduler]:
     """Get the scheduler class
 
     Args:
         sched_name: The scheduler name
             Defined in the scheduler class
 
     Returns:
```

### Comparing `xqute-0.1.5/xqute/schedulers/sge_scheduler.py` & `xqute-0.2.0/xqute/schedulers/sge_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,49 +5,61 @@
 from ..job import Job
 from ..scheduler import Scheduler
 from ..utils import a_read_text
 
 
 class SgeJob(Job):
     """SGE job"""
+
     def wrap_cmd(self, scheduler: Scheduler) -> str:
         """Wrap the command to enable status, returncode, cleaning when
         job exits
 
         Args:
             scheduler: The scheduler
 
         Returns:
             The wrapped script
         """
-        options = {key[4:]: val for key, val in scheduler.config.items()
-                   if key.startswith('sge_')}
-        jobname_prefix = scheduler.config.get('scheduler_jobprefix',
-                                              scheduler.name)
-        options['N'] = f'{jobname_prefix}.{self.index}'
-        options['cwd'] = True
-        options['o'] = self.stdout_file
-        options['e'] = self.stderr_file
+        options = {
+            key[4:]: val
+            for key, val in scheduler.config.items()
+            if key.startswith("sge_")
+        }
+        qsub_options = {
+            key[5:]: val
+            for key, val in scheduler.config.items()
+            if key.startswith("qsub_")
+        }
+        options.update(qsub_options)
+        jobname_prefix = scheduler.config.get(
+            "scheduler_jobprefix", scheduler.name
+        )
+        options["N"] = f"{jobname_prefix}.{self.index}"
+        options["cwd"] = True
+        options["o"] = self.stdout_file
+        options["e"] = self.stderr_file
 
         options_list = []
         for key, val in options.items():
             if val is True:
                 options_list.append(f"#$ -{key}")
             elif isinstance(val, (tuple, list)):
                 for optval in val:
                     options_list.append(f"#$ -{key} {optval}")
             else:
                 options_list.append(f"#$ -{key} {val}")
-        options_str = '\n'.join(options_list)
+        options_str = "\n".join(options_list)
 
         return self.CMD_WRAPPER_TEMPLATE.format(
-            shebang=f'#!{self.CMD_WRAPPER_SHELL}\n{options_str}\n',
+            shebang=f"#!{self.CMD_WRAPPER_SHELL}\n{options_str}\n",
             prescript=scheduler.config.prescript,
             postscript=scheduler.config.postscript,
-            job=self, status=JobStatus
+            job=self,
+            status=JobStatus,
         )
 
 
 class SgeScheduler(Scheduler):
     """The sge scheduler
 
     Attributes:
@@ -59,51 +71,54 @@
         qstat: path to qstat command
         qdel: path to qdel command
         sge_*: SGE options for qsub. List or tuple options will be expanded.
             For example: `sge_l=['hvmem=2G', 'gpu=1']` will be expaned into
             `-l h_vmem=2G -l gpu=1`
         ... other Scheduler args
     """
-    name: str = 'sge'
+
+    name: str = "sge"
     job_class: Type[Job] = SgeJob
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.qsub = self.config.get('qsub', 'qsub')
-        self.qdel = self.config.get('qdel', 'qdel')
-        self.qstat = self.config.get('qstat', 'qstat')
+        self.qsub = self.config.get("qsub", "qsub")
+        self.qdel = self.config.get("qdel", "qdel")
+        self.qstat = self.config.get("qstat", "qstat")
 
     async def submit_job(self, job: Job) -> str:
         """Submit a job to SGE
 
         Args:
             job: The job
 
         Returns:
             The job id
         """
         proc = await asyncio.create_subprocess_exec(
-            self.qsub, str(await job.wrapped_script(self)),
+            self.qsub,
+            str(await job.wrapped_script(self)),
             stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE
+            stderr=asyncio.subprocess.PIPE,
         )
         stdout, _ = await proc.communicate()
         # Your job 613815 (...) has been submitted
         return stdout.decode().split()[2]
 
     async def kill_job(self, job: Job):
         """Kill a job on SGE
 
         Args:
             job: The job
         """
         proc = await asyncio.create_subprocess_exec(
-            self.qdel, job.jid,
+            self.qdel,
+            str(job.jid),
             stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE
+            stderr=asyncio.subprocess.PIPE,
         )
         await proc.wait()
 
     async def job_is_running(self, job: Job) -> bool:
         """Tell if a job is really running, not only the job.jid_file
 
         In case where the jid file is not cleaned when job is done.
@@ -119,13 +134,15 @@
         except FileNotFoundError:
             return False
 
         if not jid:
             return False
 
         proc = await asyncio.create_subprocess_exec(
-            self.qstat, '-j', jid,
+            self.qstat,
+            "-j",
+            jid,
             stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE
+            stderr=asyncio.subprocess.PIPE,
         )
         await proc.wait()
         return proc.returncode == 0
```

### Comparing `xqute-0.1.5/xqute/utils.py` & `xqute-0.2.0/xqute/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 """Utilities for xqute"""
 import logging
 from os import PathLike
-from typing import Callable, Coroutine
+from typing import Callable
 
 import asyncio
 from functools import partial, wraps
 
-import aiopath as aiop
+import aiopath as aiop  # type: ignore
 import aiofile as aiof
+from rich.logging import RichHandler
 
-from .defaults import DEBUG, LOGGER_NAME
+from .defaults import LOGGER_NAME
 
 
 # helper functions to read and write the whole content of the file
 async def a_read_text(path: PathLike) -> str:
     """Read the text from a file asyncly
 
     Args:
         path: The path of the file
 
     Returns:
         The content of the file
     """
-    async with aiof.async_open(path, mode='rt') as file:
+    async with aiof.async_open(path, mode='rt') as file:  # type: ignore
         return await file.read()
 
 
 async def a_write_text(path: PathLike, content: str):
     """Write the text to a file asyncly
 
     Args:
         path: The path to the file
         content: The content to be written to the file
     """
-    async with aiof.async_open(path, mode='wt') as file:
+    async with aiof.async_open(path, mode='wt') as file:  # type: ignore
         await file.write(content)
 
 
-def asyncify(func: Callable) -> Coroutine:
+def asyncify(func: Callable) -> Callable:
     """Turn a sync function into a Coroutine, can be used as a decorator
 
     Args:
         func: The sync function
 
     Returns:
         The Coroutine
@@ -62,12 +63,23 @@
         path: The path to the directory to be made
         *args: args for `Path(path).mkdir(...)`
         **kwargs: kwargs for `Path(path).mkdir(...)`
     """
     await aiop.AsyncPath(path).mkdir(*args, **kwargs)
 
 
+class DuplicateFilter(logging.Filter):
+    def __init__(self):
+        super().__init__()
+        self.prev_msg = None
+
+    def filter(self, record):
+        message = record.getMessage()
+        if message == self.prev_msg:
+            return False
+        self.prev_msg = message
+        return True
+
+
 logger = logging.getLogger(LOGGER_NAME)
-logger.setLevel(logging.INFO)
-if DEBUG:
-    from rich.logging import RichHandler
-    logger.addHandler(RichHandler(show_path=False, omit_repeated_times=False))
+logger.addHandler(RichHandler(show_path=False, omit_repeated_times=False))
+logger.addFilter(DuplicateFilter())
```

### Comparing `xqute-0.1.5/xqute/xqute.py` & `xqute-0.2.0/xqute/xqute.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
         buffer_queue: A buffer queue to save the pushed jobs
         queue: The job queue
         scheduler: The scheduler
         task: The task of producer and consumers
 
     Args:
+        loglevel: The log level
         scheduler: The scheduler class or name
         plugins: The plugins to be enabled or disabled
             to disable a plugin, using `no:plugin_name`
             either all plugin names should be prefixed with 'no:' or none
             of them should
             To enabled plugins, objects are
         job_metadir: The job meta directory
@@ -74,25 +75,29 @@
     EMPTY_BUFFER_SLEEP_TIME: int = 1
 
     def __init__(
         self,
         scheduler: str | Type[Scheduler] = "local",
         plugins: List[Any] | None = None,
         *,
+        loglevel: str = "INFO",
         job_metadir: PathLike = DEFAULT_JOB_METADIR,
         job_submission_batch: int = DEFAULT_JOB_SUBMISSION_BATCH,
         job_error_strategy: str = DEFAULT_JOB_ERROR_STRATEGY,
         job_num_retries: int = DEFAULT_JOB_NUM_RETRIES,
         scheduler_forks: int = DEFAULT_SCHEDULER_FORKS,
         scheduler_prescript: str = "",
         scheduler_postscript: str = "",
         **scheduler_opts,
     ) -> None:
         """Construct"""
-        self.jobs = []
+        # Set log level
+        logger.setLevel(loglevel.upper())
+
+        self.jobs: List[Job] = []
 
         if plugins is not None:
             no_plugins = [
                 isinstance(plug, str) and plug.startswith("no:")
                 for plug in plugins
             ]
             if any(no_plugins) and not all(no_plugins):
@@ -120,18 +125,18 @@
 
         self.job_submission_batch = job_submission_batch
         self._job_metadir = job_metadir
         Path(self._job_metadir).mkdir(exist_ok=True)
         self._job_error_strategy = job_error_strategy
         self._job_num_retries = job_num_retries
 
-        self._cancelling = False
+        self._cancelling: bool | signal.Signals = False
 
-        self.buffer_queue = deque()
-        self.queue = asyncio.Queue()
+        self.buffer_queue: deque = deque()
+        self.queue: asyncio.Queue = asyncio.Queue()
         self.scheduler = get_scheduler(scheduler)(
             scheduler_forks,
             scheduler_prescript,
             scheduler_postscript,
             **scheduler_opts,
         )
 
@@ -219,15 +224,15 @@
                     self._job_error_strategy == JobErrorStrategy.RETRY
                 )
             if job._num_retries is None:
                 job._num_retries = self._job_num_retries
         else:
             job = self.scheduler.job_class(
                 len(self.jobs),
-                cmd,
+                cmd,  # type: ignore
                 self._job_metadir,
                 self._job_error_strategy == JobErrorStrategy.RETRY,
                 self._job_num_retries,
             )
         await plugin.hooks.on_job_init(self.scheduler, job)
         self.jobs.append(job)
         logger.info("/%s Pushing job: %r", self.name, job)
```

### Comparing `xqute-0.1.5/setup.py` & `xqute-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['xqute', 'xqute.schedulers']
+['xqute', 'xqute.schedulers', 'xqute.schedulers.ssh_scheduler']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['diot>=0.1,<0.2',
- 'psutil>=5,<6',
- 'rich>=13,<14',
- 'simplug>=0.2,<0.3',
- 'uvloop>=0,<1']
+['diot>=0.1,<0.2', 'rich>=13,<14', 'simplug>=0.3,<0.4', 'uvloop>=0,<1']
 
 extras_require = \
 {':python_version < "3.10"': ['aiopath>=0.5.0,<0.6.0'],
  ':python_version >= "3.10"': ['aiopath>=0.6,<0.7']}
 
 setup_kwargs = {
     'name': 'xqute',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': 'A job management system for python',
-    'long_description': '# xqute\n\nA job management system for python\n\n## Features\n\n- Written in async\n- Plugin system\n- Scheduler adaptor\n- Job retrying/pipeline halting when failed\n\n## Installation\n\n```\npip install xqute\n```\n\n## A toy example\n```python\nimport asyncio\nfrom xqute import Xqute\n\nasync def main():\n    # 3 jobs allowed to run at the same time\n    xqute = Xqute(scheduler_forks=3)\n    for _ in range(10):\n        await xqute.put(\'sleep 1\')\n    await xqute.run_until_complete()\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n![xqute](./xqute.png)\n\n\n## API\nhttps://pwwang.github.io/xqute/\n\n## Usage\n\n### Xqute object\n\nAn xqute is initialized by:\n```python\nxqute = Xqute(...)\n```\nAvailable arguments are:\n\n- scheduler: The scheduler class or name\n- plugins: The plugins to enable/disable for this session\n- job_metadir: The job meta directory (Default: `./.xqute/`)\n- job_error_strategy: The strategy when there is error happened\n- job_num_retries: Max number of retries when job_error_strategy is retry\n- job_submission_batch: The number of consumers to submit jobs\n- scheduler_forks: Max number of job forks\n- **scheduler_opts: Additional keyword arguments for scheduler\n\nNote that the producer must be initialized in an event loop.\n\nTo push a job into the queue:\n```python\nawait xqute.put([\'echo\', 1])\n```\n\n### Using SGE scheduler\n```python\nxqute = Xqute(\'sge\',\n              scheduler_forks=100,\n              qsub=\'path to qsub\',\n              qdel=\'path to qdel\',\n              qstat=\'path to qstat\',\n              sge_q=\'1-day\',\n              ...)\n```\nKeyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:\n`sge_l=[\'h_vmem=2G\', \'gpu=1\']` will be expanded in wrapped script like this:\n```shell\n# ...\n\n#$ -l h_vmem=2G\n#$ -l gpu=1\n\n# ...\n```\n\n### Plugins\n\nTo write a plugin for `xqute`, you will need to implement the following hooks:\n\n- `on_init(scheduler)`: Right after scheduler object is initialized\n- `on_shutdown(scheduler, sig)`: When scheduler is shutting down\n- `on_job_init(scheduler, job)`: When the job is initialized\n- `on_job_queued(scheduler, job)`: When the job is queued\n- `on_job_submitted(scheduler, job)`: When the job is submitted\n- `on_job_killing(scheduler, job)`: When the job is being killed\n- `on_job_killed(scheduler, job)`: When the job is killed\n- `on_job_failed(scheduler, job)`: When the job is failed\n- `on_job_succeeded(scheduler, job)`: When the job is succeeded\n\nNote that all hooks are corotines except `on_init` and `on_shutdown`, that means you should also implement them as corotines (sync implementations are allowed but will be warned).\n\nTo implement a hook, you have to fetch the plugin manager:\n\n```python\nfrom simplug import Simplug\npm = Simplug(\'xqute\')\n\n# or\nfrom xqute import simplug as pm\n```\n\nand then use the decorator `pm.impl`:\n\n```python\n@pm.impl\ndef on_init(scheduler):\n    ...\n```\n\n### Implementing a scheduler\n\nCurrently there are only 2 builtin schedulers: `local` and `sge`.\n\nOne can implement a scheduler by subclassing the `Scheduler` abstract class. There are three abstract methods that have to be implemented in the subclass:\n\n```python\nfrom xqute import Scheduer\n\nclass MyScheduler(Scheduler):\n    name = \'my\'\n    job_class: MyJob\n\n    async def submit_job(self, job):\n        """How to submit a job, return a unique id in the scheduler system\n        (the pid for local scheduler for example)\n        """\n\n    async def kill_job(self, job):\n        """How to kill a job"""\n\n    async def job_is_running(self, job):\n        """Check if a job is running"""\n```\n\nAs you may see, we may also need to implement a job class before `MyScheduler`. The only abstract method to be implemented is `wrap_cmd`:\n```python\nfrom xqute import Job\n\nclass MyJob(Job):\n\n    async def wrap_cmd(self, scheduler):\n        ...\n```\n\nYou have to use the trap command in the wrapped script to update job status, return code and clear the job id file.\n',
+    'long_description': '# xqute\n\nA job management system for python\n\n## Features\n\n- Written in async\n- Plugin system\n- Scheduler adaptor\n- Job retrying/pipeline halting when failed\n\n## Installation\n\n```\npip install xqute\n```\n\n## A toy example\n```python\nimport asyncio\nfrom xqute import Xqute\n\nasync def main():\n    # 3 jobs allowed to run at the same time\n    xqute = Xqute(scheduler_forks=3)\n    for _ in range(10):\n        await xqute.put(\'sleep 1\')\n    await xqute.run_until_complete()\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n![xqute](./xqute.png)\n\n\n## API\nhttps://pwwang.github.io/xqute/\n\n## Usage\n\n### Xqute object\n\nAn xqute is initialized by:\n```python\nxqute = Xqute(...)\n```\nAvailable arguments are:\n\n- loglevel: The log level (Default: `INFO`)\n- scheduler: The scheduler class or name\n- plugins: The plugins to enable/disable for this session\n- job_metadir: The job meta directory (Default: `./.xqute/`)\n- job_error_strategy: The strategy when there is error happened\n- job_num_retries: Max number of retries when job_error_strategy is retry\n- job_submission_batch: The number of consumers to submit jobs\n- scheduler_forks: Max number of job forks\n- **scheduler_opts: Additional keyword arguments for scheduler\n\nNote that the producer must be initialized in an event loop.\n\nTo push a job into the queue:\n```python\nawait xqute.put([\'echo\', 1])\n```\n\n### Using SGE scheduler\n```python\nxqute = Xqute(\n    \'sge\',\n    scheduler_forks=100,\n    qsub=\'path to qsub\',\n    qdel=\'path to qdel\',\n    qstat=\'path to qstat\',\n    sge_q=\'1-day\',  # or qsub_q=\'1-day\'\n    ...\n)\n```\nKeyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:\n`sge_l=[\'h_vmem=2G\', \'gpu=1\']` will be expanded in wrapped script like this:\n```shell\n# ...\n\n#$ -l h_vmem=2G\n#$ -l gpu=1\n\n# ...\n```\n\n\n### Using Slurm scheduler\n\n```python\nxqute = Xqute(\n    \'slurm\',\n    scheduler_forks=100,\n    sbatch=\'path to sbatch\',\n    scancel=\'path to scancel\',\n    squeue=\'path to squeue\',\n    sbatch_partition=\'1-day\',  # or slurm_partition=\'1-day\'\n    sbatch_time=\'01:00:00\',\n    ...\n)\n```\n\n### Using ssh scheduler\n\n```python\nxqute = Xqute(\n    \'ssh\',\n    scheduler_forks=100,\n    ssh=\'path to ssh\',\n    ssh_servers={\n        "server1": {\n            "user": ...,\n            "port": 22,\n            "keyfile": ...,\n            # How long to keep the ssh connection alive\n            "ctrl_persist": 600,\n            # Where to store the control socket\n            "ctrl_dir": "/tmp",\n        },\n        ...\n    }\n    ...\n)\n```\n\nSSH servers must share the same filesystem and using keyfile authentication.\n\n### Plugins\n\nTo write a plugin for `xqute`, you will need to implement the following hooks:\n\n- `on_init(scheduler)`: Right after scheduler object is initialized\n- `on_shutdown(scheduler, sig)`: When scheduler is shutting down\n- `on_job_init(scheduler, job)`: When the job is initialized\n- `on_job_queued(scheduler, job)`: When the job is queued\n- `on_job_submitted(scheduler, job)`: When the job is submitted\n- `on_job_killing(scheduler, job)`: When the job is being killed\n- `on_job_killed(scheduler, job)`: When the job is killed\n- `on_job_failed(scheduler, job)`: When the job is failed\n- `on_job_succeeded(scheduler, job)`: When the job is succeeded\n\nNote that all hooks are corotines except `on_init` and `on_shutdown`, that means you should also implement them as corotines (sync implementations are allowed but will be warned).\n\nTo implement a hook, you have to fetch the plugin manager:\n\n```python\nfrom simplug import Simplug\npm = Simplug(\'xqute\')\n\n# or\nfrom xqute import simplug as pm\n```\n\nand then use the decorator `pm.impl`:\n\n```python\n@pm.impl\ndef on_init(scheduler):\n    ...\n```\n\n### Implementing a scheduler\n\nCurrently there are only 2 builtin schedulers: `local` and `sge`.\n\nOne can implement a scheduler by subclassing the `Scheduler` abstract class. There are three abstract methods that have to be implemented in the subclass:\n\n```python\nfrom xqute import Scheduer\n\nclass MyScheduler(Scheduler):\n    name = \'my\'\n    job_class: MyJob\n\n    async def submit_job(self, job):\n        """How to submit a job, return a unique id in the scheduler system\n        (the pid for local scheduler for example)\n        """\n\n    async def kill_job(self, job):\n        """How to kill a job"""\n\n    async def job_is_running(self, job):\n        """Check if a job is running"""\n```\n\nAs you may see, we may also need to implement a job class before `MyScheduler`. The only abstract method to be implemented is `wrap_cmd`:\n```python\nfrom xqute import Job\n\nclass MyJob(Job):\n\n    async def wrap_cmd(self, scheduler):\n        ...\n```\n\nYou have to use the trap command in the wrapped script to update job status, return code and clear the job id file.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/xqute',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `xqute-0.1.5/PKG-INFO` & `xqute-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: xqute
-Version: 0.1.5
+Version: 0.2.0
 Summary: A job management system for python
 Home-page: https://github.com/pwwang/xqute
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiopath (>=0.5.0,<0.6.0) ; python_version < "3.10"
 Requires-Dist: aiopath (>=0.6,<0.7) ; python_version >= "3.10"
 Requires-Dist: diot (>=0.1,<0.2)
-Requires-Dist: psutil (>=5,<6)
 Requires-Dist: rich (>=13,<14)
-Requires-Dist: simplug (>=0.2,<0.3)
+Requires-Dist: simplug (>=0.3,<0.4)
 Requires-Dist: uvloop (>=0,<1)
 Project-URL: Repository, https://github.com/pwwang/xqute
 Description-Content-Type: text/markdown
 
 # xqute
 
 A job management system for python
@@ -69,14 +67,15 @@
 
 An xqute is initialized by:
 ```python
 xqute = Xqute(...)
 ```
 Available arguments are:
 
+- loglevel: The log level (Default: `INFO`)
 - scheduler: The scheduler class or name
 - plugins: The plugins to enable/disable for this session
 - job_metadir: The job meta directory (Default: `./.xqute/`)
 - job_error_strategy: The strategy when there is error happened
 - job_num_retries: Max number of retries when job_error_strategy is retry
 - job_submission_batch: The number of consumers to submit jobs
 - scheduler_forks: Max number of job forks
@@ -87,33 +86,76 @@
 To push a job into the queue:
 ```python
 await xqute.put(['echo', 1])
 ```
 
 ### Using SGE scheduler
 ```python
-xqute = Xqute('sge',
-              scheduler_forks=100,
-              qsub='path to qsub',
-              qdel='path to qdel',
-              qstat='path to qstat',
-              sge_q='1-day',
-              ...)
+xqute = Xqute(
+    'sge',
+    scheduler_forks=100,
+    qsub='path to qsub',
+    qdel='path to qdel',
+    qstat='path to qstat',
+    sge_q='1-day',  # or qsub_q='1-day'
+    ...
+)
 ```
 Keyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:
 `sge_l=['h_vmem=2G', 'gpu=1']` will be expanded in wrapped script like this:
 ```shell
 # ...
 
 #$ -l h_vmem=2G
 #$ -l gpu=1
 
 # ...
 ```
 
+
+### Using Slurm scheduler
+
+```python
+xqute = Xqute(
+    'slurm',
+    scheduler_forks=100,
+    sbatch='path to sbatch',
+    scancel='path to scancel',
+    squeue='path to squeue',
+    sbatch_partition='1-day',  # or slurm_partition='1-day'
+    sbatch_time='01:00:00',
+    ...
+)
+```
+
+### Using ssh scheduler
+
+```python
+xqute = Xqute(
+    'ssh',
+    scheduler_forks=100,
+    ssh='path to ssh',
+    ssh_servers={
+        "server1": {
+            "user": ...,
+            "port": 22,
+            "keyfile": ...,
+            # How long to keep the ssh connection alive
+            "ctrl_persist": 600,
+            # Where to store the control socket
+            "ctrl_dir": "/tmp",
+        },
+        ...
+    }
+    ...
+)
+```
+
+SSH servers must share the same filesystem and using keyfile authentication.
+
 ### Plugins
 
 To write a plugin for `xqute`, you will need to implement the following hooks:
 
 - `on_init(scheduler)`: Right after scheduler object is initialized
 - `on_shutdown(scheduler, sig)`: When scheduler is shutting down
 - `on_job_init(scheduler, job)`: When the job is initialized
```

