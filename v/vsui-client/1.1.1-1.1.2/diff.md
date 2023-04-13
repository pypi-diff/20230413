# Comparing `tmp/vsui_client-1.1.1.tar.gz` & `tmp/vsui_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.1.tar", max compression
+gzip compressed data, was "vsui_client-1.1.2.tar", max compression
```

## Comparing `vsui_client-1.1.1.tar` & `vsui_client-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.1/README.md
--rw-r--r--   0        0        0      855 2023-04-13 12:47:53.420564 vsui_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-13 12:39:32.724732 vsui_client-1.1.1/vsui_client/__init__.py
--rw-r--r--   0        0        0      954 2023-04-13 12:42:12.637781 vsui_client-1.1.1/vsui_client/_main.py
--rw-r--r--   0        0        0     3691 2023-04-13 12:39:40.190575 vsui_client-1.1.1/vsui_client/_oo_interface.py
--rw-r--r--   0        0        0     4016 2023-04-13 12:38:20.436809 vsui_client-1.1.1/vsui_client/_vsui_client.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.2/README.md
+-rw-r--r--   0        0        0      887 2023-04-13 13:47:24.971386 vsui_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-04-13 13:43:11.106253 vsui_client-1.1.2/vsui_client/__init__.py
+-rw-r--r--   0        0        0      917 2023-04-13 13:50:27.784220 vsui_client-1.1.2/vsui_client/_main.py
+-rw-r--r--   0        0        0     3975 2023-04-13 13:50:00.720258 vsui_client-1.1.2/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     3939 2023-04-13 13:45:59.194231 vsui_client-1.1.2/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 vsui_client-1.1.2/PKG-INFO
```

### Comparing `vsui_client-1.1.1/README.md` & `vsui_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.1/pyproject.toml` & `vsui_client-1.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.1"
+version = "1.1.2"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-socketio = {extras = ["client"], version = "^5.7.2"}
 matplotlib = "^3.6.1"
