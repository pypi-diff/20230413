# Comparing `tmp/peewee_aio-1.5.1.tar.gz` & `tmp/peewee_aio-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.5.1.tar", max compression
+gzip compressed data, was "peewee_aio-1.5.2.tar", max compression
```

## Comparing `peewee_aio-1.5.1.tar` & `peewee_aio-1.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4681 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/README.md
--rw-r--r--   0        0        0      132 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/databases.py
--rw-r--r--   0        0        0    17060 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/fields.py
--rw-r--r--   0        0        0    15756 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/manager.py
--rw-r--r--   0        0        0    17678 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/peewee_aio/types.py
--rw-r--r--   0        0        0     2585 2023-03-27 17:50:38.368032 peewee_aio-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 peewee_aio-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/README.md
+-rw-r--r--   0        0        0      132 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15756 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/manager.py
+-rw-r--r--   0        0        0    17678 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/types.py
+-rw-r--r--   0        0        0     2585 2023-04-13 07:34:45.663423 peewee_aio-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 peewee_aio-1.5.2/PKG-INFO
```

### Comparing `peewee_aio-1.5.1/README.md` & `peewee_aio-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.1/peewee_aio/databases.py` & `peewee_aio-1.5.2/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.1/peewee_aio/fields.py` & `peewee_aio-1.5.2/peewee_aio/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,24 @@
 
 
 class FetchForeignKeyField(pw.ForeignKeyField, GenericField[TV]):
     """A foreign key field that only works with prefetching"""
 
     accessor_class = FetchForeignKeyAccessor
 
+    def __init__(
+        self: FetchForeignKeyField[TVAIOModel],
+        model: Type[TVAIOModel],
+        *,
+        lazy_load: bool = True,
+        **kwargs,
+    ):
+        """Field has to be always prefetched."""
+        super().__init__(model, lazy_load=False, **kwargs)
+
     if TYPE_CHECKING:
 
         @overload
         def __new__(
             cls, model: Type[TVAIOModel], *, null: Literal[False] = False, **kwargs
         ) -> FetchForeignKeyField[TVAIOModel]:
             ...
```

### Comparing `peewee_aio-1.5.1/peewee_aio/manager.py` & `peewee_aio-1.5.2/peewee_aio/manager.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.1/peewee_aio/model.py` & `peewee_aio-1.5.2/peewee_aio/model.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.1/pyproject.toml` & `peewee_aio-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.5.1"
+version = "1.5.2"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.5.1/PKG-INFO` & `peewee_aio-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.5.1
+Version: 1.5.2
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

