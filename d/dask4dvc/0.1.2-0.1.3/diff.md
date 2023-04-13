# Comparing `tmp/dask4dvc-0.1.2.tar.gz` & `tmp/dask4dvc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.1.2.tar", max compression
+gzip compressed data, was "dask4dvc-0.1.3.tar", max compression
```

## Comparing `dask4dvc-0.1.2.tar` & `dask4dvc-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    13576 2022-08-04 12:36:17.183461 dask4dvc-0.1.2/LICENSE
--rw-r--r--   0        0        0     1351 2022-11-22 09:53:51.388916 dask4dvc-0.1.2/README.md
--rw-r--r--   0        0        0      521 2022-11-21 16:27:25.941273 dask4dvc-0.1.2/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2022-11-21 16:27:25.964261 dask4dvc-0.1.2/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     4451 2022-11-23 16:10:55.767378 dask4dvc-0.1.2/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     3037 2022-11-23 17:12:38.917158 dask4dvc-0.1.2/dask4dvc/methods.py
--rw-r--r--   0        0        0      166 2022-11-21 16:27:26.012268 dask4dvc-0.1.2/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      413 2022-11-23 12:40:55.800306 dask4dvc-0.1.2/dask4dvc/utils/config.py
--rw-r--r--   0        0        0      625 2022-11-23 17:12:38.921150 dask4dvc-0.1.2/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0     5807 2022-11-23 16:10:52.218429 dask4dvc-0.1.2/dask4dvc/utils/dvc.py
--rw-r--r--   0        0        0      951 2022-11-21 16:27:26.053283 dask4dvc-0.1.2/dask4dvc/utils/git.py
--rw-r--r--   0        0        0      823 2022-11-23 13:49:34.066979 dask4dvc-0.1.2/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1255 2022-11-23 17:13:15.571161 dask4dvc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 dask4dvc-0.1.2/setup.py
--rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 dask4dvc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1456 2023-04-13 11:02:16.857294 dask4dvc-0.1.3/README.md
+-rw-r--r--   0        0        0      521 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     5896 2023-04-13 11:06:02.374819 dask4dvc-0.1.3/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     3037 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/methods.py
+-rw-r--r--   0        0        0      166 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0      413 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/config.py
+-rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.1.3/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0     5807 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/dvc.py
+-rw-r--r--   0        0        0      951 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/git.py
+-rw-r--r--   0        0        0      903 2023-04-13 12:46:43.228695 dask4dvc-0.1.3/dask4dvc/utils/main.py
+-rw-r--r--   0        0        0     1241 2023-04-13 12:45:20.249602 dask4dvc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 dask4dvc-0.1.3/PKG-INFO
```

### Comparing `dask4dvc-0.1.2/LICENSE` & `dask4dvc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.2/README.md` & `dask4dvc-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Coverage Status](https://coveralls.io/repos/github/zincware/dask4dvc/badge.svg?branch=main)](https://coveralls.io/github/zincware/dask4dvc?branch=main)
 ![PyTest](https://github.com/zincware/dask4dvc/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
+[![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
@@ -27,8 +28,8 @@
     job_cpu=1,
     job_extra=['-N 1', '--cpus-per-task=1', '--tasks-per-node=64', "--gres=gpu:1"],
     scheduler_options={"port": 31415}
 )
 cluster.adapt()
 ```
 
-with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
+with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
```

### Comparing `dask4dvc-0.1.2/dask4dvc/__init__.py` & `dask4dvc-0.1.3/dask4dvc/__init__.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.2/dask4dvc/cli/main.py` & `dask4dvc-0.1.3/dask4dvc/cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """All methods that come directly from 'dask4dvc' CLI interace."""
 
 import importlib.metadata
 import logging
 import shutil
+import subprocess
 import typing
 
 import dask.distributed
 import typer
 
 from dask4dvc import methods, utils
 
@@ -27,25 +28,46 @@
     )
     leave: str = "Ask before stopping the client"
     option: str = (
         "Additional options to pass to 'dvc repro'. E.g. '--option=--force"
         " --option=--downstream'. Notice that some options like '--force' might show"
         " unexpected behavior."
     )
-    target: str = "Names of the stage to reproduce"
+    target: str = "Names of the stage to reproduce. Leave empty to run all stages."
+    detach: str = (
+        "Run the process in detached mode (Ctrl + C will not close 'dask4dvc' in the"
+        " background)."
+    )
+    config: str = "path to config file, e.g. 'dask4dvc.yaml'"
 
 
 @app.command()
 def repro(
     address: str = typer.Option(None, help=Help.address),
     option: typing.List[str] = typer.Option(None, help=Help.option),
-    target: typing.List[str] = typer.Option(None, help=Help.target),
     leave: bool = typer.Option(True, help=Help.leave),
+    detach: bool = typer.Option(False, "--detach", "-d", help=Help.detach),
+    config: str = typer.Option(None, help=Help.config),
+    target: list[str] = typer.Argument(None, help=Help.target, show_default=False),
 ) -> None:
     """Replicate 'dvc repro' command using dask."""
+    if detach:
+        cmd = ["dask4dvc", "repro"]
+        if address is not None:
+            cmd += ["--address", address]
+        if config is not None:
+            cmd += ["--config", config]
+        _ = subprocess.Popen(cmd, start_new_session=True)
+        # TODO add all kwargs!
+        return
+
+    if config is not None:
+        assert address is None, "Can not use address and config file"
+        address = utils.dask.get_cluster_from_config(config)
+
     with dask.distributed.Client(address) as client:
         log.info(client)
         result = client.submit(
             utils.dvc.repro, targets=target, options=option, pure=False
         )
 
         utils.dask.wait_for_futures(result)
@@ -68,20 +90,36 @@
     ),
     delete: typing.List[str] = typer.Option(
         ["branches", "temp"],
         "-D",
         "--delete",
         help="Remove the temporary branches and directories",
     ),
+    detach: bool = typer.Option(False, "--detach", "-d", help=Help.detach),
+    config: str = typer.Option(None, help=Help.config),
 ) -> None:
     """Replicate 'dvc exp run --run-all' command using dask.
 
     This will run the available experiments in parallel using dask.
     When finished, it will load the experiments using 'dvc exp run --run-all'.
     """
