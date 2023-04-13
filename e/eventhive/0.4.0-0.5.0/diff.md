# Comparing `tmp/eventhive-0.4.0.tar.gz` & `tmp/eventhive-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhive-0.4.0.tar", last modified: Wed Apr  5 00:39:36 2023, max compression
+gzip compressed data, was "eventhive-0.5.0.tar", last modified: Thu Apr 13 11:31:20 2023, max compression
```

## Comparing `eventhive-0.4.0.tar` & `eventhive-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-05 00:39:25.000000 eventhive-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-05 00:39:36.582928 eventhive-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-05 00:39:25.000000 eventhive-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/eventhive/
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/eventhive/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/connectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/connectors/fastapi_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/connectors/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/eventhive/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/external/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/eventhive/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-05 00:39:25.000000 eventhive-0.4.0/eventhive/servers/fastapi_srv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/eventhive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:39:36.000000 eventhive-0.4.0/eventhive.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-05 00:39:25.000000 eventhive-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-05 00:39:25.000000 eventhive-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-05 00:39:36.586928 eventhive-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:39:36.582928 eventhive-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-05 00:39:25.000000 eventhive-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-05 00:39:25.000000 eventhive-0.4.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-05 00:39:25.000000 eventhive-0.4.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-05 00:39:25.000000 eventhive-0.4.0/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-05 00:39:25.000000 eventhive-0.4.0/tests/test_zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 11:31:10.000000 eventhive-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-13 11:31:20.563711 eventhive-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-13 11:31:10.000000 eventhive-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/eventhive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/eventhive/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/connectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/connectors/fastapi_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/connectors/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/eventhive/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/external/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/eventhive/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 11:31:10.000000 eventhive-0.5.0/eventhive/servers/fastapi_srv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/eventhive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:31:20.000000 eventhive-0.5.0/eventhive.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 11:31:10.000000 eventhive-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 11:31:10.000000 eventhive-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 11:31:20.563711 eventhive-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:31:20.563711 eventhive-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-13 11:31:10.000000 eventhive-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-13 11:31:10.000000 eventhive-0.5.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-13 11:31:10.000000 eventhive-0.5.0/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-13 11:31:10.000000 eventhive-0.5.0/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 11:31:10.000000 eventhive-0.5.0/tests/test_zeroconf.py
```

### Comparing `eventhive-0.4.0/LICENSE` & `eventhive-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/PKG-INFO` & `eventhive-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhive
-Version: 0.4.0
+Version: 0.5.0
 Summary: Network PubSub and Async Message Passing for Humans
 Home-page: https://github.com/operatorequals/eventhive
 Author: attr: eventhive.__meta__.__author__
 Author-email: "john.torakis@gmail.com"
 License: MIT
 Keywords: pubsub,microservice,iot,rpc
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eventhive-0.4.0/README.md` & `eventhive-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/__init__.py` & `eventhive-0.5.0/eventhive/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from .broadcast import Broadcast, init_from_broadcast
+from .servers import fastapi_srv
+from .logger import logger
+from .exceptions import ConnectorInitializationException
+from .config import PUBSUB_TYPES
+# Import config APIs
+from .config import CONFIG as CONFIG_DICT
+from . import config as CONFIG
 # Inherit hooker API
-from hooker import EVENTS, get_event_name, hook, reset, events
+from hooker import EVENTS, get_event_name, reset, events
 from hooker import logger as hooker_logger
+from hooker import hook as hooker_hook
 
 import logging
 hooker_logger.handlers = [logging.NullHandler()]
 
-# Import config APIs
-from . import config as CONFIG
-from .config import CONFIG as CONFIG_DICT
-from .config import PUBSUB_TYPES
-
-from .logger import logger
-
-from .servers import fastapi_srv
-from .broadcast import Broadcast, init_from_broadcast
-
 CONNECTORS = {}
 SERVERS = {}
 BROADCASTERS = {}
 
 SERVER_CLASS = {
     'fastapi': fastapi_srv.FastAPIPubSubServer,
 }
 
