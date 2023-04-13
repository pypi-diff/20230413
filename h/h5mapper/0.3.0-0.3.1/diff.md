# Comparing `tmp/h5mapper-0.3.0.tar.gz` & `tmp/h5mapper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5mapper-0.3.0.tar", last modified: Fri Apr  7 05:45:11 2023, max compression
+gzip compressed data, was "h5mapper-0.3.1.tar", last modified: Thu Apr 13 21:08:06 2023, max compression
```

## Comparing `h5mapper-0.3.0.tar` & `h5mapper-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-07 05:45:11.890708 h5mapper-0.3.0/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1070 2021-06-12 05:09:31.000000 h5mapper-0.3.0/LICENSE
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     8117 2023-04-07 05:45:11.890708 h5mapper-0.3.0/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     7272 2023-01-29 14:46:01.000000 h5mapper-0.3.0/README.md
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-07 05:45:11.886708 h5mapper-0.3.0/h5mapper/
--rw-------   0 antoine   (1000) antoine   (1000)      178 2023-04-07 05:42:48.000000 h5mapper-0.3.0/h5mapper/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    16134 2023-01-15 11:13:05.000000 h5mapper-0.3.0/h5mapper/core.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4854 2023-01-11 12:03:31.000000 h5mapper-0.3.0/h5mapper/create.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2227 2021-07-05 05:54:16.000000 h5mapper-0.3.0/h5mapper/create_container.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     6279 2022-11-18 15:00:43.000000 h5mapper-0.3.0/h5mapper/crud.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4685 2023-01-08 18:02:50.000000 h5mapper-0.3.0/h5mapper/features.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2562 2023-01-08 18:02:50.000000 h5mapper-0.3.0/h5mapper/file_walker.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     6819 2023-01-29 14:47:43.000000 h5mapper-0.3.0/h5mapper/serve.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      556 2021-10-05 04:31:27.000000 h5mapper-0.3.0/h5mapper/utils.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-07 05:45:11.890708 h5mapper-0.3.0/h5mapper.egg-info/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     8117 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      404 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      108 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/entry_points.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       70 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        9 2023-04-07 05:45:11.000000 h5mapper-0.3.0/h5mapper.egg-info/top_level.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2023-04-07 05:45:11.890708 h5mapper-0.3.0/setup.cfg
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1865 2021-10-06 06:53:17.000000 h5mapper-0.3.0/setup.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 21:08:06.867787 h5mapper-0.3.1/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1070 2021-06-12 05:09:31.000000 h5mapper-0.3.1/LICENSE
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     8117 2023-04-13 21:08:06.867787 h5mapper-0.3.1/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     7272 2023-01-29 14:46:01.000000 h5mapper-0.3.1/README.md
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 21:08:06.867787 h5mapper-0.3.1/h5mapper/
+-rw-------   0 antoine   (1000) antoine   (1000)      178 2023-04-13 21:07:19.000000 h5mapper-0.3.1/h5mapper/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    16134 2023-01-15 11:13:05.000000 h5mapper-0.3.1/h5mapper/core.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     4854 2023-01-11 12:03:31.000000 h5mapper-0.3.1/h5mapper/create.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2227 2021-07-05 05:54:16.000000 h5mapper-0.3.1/h5mapper/create_container.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     6279 2022-11-18 15:00:43.000000 h5mapper-0.3.1/h5mapper/crud.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     4685 2023-01-08 18:02:50.000000 h5mapper-0.3.1/h5mapper/features.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2562 2023-01-08 18:02:50.000000 h5mapper-0.3.1/h5mapper/file_walker.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     6779 2023-04-13 21:06:47.000000 h5mapper-0.3.1/h5mapper/serve.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      556 2021-10-05 04:31:27.000000 h5mapper-0.3.1/h5mapper/utils.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 21:08:06.867787 h5mapper-0.3.1/h5mapper.egg-info/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     8117 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      404 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      108 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/entry_points.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       70 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)        9 2023-04-13 21:08:06.000000 h5mapper-0.3.1/h5mapper.egg-info/top_level.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2023-04-13 21:08:06.867787 h5mapper-0.3.1/setup.cfg
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1865 2021-10-06 06:53:17.000000 h5mapper-0.3.1/setup.py
```

### Comparing `h5mapper-0.3.0/LICENSE` & `h5mapper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/PKG-INFO` & `h5mapper-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5mapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: pythonic ORM tool for reading and writing HDF5 data
 Home-page: https://github.com/ktonal/h5mapper
 Download-URL: https://github.com/ktonal/h5mapper
 Author: Antoine Daurat
 Author-email: antoinedaurat@gmail.com
 License: MIT License
 Keywords: hdf5 h5py ORM deep-learning machine-learning
```

### Comparing `h5mapper-0.3.0/README.md` & `h5mapper-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/core.py` & `h5mapper-0.3.1/h5mapper/core.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/create.py` & `h5mapper-0.3.1/h5mapper/create.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/create_container.py` & `h5mapper-0.3.1/h5mapper/create_container.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/crud.py` & `h5mapper-0.3.1/h5mapper/crud.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/features.py` & `h5mapper-0.3.1/h5mapper/features.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/file_walker.py` & `h5mapper-0.3.1/h5mapper/file_walker.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper/serve.py` & `h5mapper-0.3.1/h5mapper/serve.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import librosa
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 from typing import Optional, Callable, Union
 import re
-from torch._six import string_classes
 import collections
 
 
 __all__ = [
     'Setter',
     'Getter',
     'AsSlice',
@@ -168,15 +167,15 @@
     elem_type = type(batch)
     if test(batch):
         return func(batch)
     elif isinstance(batch, collections.abc.Mapping):
         return {key: process_batch(batch[key], test, func) for key in batch}
     elif isinstance(batch, tuple) and hasattr(batch, '_fields'):  # namedtuple
         return elem_type(*(process_batch(d, test, func) for d in batch))
-    elif isinstance(batch, collections.abc.Sequence) and not isinstance(batch, string_classes):
+    elif isinstance(batch, collections.abc.Sequence) and not isinstance(batch, (str, bytes)):
         return [process_batch(d, test, func) for d in batch]
     else:
         return batch
 
 
 def _is_batchitem(obj):
     return isinstance(obj, (Input, Target))
```

### Comparing `h5mapper-0.3.0/h5mapper/utils.py` & `h5mapper-0.3.1/h5mapper/utils.py`

 * *Files identical despite different names*

### Comparing `h5mapper-0.3.0/h5mapper.egg-info/PKG-INFO` & `h5mapper-0.3.1/h5mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5mapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: pythonic ORM tool for reading and writing HDF5 data
 Home-page: https://github.com/ktonal/h5mapper
 Download-URL: https://github.com/ktonal/h5mapper
 Author: Antoine Daurat
 Author-email: antoinedaurat@gmail.com
 License: MIT License
 Keywords: hdf5 h5py ORM deep-learning machine-learning
```

### Comparing `h5mapper-0.3.0/setup.py` & `h5mapper-0.3.1/setup.py`

 * *Files identical despite different names*

