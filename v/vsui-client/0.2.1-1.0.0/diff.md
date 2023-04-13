# Comparing `tmp/vsui_client-0.2.1.tar.gz` & `tmp/vsui_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-0.2.1.tar", max compression
+gzip compressed data, was "vsui_client-1.0.0.tar", max compression
```

## Comparing `vsui_client-0.2.1.tar` & `vsui_client-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1308 2022-11-21 13:42:36.289300 vsui_client-0.2.1/README.md
--rw-r--r--   0        0        0      469 2022-12-09 09:22:59.651351 vsui_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-02 12:17:39.300807 vsui_client-0.2.1/vsui_client/__init__.py
--rw-r--r--   0        0        0     3232 2022-12-08 16:24:54.645567 vsui_client-0.2.1/vsui_client/vsui_client.py
--rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 vsui_client-0.2.1/setup.py
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 vsui_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.0.0/README.md
+-rw-r--r--   0        0        0      855 2023-04-13 10:41:11.799098 vsui_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 12:01:56.738617 vsui_client-1.0.0/vsui_client/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-13 10:40:07.880084 vsui_client-1.0.0/vsui_client/vsui_client.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.0.0/PKG-INFO
```

### Comparing `vsui_client-0.2.1/README.md` & `vsui_client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-0.2.1/vsui_client/vsui_client.py` & `vsui_client-1.0.0/vsui_client/vsui_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 import socketio
-from typing import Any
+from typing import Any, Callable
 import logging
 from matplotlib import pyplot as plt
 import io
 import sys
 import base64
-import atexit
+import time
 
 sio = socketio.Client()
 task_id = None
 # target log for where intercepted logs should be forwarded to
 logging_target = None
-timeout_target = 5
 
 timeout_count = 0
 
 def encode_image(arr,
-title: str = '',
-format : str = 'jpg',
-figsize: tuple = (8, 8),
-cmap: str = "gray"):
+    title: str = '',
+    format : str = 'jpg',
+    figsize: tuple = (8, 8),
+    cmap: str = "gray"
+):
     fig = plt.figure(figsize=figsize)
     plt.imshow(arr, cmap=cmap)
     plt.suptitle(title, fontsize=16)
     my_stringIObytes = io.BytesIO()
     plt.savefig(my_stringIObytes, format=format)
     my_stringIObytes.seek(0)
     my_base64_jpgData = base64.b64encode(my_stringIObytes.read()).decode()
-    plt.close()
     return my_base64_jpgData
 
-def exit_handler():
-    logging.info('VSUI exit handler triggered')
-    disconnect()
-                    
 # https://stackoverflow.com/a/51981833
-def vsui_process():
-    def decorator(func):
+def vsui_process() -> Callable:
+    ''' Decorator for functions that should be run as a vsui task 
+        This decorator will catch any exceptions and send a message to the server
+        returns the decorator
+    '''
+    def decorator(func) -> Callable:
         def wrapper(*args, **kwargs):
+            print('decorating')
+            r = None
             try:
-                r = None
-                print('VSUI process started')
-                #atexit.register(exit_handler)
                 r = func(*args, **kwargs)
-                return r
+            except SystemExit as e:
+                print('system exit')
+                print(f'exception caught: {e}')
+                safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
+                r = disconnect()
+                time.sleep(1)
+                sys.exit(1)
             except Exception as e:
-                logging.error(e)
-                disconnect()
+                print(f'exception caught: {e}')
+                safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
+                r = disconnect()
+                time.sleep(1)
                 sys.exit(1)
+            finally:
+                print('wrapper finished')
+                return r
         return wrapper
     return decorator
 
 def safe_emit(event, data):
     ''' emit a socketio event with exception handling '''
+    global timeout_count
     try:
         sio.emit(event, data)
-    except Exception as e:
-        logging.warning(e)
-        pass
+        timeout_count = 0
+    except:
+        timeout_count += 1
+        if timeout_count == 5:
+            disconnect()
+            sys.exit(1)
 
 def connect(HOST : str = 'localhost', PORT : str = '8000') -> None:
     ''' initiate a socketio session with a server '''
     sio.connect('http://' + HOST + ':' + PORT, headers={'type':'app', 'id': task_id})
     print(f'sid is {sio.sid}')
 
 def disconnect() -> None:
```

### Comparing `vsui_client-0.2.1/PKG-INFO` & `vsui_client-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 0.2.1
+Version: 1.0.0
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.2.3,<3.0.0)
+Requires-Dist: flask-socketio (>=5.3.3,<6.0.0)
+Requires-Dist: gevent (>=22.10.2,<23.0.0)
+Requires-Dist: gevent-websocket (>=0.10.1,<0.11.0)
 Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
+Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-socketio[client] (>=5.7.2,<6.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Volume Segmantics User Interface Client
 
 This package allows a python script to connect to the volume segmantics server and update the server's information about a corresponding process. <br>
 The task id must match the name of a process definition in the connected server. The provided methods are:
 - **set_task_id** (id : str)
```

