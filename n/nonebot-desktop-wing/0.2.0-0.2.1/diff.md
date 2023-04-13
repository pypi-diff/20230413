# Comparing `tmp/nonebot-desktop-wing-0.2.0.tar.gz` & `tmp/nonebot-desktop-wing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.2.0.tar", last modified: Sun Apr  9 14:04:26 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.2.1.tar", last modified: Thu Apr 13 14:19:21 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.2.0.tar` & `nonebot-desktop-wing-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.807494 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 14:04:26.000000 nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 14:04:16.000000 nonebot-desktop-wing-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:04:26.811494 nonebot-desktop-wing-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.122456 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.2.0/LICENSE` & `nonebot-desktop-wing-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.0/PKG-INFO` & `nonebot-desktop-wing-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -60,13 +60,7 @@
 |getdist                    |Get installed packages in a project.|
 |create                     |Create a new project.|
 |get_builtin_plugins        |Get available built-in plugins.|
 |find_env_file              |Find dotenv files in a directory.|
 |recursive_find_env_config  |Search dotenv files for a configuration in a directory.|
 |recursive_update_env_config|Update a configuration in dotenv files in a directory.|
 |get_toml_config            |Get toml data manager from a directory.|
-
-### Resources
-
-|Name                |Description|
-|:-------------------|:----------|
-|load_module_data_raw|Get raw data of NoneBot packages online.|
```

### Comparing `nonebot-desktop-wing-0.2.0/README.md` & `nonebot-desktop-wing-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -48,13 +48,7 @@
 |getdist                    |Get installed packages in a project.|
 |create                     |Create a new project.|
 |get_builtin_plugins        |Get available built-in plugins.|
 |find_env_file              |Find dotenv files in a directory.|
 |recursive_find_env_config  |Search dotenv files for a configuration in a directory.|
 |recursive_update_env_config|Update a configuration in dotenv files in a directory.|
 |get_toml_config            |Get toml data manager from a directory.|
-
-### Resources
-
-|Name                |Description|
-|:-------------------|:----------|
-|load_module_data_raw|Get raw data of NoneBot packages online.|
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,9 +17,8 @@
     getdist as getdist,
     create as create,
     get_builtin_plugins as get_builtin_plugins,
     find_env_file as find_env_file,
     recursive_find_env_config as recursive_find_env_config,
     recursive_update_env_config as recursive_update_env_config,
     get_toml_config as get_toml_config
-)
-from .resources import load_module_data_raw as load_module_data_raw
+)
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/hindsight.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from queue import Empty, Queue
 from threading import Thread
 from typing import IO, Callable, Generic, List, Optional, ParamSpec, TypeVar
 
 T = TypeVar("T")
 AnyStr_T = TypeVar("AnyStr_T", str, bytes)
 P = ParamSpec("P")
 
 
 class BackgroundObject(Generic[P, T]):
+    """A descriptor for running functions in background."""
     def __init__(
-        self,
-        func: Callable[P, T],
-        *args: P.args,
-        **kwargs: P.kwargs
+        self, func: Callable[P, T], *args: P.args, **kwargs: P.kwargs
     ) -> None:
         """
-        A descriptor for running functions in background.
+        Initialize (start) a call in background.
+
+        - func: `(P...) -> T`   - A callable to be called in background.
+        - *args: `P.args`       - Positional args for the callable.
+        - **kwargs: `P.kwargs`  - Keyword args for the callable.
         """
         self._func = func
         self._thread = Thread(None, self._work, None, args, kwargs)
         self._thread.start()
         # bgobject_log_func(
         #     f"[BackgroundObject] '{func.__module__}.{func.__name__}' is "
         #     f"running in background with {args=}, {kwargs=}"
@@ -32,20 +33,23 @@
         self._value = self._func(*args, **kwargs)
         # bgobject_log_func(
         #     f"[BackgroundObject] '{self._func.__module__}."
         #     f"{self._func.__name__}' is done with {args=}, {kwargs=}"
         # )
 
     def get(self) -> T:
+        """Wait for value."""
         self._thread.join()
         return self._value
 
 
 class RealtimeIOPipe(Generic[AnyStr_T]):
-    def __init__(self, stream: IO[AnyStr_T], writer: Callable[[AnyStr_T], object]) -> None:
+    def __init__(
+        self, stream: IO[AnyStr_T], writer: Callable[[AnyStr_T], object]
+    ) -> None:
         self.stream = stream
         self.thread = Thread(target=self._pull)
         self.writer = writer
         self.thread.start()
 
     def _pull(self) -> None:
         while True:
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.py` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 
 class _nb_cli:
     handlers = BackgroundObject(import_with_lock, "nb_cli.handlers", "*")
     config = BackgroundObject(import_with_lock, "nb_cli.config", "*")
 
 
-nb_cli = _nb_cli()
+nb_cli = _nb_cli
 
 
 class _meta:
-    drivers = BackgroundObject(asyncio.run, nb_cli.handlers.load_module_data("driver"))
-    adapters = BackgroundObject(asyncio.run, nb_cli.handlers.load_module_data("adapter"))
-    plugins = BackgroundObject(asyncio.run, nb_cli.handlers.load_module_data("plugin"))
+    drivers = BackgroundObject(asyncio.run, nb_cli().handlers.load_module_data("driver"))
+    adapters = BackgroundObject(asyncio.run, nb_cli().handlers.load_module_data("adapter"))
+    plugins = BackgroundObject(asyncio.run, nb_cli().handlers.load_module_data("plugin"))
     raw_drivers = BackgroundObject(load_module_data_raw, "drivers")
     raw_adapters = BackgroundObject(load_module_data_raw, "adapters")
     raw_plugins = BackgroundObject(load_module_data_raw, "plugins")
 
 
-meta = _meta()
+meta = _meta
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import List
+from typing import List, Type
 from nb_cli import handlers as _handlers
 from nb_cli import config as _config
 from nb_cli.config import Driver, Plugin, Adapter
 
 
 class _nb_cli:
     handlers = _handlers
     config = _config
 
 
-nb_cli: _nb_cli
+nb_cli: Type[_nb_cli]
 
 RawInfo = dict[
     {
         "module_name": str,
         "project_link": str,
         "name": str,
         "desc": str,
@@ -30,8 +30,8 @@
     adapters: List[Adapter]
     plugins: List[Plugin]
     raw_drivers: List[RawInfo]
     raw_adapters: List[RawInfo]
     raw_plugins: List[RawInfo]
 
 
-meta: _meta
+meta: Type[_meta]
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, List, Literal
 
 
 @cache
 def load_module_data_raw(
     module_name: Literal["adapters", "plugins", "drivers"]
 ) -> List[Dict[str, Any]]:
+    """Get raw module data."""
     from concurrent.futures import ThreadPoolExecutor, as_completed
     import httpx
     exceptions: List[Exception] = []
     urls = [
         f"https://v2.nonebot.dev/{module_name}.json",
         f"https://raw.fastgit.org/nonebot/nonebot2/master/website/static/{module_name}.json",
         f"https://cdn.jsdelivr.net/gh/nonebot/nonebot2/website/static/{module_name}.json",
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -60,13 +60,7 @@
 |getdist                    |Get installed packages in a project.|
 |create                     |Create a new project.|
 |get_builtin_plugins        |Get available built-in plugins.|
 |find_env_file              |Find dotenv files in a directory.|
 |recursive_find_env_config  |Search dotenv files for a configuration in a directory.|
 |recursive_update_env_config|Update a configuration in dotenv files in a directory.|
 |get_toml_config            |Get toml data manager from a directory.|
-
-### Resources
-
-|Name                |Description|
-|:-------------------|:----------|
-|load_module_data_raw|Get raw data of NoneBot packages online.|
```

### Comparing `nonebot-desktop-wing-0.2.0/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.0/pyproject.toml` & `nonebot-desktop-wing-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.2.0"
+version = "0.2.1"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23"]
 requires-python = ">=3.8"
```

