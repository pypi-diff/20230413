# Comparing `tmp/countess-0.0.21.tar.gz` & `tmp/countess-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.21.tar", last modified: Fri Mar 31 02:51:47 2023, max compression
+gzip compressed data, was "countess-0.0.22.tar", last modified: Thu Apr 13 06:54:52 2023, max compression
```

## Comparing `countess-0.0.21.tar` & `countess-0.0.22.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.251424 countess-0.0.21/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.21/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-03-31 02:51:47.251424 countess-0.0.21/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-03-30 22:32:14.000000 countess-0.0.21/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.247424 countess-0.0.21/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-03-30 22:32:06.000000 countess-0.0.21/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.247424 countess-0.0.21/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.21/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-03-01 01:42:03.000000 countess-0.0.21/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-03-02 01:10:40.000000 countess-0.0.21/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1755 2023-03-30 03:12:18.000000 countess-0.0.21/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14808 2023-03-31 00:46:10.000000 countess-0.0.21/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5289 2023-03-30 03:12:18.000000 countess-0.0.21/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14006 2023-03-31 00:46:10.000000 countess-0.0.21/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.251424 countess-0.0.21/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:35.000000 countess-0.0.21/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19259 2023-03-31 00:46:10.000000 countess-0.0.21/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5139 2023-03-30 03:12:18.000000 countess-0.0.21/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    33534 2023-03-31 00:46:10.000000 countess-0.0.21/countess/gui/main.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.251424 countess-0.0.21/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:47.000000 countess-0.0.21/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6126 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1319 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/embed_python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1816 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1387 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1768 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3123 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      343 2023-03-06 22:57:42.000000 countess-0.0.21/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5528 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6955 2023-03-31 00:46:10.000000 countess-0.0.21/countess/plugins/regex.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.251424 countess-0.0.21/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.21/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1954 2023-03-31 00:46:10.000000 countess-0.0.21/countess/utils/dask.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.247424 countess-0.0.21/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      877 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      686 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      204 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-03-31 02:51:47.000000 countess-0.0.21/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2265 2023-03-31 02:51:40.000000 countess-0.0.21/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-03-31 02:51:47.251424 countess-0.0.21/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-02-28 22:32:19.000000 countess-0.0.21/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-31 02:51:47.251424 countess-0.0.21/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-02-28 22:34:37.000000 countess-0.0.21/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.22/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-13 06:54:52.581817 countess-0.0.22/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-13 01:06:20.000000 countess-0.0.22/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-13 01:06:30.000000 countess-0.0.22/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.22/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-03-01 01:42:03.000000 countess-0.0.22/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-03-02 01:10:40.000000 countess-0.0.22/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1755 2023-03-30 03:12:18.000000 countess-0.0.22/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14810 2023-04-11 06:55:31.000000 countess-0.0.22/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5289 2023-04-13 04:45:45.000000 countess-0.0.22/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14246 2023-04-13 06:53:19.000000 countess-0.0.22/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:35.000000 countess-0.0.22/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19707 2023-04-13 06:53:19.000000 countess-0.0.22/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5855 2023-04-13 05:47:03.000000 countess-0.0.22/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    33604 2023-04-13 06:53:20.000000 countess-0.0.22/countess/gui/main.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:47.000000 countess-0.0.22/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6110 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1303 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/embed_python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1800 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1465 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1781 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3107 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      343 2023-03-06 22:57:42.000000 countess-0.0.22/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5592 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6953 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2243 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.22/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2133 2023-04-11 06:55:31.000000 countess-0.0.22/countess/utils/dask.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9681 2023-04-13 05:33:29.000000 countess-0.0.22/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      931 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      238 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2365 2023-04-12 05:45:07.000000 countess-0.0.22/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-13 06:54:52.581817 countess-0.0.22/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-02-28 22:32:19.000000 countess-0.0.22/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-02-28 22:34:37.000000 countess-0.0.22/tests/test_gui.py
```

### Comparing `countess-0.0.21/LICENSE.txt` & `countess-0.0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/PKG-INFO` & `countess-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.21
+Version: 0.0.22
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.21
+# CountESS 0.0.22
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.21/README.md` & `countess-0.0.22/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.21
+# CountESS 0.0.22
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.21/countess/core/cmd.py` & `countess-0.0.22/countess/core/cmd.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/countess/core/config.py` & `countess-0.0.22/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/countess/core/logger.py` & `countess-0.0.22/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/countess/core/parameters.py` & `countess-0.0.22/countess/core/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,15 @@
 class ColumnChoiceParam(ChoiceParam):
     """A ChoiceParam which DaskTransformPlugin knows
     it should automatically update with a list of columns"""
 
     def set_column_choices(self, choices):
         self.set_choices(list(choices))
 
