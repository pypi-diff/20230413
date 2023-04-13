# Comparing `tmp/vsui_client-1.0.0.tar.gz` & `tmp/vsui_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.0.0.tar", max compression
+gzip compressed data, was "vsui_client-1.1.0.tar", max compression
```

## Comparing `vsui_client-1.0.0.tar` & `vsui_client-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.0.0/README.md
--rw-r--r--   0        0        0      855 2023-04-13 10:41:11.799098 vsui_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 12:01:56.738617 vsui_client-1.0.0/vsui_client/__init__.py
--rw-r--r--   0        0        0     3857 2023-04-13 10:40:07.880084 vsui_client-1.0.0/vsui_client/vsui_client.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.0/README.md
+-rw-r--r--   0        0        0      855 2023-04-13 12:17:32.322867 vsui_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-04-13 12:17:26.602637 vsui_client-1.1.0/vsui_client/__init__.py
+-rw-r--r--   0        0        0     3680 2023-04-13 12:14:13.577905 vsui_client-1.1.0/vsui_client/oo_interface.py
+-rw-r--r--   0        0        0     4018 2023-04-13 12:13:23.925636 vsui_client-1.1.0/vsui_client/vsui_client.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 vsui_client-1.1.0/PKG-INFO
```

### Comparing `vsui_client-1.0.0/README.md` & `vsui_client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.0.0/pyproject.toml` & `vsui_client-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.0.0"
+version = "1.1.0"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.0.0/vsui_client/vsui_client.py` & `vsui_client-1.1.0/vsui_client/vsui_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 sio = socketio.Client()
 task_id = None
 # target log for where intercepted logs should be forwarded to
 logging_target = None
 
 timeout_count = 0
 
-def encode_image(arr,
+def encode_image(
+    arr,
     title: str = '',
     format : str = 'jpg',
     figsize: tuple = (8, 8),
     cmap: str = "gray"
 ):
     fig = plt.figure(figsize=figsize)
     plt.imshow(arr, cmap=cmap)
@@ -65,15 +66,18 @@
     global timeout_count
     try:
         sio.emit(event, data)
         timeout_count = 0
     except:
         timeout_count += 1
         if timeout_count == 5:
+            print('socketio timeout')
+            safe_emit('exception', {'task_id' : task_id, 'exception' : 'socketio timeout'})
             disconnect()
+            time.sleep(1)
             sys.exit(1)
 
 def connect(HOST : str = 'localhost', PORT : str = '8000') -> None:
     ''' initiate a socketio session with a server '''
     sio.connect('http://' + HOST + ':' + PORT, headers={'type':'app', 'id': task_id})
     print(f'sid is {sio.sid}')
```

### Comparing `vsui_client-1.0.0/PKG-INFO` & `vsui_client-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

