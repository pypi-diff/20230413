# Comparing `tmp/mongomancy-0.0.5.tar.gz` & `tmp/mongomancy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.0.5.tar", last modified: Wed Apr 12 12:27:09 2023, max compression
+gzip compressed data, was "mongomancy-0.0.6.tar", last modified: Thu Apr 13 12:07:23 2023, max compression
```

## Comparing `mongomancy-0.0.5.tar` & `mongomancy-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.646882 mongomancy-0.0.5/
--rw-r--r--   0 trval     (1000) trval     (1000)     1027 2023-04-12 12:22:43.000000 mongomancy-0.0.5/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.0.5/LICENSE
--rw-rw-r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:09:27.000000 mongomancy-0.0.5/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-04-12 12:27:09.646882 mongomancy-0.0.5/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.0.5/README.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:26:56.000000 mongomancy-0.0.5/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.0.5/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-04-12 12:27:09.646882 mongomancy-0.0.5/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.643549 mongomancy-0.0.5/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.643549 mongomancy-0.0.5/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-04-12 12:22:43.000000 mongomancy-0.0.5/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13857 2023-04-04 08:06:59.000000 mongomancy-0.0.5/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.0.5/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:06:01.000000 mongomancy-0.0.5/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    12666 2023-04-04 11:41:42.000000 mongomancy-0.0.5/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5687 2023-04-04 08:06:59.000000 mongomancy-0.0.5/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.646882 mongomancy-0.0.5/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1112 2023-04-13 12:06:01.000000 mongomancy-0.0.6/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.0.6/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.0.6/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-04-13 12:07:23.179283 mongomancy-0.0.6/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.0.6/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.0.6/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.0.6/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-04-13 12:07:23.179283 mongomancy-0.0.6/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.175949 mongomancy-0.0.6/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13420 2023-04-12 12:30:41.000000 mongomancy-0.0.6/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.0.6/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.0.6/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    12445 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5603 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.0.5/CHANGELOG.md` & `mongomancy-0.0.6/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.0.6] - 2023-04-13
+
+### Fixed
+
+- typing of required fields of index more broad
+
 ## [0.0.5] - 2023-04-12
 
 ### Added
 
 - Include `py.typed` for python typing support.
 
 ## [0.0.4] - 2023-04-04
```

### Comparing `mongomancy-0.0.5/CONTRIBUTING.md` & `mongomancy-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.5/LICENSE` & `mongomancy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.5/PKG-INFO` & `mongomancy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.0.5/README.md` & `mongomancy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.5/pyproject.toml` & `mongomancy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.5/src/mongomancy/engine.py` & `mongomancy-0.0.6/src/mongomancy/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import atexit
 import logging
 import time
 import traceback
-from typing import (
-    List, Sequence, Union, Set, TypeVar, Mapping, Any, ClassVar, Type, Optional, Callable, Iterable
-)
+from typing import List, Sequence, Union, Set, TypeVar, Mapping, Any, ClassVar, Type, Optional, Callable, Iterable
 
 import pymongo
 import pymongo.command_cursor
 import pymongo.database
 import pymongo.results
 import pymongo.typings
 from pymongo.errors import PyMongoError
 
 from . import mongo_errors, types
 
-__all__ = (
-    "Engine",
-)
+__all__ = ("Engine",)
 
 LoggerType = Union[logging.Logger, logging.LoggerAdapter]
 _CommandReturn = TypeVar("_CommandReturn")
 
 ExecutorLike = TypeVar("ExecutorLike", bound=types.Executor)
 
 
 class Engine(types.Executor):
     """
     Client of Mongo Database storage. All DB communication should be handled through this class.
     """
+
     CONNECTION_ERRORS: ClassVar[Type[pymongo.errors.PyMongoError]] = (
         pymongo.errors.AutoReconnect,
         pymongo.errors.ConnectionFailure,
     )
 
     client: pymongo.MongoClient
     logger: LoggerType