+
 class ColumnOrIndexChoiceParam(ColumnChoiceParam):
     INDEX_VALUE = "— INDEX —"
 
     def set_choices(self, choices: Iterable[str]):
         super().set_choices([self.INDEX_VALUE] + list(choices))
 
     def is_index(self):
@@ -428,14 +429,15 @@
         return digest.hexdigest()
 
     def set_column_choices(self, choices):
         self.param.set_column_choices(choices)
         for p in self.params:
             p.set_column_choices(choices)
 
+
 class FileArrayParam(ArrayParam):
     """FileArrayParam is an ArrayParam arranged per-file.  Using this class
     really just marks it as expecting to be populated from an open file
     dialog."""
 
     def find_fileparam(self):
         if isinstance(self.param, FileParam):
```

### Comparing `countess-0.0.21/countess/core/pipeline.py` & `countess-0.0.22/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/countess/core/plugins.py` & `countess-0.0.22/countess/core/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 
 import hashlib
 import importlib
 import importlib.metadata
 import logging
 import os.path
 import sys
-from collections.abc import Iterable, Mapping, MutableMapping
+from collections.abc import Mapping, MutableMapping
 from typing import Any, List, Optional
 
 import dask.dataframe as dd
 import numpy as np
-import pandas as pd  # type: ignore
+import pandas as pd
 from dask.callbacks import Callback
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
     BaseParam,
     ChoiceParam,
     FileArrayParam,
     FileParam,
     FileSaveParam,
     MultiParam,
     StringParam,
 )
-from countess.utils.dask import concat_dataframes, crop_dataframe
+from countess.utils.dask import concat_dataframes, crop_dataframe, empty_dask_dataframe
 
 PRERUN_ROW_LIMIT = 100
 
 
 def get_plugin_classes():
     plugin_classes = set()
     for ep in importlib.metadata.entry_points(group="countess_plugins"):
@@ -289,29 +289,29 @@
         file_params.update(self.file_params)
 
         self.parameters = dict(
             [("files", FileArrayParam("Files", MultiParam("File", file_params)))]
             + list(self.parameters.items())
         )
 
-    def combine_dfs(self, dfs: list[dd.DataFrame]) -> dd.DataFrame:
+    def combine_dfs(self, dfs: list[pd.DataFrame | dd.DataFrame]) -> dd.DataFrame | pd.DataFrame:
         """First stage: collect all the files together in whatever
         way is appropriate.  Override this to do it differently
         or do more work on the dataframes (eg: counting, renaming, etc)"""
         return concat_dataframes(dfs)
 
     def load_files(
         self,
         logger: Logger,
         row_limit: Optional[int] = None,
-    ) -> Iterable[dd.DataFrame]:
+    ) -> pd.DataFrame | dd.DataFrame:
         assert isinstance(self.parameters["files"], ArrayParam)
         fps = self.parameters["files"].params
         if not fps:
-            return []
+            return empty_dask_dataframe()
 
         if len(fps) == 1:
             with DaskProgressCallback(logger):
                 file_param = self.parameters["files"].params[0]
                 assert isinstance(file_param, MultiParam)
                 ddf = self.read_file_to_dataframe(file_param, logger, row_limit)
                 ddf = self.combine_dfs([ddf])
