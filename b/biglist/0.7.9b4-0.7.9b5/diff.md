# Comparing `tmp/biglist-0.7.9b4.tar.gz` & `tmp/biglist-0.7.9b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b4.tar", last modified: Wed Apr 12 20:07:25 2023, max compression
+gzip compressed data, was "biglist-0.7.9b5.tar", last modified: Thu Apr 13 07:47:04 2023, max compression
```

## Comparing `biglist-0.7.9b4.tar` & `biglist-0.7.9b5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b4/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b4/README.rst
--rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b4/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-12 19:30:05.357161 biglist-0.7.9b4/src/biglist/__init__.py
--rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b4/src/biglist/_base.py
--rw-r--r--   0        0        0    43817 2023-04-12 20:05:04.951149 biglist-0.7.9b4/src/biglist/_biglist.py
--rw-r--r--   0        0        0    33845 2023-04-12 19:44:51.303943 biglist-0.7.9b4/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b4/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b4/src/biglist/py.typed
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b5/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b5/README.rst
+-rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b5/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-13 07:43:36.928982 biglist-0.7.9b5/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18555 2023-04-13 07:44:02.101802 biglist-0.7.9b5/src/biglist/_base.py
+-rw-r--r--   0        0        0    44004 2023-04-13 07:44:02.431804 biglist-0.7.9b5/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34691 2023-04-13 07:44:02.651805 biglist-0.7.9b5/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b5/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b5/src/biglist/py.typed
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b5/PKG-INFO
```

### Comparing `biglist-0.7.9b4/LICENSE` & `biglist-0.7.9b5/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b4/README.rst` & `biglist-0.7.9b5/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b4/pyproject.toml` & `biglist-0.7.9b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b4/src/biglist/__init__.py` & `biglist-0.7.9b5/src/biglist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b4"
+__version__ = "0.7.9b5"
```

### Comparing `biglist-0.7.9b4/src/biglist/_base.py` & `biglist-0.7.9b5/src/biglist/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 
     def __repr__(self):
         return f"<{self.__class__.__name__} for '{self.path}'>"
 
     def __str__(self):
         return self.__repr__()
 
+    def __getstate__(self):
+        return self.path, self.loader
+
+    def __setstate__(self, data):
+        self.path, self.loader = data
+
     @abstractmethod
     def load(self) -> None:
         """
         This method *eagerly* loads all the data from the file.
 
         Once this method has been called, typically the entire data file is loaded
         into memory, and subsequent data consumption should all draw upon this
```

### Comparing `biglist-0.7.9b4/src/biglist/_biglist.py` & `biglist-0.7.9b5/src/biglist/_biglist.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,14 +731,21 @@
         loader
             Usually this is :meth:`Biglist.load_data_file`.
             If you customize this, please see the doc of :meth:`FileReader.__init__`.
         """
         self._data: Optional[list] = None
         super().__init__(path, loader)
 
+    def __getstate__(self):
+        return super().__getstate__()
+
+    def __setstate__(self, data):
+        super().__setstate__(data)
+        self._data = None
+
     def load(self) -> None:
         if self._data is None:
             self._data = self.loader(self.path)
 
     def data(self) -> list[Element]:
         """Return the data loaded from the file."""
         self.load()
@@ -923,15 +930,17 @@
             However, there are no strong reasons to use this facility on a local machine.
 
             Usually this class is used to distribute data to a cluster of machines, hence
             this path points to a location in a cloud storage that is supported by ``upathlib``.
         """
         path = resolve_path(path)
         bl = Biglist.new(
-            path / "data", batch_size=batch_size, storage_format=storage_format,
+            path / "data",
+            batch_size=batch_size,
+            storage_format=storage_format,
         )
         bl.extend(data)
         bl.flush()
         assert len(bl) > 0
         return cls(path)
 
     def __init__(
```

### Comparing `biglist-0.7.9b4/src/biglist/_parquet.py` & `biglist-0.7.9b5/src/biglist/_parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from __future__ import annotations
 
 import itertools
 import logging
 from collections.abc import Iterable, Iterator, Sequence
+from multiprocessing.util import Finalize
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 import pyarrow
 from deprecation import deprecated
 from pyarrow.fs import FileSystem, GcsFileSystem
 from pyarrow.parquet import FileMetaData, ParquetFile
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
+try:
+    from google.cloud.storage import retry as gcs_retry
+    from upathlib.gcs import get_google_auth
+except ImportError:
+    pass
+
 from ._base import (
     BiglistBase,
     FileReader,
     FileSeq,
     Seq,
     _get_global_thread_pool,
 )
@@ -56,39 +63,53 @@
         Obtain a `pyarrow.fs.GcsFileSystem`_ object with credentials given so that
         the GCP default process of inferring credentials (which involves
         env vars and file reading etc) will not be triggered.
 
         This is provided under the (un-verified) assumption that the
         default credential inference process is a high overhead.
         """
