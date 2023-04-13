# Comparing `tmp/fastpg-0.0.4.tar.gz` & `tmp/fastpg-0.0.5.tar.gz`

## Comparing `fastpg-0.0.4.tar` & `fastpg-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 fastpg-0.0.4/src/fastpg/__init__.py
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 fastpg-0.0.4/src/fastpg/core.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastpg-0.0.4/src/fastpg/exceptions.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastpg-0.0.4/src/fastpg/utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastpg-0.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastpg-0.0.4/LICENSE
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastpg-0.0.4/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastpg-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastpg-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 fastpg-0.0.5/Makefile
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/16e9276ce601f9d4
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/1ab6d1f4b669f5fa
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/2f4daf4fe347aac7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/454c8a0d424ee8b4
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/55a4dd45d1da5c6d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/82b86688b82b071e
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/e1f19352ed1a2f17
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/__init__.py
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/core.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/exceptions.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastpg-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastpg-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastpg-0.0.5/README.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastpg-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 fastpg-0.0.5/PKG-INFO
```

### Comparing `fastpg-0.0.4/src/fastpg/core.py` & `fastpg-0.0.5/src/fastpg/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 from collections.abc import Mapping
 from contextlib import asynccontextmanager
-from typing import (Any, Dict, Iterable, Iterator, List, Mapping, Optional,
-                    Sequence, Tuple, overload)
+from typing import Any, Iterator, List, Optional, Sequence, Tuple
 
 import asyncpg
 from asyncpg.pgproto.pgproto import UUID
 
 from .utils import compile_query, compile_value
 
 
@@ -34,15 +33,15 @@
 
     def values(self) -> Tuple[Any]:
         return tuple([self._get(k) for k in self._rec.keys()])
 
     def items(self) -> List[Tuple[str, Any]]:
         return list(zip(self.keys(), self.values()))
 
-    def __len__(self) -> int:  # type: ignore
+    def __len__(self) -> int:
         return len(self._rec)
 
     def __getitem__(self, key: Any) -> Any:
         return self._get(key)
 
     def __iter__(self) -> Iterator:
         return iter(self._rec.keys())
@@ -55,36 +54,38 @@
         *,
         user: str | None = None,
         password: str | None = None,
         host: str | None = None,
         port: int | None = None,
         database: str | None = None,
         force_rollback: bool = False,
+        **kwargs,
     ):
-        if dsn == None:
+        if dsn is None:
             assert user is not None, "Missing user (no DSN provided)"
             assert password is not None, "Missing password (no DSN provided)"
             assert host is not None, "Missing host (no DSN provided)"
             assert port is not None, "Missing port (no DSN provided)"
             dsn = f"postgresql://{user}:{password}@{host}:{port}/{database}"
         self.dsn = dsn
+        self.kwargs = kwargs
 
         self._force_rollback = force_rollback
 
         self._pool: asyncpg.Pool | None = None
         self._global_connection: Connection | None = None
 
     async def connect(self):
         if self._force_rollback:
             assert self._global_connection is None, "Database already connected"
-            self._global_connection = await asyncpg.connect(self.dsn)
+            self._global_connection = await asyncpg.connect(self.dsn, **self.kwargs)
             return
 
         assert self._pool is None, "Database already connected"
-        self._pool = await asyncpg.create_pool(self.dsn)
+        self._pool = await asyncpg.create_pool(self.dsn, **self.kwargs)
 
     async def disconnect(self, timeout: float = 30):
         if self._force_rollback:
             assert self._global_connection is not None, "Database is not connected"
             await self._global_connection.close()
             self._global_connection = None
             return
```

### Comparing `fastpg-0.0.4/src/fastpg/utils.py` & `fastpg-0.0.5/src/fastpg/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import re
 from enum import Enum
-from typing import Any, List
+from typing import List
 from uuid import UUID
 
-from ipdb import set_trace
 
 
 def compile_value(value):
     if isinstance(value, dict):
         return json.dumps(value)
     elif isinstance(value, UUID):
         return str(value)
```

### Comparing `fastpg-0.0.4/LICENSE` & `fastpg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpg-0.0.4/README.md` & `fastpg-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastpg-0.0.4/pyproject.toml` & `fastpg-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastpg"
-version = "0.0.4"
+version = "0.0.5"
 description = "A fast Postgres client library for Python"
 readme = "README.md"
 requires-python = ">=3.10.4"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "postgres", "asyncio", "asyncpg"]
 classifiers = [
@@ -27,9 +27,12 @@
 ]
 dependencies = ["asyncpg==0.27.0"]
 
 [project.urls]
 Homepage = "https://github.com/waydegg/fastpg"
 Source = "https://github.com/waydegg/fastpg"
 
-[tool.hatch.build]
-only-packages = true
+[project.optional-dependencies]
+dev = ["ruff", "ipdb", "ipython"]
+
+[tool.ruff]
+line-length = 88
```

### Comparing `fastpg-0.0.4/PKG-INFO` & `fastpg-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpg
-Version: 0.0.4
+Version: 0.0.5
 Summary: A fast Postgres client library for Python
 Project-URL: Homepage, https://github.com/waydegg/fastpg
 Project-URL: Source, https://github.com/waydegg/fastpg
 Author-email: Wayde Gilliam <waydegilliam@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: asyncio,asyncpg,postgres,python
@@ -18,14 +18,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.4
 Requires-Dist: asyncpg==0.27.0
+Provides-Extra: dev
+Requires-Dist: ipdb; extra == 'dev'
+Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # fastpg
 
 [![PyPI version](https://badge.fury.io/py/fastpg.svg)](https://pypi.org/project/fastpg/)
 
 A fast Postgres client library for Python.
```