@@ -365,26 +365,31 @@
 
     def prepare_dask(self, df, logger):
         super().prepare(df, logger)
         for pp in self.parameters["scores"]:
             for ppp in pp.counts:
                 ppp.choices = self.input_columns
 
-    def run_dask(self, df: dd.DataFrame, logger: Logger) -> dd.DataFrame:
+    def run_dask(
+        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
+    ) -> pd.DataFrame | dd.DataFrame:
         assert isinstance(self.parameters["scores"], ArrayParam)
         score_cols = []
         for pp in self.parameters["scores"]:
             scol = pp.score.value
             ccols = [ppp.value for ppp in pp.counts]
 
             if scol and all(ccols):
                 df[scol] = self.score([df[col] for col in ccols])
                 score_cols.append(scol)
 
-        return df.replace([np.inf, -np.inf], np.nan).dropna(how="all", subset=score_cols)
+        df = df.replace([np.inf, -np.inf], np.nan)
+        assert isinstance(df, (pd.DataFrame, dd.DataFrame))
+        df.dropna(how="all", subset=score_cols, inplace=True)
+        return df
 
     def score(self, columns: List[dd.Series]) -> dd.Series:
         raise NotImplementedError("Subclass DaskScoringPlugin and provide a score() method")
 
 
 class DaskReindexPlugin(DaskTransformPlugin):
     # XXX not really useful?
@@ -393,12 +398,14 @@
 
     def translate(self, value):
         raise NotImplementedError(f"Implement {self.__class__.__name__}.translate")
 
     def translate_row(self, row):
         return self.translate(row.name)
 
-    def run_dask(self, df: dd.DataFrame, logger: Logger) -> dd.DataFrame:
+    def run_dask(
+        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
+    ) -> pd.DataFrame | dd.DataFrame:
         df["__reindex"] = df.apply(
             self.translate_row, axis=1, meta=pd.Series(self.translate_type())
         )
         return df.groupby("__reindex").sum()
```

### Comparing `countess-0.0.21/countess/gui/config.py` & `countess-0.0.22/countess/gui/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tkinter as tk
 from functools import partial
 from tkinter import filedialog, ttk
 from typing import Mapping, Optional
 
 import dask.dataframe as dd
 import numpy as np