+def register(event, function, dependencies=None, expand=True):
+    return hook(event)(function, expand=expand)
+
+def hook(event, dependencies=None, expand=True):
+    # Test if event (can be 'str' or 'iterable')
+    # is totally included in created events)
+    if set(event) == set(events("**")) & set(event):
+        EVENTS.append(event)
+    return hooker_hook(event, dependencies=dependencies, expand=expand)
 
-def init():
+def init(required=[]):
     CONFIG_DICT = CONFIG.CONFIG  # renew the config state
 
     # =========== Servers
 
     for k, v in CONFIG_DICT['servers'].items():
 
         if v['create'] == 'needed':
@@ -74,22 +82,24 @@
             if v['pubsub_type'] == 'redis':
                 from .connectors import redis as redis_class
                 connector_class = redis_class.RedisConnector
             elif v['pubsub_type'] == 'fastapi':
                 from .connectors import fastapi_pubsub as fastapi_class
                 connector_class = fastapi_class.FastAPIPubSubConnector
             else:
-                logger.error("PubSub backend: '%s' is not recognised in connector '%s'. Moving to next connector." % (
+                logger.error("PubSub backend: '%s' is not recognised in connector '%s'." % (
                     v['pubsub_type'], k))
-                continue
+                raise KeyError("%s not in %s" % (v['pubsub_type'], PUBSUB_TYPES))
 
             CONNECTORS[k] = connector_class(k, v, CONFIG_DICT['eventhive'])
 
         except Exception as e:
             logger.error("%s: Could not connect to PubSub '%s'" % (e, k))
+            if k in required:
+                raise ConnectorInitializationException("Connector '%s' is required." % k)
             continue
 
         # connector_events = events('*/*')
         # logger.debug("Events that follow pattern '%s/*/*' (%s) will be emitted for connector %s" % (k, connector_events, k))
         # CONNECTORS[k]._publishers[k] = hook(connector_events)(
         #     lambda message: CONNECTORS[k].send_to_pubsub(message))
         CONNECTORS[k]._publishers[k] = hook(['*'])(
```

### Comparing `eventhive-0.4.0/eventhive/broadcast.py` & `eventhive-0.5.0/eventhive/broadcast.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/cli.py` & `eventhive-0.5.0/eventhive/cli.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/config.py` & `eventhive-0.5.0/eventhive/config.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/connectors/base.py` & `eventhive-0.5.0/eventhive/connectors/base.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/connectors/fastapi_pubsub.py` & `eventhive-0.5.0/eventhive/connectors/fastapi_pubsub.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/connectors/redis.py` & `eventhive-0.5.0/eventhive/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/crypto.py` & `eventhive-0.5.0/eventhive/crypto.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/external/aes.py` & `eventhive-0.5.0/eventhive/external/aes.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/logger.py` & `eventhive-0.5.0/eventhive/logger.py`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/eventhive/servers/fastapi_srv.py` & `eventhive-0.5.0/eventhive/servers/fastapi_srv.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         endpoint = self.conn_conf['init']['endpoint']
         self.endpoint = endpoint if endpoint.startswith(
             '/') else '/' + endpoint
 
         self.app = FastAPI()
         router = APIRouter()
         endpoint = PubSubEndpoint()
-        endpoint.register_route(router)
+        endpoint.register_route(router, path=self.endpoint)
         self.app.include_router(router)
         self.uvicorn_config = uvicorn.Config(self.app, host=self.host, port=self.port)
         self.uvicorn_server = uvicorn.Server(config=self.uvicorn_config)
 
         logger.info("FastAPI PubSub Server '%s' initialized" % self.conn_id)
 
     def run(self):
```

### Comparing `eventhive-0.4.0/eventhive.egg-info/PKG-INFO` & `eventhive-0.5.0/eventhive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhive
-Version: 0.4.0
+Version: 0.5.0
 Summary: Network PubSub and Async Message Passing for Humans
 Home-page: https://github.com/operatorequals/eventhive
 Author: attr: eventhive.__meta__.__author__
 Author-email: "john.torakis@gmail.com"
 License: MIT
 Keywords: pubsub,microservice,iot,rpc
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eventhive-0.4.0/eventhive.egg-info/SOURCES.txt` & `eventhive-0.5.0/eventhive.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 eventhive/__init__.py
 eventhive/__meta__.py
 eventhive/broadcast.py
 eventhive/cli.py
 eventhive/config.py
 eventhive/crypto.py
+eventhive/exceptions.py
 eventhive/logger.py
 eventhive.egg-info/PKG-INFO
 eventhive.egg-info/SOURCES.txt
 eventhive.egg-info/dependency_links.txt
 eventhive.egg-info/entry_points.txt
 eventhive.egg-info/requires.txt
 eventhive.egg-info/top_level.txt
```

### Comparing `eventhive-0.4.0/setup.cfg` & `eventhive-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `eventhive-0.4.0/tests/test_redis.py` & `eventhive-0.5.0/tests/test_redis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import docker
-from importlib import reload
 import atexit
-import unittest
-import sys
-import os
-import time
-import threading
+import logging
 import json
 
 import eventhive
 from eventhive.logger import logger
 
 import tests
 
-logger.setLevel(0)  # DEBUG
+logger.setLevel(logging.DEBUG)  # DEBUG
 
 # Setup Docker ==============================
 
 DOCKER = docker.from_env()
 REDIS_CONTAINER_NAME = "eventhive-test-redis"
 REDIS_ADDRESS = ("127.0.0.1", "6379")
 
@@ -29,101 +24,78 @@
         name=REDIS_CONTAINER_NAME,
         ports={"6379/tcp": REDIS_ADDRESS},
     )
 atexit.register(REDIS_CONTAINER.remove)
 # ===========================================
 
 
-class TestEvent(unittest.TestCase):
+class TestEvent(tests.TestEventhive):
+
     def setUp(self):
         REDIS_CONTAINER.start()
 
     def tearDown(self):
-        time.sleep(1)
-        eventhive.stop()
-        for k in list(sys.modules.keys()):
-            if k.startswith('eventhive'):
-                sys.modules.pop(k)
+        super().tearDown()
         REDIS_CONTAINER.stop()
 
     def test_subscription(self, event='',
                           receiver="receiver", connector='redis',
                           data={'key': 'value'}
                           ):
-        eventhive.CONFIG.read_string(
-            """
+        eventhive.CONFIG.read_string("""
 connectors:
   %s:
     pubsub_type: redis
     input_channel: ''
     init:
       host: %s
       port: %s
       db: 0
 """ % (connector, REDIS_ADDRESS[0], REDIS_ADDRESS[1]))
         event = tests.get_function_name()
         event_name = "%s/%s/%s" % (connector, receiver, event)
-        eventhive.EVENTS.append(event_name, "test subscription")
+        eventhive.EVENTS.append(event_name, event)
 
         eventhive.init()
 
-        sender_thr = threading.Thread(
-            target=tests.fire_later,
-            args=(event_name, data)
-        )
-
-        sender_thr.daemon = True
-        sender_thr.start()
-        # sender_thr.join()
+        self.sender_thr = tests.fire_later_thread_start(event_name, data)
 
         output = tests.call_eventhive_cli(
             connector, receiver, event, "tests/configs/receiver-redis.yaml")
-        output = str(output, 'utf8')
         print("OUTPUT: " + output)
         message = json.loads(output)
-        # sender_thr.join()
 
         self.assertTrue(
             eventhive.CONFIG_DICT['eventhive']['metadata_key'] in message)
 
     def test_no_metadata(self, event='',
                          receiver="receiver", connector='redis',
                          data={'key': 'value'}
                          ):
-        eventhive.CONFIG.read_string(
-            """
+        eventhive.CONFIG.read_string("""
 eventhive:
   remove_metadata: true
 connectors:
   %s:
     pubsub_type: redis
     input_channel: ''
     init:
       host: %s
       port: %s
       db: 0
 """ % (connector, REDIS_ADDRESS[0], REDIS_ADDRESS[1]))
 
         event = tests.get_function_name()
         event_name = "%s/%s/%s" % (connector, receiver, event)
-        eventhive.EVENTS.append(event_name, "test no metadata")
+        eventhive.EVENTS.append(event_name, event)
 
         eventhive.init()
 
-        sender_thr = threading.Thread(
-            target=tests.fire_later,
-            args=(event_name, data)
-        )
-
-        sender_thr.daemon = True
-        sender_thr.start()
-        # sender_thr.join()
+        self.sender_thr = tests.fire_later_thread_start(event_name, data)
 
         output = tests.call_eventhive_cli(
             connector, receiver, event, "tests/configs/receiver-redis.yaml")
-        output = str(output, 'utf8')
         print("OUTPUT: " + output)
         message = json.loads(output)
-        # sender_thr.join()
 
         self.assertTrue(
             eventhive.CONFIG_DICT['eventhive']['metadata_key'] not in message)
```

### Comparing `eventhive-0.4.0/tests/test_zeroconf.py` & `eventhive-0.5.0/tests/test_fastapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,77 @@
-from importlib import reload
-import atexit
-import unittest
-import sys
-import os
-import time
-import threading
 import json
+import logging
 
 import eventhive
 from eventhive.logger import logger
-from eventhive.servers.fastapi_srv import FastAPIPubSubServer
 
 import tests
 
-logger.setLevel(0)  # DEBUG
+logger.setLevel(logging.DEBUG)  # DEBUG
 
+FASTAPI_ADDRESS = ["127.0.0.1", "8085"]
 
-class TestEvent(unittest.TestCase):
 
-    def tearDown(self):
-        time.sleep(1)
-        eventhive.stop()
-        for k in list(sys.modules.keys()):
-            if k.startswith('eventhive'):
-                sys.modules.pop(k)
+class TestEvent(tests.TestEventhive):
 
     def test_subscription(self, event='',
                           receiver="receiver", connector='fastapi',
                           data={'key': 'value'}
                           ):
         eventhive.CONFIG.read_string(
             """
 connectors:
   %s:
     pubsub_type: fastapi
     input_channel: ''
-    from_broadcast: true # <---
-""" % (connector))
+    init:
+      host: %s
+      port: %s
+""" % (connector, FASTAPI_ADDRESS[0], FASTAPI_ADDRESS[1]))
         event = tests.get_function_name()
         event_name = "%s/%s/%s" % (connector, receiver, event)
         eventhive.EVENTS.append(event_name, "test subscription")
 
-        sender_thr = threading.Thread(
-            target=lambda: eventhive.init() or tests.fire_later(
-                event_name, data))
+        eventhive.init()
 
-        sender_thr.daemon = True
-        sender_thr.start()
+        self.sender_thr = tests.fire_later_thread_start(event_name, data)
 
         output = tests.call_eventhive_cli(
-            connector,
-            receiver,
-            event,
-            "tests/configs/server-fastapi-broadcast.yaml",
-            timeout=6)
-
-        output = str(output, 'utf8')
+            connector, receiver, event, "tests/configs/server-fastapi.yaml")
         print("OUTPUT: '%s'" % output)
         message = json.loads(output)
-        sender_thr.join()
 
         self.assertTrue(
             eventhive.CONFIG_DICT['eventhive']['metadata_key'] in message)
+
+    def test_no_metadata(self, event='',
+                         receiver="receiver", connector='fastapi',
+                         data={'key': 'value'}
+                         ):
+        eventhive.CONFIG.read_string(
+            """
+eventhive:
+  remove_metadata: true
+connectors:
+  %s:
+    pubsub_type: fastapi
+    input_channel: ''
+    init:
+      host: %s
+      port: %s
+""" % (connector, FASTAPI_ADDRESS[0], FASTAPI_ADDRESS[1]))
+
+        event = tests.get_function_name()
+        event_name = "%s/%s/%s" % (connector, receiver, event)
+        eventhive.EVENTS.append(event_name, "test no metadata")
+
+        eventhive.init()
+
+        self.sender_thr = tests.fire_later_thread_start(event_name, data)
+
+        output = tests.call_eventhive_cli(
+            connector, receiver, event, "tests/configs/server-fastapi.yaml")
+        print("OUTPUT: " + output)
+        message = json.loads(output)
+
+        self.assertTrue(
+            eventhive.CONFIG_DICT['eventhive']['metadata_key'] not in message)
```