+    if config is not None:
+        assert address is None, "Can not use address and config file"
+        address = utils.dask.get_cluster_from_config(config)
+
+    if detach:
+        cmd = ["dask4dvc", "run"]
+        if address is not None:
+            cmd += ["--address", address]
+        if config is not None:
+            cmd += ["--config", config]
+        # TODO add all kwargs!
+        _ = subprocess.Popen(cmd, start_new_session=True)
+        return
+
     with methods.get_experiment_repos(delete=delete) as repos:
         with dask.distributed.Client(address) as client:
             log.info(client)
             results = {
                 name: client.submit(
                     utils.dvc.repro,
                     options=option,
```

### Comparing `dask4dvc-0.1.2/dask4dvc/methods.py` & `dask4dvc-0.1.3/dask4dvc/methods.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.2/dask4dvc/utils/dvc.py` & `dask4dvc-0.1.3/dask4dvc/utils/dvc.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.2/dask4dvc/utils/git.py` & `dask4dvc-0.1.3/dask4dvc/utils/git.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.2/dask4dvc/utils/main.py` & `dask4dvc-0.1.3/dask4dvc/utils/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 import time
 import typing
 
 log = logging.getLogger(__name__)
 
 
 def timeit(func: typing.Callable) -> typing.Callable:
-    """Timeit decorator for benchmarking."""
+    """Timeit decorator for benchmarking.
+
+    # TODO remove and replace with proper benchmarking / profiling
+    """
 
     @functools.wraps(func)
     def wrapper(*args: tuple, **kwargs: dict) -> typing.Any:
-        """Wrapper for timeit."""
+        """Wrap to time the function."""
         start_time = time.time()
         result = func(*args, **kwargs)
         stop_time = time.time()
         log.debug(f"'{func.__name__}' took {stop_time - start_time:4f} s")
         return result
 
     return wrapper
```

### Comparing `dask4dvc-0.1.2/pyproject.toml` & `dask4dvc-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.1.2"
+version = "0.1.3"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -12,15 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dask = "^2022.7.1"
 distributed = "^2022.7.1"
 dask-jobqueue = "^0.8.1"
 dvc = "^2.34.3"
-typer = "^0.6.1"
+typer = "^0.7.0"
 bokeh = "^2"
 # for bokeh see https://distributed.dask.org/en/stable/changelog.html#v2022-11-1
 
 [tool.poetry.scripts]
 dask4dvc = 'dask4dvc.cli.main:app'
 
 [tool.poetry.group.dev.dependencies]
@@ -28,18 +28,19 @@
 black = "^22.6.0"
 isort = "^5.10.1"
 ruff = "^0.0.126"
 pytest = "^7.1.2"
 pytest-xdist = "^2.5.0"
 coverage = "^6.4.2"
 pre-commit = "^2.20.0"
-zntrack = {git = "https://github.com/zincware/ZnTrack.git"}
+zntrack = "^0.4.0"	
 pylint = "^2.15.5"
 znlib = {extras = ["zntrack"], version = "^0.1.0"}
 
+# TODO remove znlib here!
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 90
```

### Comparing `dask4dvc-0.1.2/PKG-INFO` & `dask4dvc-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask4dvc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use dask to run the DVC graph
 License: Apache-2.0
 Keywords: data-science,HPC,dask,DVC
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=2,<3)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
 Requires-Dist: dask-jobqueue (>=0.8.1,<0.9.0)
 Requires-Dist: distributed (>=2022.7.1,<2023.0.0)
 Requires-Dist: dvc (>=2.34.3,<3.0.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: repository, https://github.com/zincware/dask4dvc
 Description-Content-Type: text/markdown
 
 [![Coverage Status](https://coveralls.io/repos/github/zincware/dask4dvc/badge.svg?branch=main)](https://coveralls.io/github/zincware/dask4dvc?branch=main)
 ![PyTest](https://github.com/zincware/dask4dvc/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
+[![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
@@ -52,7 +53,8 @@
     job_extra=['-N 1', '--cpus-per-task=1', '--tasks-per-node=64', "--gres=gpu:1"],
     scheduler_options={"port": 31415}
 )
 cluster.adapt()
 ```
 
 with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
+
```