+
+[tool.poetry.dev-dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 tqdm = "^4.65.0"
 flask = "^2.2.3"
 flask-socketio = "^5.3.3"
 gevent = "^22.10.2"
 gevent-websocket = "^0.10.1"
```

### Comparing `vsui_client-1.1.1/vsui_client/_main.py` & `vsui_client-1.1.2/vsui_client/_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from vsui_client import _oo_interface
-from vsui_client import _vsui_client
 
 client = None
 
 def get_client() -> _oo_interface.VSUIClient:
     ''' return the current vsui client instance
     Returns:
         _oo_interface.VSUIClient: the client instance
```

### Comparing `vsui_client-1.1.1/vsui_client/_oo_interface.py` & `vsui_client-1.1.2/vsui_client/_oo_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # oo interface for vsui client, idea is to allow better control over enabling/disabling
 
+from typing import Union
 import logging
 from abc import ABC, abstractmethod
 import vsui_client._vsui_client as _vsui_client
 
 class VSUIClient(ABC):
-    ''' Wrapper for vsui_client that allows for better control over enabling/disabling '''
+    ''' Baseclass wrapper for vsui_client that allows for better control over enabling/disabling '''
     _handler = None
     @abstractmethod
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         pass
     
     @abstractmethod
     def disconnect(self) -> None:
         pass
     
     @abstractmethod
-    def edit_element(self, data : dict) -> None:
+    def edit_element(self, element_uid: str, value: Union[dict, str]) -> None:
         pass
 
     @abstractmethod
     def deactivate_task(self) -> None:
         pass
 
     @abstractmethod
@@ -47,22 +48,23 @@
         pass
 
     @abstractmethod
     def get_handler(self) -> logging.Handler:
         pass
 
 class VSUIEnabled():
+    ''' OO interface for vsui client, when vsui is enabled '''
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         return _vsui_client.connect(host, port)
     
     def disconnect(self) -> None:
         return _vsui_client.disconnect()
     
-    def edit_element(self, data : dict) -> None:
-        return _vsui_client.edit_element(data)
+    def edit_element(self, element_uid: str, value: Union[dict, str]) -> None:
+        return _vsui_client.edit_element(element_uid=element_uid, value=value)
     
     def deactivate_task(self) -> None:
         return _vsui_client.deactivate_task()
 
     def notify(self, txt : str, type : str) -> None:
         return _vsui_client.notify(txt, type)
 
@@ -90,23 +92,24 @@
     
     def get_handler(self) -> logging.Handler:
         if self.get_handler is None:
             self._handler = _vsui_client.RequestHandler()
         return self._handler
 
 class VSUIDisabled():
+    ''' OO interface for vsui client, when vsui is disabled '''
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         ''' do nothing - not in UI mode '''
         pass
     
     def disconnect(self) -> None:
         ''' do nothing - not in UI mode '''
         pass
 
-    def edit_element(self, data : dict) -> None:
+    def edit_element(self, element_uid: str, value: Union[dict, str]) -> None:
         ''' do nothing - not in UI mode '''
         pass
 
     def deactivate_task(self) -> None:
         ''' do nothing - not in UI mode '''
         pass
```

### Comparing `vsui_client-1.1.1/vsui_client/_vsui_client.py` & `vsui_client-1.1.2/vsui_client/_vsui_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,75 +3,70 @@
 import logging
 from matplotlib import pyplot as plt
 import io
 import sys
 import base64
 import time
 
+from vsui_client import _vsui_logger
+
 sio = socketio.Client()
 task_id = None
 # target log for where intercepted logs should be forwarded to
 logging_target = None
 timeout_count = 0
 
 # https://stackoverflow.com/a/51981833
 def vsui_process() -> Callable:
     ''' Decorator for functions that should be run as a vsui task 
         This decorator will catch any exceptions and send a message to the server
         returns the decorator
     '''
     def decorator(func) -> Callable:
         def wrapper(*args, **kwargs):
-            print('decorating')
+            _vsui_logger.info(f'running {func.__name__} as vsui process')
             r = None
             try:
                 r = func(*args, **kwargs)
-            except SystemExit as e:
-                print('system exit')
-                print(f'exception caught: {e}')
-                safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
-                r = disconnect()
-                time.sleep(1)
-                sys.exit(1)
-            except Exception as e:
-                print(f'exception caught: {e}')
+            except (SystemExit, Exception) as e:
+                _vsui_logger.exception(f'exception caught: {e}')
                 safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
                 r = disconnect()
                 time.sleep(1)
                 sys.exit(1)
             finally:
-                print('wrapper finished')
+                _vsui_logger.info(f'finished running {func.__name__} as vsui process')
                 return r
         return wrapper
     return decorator
 
 def safe_emit(event, data):
     ''' emit a socketio event with exception handling '''
     global timeout_count
     try:
         sio.emit(event, data)
         timeout_count = 0
     except:
         timeout_count += 1
         if timeout_count == 5:
-            print('socketio timeout')
+            _vsui_logger.exception('socketio timeout')
             safe_emit('exception', {'task_id' : task_id, 'exception' : 'socketio timeout'})
             disconnect()
             time.sleep(1)
             sys.exit(1)
 
 def connect(HOST : str = 'localhost', PORT : str = '8000') -> None:
     ''' initiate a socketio session with a server '''
     sio.connect('http://' + HOST + ':' + PORT, headers={'type':'app', 'id': task_id})
-    print(f'sid is {sio.sid}')
+    _vsui_logger.info(f'connected to {HOST}:{PORT} with sid {sio.sid}')
 
 def disconnect() -> None:
     ''' disconnect the socketio session '''
     sio.disconnect()
-    print('socket disconnected')
+    _vsui_logger.info('disconnected')
 
 # struct: { 'name' : 'type' }
 # send a new task to be added to the server's task manager
 def set_task_id(id : str) -> None:
     ''' set the id of this task '''
     global task_id
     task_id = id
```

### Comparing `vsui_client-1.1.1/PKG-INFO` & `vsui_client-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flask (>=2.2.3,<3.0.0)
-Requires-Dist: flask-socketio (>=5.3.3,<6.0.0)
-Requires-Dist: gevent (>=22.10.2,<23.0.0)
-Requires-Dist: gevent-websocket (>=0.10.1,<0.11.0)
 Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
-Requires-Dist: pytest (>=7.3.0,<8.0.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-socketio[client] (>=5.7.2,<6.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Volume Segmantics User Interface Client
 
 This package allows a python script to connect to the volume segmantics server and update the server's information about a corresponding process. <br>
 The task id must match the name of a process definition in the connected server. The provided methods are:
 - **set_task_id** (id : str)
```