@@ -56,31 +53,31 @@
         "retry_codes",
         "_address",
         "_connection_params",
         "reconnect_hooks",
     )
 
     def __init__(
-            self,
-            host: str = "localhost",
-            port: int = 27017,
-            max_pool_size: int = 1,
-            queue_timeout: int = 400,
-            auth_source: Optional[str] = None,
-            auth_mechanism: Optional[str] = None,
-            user: Optional[str] = "kanturek",
-            password: Optional[str] = "kajot",
-            connect_timeout: Optional[int] = 15000,
-            write_retry: int = 3,
-            write_retry_delay: Union[float, int] = 1.3,
-            read_retry: int = 2,
-            read_retry_delay: Union[float, int] = 0.701,
-            retry_codes: Optional[Sequence[int]] = None,
-            logger: Optional[LoggerType] = None,
-            **kwargs,
+        self,
+        host: str = "localhost",
+        port: int = 27017,
+        max_pool_size: int = 1,
+        queue_timeout: int = 400,
+        auth_source: Optional[str] = None,
+        auth_mechanism: Optional[str] = None,
+        user: Optional[str] = "kanturek",
+        password: Optional[str] = "kajot",
+        connect_timeout: Optional[int] = 15000,
+        write_retry: int = 3,
+        write_retry_delay: Union[float, int] = 1.3,
+        read_retry: int = 2,
+        read_retry_delay: Union[float, int] = 0.701,
+        retry_codes: Optional[Sequence[int]] = None,
+        logger: Optional[LoggerType] = None,
+        **kwargs,
     ) -> None:
         """
         Create connection engine for mongo(s) server.
 
         :param host: database server host
         :param port: database server port
         :param max_pool_size: To support concurrent MongoDB operations within one process increase this value to 2+.
@@ -205,21 +202,21 @@
         except (IOError, pymongo.errors.PyMongoError) as e:
             self.logger.error(f"{type(self).__qualname__} - cannot reconnect to mongo server because: {e}")
         for hook in self.reconnect_hooks:
             _ = hook(self)
         self.logger.info(f"{type(self).__qualname__} - reconnected client")
 
     def _retry_command(
-            self,
-            collection: pymongo.collection.Collection,
-            command: Callable[[...], _CommandReturn],
-            /,
-            *args,
-            command_name_: Optional[str] = None,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        command: Callable[[...], _CommandReturn],
+        /,
+        *args,
+        command_name_: Optional[str] = None,
+        **kwargs,
     ) -> _CommandReturn:
         """
         Execute command and retry if error is caused by switched master in remote DB cluster.
 
         :param collection: collection of method used; f.e.: `game` in `game.find_one`
         :param command: method to execute; f.e.: `game.find_one`
         :param args: arguments for command
@@ -234,142 +231,136 @@
             attempt += 1
             try:
                 result = command(*args, **kwargs)
                 _error = None
             except pymongo.errors.AutoReconnect as e:
                 command_name_ = command_name_ or getattr(command, "__qualname__", "<unknown_command>")
                 self.logger.info(
-                    f"fail {attempt}/{self.write_retry} - {command_name_} "
-                    f"args={args}, kwargs={kwargs} e={e}"
+                    f"fail {attempt}/{self.write_retry} - {command_name_} " f"args={args}, kwargs={kwargs} e={e}"
                 )
                 _error = e
                 time.sleep(self.write_retry_delay)
                 self.reconnect()
             except pymongo.errors.WriteError as e:
                 command_name_ = command_name_ or getattr(command, "__qualname__", "<unknown_command>")
                 if e.code not in self.retry_codes:
-                    self.logger.error(
-                        f"failed to write - {command_name_} args={args}, kwargs={kwargs} e={e}"
-                    )
+                    self.logger.error(f"failed to write - {command_name_} args={args}, kwargs={kwargs} e={e}")
                     raise e from e
                 self.logger.info(
-                    f"fail {attempt}/{self.write_retry} - {command_name_} "
-                    f"args={args}, kwargs={kwargs} e={e}"
+                    f"fail {attempt}/{self.write_retry} - {command_name_} " f"args={args}, kwargs={kwargs} e={e}"
                 )
                 _error = e
                 time.sleep(self.write_retry_delay)
                 self.reconnect()
             if _error:
                 collection = self.client[collection.database.name][collection.name]
         if _error:
             command_name_ = command_name_ or getattr(command, "__qualname__", "<unknown_command>")
