# Comparing `tmp/fastapi-async-sqlalchemy-0.3.9.tar.gz` & `tmp/fastapi-async-sqlalchemy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-async-sqlalchemy-0.3.9.tar", last modified: Fri Oct 22 22:04:56 2021, max compression
+gzip compressed data, was "fastapi-async-sqlalchemy-0.4.0.tar", last modified: Thu Apr 13 14:04:35 2023, max compression
```

## Comparing `fastapi-async-sqlalchemy-0.3.9.tar` & `fastapi-async-sqlalchemy-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 22:04:56.274247 fastapi-async-sqlalchemy-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2021-10-22 22:04:56.270247 fastapi-async-sqlalchemy-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 22:04:56.270247 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 22:04:56.270247 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-10-22 22:04:56.000000 fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 22:04:56.274247 fastapi-async-sqlalchemy-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-10-22 22:04:46.000000 fastapi-async-sqlalchemy-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/setup.py
```

### Comparing `fastapi-async-sqlalchemy-0.3.9/LICENSE` & `fastapi-async-sqlalchemy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/exceptions.py` & `fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 class MissingSessionError(Exception):
-    """Excetion raised for when the user tries to access a database session before it is created."""
+    """
+    Exception raised for when the user tries to access a database session before it is created.
+    """
 
     def __init__(self):
         msg = """
         No session found! Either you are not currently in a request context,
         or you need to manually create a session context by using a `db` instance as
         a context manager e.g.:
 
@@ -11,15 +13,17 @@
             await db.session.execute(foo.select()).fetchall()
         """
 
         super().__init__(msg)
 
 
 class SessionNotInitialisedError(Exception):
-    """Exception raised when the user creates a new DB session without first initialising it."""
+    """
+    Exception raised when the user creates a new DB session without first initialising it.
+    """
 
     def __init__(self):
         msg = """
         Session not initialised! Ensure that DBSessionMiddleware has been initialised before
         attempting database access.
         """
```

### Comparing `fastapi-async-sqlalchemy-0.3.9/fastapi_async_sqlalchemy/middleware.py` & `fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from contextvars import ContextVar
 from typing import Dict, Optional, Union
 
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.url import URL
-from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.ext.asyncio import AsyncSession, async_sessionmaker, create_async_engine
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.types import ASGIApp
 
 from fastapi_async_sqlalchemy.exceptions import MissingSessionError, SessionNotInitialisedError
 
-_Session: Optional[sessionmaker] = None
+_Session: Optional[async_sessionmaker] = None
 _session: ContextVar[Optional[AsyncSession]] = ContextVar("_session", default=None)
 
 
 class SQLAlchemyMiddleware(BaseHTTPMiddleware):
     def __init__(
         self,
         app: ASGIApp,
@@ -34,15 +33,15 @@
             raise ValueError("You need to pass a db_url or a custom_engine parameter.")
         if not custom_engine:
             engine = create_async_engine(db_url, **engine_args)
         else:
             engine = custom_engine
 
         global _Session
-        _Session = sessionmaker(engine, class_=AsyncSession, expire_on_commit=False, **session_args)
+        _Session = async_sessionmaker(engine, expire_on_commit=False, **session_args)
 
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint):
         async with db(commit_on_exit=self.commit_on_exit):
             return await call_next(request)
 
 
 class DBSessionMeta(type):
@@ -64,19 +63,19 @@
 class DBSession(metaclass=DBSessionMeta):
     def __init__(self, session_args: Dict = None, commit_on_exit: bool = False):
         self.token = None
         self.session_args = session_args or {}
         self.commit_on_exit = commit_on_exit
 
     async def __aenter__(self):
-        if not isinstance(_Session, sessionmaker):
+        if not isinstance(_Session, async_sessionmaker):
             raise SessionNotInitialisedError
 
-        self.token = _session.set(_Session(**self.session_args))
-        return self.token
+        self.token = _session.set(_Session(**self.session_args))  # type: ignore
+        return type(self)
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         session = _session.get()
         if exc_type is not None:
             await session.rollback()
 
         if self.commit_on_exit:
```

### Comparing `fastapi-async-sqlalchemy-0.3.9/setup.py` & `fastapi-async-sqlalchemy-0.4.0/setup.py`

 * *Files identical despite different names*

