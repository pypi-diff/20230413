# Comparing `tmp/vsui_client-1.1.0.tar.gz` & `tmp/vsui_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.0.tar", max compression
+gzip compressed data, was "vsui_client-1.1.1.tar", max compression
```

## Comparing `vsui_client-1.1.0.tar` & `vsui_client-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.0/README.md
--rw-r--r--   0        0        0      855 2023-04-13 12:17:32.322867 vsui_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      170 2023-04-13 12:17:26.602637 vsui_client-1.1.0/vsui_client/__init__.py
--rw-r--r--   0        0        0     3680 2023-04-13 12:14:13.577905 vsui_client-1.1.0/vsui_client/oo_interface.py
--rw-r--r--   0        0        0     4018 2023-04-13 12:13:23.925636 vsui_client-1.1.0/vsui_client/vsui_client.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.1/README.md
+-rw-r--r--   0        0        0      855 2023-04-13 12:47:53.420564 vsui_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-13 12:39:32.724732 vsui_client-1.1.1/vsui_client/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-13 12:42:12.637781 vsui_client-1.1.1/vsui_client/_main.py
+-rw-r--r--   0        0        0     3691 2023-04-13 12:39:40.190575 vsui_client-1.1.1/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     4016 2023-04-13 12:38:20.436809 vsui_client-1.1.1/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.1.1/PKG-INFO
```

### Comparing `vsui_client-1.1.0/README.md` & `vsui_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.0/pyproject.toml` & `vsui_client-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.0"
+version = "1.1.1"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.1.0/vsui_client/oo_interface.py` & `vsui_client-1.1.1/vsui_client/_oo_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # oo interface for vsui client, idea is to allow better control over enabling/disabling
 
 import logging
 from abc import ABC, abstractmethod
-import vsui_client.vsui_client as vsui_client
+import vsui_client._vsui_client as _vsui_client
 
 class VSUIClient(ABC):
     ''' Wrapper for vsui_client that allows for better control over enabling/disabling '''
     _handler = None
     @abstractmethod
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         pass
@@ -48,53 +48,53 @@
 
     @abstractmethod
     def get_handler(self) -> logging.Handler:
         pass
 
 class VSUIEnabled():
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
-        return vsui_client.connect(host, port)
+        return _vsui_client.connect(host, port)
     
     def disconnect(self) -> None:
-        return vsui_client.disconnect()
+        return _vsui_client.disconnect()
     
     def edit_element(self, data : dict) -> None:
-        return vsui_client.edit_element(data)
+        return _vsui_client.edit_element(data)
     
     def deactivate_task(self) -> None:
-        return vsui_client.deactivate_task()
+        return _vsui_client.deactivate_task()
 
     def notify(self, txt : str, type : str) -> None:
-        return vsui_client.notify(txt, type)
+        return _vsui_client.notify(txt, type)
 
     def set_task_id(self, id : str) -> None:
-        return vsui_client.set_task_id(id)
+        return _vsui_client.set_task_id(id)
     
     def set_logging_target(self, key : str) -> None:
-        return vsui_client.set_logging_target(key)
+        return _vsui_client.set_logging_target(key)
 
     def encode_image(
         self,
         arr,
         title: str = '',
         format : str = 'jpg',
         figsize: tuple = (8, 8),
         cmap: str = "gray"
     ) -> str:
-        return vsui_client.encode_image(
+        return _vsui_client.encode_image(
             arr=arr,
             title=title,
             format=format,
             figsize=figsize,
             cmap=cmap
         )
     
     def get_handler(self) -> logging.Handler:
         if self.get_handler is None:
-            self._handler = vsui_client.RequestHandler()
+            self._handler = _vsui_client.RequestHandler()
         return self._handler
 
 class VSUIDisabled():
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         ''' do nothing - not in UI mode '''
         pass
```

### Comparing `vsui_client-1.1.0/vsui_client/vsui_client.py` & `vsui_client-1.1.1/vsui_client/_vsui_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,33 +7,16 @@
 import base64
 import time
 
 sio = socketio.Client()
 task_id = None
 # target log for where intercepted logs should be forwarded to
 logging_target = None
-
 timeout_count = 0
 
-def encode_image(
-    arr,
-    title: str = '',
-    format : str = 'jpg',
-    figsize: tuple = (8, 8),
-    cmap: str = "gray"
-):
-    fig = plt.figure(figsize=figsize)
-    plt.imshow(arr, cmap=cmap)
-    plt.suptitle(title, fontsize=16)
-    my_stringIObytes = io.BytesIO()
-    plt.savefig(my_stringIObytes, format=format)
-    my_stringIObytes.seek(0)
-    my_base64_jpgData = base64.b64encode(my_stringIObytes.read()).decode()
-    return my_base64_jpgData
-
 # https://stackoverflow.com/a/51981833
 def vsui_process() -> Callable:
     ''' Decorator for functions that should be run as a vsui task 
         This decorator will catch any exceptions and send a message to the server
         returns the decorator
     '''
     def decorator(func) -> Callable:
@@ -119,7 +102,23 @@
         logging.error('No logging target set.')
 
 # http://naoko.github.io/intercept-python-logging/
 class RequestHandler(logging.Handler):
     def emit(self, record):
         ''' Intercept logs '''
         logging_intercept(record.getMessage())
+
+def encode_image(
+    arr,
+    title: str = '',
+    format : str = 'jpg',
+    figsize: tuple = (8, 8),
+    cmap: str = "gray"
+):
+    fig = plt.figure(figsize=figsize)
+    plt.imshow(arr, cmap=cmap)
+    plt.suptitle(title, fontsize=16)
+    my_stringIObytes = io.BytesIO()
+    plt.savefig(my_stringIObytes, format=format)
+    my_stringIObytes.seek(0)
+    my_base64_jpgData = base64.b64encode(my_stringIObytes.read()).decode()
+    return my_base64_jpgData
```

### Comparing `vsui_client-1.1.0/PKG-INFO` & `vsui_client-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