-            self.logger.warning(
-                f"fatal fail - {command_name_} args={args}, kwargs={kwargs} - after {attempt}x retry"
-            )
+            self.logger.warning(f"fatal fail - {command_name_} args={args}, kwargs={kwargs} - after {attempt}x retry")
             raise _error from _error
         return result
 
     def find_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> Optional[types.BsonDict]:
         return self._retry_command(collection, collection.find_one, where, *args, **kwargs)
 
     def find(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.cursor.Cursor[types.BsonDict]:
         return self._retry_command(collection, collection.find, where, *args, **kwargs)
 
     def find_one_and_update(
-            self,
-            collection: pymongo.collection.Collection,
-            where: types.BsonDict,
-            changes: types.BsonDict | types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: types.BsonDict,
+        changes: types.BsonDict | types.BsonList,
+        *args,
+        **kwargs,
     ) -> Optional[types.BsonDict]:
         return self._retry_command(
             collection,
             collection.find_one_and_update,
             where,
             changes,
             *args,
             **kwargs,
         )
 
     def aggregate(
-            self,
-            collection: pymongo.collection.Collection,
-            pipeline: types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        pipeline: types.BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.command_cursor.CommandCursor:
         return self._retry_command(
             collection,
             collection.aggregate,
             pipeline,
             *args,
             **kwargs,
         )
 
     def update_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            changes: types.BsonDict | Sequence[Mapping[str, Any]],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        changes: types.BsonDict | Sequence[Mapping[str, Any]],
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         return self._retry_command(collection, collection.update_one, where, changes, *args, **kwargs)
 
     def update_many(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            changes: types.BsonDict | types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        changes: types.BsonDict | types.BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         return self._retry_command(collection, collection.update_many, where, changes, *args, **kwargs)
 
     def insert_one(
-            self,
-            collection: pymongo.collection.Collection,
-            document: types.BsonDict,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        document: types.BsonDict,
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertOneResult:
         return self._retry_command(collection, collection.insert_one, document, *args, **kwargs)
 
     def insert_many(
-            self,
-            collection: pymongo.collection.Collection,
-            documents: Iterable[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        documents: Iterable[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertManyResult:
         return self._retry_command(collection, collection.insert_many, documents, *args, **kwargs)
 
     def delete_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         return self._retry_command(collection, collection.delete_one, where, *args, **kwargs)
 
     def delete_many(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         return self._retry_command(collection, collection.delete_many, where, *args, **kwargs)
```

### Comparing `mongomancy-0.0.5/src/mongomancy/mongo_errors.py` & `mongomancy-0.0.6/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.5/src/mongomancy/schema.py` & `mongomancy-0.0.6/src/mongomancy/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import logging
 import time
 import traceback
 from dataclasses import dataclass
 from typing import (
-    List, Tuple, Union, TypeVar, Mapping, Any, Optional, Dict, Iterable
+    List,
+    Tuple,
+    Union,
+    TypeVar,
+    Mapping,
+    Any,
+    Optional,
+    Dict,
+    Iterable,
 )
 
 import pymongo
 import pymongo.command_cursor
 import pymongo.database
 import pymongo.results
 import pymongo.typings
@@ -29,101 +37,102 @@
 
 @dataclass(slots=True)
 class Collection:
     """
     Abstraction of existing collection.
     Wraps `pymongo.collection.Collection` for easier reconnect.
     """
+
     mongo_collection: pymongo.collection.Collection
     engine: types.Executor
 
     @property
     def name(self) -> str:
         return self.mongo_collection.name
 
     def find_one(
-            self,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> Optional[DocumentType]:
         return self.engine.find_one(self.mongo_collection, where, *args, **kwargs)
 
     def find(
-            self,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.cursor.Cursor[types.BsonDict]:
         return self.engine.find(self.mongo_collection, where, *args, **kwargs)
 
     def find_one_and_update(
-            self,
-            where: types.BsonDict,
-            changes: types.BsonDict | types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        where: types.BsonDict,
+        changes: types.BsonDict | types.BsonList,
+        *args,
+        **kwargs,
     ) -> Optional[types.BsonDict]:
         return self.engine.find_one_and_update(self.mongo_collection, where, changes, *args, **kwargs)
 
     def update_one(
-            self,
-            where: Optional[types.BsonDict],
-            changes: types.BsonDict | types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        changes: types.BsonDict | types.BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         return self.engine.update_one(self.mongo_collection, where, changes, *args, **kwargs)
 
     def update_many(
-            self,
-            where: Optional[types.BsonDict],
-            changes: types.BsonDict | types.BsonList,
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        changes: types.BsonDict | types.BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         return self.engine.update_many(self.mongo_collection, where, changes, *args, **kwargs)
 
     def insert_one(
-            self,
-            document: types.BsonDict,
-            *args,
-            **kwargs,
+        self,
+        document: types.BsonDict,
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertOneResult:
         return self.engine.insert_one(self.mongo_collection, document, *args, **kwargs)
 
     def insert_many(
-            self,
-            documents: Iterable[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        documents: Iterable[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertManyResult:
         return self.engine.insert_many(self.mongo_collection, documents, *args, **kwargs)
 
     def delete_one(
-            self,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         return self.engine.delete_one(self.mongo_collection, where, *args, **kwargs)
 
     def delete_many(
-            self,
-            where: Optional[types.BsonDict],
-            *args,
-            **kwargs,
+        self,
+        where: Optional[types.BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         return self.engine.delete_many(self.mongo_collection, where, *args, **kwargs)
 
     def aggregate(
-            self,
-            pipeline: Optional[types.List],
-            *args,
-            **kwargs,
+        self,
+        pipeline: Optional[types.List],
+        *args,
+        **kwargs,
     ) -> pymongo.command_cursor.CommandCursor:
         return self.engine.aggregate(self.mongo_collection, pipeline, *args, **kwargs)
 
 
 class Database:
     """
     Database abstraction with reconnect support
@@ -136,14 +145,15 @@
         player = CollectionDefinition(name="player", indices=[Index(fields={"player_id": 1}, unique=True)])
         db.add_definition(game)
         db.add_definition(player)
         db.create_all()
         db["game"].find_one({"game_id": 1, "name": "game 1"})
 
     """
+
     engine: types.Executor
     topology: List[types.CollectionDefinition]
     _database: pymongo.database.Database
     _collections: Dict[str, Collection]
     logger: LoggerType
 
     __slots__ = (
@@ -151,19 +161,19 @@
         "topology",
         "_database",
         "_collections",
         "logger",
     )
 
     def __init__(
-            self,
-            name: str,
-            logger: LoggerType,
-            engine: types.Executor,
-            *collections: types.CollectionDefinition,
+        self,
+        name: str,
+        logger: LoggerType,
+        engine: types.Executor,
+        *collections: types.CollectionDefinition,
     ) -> None:
         self._collections = {}
         self.topology = []
         self.logger = logger
         self.engine = engine
         self._database = engine.get_database(name)
         for coll in collections:
@@ -228,17 +238,17 @@
 
         :param skip_existing: skip collection init if collection already exists in db
         """
         for collection_definition in self.topology:
             _ = self.create_collection(collection_definition, skip_existing)
 
     def create_collection(
-            self,
-            definition: types.CollectionDefinition,
-            skip_existing: bool = True,
+        self,
+        definition: types.CollectionDefinition,
+        skip_existing: bool = True,
     ) -> Collection:
         """
         Create new entity and bind it to this database.
         As side effect collection is added to `self._collections`.
 
         :param definition: CollectionDefinition to create
         :param skip_existing: skip collection init if collection already exists in db
@@ -263,16 +273,16 @@
         Perform a ping command on database.
 
         :return: true if PING return OK, false otherwise.
         """
         return self.engine.ping(database=self.name)
 
     def _create_mongo_collection(
-            self,
-            definition: types.CollectionDefinition,
+        self,
+        definition: types.CollectionDefinition,
     ) -> Tuple[pymongo.collection.Collection, bool]:
         """
         Create a new collection in this database if not exists, return existing otherwise.
 
         :param definition:
         :return: tuple(collection, is created as new ?)
         """
@@ -287,18 +297,18 @@
         except pymongo.errors.CollectionInvalid:
             self.logger.info(f"{self.name} - (probable race condition) skipped collection create {definition.name!r}")
             time.sleep(0.5)
             new_collection = self._database[definition.name]
         return new_collection, True
 
     def _create_indices(
-            self,
-            definition: types.CollectionDefinition,
-            mongo_collection: pymongo.collection.Collection,
-            silent: bool = True,
+        self,
+        definition: types.CollectionDefinition,
+        mongo_collection: pymongo.collection.Collection,
+        silent: bool = True,
     ) -> None:
         """
         Create indices if not exists on collection.
 
         :param mongo_collection: collection to create indices on
         :param definition: collection structure
         :param silent: suppress errors?
@@ -307,18 +317,18 @@
         definition.fill_index_names()
         for index in definition.indices:
             if index.name not in mongo_collection.index_information():
                 # in place check -> prevents a few conflicts, not all of them
                 self._create_index(mongo_collection, index, silent)
 
     def _create_index(
-            self,
-            mongo_collection: pymongo.collection.Collection,
-            index: types.Index,
-            silent: bool = True,
+        self,
+        mongo_collection: pymongo.collection.Collection,
+        index: types.Index,
+        silent: bool = True,
     ) -> None:
         """
         Create index over collection.
 
         :param mongo_collection: collection to create indices on
         :param index: describes index
         :param silent: suppress errors?
@@ -335,17 +345,17 @@
         except PyMongoError as e:
             self.logger.warning(f"{mongo_collection.full_name} - failed to create index {index.name!r} because '{e}'")
             if not silent:
                 raise e from e
             self.logger.warning(traceback.format_stack())
 
     def _insert_defaults(
-            self,
-            docs: Iterable[types.Document],
-            collection: Collection,
+        self,
+        docs: Iterable[types.Document],
+        collection: Collection,
     ) -> int:
         """
         Insert default data from definition into collection.
 
         :param docs: default docs
         :param collection: new collection to insert defaults into
         :return: docs created
```

### Comparing `mongomancy-0.0.5/src/mongomancy/types.py` & `mongomancy-0.0.6/src/mongomancy/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import abc
 import datetime as dt
 import sys
 from dataclasses import dataclass, field
 from typing import (
-    OrderedDict,
+    OrderedDict as OrderedDictType,
     List,
     Tuple,
     Sequence,
     Union,
     Optional,
     Mapping,
     Dict,
     Any,
     Iterable,
     Callable,
-    TypeVar,
 )
-
+from collections import OrderedDict
 import pymongo.database
 import pymongo.results
 from bson import ObjectId
 from pymongo.command_cursor import CommandCursor
 
 __all__ = (
     "Bson",
@@ -33,39 +32,42 @@
     "CommandCursor",
 )
 
 Bson = Union[None, int, float, bool, str, ObjectId, dt.datetime, Sequence["Bson"], Mapping[str, "Bson"]]
 BsonDict = Mapping[str, Bson]
 BsonList = Sequence[Bson]
 
-OrderedDictType = OrderedDict
-if sys.version_info >= 3.7:
-    OrderedDictType = TypeVar("OrderedDictType", bound=Dict)
+OrderedFields = OrderedDictType[str, Union[str, int]]
+if sys.version_info >= (3, 7):
+    OrderedFields = Dict[str, Union[str, int]]
+
+OrderedPairs = Union[OrderedFields, Sequence[Tuple[str, Union[str, int]]]]
 
 
 @dataclass(init=False)
 class Index:
     """Collection Index data container"""
-    fields: OrderedDictType[str, Union[str, int]]
+
+    fields: OrderedDict[str, Union[str, int]]
     name: Optional[str]
     unique: Optional[bool]
 
     __slots__ = (
         "fields",
         "name",
         "unique",
     )
 
     def __init__(
-            self,
-            fields: OrderedDictType[str, Union[str, int]],
-            name: Optional[str] = None,
-            unique: Optional[bool] = False,
+        self,
+        fields: OrderedPairs,
+        name: Optional[str] = None,
+        unique: Optional[bool] = False,
     ) -> None:
-        self.fields = fields
+        self.fields = OrderedDict(fields)
         self.name = name
         self.unique = unique
 
     def field_for_mongo(self) -> List[Tuple[str, Union[str, int]]]:
         """Format out fields as order of tuples"""
         return [(k, v) for k, v in self.fields.items()]
 
@@ -74,26 +76,32 @@
 class Document:
     """
     Abstraction of a MongoDB document where unique_key is one or more elements clearly identifying one document
 
     Example:
         Document(unique_key={"color_name": "red"}, data={"color_name": "red", "color_hex": "#ff0000"})
     """
+
     unique_key: Optional[BsonDict]
     data: Bson
 
 
 @dataclass(slots=True)
 class CollectionDefinition:
     """
     Collection Definition of name and indexed field
     """
+
     name: str
-    indices: Sequence[Index] = field(default_factory=tuple, )
-    default_docs: Sequence[Document] = field(default_factory=tuple, )
+    indices: Sequence[Index] = field(
+        default_factory=tuple,
+    )
+    default_docs: Sequence[Document] = field(
+        default_factory=tuple,
+    )
 
     def fill_index_names(self):
         """
         Do through indices and fill missing `index.name`s. Affects internal state of `self.indices` !
         """
         for index in self.indices:
             if index.name is None:
@@ -101,116 +109,117 @@
 
 
 class Executor(metaclass=abc.ABCMeta):
     """
     Reconnect-able interface of MongoDB mongo_driver that allows to execute commands like:
     `find`, `insert_one`, `update_many`, `delete_one`.
     """
+
     __slots__ = ()
 
     @abc.abstractmethod
     def find_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        *args,
+        **kwargs,
     ) -> Optional[Dict[str, Any]]:
         ...
 
     @abc.abstractmethod
     def find(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.cursor.Cursor:
         ...
 
     @abc.abstractmethod
     def find_one_and_update(
-            self,
-            collection: pymongo.collection.Collection,
-            where: BsonDict,
-            changes: BsonDict | BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: BsonDict,
+        changes: BsonDict | BsonList,
+        *args,
+        **kwargs,
     ) -> Optional[BsonDict]:
         ...
 
     @abc.abstractmethod
     def update_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            changes: BsonDict | BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        changes: BsonDict | BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         ...
 
     @abc.abstractmethod
     def update_many(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            changes: BsonDict | BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        changes: BsonDict | BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.results.UpdateResult:
         ...
 
     @abc.abstractmethod
     def insert_one(
-            self,
-            collection: pymongo.collection.Collection,
-            document: Optional[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        document: Optional[BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertOneResult:
         ...
 
     @abc.abstractmethod
     def insert_many(
-            self,
-            collection: pymongo.collection.Collection,
-            documents: Iterable[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        documents: Iterable[BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.InsertManyResult:
         ...
 
     @abc.abstractmethod
     def delete_one(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         ...
 
     @abc.abstractmethod
     def delete_many(
-            self,
-            collection: pymongo.collection.Collection,
-            where: Optional[BsonDict],
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        where: Optional[BsonDict],
+        *args,
+        **kwargs,
     ) -> pymongo.results.DeleteResult:
         ...
 
     @abc.abstractmethod
     def aggregate(
-            self,
-            collection: pymongo.collection.Collection,
-            pipeline: BsonList,
-            *args,
-            **kwargs,
+        self,
+        collection: pymongo.collection.Collection,
+        pipeline: BsonList,
+        *args,
+        **kwargs,
     ) -> pymongo.command_cursor.CommandCursor:
         ...
 
     @abc.abstractmethod
     def register_hook(self, reconnect_hook: Callable[["Executor"], None]) -> None:
         ...
```

### Comparing `mongomancy-0.0.5/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.0.6/src/mongomancy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