-        # Import here b/c user may not be on GCP
-        from upathlib.gcs import get_google_auth
-
-        cls._GCP_PROJECT_ID, cls._GCP_CREDENTIALS, _ = get_google_auth(
+        cls._GCP_PROJECT_ID, cls._GCP_CREDENTIALS, renewed = get_google_auth(
             project_id=getattr(cls, '_GCP_PROJECT_ID', None),
             credentials=getattr(cls, "_GCP_CREDENTIALS", None),
             valid_for_seconds=good_for_seconds,
         )
-        return GcsFileSystem(
-            access_token=cls._GCP_CREDENTIALS.token,
-            credential_token_expiration=cls._GCP_CREDENTIALS.expiry
-        )
+        if renewed or getattr(cls, '_GCSFS', None) is None:
+            fs = GcsFileSystem(
+                access_token=cls._GCP_CREDENTIALS.token,
+                credential_token_expiration=cls._GCP_CREDENTIALS.expiry,
+            )
+            cls._GCSFS = fs
+        return cls._GCSFS
+
+    @classmethod
+    def _gcs_retry(cls):
+        def _should_retry(exc):
+            if isinstance(exc, pyarrow.lib.ArrowException) and str(exc).startswith(
+                'Unknown error'
+            ):
+                return True
+            return gcs_retry.DEFAULT_RETRY._predicate(exc)
+
+        return gcs_retry.DEFAULT_RETRY.with_predicate(_should_retry)
 
     @classmethod
     def load_data_file(cls, path: Upath) -> ParquetFile:
         """
         Load the data file given by ``path``.
 
         This function is used as the argument ``loader`` to :meth:`ParquetFileReader.__init__`.
         The value it returns is contained in :class:`FileReader` for subsequent use.
         """
         ff, pp = FileSystem.from_uri(str(path))
         if isinstance(ff, GcsFileSystem):
             ff = cls.get_gcsfs()
-        return ParquetFile(ff.open_input_file(pp))
+            pf = cls._gcs_retry()(ParquetFile)  # a retry-wrapped func
+        else:
+            pf = ParquetFile
+        return pf(pp, filesystem=ff)
 
     @classmethod
     def new(
         cls,
         data_path: PathType | Sequence[PathType],
         path: Optional[PathType] = None,
         *,
@@ -137,38 +158,36 @@
         """
         if isinstance(data_path, (str, Path, Upath)):
             #  TODO: in py 3.10, we will be able to do `isinstance(data_path, PathType)`
             data_path = [resolve_path(data_path)]
         else:
             data_path = [resolve_path(p) for p in data_path]
 
-        def get_file_meta(f, p: Upath):
-            meta = f(p).metadata
+        def get_file_meta(p: Upath):
+            with cls.load_data_file(p) as ff:
+                meta = ff.metadata
             return {
                 "path": str(p),  # str of full path
                 "num_rows": meta.num_rows,
                 # "row_groups_num_rows": [
                 #     meta.row_group(k).num_rows for k in range(meta.num_row_groups)
                 # ],
             }
 
         pool = _get_global_thread_pool()
         tasks = []
-        read_parquet = cls.load_data_file
         for p in data_path:
             if p.is_file():
                 if suffix == "*" or p.name.endswith(suffix):
-                    tasks.append(pool.submit(get_file_meta, read_parquet, p))
+                    tasks.append(pool.submit(get_file_meta, p))
             else:
                 tt = []
                 for pp in p.riterdir():
                     if suffix == "*" or pp.name.endswith(suffix):
-                        tt.append(
-                            (str(pp), pool.submit(get_file_meta, read_parquet, pp))
-                        )
+                        tt.append((str(pp), pool.submit(get_file_meta, pp)))
                 tt.sort()
                 for p, t in tt:
                     tasks.append(t)
 
         assert tasks
         datafiles = []
         for k, t in enumerate(tasks):
@@ -254,30 +273,39 @@
         ----------
         path
             Path of a Parquet file.
         loader
             Usually this is :meth:`ParquetBiglist.load_data_file`.
             If you customize this, please see the doc of :meth:`FileReader.__init__`.
         """
+        super().__init__(path, loader)
+        self._reset()
+
+    def _reset(self):
         self._file: Optional[ParquetFile] = None
         self._data: Optional[ParquetBatchData] = None
 
         self._row_groups_num_rows = None
         self._row_groups_num_rows_cumsum = None
         self._row_groups: Optional[list[ParquetBatchData]] = None
 
         self._column_names = None
         self._columns = {}
         self._getitem_last_row_group = None
 
-        super().__init__(path, loader)
-
         self._scalar_as_py = None
         self.scalar_as_py = True
 
+    def __getstate__(self):
+        return super().__getstate__()
+
+    def __setstate__(self, data):
+        super().__setstate__(data)
+        self._reset()
+
     @property
     def scalar_as_py(self) -> bool:
         """
         ``scalar_as_py`` controls whether the values returned by :meth:`__getitem__`
         (or indirectly by :meth:`__iter__`) are converted from a `pyarrow.Scalar`_ type
         such as `pyarrow.lib.StringScalar`_ to a Python builtin type such as ``str``.
 
@@ -321,14 +349,15 @@
         Upon initiation of a :class:`ParquetFileReader` object,
         the file is not read at all. When this property is requested,
         the file is accessed to construct a `pyarrow.parquet.ParquetFile`_ object,
         but this only reads *meta* info; it does not read the *data*.
         """
         if self._file is None:
             self._file = self.loader(self.path)
+            Finalize(self, self._file.close)
         return self._file
 
     @property
     def metadata(self) -> FileMetaData:
         return self.file.metadata
 
     @property
```

### Comparing `biglist-0.7.9b4/src/biglist/_util.py` & `biglist-0.7.9b5/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b4/PKG-INFO` & `biglist-0.7.9b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b4
+Version: 0.7.9b5
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

