# Comparing `tmp/lightning-habana-0.1.0.tar.gz` & `tmp/lightning-habana-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-habana-0.1.0.tar", last modified: Thu Apr 13 09:17:53 2023, max compression
+gzip compressed data, was "lightning-habana-0.1.0rc0.tar", last modified: Tue Mar 14 18:25:37 2023, max compression
```

## Comparing `lightning-habana-0.1.0.tar` & `lightning-habana-0.1.0rc0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.614523 lightning-habana-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.618523 lightning-habana-0.1.0/src/lightning_habana/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/src/lightning_habana/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/src/lightning_habana/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-13 09:17:41.000000 lightning-habana-0.1.0/src/lightning_habana/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:53.622523 lightning-habana-0.1.0/src/lightning_habana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 09:17:53.000000 lightning-habana-0.1.0/src/lightning_habana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-14 18:25:21.000000 lightning-habana-0.1.0rc0/src/lightning_habana/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:25:37.570026 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 18:25:37.000000 lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/top_level.txt
```

### Comparing `lightning-habana-0.1.0/LICENSE` & `lightning-habana-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/MANIFEST.in` & `lightning-habana-0.1.0rc0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/setup.py` & `lightning-habana-0.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/__init__.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/accelerator.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/plugins/__init__.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/plugins/io_plugin.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/plugins/precision.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/plugins/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/strategies/__init__.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-0.1.0/src/lightning_habana/strategies/parallel.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/strategies/parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 # limitations under the License.
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch.distributed
 from lightning_utilities import module_available
-from torch.distributed import broadcast_object_list
 
 if module_available("lightning"):
     from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning.fabric.utilities.distributed import group as _group
     from lightning.pytorch import LightningModule
     from lightning.pytorch.accelerators import Accelerator
     from lightning.pytorch.plugins.io.wrapper import _WrappingCheckpointIO
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.ddp import DDPStrategy
 elif module_available("pytorch_lightning"):
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning_fabric.utilities.distributed import group as _group
     from pytorch_lightning import LightningModule
     from pytorch_lightning.accelerators import Accelerator
+    from pytorch_lightning.overrides.torch_distributed import broadcast_object_list
     from pytorch_lightning.plugins.io.hpu_plugin import HPUCheckpointIO
     from pytorch_lightning.plugins.io.wrapper import _WrappingCheckpointIO
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.ddp import DDPStrategy
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 from torch.nn import Module
@@ -90,15 +90,15 @@
         elif isinstance(self._checkpoint_io, _WrappingCheckpointIO):
             self._checkpoint_io.checkpoint_io = HPUCheckpointIO()
 
         return self._checkpoint_io
 
     @checkpoint_io.setter
     def checkpoint_io(self, io: Optional[CheckpointIO]) -> None:
-        self._checkpoint_io = io  # type: ignore[assignment]
+        self._checkpoint_io = io
 
     def setup_environment(self) -> None:
         os.environ["ID"] = str(self.local_rank)
         if self._process_group_backend == "hccl":
             # this env is used in overrides to check the backend initiated
             os.environ["HCCL_DISTRIBUTED_BACKEND"] = str(1)
         super().setup_environment()
```

### Comparing `lightning-habana-0.1.0/src/lightning_habana/strategies/single.py` & `lightning-habana-0.1.0rc0/src/lightning_habana/strategies/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         elif isinstance(self._checkpoint_io, _WrappingCheckpointIO):
             self._checkpoint_io.checkpoint_io = HPUCheckpointIO()
 
         return self._checkpoint_io
 
     @checkpoint_io.setter
     def checkpoint_io(self, io: Optional[CheckpointIO]) -> None:
-        self._checkpoint_io = io  # type: ignore[assignment]
+        self._checkpoint_io = io
 
     @property
     def is_distributed(self) -> bool:
         return False
 
     def setup(self, trainer: Trainer) -> None:
         self.model_to_device()
```

### Comparing `lightning-habana-0.1.0/src/lightning_habana.egg-info/SOURCES.txt` & `lightning-habana-0.1.0rc0/src/lightning_habana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

