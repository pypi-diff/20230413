# Comparing `tmp/osint-python-starter-service-2.0.5.tar.gz` & `tmp/osint-python-starter-service-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.5.tar", last modified: Wed Apr 12 13:50:00 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.6.tar", last modified: Thu Apr 13 20:24:22 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.5.tar` & `osint-python-starter-service-2.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.5/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.5/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 13:49:34.000000 osint-python-starter-service-2.0.5/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.5/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.5/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.5/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.5/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2980 2023-04-12 13:10:08.000000 osint-python-starter-service-2.0.5/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1274 2023-04-12 13:48:58.000000 osint-python-starter-service-2.0.5/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.5/starter_service/examples/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/examples/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-12 13:43:03.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-12 13:43:03.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/metadata_item_key_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-12 13:49:22.000000 osint-python-starter-service-2.0.5/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.5/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.5/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6239 2023-04-12 13:42:48.000000 osint-python-starter-service-2.0.5/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.6/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.6/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-13 20:23:17.000000 osint-python-starter-service-2.0.6/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.6/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.6/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6865 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.6/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.6/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3061 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.6/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-13 20:22:15.000000 osint-python-starter-service-2.0.6/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.6/starter_service/examples/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/examples/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:13:48.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-13 20:19:59.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-13 20:19:59.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/metadata_item_key_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-13 20:22:57.000000 osint-python-starter-service-2.0.6/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.6/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.6/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6239 2023-04-12 13:42:48.000000 osint-python-starter-service-2.0.6/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.5/LICENSE` & `osint-python-starter-service-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/PKG-INFO` & `osint-python-starter-service-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.5/README.md` & `osint-python-starter-service-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/setup.py` & `osint-python-starter-service-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.5",
+    version="2.0.6",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.5/starter_service/api.py` & `osint-python-starter-service-2.0.6/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/api_server.py` & `osint-python-starter-service-2.0.6/starter_service/api_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 from starter_service.schemas import SchemaRegistry
 
 _schema = SchemaRegistry()
 
 
 class APIServer:
 
-    def __init__(self, ready: callable = None, health: callable = None, kafka_status: str = None, base_service=None,
-                 **kwargs):
+    def __init__(self, name=None, ready: callable = None, health: callable = None, kafka_status: str = None,
+                 base_service=None, **kwargs):
+        self.name = name
         self._validated()
-        self.app = FastAPI()
+        self.app = FastAPI(title=self.name)
         self.router = APIRouter()
 
         @self.app.exception_handler(Exception)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
```

### Comparing `osint-python-starter-service-2.0.5/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.6/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/base_service.py` & `osint-python-starter-service-2.0.6/starter_service/base_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class StarterService(ABC):
     """Base class for all services."""
     name = None  # Change this to the name of your service or use CLIENT_ID environment variable
 
     def __init__(self):
         self.logger = logging.getLogger(__name__)
+        self._name = None
         self._kafka = None
         self._api = None
         self._schemas = None
         self._functions = None
         self._initialize()
 
     @abstractmethod
@@ -29,15 +30,15 @@
     @abstractmethod
     def health(self) -> str:
         """Return service health status."""
         pass
 
     def _initialize(self):
         """Initialize services"""
-        ENV.CLIENT_ID = ENV.CLIENT_ID or self.name
+        self.name = ENV.CLIENT_ID = ENV.CLIENT_ID or self.name or self.__class__.__name__
 
         def _schema_callback():
             """Callback for Schema Registry, called when Schema Registry is ready or when an error occurs"""
             self.logger.info("Schema callback")
             self._register_api(_kafka_status)
 
         def _kafka_callback():
@@ -61,15 +62,15 @@
         try:
             callback()
         except Exception as e:
             self.logger.error(f'Error initializing schema registry: {e}')
 
     def _register_api(self, _kafka_status):
         try:
-            self._api = APIServer(ready=self.ready, health=self.health, kafka_status=_kafka_status,
+            self._api = APIServer(name=self.name, ready=self.ready, health=self.health, kafka_status=_kafka_status,
                                   base_service=self)
             self._api.start()
             self.logger.info(f"REST API initialized.")
         except Exception as e:
             self.logger.error(f'Error initializing api: {e}')
             traceback.print_exc()
```

### Comparing `osint-python-starter-service-2.0.5/starter_service/env.py` & `osint-python-starter-service-2.0.6/starter_service/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # TOPICS
     CONSUME = [c.strip() for c in _env('CONSUME', '').split(',') if c.strip()]
     PRODUCE = [p.strip() for p in _env('PRODUCE', '').split(',') if p.strip()]
     CLIENT_ID = _env('CLIENT_ID', None)
 
     # KAFKA
     KAFKA_HOST = _env('KAFKA_HOST', '127.0.0.1:3501')
-    SCHEMA_REGISTRY = _env('SCHEMA_REGISTRY', 'http://localhost:8081')  # 3502')
+    SCHEMA_REGISTRY = _env('SCHEMA_REGISTRY', 'http://localhost:3502')
     PARTITIONER = _env("PARTITIONER", "random")
     MESSAGE_MAX_BYTES = _env.int('MESSAGE_MAX_BYTES', 1000000)
     HEARTBEAT_INTERVAL = _env.int('HEARTBEAT_INTERVAL', 10)
     OFFSET_TYPE = _env('OFFSET_TYPE', 'earliest')
     STRING_BASED_KEYS = _env.bool('STRING_BASED_KEYS', True)
 
     # REST API
```

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/classes/article_raw_en.py` & `osint-python-starter-service-2.0.6/starter_service/examples/classes/article_raw_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/classes/metadata_item_key_en.py` & `osint-python-starter-service-2.0.6/starter_service/examples/classes/metadata_item_key_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/error.py` & `osint-python-starter-service-2.0.6/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.6/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.6/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/examples/single.py` & `osint-python-starter-service-2.0.6/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.6/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/messages.py` & `osint-python-starter-service-2.0.6/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.5/starter_service/schemas.py` & `osint-python-starter-service-2.0.6/starter_service/schemas.py`

 * *Files identical despite different names*

