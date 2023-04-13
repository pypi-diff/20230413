# Comparing `tmp/snapstream-0.0.0.dev3.tar.gz` & `tmp/snapstream-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.0.dev3.tar", max compression
+gzip compressed data, was "snapstream-0.0.1.tar", max compression
```

## Comparing `snapstream-0.0.0.dev3.tar` & `snapstream-0.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/LICENSE
--rw-r--r--   0        0        0     1735 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/README.md
--rw-r--r--   0        0        0     1067 2023-04-02 14:10:12.160111 snapstream-0.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     1703 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/__init__.py
--rw-r--r--   0        0        0     3699 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/caching.py
--rw-r--r--   0        0        0      663 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/codecs.py
--rw-r--r--   0        0        0     5719 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/core.py
--rw-r--r--   0        0        0     1182 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/utils.py
--rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 snapstream-0.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-13 20:05:46.184868 snapstream-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-13 20:05:46.184868 snapstream-0.0.1/README.md
+-rw-r--r--   0        0        0     1265 2023-04-13 20:06:00.020870 snapstream-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1673 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/__init__.py
+-rw-r--r--   0        0        0     9660 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/caching.py
+-rw-r--r--   0        0        0     2538 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/codecs.py
+-rw-r--r--   0        0        0     8396 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/core.py
+-rw-r--r--   0        0        0     1033 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/utils.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 snapstream-0.0.1/PKG-INFO
```

### Comparing `snapstream-0.0.0.dev3/LICENSE` & `snapstream-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev3/pyproject.toml` & `snapstream-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.0.dev3"
+version = "0.0.1"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
-homepage = "https://github.com/Menziess/snapstream"
-
+repository = "https://github.com/Menziess/snapstream"
+license = "MIT"
+keywords = ["kafka", "pubsub"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8.1"
 confluent-kafka = "^2.0.2"
 rocksdict = "^0.3.10"
 pypubsub = "^4.0.3"
+avro = "^1.11.1"
+toolz = "^0.12.0"
+pyright = "^1.1.302"
 
 [tool.poetry.group.dev.dependencies]
 pydocstyle = "^6.3.0"
 autopep8 = "^2.0.2"
 pyright = "^1.1.300"
 flake8 = "^6.0.0"
 bandit = "^1.7.5"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.2.1"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["snapstream"]
@@ -33,7 +38,14 @@
 venv = ".venv"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
+testpaths = [
+    "snapstream",
+    "tests",
+]
+markers = [
+    "serial"
+]
```

### Comparing `snapstream-0.0.0.dev3/snapstream/__init__.py` & `snapstream-0.0.1/snapstream/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 
 from typing import Iterable
 
 from pubsub import pub
 
 from snapstream.caching import Cache
 from snapstream.core import READ_FROM_END, READ_FROM_START, Conf, Topic
-from snapstream.utils import Sink
 
 __all__ = [
-    'Conf',
-    'Topic',
     'snap',
     'stream',
+    'Conf',
+    'Topic',
     'Cache',
     'READ_FROM_START',
     'READ_FROM_END',
 ]
 
 
 def snap(
     *iterable: Iterable,
-    sink: Iterable[Sink]
+    sink: Iterable = []
 ):
     """Snaps function to stream.
 
     Ex:
-        >>> topic = Topic('demo')
-        >>> cache = Cache('state/demo')
+        >> topic = Topic('demo')
+        >> cache = Cache('state/demo')
 
-        >>> @snap(my_topic, sink=[print, cache])
-        ... def handler(msg, **kwargs):
-        ...     return msg.key(), msg.value()
+        >> @snap(topic, sink=[print, cache])
+        .. def handler(msg, **kwargs):
+        ..     return msg.key(), msg.value()
     """
     c = Conf()
 
     def sink_output(s, output):
         if not isinstance(output, tuple) and isinstance(s, (Cache)):
             # Sink requires Tuple[key, val]
             raise ValueError('Cache sink expects: Tuple[key, val].')
@@ -51,25 +50,25 @@
                 output = f(msg, **kwargs)
             except TypeError:
                 output = f(msg)
             for s in sink:
                 sink_output(s, output)
 
         for it in iterable:
-            c.register_iterables(it)
             iterable_key = str(id(it))
+            c.register_iterables((iterable_key, it))
             pub.subscribe(_handler, iterable_key)
         return _handler
 
     return _deco
 
 
 def stream(**kwargs):
     """Start the streams.
 
     Ex:
-        >>> args = {
-        ...     'env': 'DEV',
-        ... }
-        >>> start(**args)
+        >> args = {
+        ..     'env': 'DEV',
+        .. }
+        >> stream(**args)
     """
     Conf().start(**kwargs)
```

### Comparing `snapstream-0.0.0.dev3/snapstream/utils.py` & `snapstream-0.0.1/snapstream/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Snapstream utilities."""
 
 import logging
-from typing import Any, Dict, Protocol
+from typing import Any, Dict
 
 
 class Singleton(type):
     """Maintain a single instance of a class."""
 
     _instances: Dict['Singleton', Any] = {}
 
@@ -19,22 +19,14 @@
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         instance = cls._instances[cls]
         instance.__update__(*args, **kwargs)
         return instance
 
 
-class Sink(Protocol):
-    """Can sink data."""
-
-    def __call__(self, *args: Any) -> None:
-        """Must accept *args."""
-        ...
-
-
 class KafkaIgnoredPropertyFilter(logging.Filter):
     """Filter out specific kafka logging."""
 
     def filter(self, record):
         """Suppress CONFWARN messages with specific config keys."""
         return not (
             record.levelno == logging.WARNING
```