+import pandas as pd
 
 from ..core.parameters import (
     ArrayParam,
     BaseParam,
     BooleanParam,
     ChoiceParam,
     FileArrayParam,
@@ -75,14 +76,17 @@
         elif isinstance(parameter, BooleanParam):
             self.entry = tk.Button(tk_parent, width=2, command=self.toggle_checkbox_callback)
             self.set_checkbox_value(parameter.value)
         elif isinstance(parameter, FileParam):
             self.var = tk.StringVar(tk_parent, value=parameter.value)
             self.entry = ttk.Entry(tk_parent, textvariable=self.var)
             self.entry.state(["readonly"])
+            self.button = tk.Button(
+                tk_parent, text="Select", width=3, command=self.change_file_callback
+            )
         elif isinstance(parameter, TextParam):
             # tk.Text widget doesn't have a variable, for whatever reason,
             # so we use a different method!
             # XXX is this a simpler way to handle other kinds of fields too?
             self.entry = tk.Text(tk_parent, height=10)
             self.entry.insert("1.0", parameter.value)
             if parameter.read_only:
@@ -328,14 +332,21 @@
         else:
             self.parameter.del_subparam(parameter_wrapper.parameter)
 
         self.update()
         if self.callback is not None:
             self.callback(self.parameter)
 
+    def change_file_callback(self, *_):
+        file_types = self.parameter.file_types
+        filename = filedialog.askopenfilename(filetypes=file_types)
+        self.parameter.value = filename
+        self.var.set(self.parameter.value)
+        self.callback(self.parameter)
+
     def set_value(self, value):
         # self.parameter.value is a property, and some cleaning may occur, so we just
         # check before and after to see if it has changed.
         old_parameter_value = self.parameter.value
         self.parameter.value = value
         new_parameter_value = self.parameter.value
         if old_parameter_value != new_parameter_value and self.callback is not None:
@@ -455,15 +466,15 @@
         self.treeview.grid(row=1, column=0, sticky=tk.NSEW)
         self.scrollbar_x.grid(row=2, column=0, sticky=tk.EW)
         self.scrollbar_y.grid(row=1, column=1, stick=tk.NS)
 
         if ddf is not None:
             self.update(ddf)
 
-    def update(self, ddf: dd.DataFrame):
+    def update(self, ddf: pd.DataFrame | dd.DataFrame):
         if len(ddf) > 1000:
             self.label["text"] = f"DataFrame Preview (1000 rows out of {len(ddf)})"
             ddf = crop_dataframe(ddf, 1000)
         else:
             self.label["text"] = f"DataFrame Preview {len(ddf)} rows"
 
         # XXX could handle multiindex columns more elegantly than this
```

### Comparing `countess-0.0.21/countess/gui/logger.py` & `countess-0.0.22/countess/gui/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-import sys
+import queue
 import tkinter as tk
 from tkinter import ttk
 from typing import MutableMapping, Optional
 
 from countess.core.logger import Logger
 
 
@@ -95,41 +95,58 @@
         self.name = name
         self.count = 0
         self.treeview["height"] = 0
         self.detail: MutableMapping[str, str] = {}
 
         self.treeview.bind("<<TreeviewSelect>>", self.on_click)
 
+        self.queue: queue.Queue = queue.Queue()
+        self.on_poll()
+
     def on_click(self, event):
         # XXX display detail more nicely
         TreeviewDetailWindow(self.detail[self.treeview.focus()])
 
+    def on_poll(self):
+        # XXX dask apply etc don't seem to be thread safe when updating Tk, so
+        # this adds in a queue to separate the two.
+        try:
+            while True:
+                level, message, detail = self.queue.get_nowait()
+                if level == "progress":
+                    self.progress_bar.grid(sticky=tk.EW)
+                    if detail is not None:
+                        self.progress_bar.config(mode="determinate", value=detail)
+                        self.progress_bar.update_label(f"{self.name}: {message} {detail}%")
+                    else:
+                        self.progress_bar.config(mode="indeterminate")
+                        self.progress_bar.step(5)
+                        self.progress_bar.update_label(f"{self.name}: {message}")
+                else:
+                    self.count += 1
+                    datetime_now = datetime.datetime.now()
+                    values = [self.name, message]
+                    iid = self.treeview.insert(
+                        "", "end", text=datetime_now.isoformat(), values=values
+                    )
+                    if detail is not None:
+                        self.detail[iid] = detail
+                    self.treeview["height"] = min(self.count, 10)
+
+        except queue.Empty:
+            pass
+
+        self.treeview.after(1000, self.on_poll)
+
     def log(self, level: str, message: str, detail: Optional[str] = None):
-        # XXX temporary
-        sys.stderr.write(message + "\n")
-        if detail:
-            sys.stderr.write(detail + "\n\n")
-
-        self.count += 1
-        datetime_now = datetime.datetime.now()
-        values = [self.name, message]
-        iid = self.treeview.insert("", "end", text=datetime_now.isoformat(), values=values)
-        if detail is not None:
-            self.detail[iid] = detail
-        self.treeview["height"] = min(self.count, 10)
+        print(level, message, detail)
+        self.queue.put((level, message, detail))
 
     def progress(self, message: str = "Running", percentage: Optional[int] = None):
-        self.progress_bar.grid(sticky=tk.EW)
-        if percentage is not None:
-            self.progress_bar.config(mode="determinate", value=percentage)
-            self.progress_bar.update_label(f"{self.name}: {message} {percentage}%")
-        else:
-            self.progress_bar.config(mode="indeterminate")
-            self.progress_bar.step(5)
-            self.progress_bar.update_label(f"{self.name}: {message}")
+        self.queue.put(("progress", message, percentage))
 
     def progress_hide(self):
         self.progress_bar.grid_forget()
 
     def clear(self):
         self.progress_bar.config(mode="determinate", value=0)
         self.progress_bar.update_label("")
```

### Comparing `countess-0.0.21/countess/gui/main.py` & `countess-0.0.22/countess/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import webbrowser
 from enum import Enum, IntFlag
 from functools import partial
 from tkinter import filedialog, messagebox, ttk
 from typing import Optional
 
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.config import export_config_graphviz, read_config, write_config
 from countess.core.logger import ConsoleLogger
 from countess.core.pipeline import PipelineGraph, PipelineNode
 from countess.core.plugins import get_plugin_classes
 from countess.gui.config import DataFramePreview, PluginConfigurator
@@ -259,23 +259,21 @@
 
         self.columnconfigure(0, weight=1)
 
         label_frame = tk.LabelFrame(self, text=title, padx=10, pady=10)
         label_frame.grid(row=1, column=0, sticky=tk.EW, padx=10, pady=10)
 
         for n, plugin_class in enumerate(plugin_classes):
-            label_text = plugin_class.description.split('. ')[0]
+            label_text = plugin_class.description.split(". ")[0]
             ttk.Button(
                 label_frame,
                 text=plugin_class.name,
                 command=lambda plugin_class=plugin_class: callback(plugin_class),
             ).grid(row=n + 1, column=0, sticky=tk.EW)
-            ttk.Label(label_frame, text=label_text).grid(
-                row=n + 1, column=1, sticky=tk.W, padx=10
-            )
+            ttk.Label(label_frame, text=label_text).grid(row=n + 1, column=1, sticky=tk.W, padx=10)
 
 
 class FlippyCanvas(FixedUnbindMixin, tk.Canvas):
     """A canvas which flips all its children's X and Y
     coordinates when it goes from portrait to landscape.
     Place children with .place(relx=, rely=) for best results."""
 
@@ -622,14 +620,15 @@
         self.show_config_subframe()
         if self.node.plugin:
             self.show_preview_subframe()
 
     def show_config_subframe(self):
         if self.config_subframe:
             self.config_subframe.destroy()
+        self.node.prepare(self.logger)
         if self.node.plugin:
             self.label["text"] = "%s %s — %s" % (
                 self.node.plugin.name,
                 self.node.plugin.version,
                 self.node.plugin.description,
             )
             if self.node.plugin.link:
@@ -672,18 +671,19 @@
         else:
             self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.columnconfigure(0, weight=1)
             tk.Label(self.preview_subframe, text="no result").grid(sticky=tk.EW)
 
         self.preview_subframe.grid(row=4, columnspan=2, sticky=tk.NSEW)
 
-        if self.logger.count > 0:
-            self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
-        else:
-            self.logger_subframe.grid_forget()
+        self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
+        # if self.logger.count > 0:
+        #    self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
+        # else:
+        #    self.logger_subframe.grid_forget()
 
     def name_changed_callback(self, *_):
         name = self.name_var.get()
         self.node.name = name
         self.change_callback(self.node)
 
     def notes_modified_callback(self, *_):
```

### Comparing `countess-0.0.21/countess/plugins/csv.py` & `countess-0.0.22/countess/plugins/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 from io import StringIO
 from typing import Any, Optional
 
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import (
     ArrayParam,
     BooleanParam,
     ChoiceParam,
     DataTypeOrNoneChoiceParam,
```

### Comparing `countess-0.0.21/countess/plugins/embed_python.py` & `countess-0.0.22/countess/plugins/embed_python.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import ArrayParam, TextParam
 from countess.core.plugins import DaskTransformPlugin
```

### Comparing `countess-0.0.21/countess/plugins/fastq.py` & `countess-0.0.22/countess/plugins/fastq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from itertools import islice
 
-import pandas as pd  # type: ignore
+import pandas as pd
 from fqfa.fastq.fastq import parse_fastq_reads  # type: ignore
 
 from countess import VERSION
 from countess.core.parameters import BooleanParam, FloatParam
 from countess.core.plugins import DaskInputPlugin
 from countess.utils.dask import concat_dataframes
```

### Comparing `countess-0.0.21/countess/plugins/group_by.py` & `countess-0.0.22/countess/plugins/group_by.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import ChoiceParam, ColumnOrIndexChoiceParam
 from countess.core.plugins import DaskTransformPlugin
 
 
 class GroupByPlugin(DaskTransformPlugin):
@@ -25,16 +25,18 @@
         "operation": ChoiceParam(
             "Operation",
             "sum",
             choices=["sum", "size", "std", "var", "sem", "min", "max"],
         ),
     }
 
-    def run_dask(self, df: pd.DataFrame | dd.DataFrame, logger) -> dd.DataFrame:
+    def run_dask(self, df: pd.DataFrame | dd.DataFrame, logger) -> pd.DataFrame | dd.DataFrame:
         assert isinstance(self.parameters["column"], ColumnOrIndexChoiceParam)
         if self.parameters["column"].is_index():
             col = df.index
         else:
             col = df[self.parameters["column"].value]
         oper = self.parameters["operation"].value
 
-        return df.groupby(col).agg(oper)
+        df2 = df.groupby(col).agg(oper)
+        assert isinstance(df2, (pd.DataFrame, dd.DataFrame))
+        return df2
```

### Comparing `countess-0.0.21/countess/plugins/hdf5.py` & `countess-0.0.22/countess/plugins/hdf5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 
-import pandas as pd  # type: ignore
+import dask.dataframe as dd
+import pandas as pd
 
 try:
     import tables  # type: ignore  # pylint: disable=unused-import
 except ImportError as exc:
     raise NotImplementedError("HDF5 Plugin needs Pytables") from exc
 
 from countess import VERSION
 from countess.core.parameters import ChoiceParam, MultiParam
 from countess.core.plugins import DaskInputPlugin
-from countess.utils.dask import empty_dask_dataframe
 
 
 class LoadHdfPlugin(DaskInputPlugin):
     name = "HDF5 Load"
     description = "Loads counts from HDF5 files"
     version = VERSION
 
@@ -23,26 +23,28 @@
         "key": ChoiceParam("HDF Key"),
     }
 
     keys: list[str] = []
 
     def read_file_to_dataframe(
         self, file_params: MultiParam, logger, row_limit: Optional[int] = None
-    ) -> pd.DataFrame:
+    ) -> pd.DataFrame | dd.DataFrame:
         kp = file_params.key
         filename = file_params.filename.value
         with pd.HDFStore(filename) as hs:
             kp.set_choices(sorted(hs.keys()))
 
         if kp.value is None:
-            return empty_dask_dataframe()
+            return pd.DataFrame([])
 
         with pd.HDFStore(filename) as hs:
             df = hs.select(kp.value, start=0, stop=row_limit)
 
+        assert isinstance(df, pd.DataFrame)
+
         return df
 
 
 # class StoreHdfPlugin(DaskBasePlugin):
 #    name = "HDF Writer"
 #    description = "Write to HDF5"
 #
```

### Comparing `countess-0.0.21/countess/plugins/join.py` & `countess-0.0.22/countess/plugins/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Mapping, MutableMapping
 from typing import Optional
 
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import ArrayParam, BooleanParam, ChoiceParam, MultiParam
 from countess.core.plugins import DaskBasePlugin
 
 INDEX = "— INDEX —"
```

### Comparing `countess-0.0.21/countess/plugins/pivot.py` & `countess-0.0.22/countess/plugins/pivot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools
 from collections import defaultdict
 
 import dask.dataframe as dd
+import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
     ChoiceParam,
     ColumnChoiceParam,
@@ -39,15 +40,17 @@
                 },
             ),
         ),
     }
 
     # XXX It'd be nice to also have "non pivoted" aggregated columns as well.
 
-    def run_dask(self, df: dd.DataFrame, logger: Logger) -> dd.DataFrame:
+    def run_dask(
+        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
+    ) -> pd.DataFrame | dd.DataFrame:
         assert isinstance(self.parameters["index"], ArrayParam)
         assert isinstance(self.parameters["pivot"], ArrayParam)
         assert isinstance(self.parameters["agg"], ArrayParam)
 
         index_cols = [
             p.value
             for p in self.parameters["index"].params
```

### Comparing `countess-0.0.21/countess/plugins/regex.py` & `countess-0.0.22/countess/plugins/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from functools import partial
 
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import (
     ArrayParam,
     BooleanParam,
     ColumnOrIndexChoiceParam,
     DataTypeChoiceParam,
@@ -88,30 +88,30 @@
                 column_name = regex_parameter["column"].value
 
             # XXX not totally happy with this
             func = partial(self.apply_func, column_name, compiled_re, output_params, logger)
 
             if isinstance(df, dd.DataFrame):
                 # dask likes a hint about column types
-                meta = dict(zip(output_names, output_types))
+                meta = dict(enumerate(output_types))
                 re_groups_df = df.apply(func, axis=1, result_type="expand", meta=meta)
             else:
                 # pandas infers the column types
                 re_groups_df = df.apply(func, axis=1, result_type="expand")
 
             for n in range(0, compiled_re.groups):
                 df[output_names[n]] = re_groups_df[n]
 
         drop_columns = set(
             rp["column"].value for rp in self.parameters["regexes"] if rp["drop_column"].value
         )
-        if "__index__" in df:
+        if "__index" in df:
             drop_columns.add("__index")
 
-        return df.drop(columns=drop_columns)
+        return df.drop(columns=drop_columns) if drop_columns else df
 
 
 class RegexReaderPlugin(DaskInputPlugin):
     name = "Regex Reader"
     description = """Loads arbitrary data from line-delimited files, applying a regular expression
       to each line to extract fields.  If you're trying to read generic CSV or TSV files, use the CSV
       plugin instead as it handles escaping correctly."""
```

### Comparing `countess-0.0.21/countess/utils/dask.py` & `countess-0.0.22/countess/utils/dask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utility functions for manipulating Dask DataFrames"""
 
 from typing import Collection, Optional
 
 import dask.dataframe as dd
-import pandas as pd  # type: ignore
+import pandas as pd
 
 
 def empty_dask_dataframe() -> dd.DataFrame:
     """Returns an empty dask DataFrame for consistency."""
     edf = dd.from_pandas(pd.DataFrame([]), npartitions=1)
     assert isinstance(edf, dd.DataFrame)  # reassure mypy
     return edf
@@ -24,36 +24,43 @@
         elif isinstance(df, dd.DataFrame):
             return df.head(row_limit, npartitions=-1, compute=False)
         else:
             raise TypeError("Expecting pd.DataFrame or dd.DataFrame")
     return df
 
 
-def concat_dataframes(dfs: Collection[pd.DataFrame | dd.DataFrame]) -> pd.DataFrame | dd.DataFrame:
+def concat_dataframes(dfs: Collection[pd.DataFrame | dd.DataFrame]) -> dd.DataFrame:
     """Concat dask dataframes, but include special cases for 0 and 1 inputs"""
 
     # extra special case for empty dataframes
     dfs = [df for df in dfs if len(df) > 0]
 
     if len(dfs) == 0:
         return empty_dask_dataframe()
     elif len(dfs) == 1:
-        return dfs[0].copy()
+        if isinstance(dfs[0], dd.DataFrame):
+            return dfs[0].copy()
+        else:
+            return dd.from_pandas(dfs[0], npartitions=1)
     else:
         return dd.concat(dfs)
 
 
 def merge_dataframes(dfs: list[dd.DataFrame | pd.DataFrame], how: str = "outer") -> dd.DataFrame:
     """Merge multiple dask/pandas dataframes together on their index.
     Always returns a new Dask dataframe even if there's one or zero input dataframes."""
 
     # XXX should be smarter about merge strategies?
 
     if not dfs:
         return empty_dask_dataframe()
 
     left, *rest = dfs
-    if isinstance(left, pd.Dataframe):
+    if isinstance(left, pd.DataFrame):
         left = dd.from_pandas(left, npartitions=1)
+    assert isinstance(left, dd.DataFrame)
+
     for right in rest:
         left = left.merge(right, how=how)
+        assert isinstance(left, dd.DataFrame)
+
     return left
```

### Comparing `countess-0.0.21/countess.egg-info/PKG-INFO` & `countess-0.0.22/countess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.21
+Version: 0.0.22
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.21
+# CountESS 0.0.22
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.21/countess.egg-info/SOURCES.txt` & `countess-0.0.22/countess.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -27,10 +27,12 @@
 countess/plugins/fastq.py
 countess/plugins/group_by.py
 countess/plugins/hdf5.py
 countess/plugins/join.py
 countess/plugins/log_score.py
 countess/plugins/pivot.py
 countess/plugins/regex.py
+countess/plugins/variant.py
 countess/utils/__init__.py
 countess/utils/dask.py
+countess/utils/variant.py
 tests/test_gui.py
```

### Comparing `countess-0.0.21/countess.egg-info/entry_points.txt` & `countess-0.0.22/countess.egg-info/entry_points.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 load_fastq = countess.plugins.fastq:LoadFastqPlugin
 load_hdf = countess.plugins.hdf5:LoadHdfPlugin
 log_score = countess.plugins.log_score:LogScorePlugin
 pivot = countess.plugins.pivot:DaskPivotPlugin
 regex_reader = countess.plugins.regex:RegexReaderPlugin
 regex_tool = countess.plugins.regex:RegexToolPlugin
 save_csv = countess.plugins.csv:SaveCsvPlugin
+variants = countess.plugins.variant:VariantPlugin
 
 [gui_scripts]
 countess_gui = countess.gui.main:main
```

### Comparing `countess-0.0.21/pyproject.toml` & `countess-0.0.22/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 dependencies = [
     'dask>=2022.8.0',
     'distributed>=2022.8.0',
     'fqfa~=1.2.3',
     'more_itertools>=8.14.0',
     'numpy~=1.23',
     'pandas~=1.4',
+    'rapidfuzz~=2.13',
     'ttkthemes~=3.2',
 ]
 
 [project.optional-dependencies]
 dev = [
     'black<24',
     'mypy~=1.0.1',
     'pylint~=2.16',
     'types-ttkthemes~=3.2',
+    'pandas-stubs~=1.4',
     'pytest~=7.2',
 ]
 
 hdf = [
      'tables~=3.7',
 ]
 
@@ -50,14 +52,15 @@
 group_by = "countess.plugins.group_by:GroupByPlugin"
 embed_py = "countess.plugins.embed_python:EmbeddedPythonPlugin"
 pivot = "countess.plugins.pivot:DaskPivotPlugin"
 join = "countess.plugins.join:DaskJoinPlugin"
 save_csv = "countess.plugins.csv:SaveCsvPlugin"
 regex_tool = "countess.plugins.regex:RegexToolPlugin"
 regex_reader = "countess.plugins.regex:RegexReaderPlugin"
+variants = "countess.plugins.variant:VariantPlugin"
 
 [project.entry-points.gui_scripts]
 countess_gui = "countess.gui.main:main"
 
 [project.entry-points.console_scripts]
 countess_cmd = "countess.core.cmd:main"
```

### Comparing `countess-0.0.21/setup.cfg` & `countess-0.0.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `countess-0.0.21/tests/test_gui.py` & `countess-0.0.22/tests/test_gui.py`

 * *Files identical despite different names*

