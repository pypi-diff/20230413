# Comparing `tmp/taichu-serve-1.0.11.tar.gz` & `tmp/taichu-serve-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-1.0.11.tar", last modified: Tue Apr 11 08:59:04 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.0.tar", last modified: Thu Apr 13 09:34:05 2023, max compression
```

## Comparing `taichu-serve-1.0.11.tar` & `taichu-serve-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.811370 taichu-serve-1.0.11/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.811127 taichu-serve-1.0.11/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809610 taichu-serve-1.0.11/model_service/
--rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     8308 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/app.py
--rw-r--r--   0 chen       (501) staff       (20)     1302 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/command.py
--rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.11/model_service/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.11/model_service/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3572 2023-04-11 04:36:47.000000 taichu-serve-1.0.11/model_service/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.11/model_service/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809947 taichu-serve-1.0.11/model_service/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/model_def.py
--rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.11/model_service/model_service.py
--rw-r--r--   0 chen       (501) staff       (20)     1061 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/settings.py
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-11 08:59:04.811428 taichu-serve-1.0.11/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      952 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.810922 taichu-serve-1.0.11/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409543 taichu-serve-2.0.0/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 09:34:05.409395 taichu-serve-2.0.0/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-13 09:34:05.409588 taichu-serve-2.0.0/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:33:23.000000 taichu-serve-2.0.0/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.408188 taichu-serve-2.0.0/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3325 2023-04-13 09:12:09.000000 taichu-serve-2.0.0/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)    10809 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     2077 2023-04-13 09:34:02.000000 taichu-serve-2.0.0/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-2.0.0/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3800 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2103 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409227 taichu-serve-2.0.0/taichu_serve/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.0/taichu_serve/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     5233 2023-04-13 09:13:03.000000 taichu-serve-2.0.0/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     1908 2023-04-13 06:27:18.000000 taichu-serve-2.0.0/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409087 taichu-serve-2.0.0/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      587 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       56 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-1.0.11/model_service/app.py` & `taichu-serve-2.0.0/taichu_serve/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 # -*- coding: utf-8 -*-
 """
 DL webservice app
 """
+import ctypes
 import inspect
 import json
 import logging
 import os
 import threading
 import time
 import traceback
 import uuid
 
 from flask import Flask, request, g
 
-import log
-from settings import parse_args
+from taichu_serve.log import init_logger
+from taichu_serve.settings import parse_args
+from taichu_serve.ratelimiter import semaphore
 
-log.init_logger()
+init_logger()
 
 app = Flask("aa")
 
-from error_code import ModelNotFoundError, ModelPredictError
+from taichu_serve.error_code import ModelNotFoundError, ModelPredictError
 
 LOGGER = logging.getLogger(__name__)
-import argparse
 
-from model_service.model_service import SingleNodeService
+from taichu_serve.model_server import SingleNodeService
+import multiprocessing
 
+workers_pool = multiprocessing.Queue()
+workers_status = []
 
-def init_model_service_instance():
+
+def worker_main_loop(args, pipe, status):
     # pwd = os.path.dirname(os.path.abspath(__file__))
 
-    args = parse_args()
+    # args = parse_args()
 
     LOGGER.info("args: %s", args)
 
-    from model_service.model_service import load_service
+    from taichu_serve.model_server import load_service
     dict_model_service = {}
 
     model_path = os.path.abspath(args.model_path)
     # model_name = args.model_name
 
     model_service_file = args.service_file
 
@@ -64,44 +69,104 @@
     #     raise Exception(
     #         'There should be one user defined service derived from ModelService.'
     #     )
 
     for c in class_defs:
         LOGGER.info("class_defs: %s", c.__name__)
         instance = c(model_path)
-        threading.Thread(target=instance.warmup).start()
+        # threading.Thread(target=instance.warmup).start()
+        instance.warmup()
         dict_model_service[f'{str(c.__name__).lower()}_{instance.model_version.lower()}'] = instance
 
     # model_service = class_defs[0](model_path)
+    status.value = 0
+    LOGGER.info("model service init done")
 
-    return dict_model_service
-
+    while True:
+        data = pipe.recv()
+        try:
+            model_name = data.get('model_name')
+            model_version = data.get('model_version')
+            ins = dict_model_service.get(f'{model_name.lower()}_{model_version.lower()}', None)
+            if ins is None:
+                ret = {
+                    'data': None,
+                    'status': 'error',
+                    'error': 'model not found',
+                }
+            else:
+                ret = {
+                    'data': ins.inference(data.get('data'), data.get('context', {})),
+                    'status': 'ok',
+                }
+        except Exception as e:
+            LOGGER.error(traceback.format_exc())
+            ret = {
+                'data': None,
+                'status': 'error',
+                'error': str(e),
+            }
+        pipe.send(ret)
+
+    # return dict_model_service
+
+
+def model_inference(model_name, model_version, data, context={}):
+    p = workers_pool.get(timeout=1)
+    p.send({'model_name': model_name, 'model_version': model_version, 'data': data, 'context': context})
+    ret = p.recv()
+    workers_pool.put(p)
+    if ret.get('status') == 'error':
+        raise ModelPredictError(message=ret.get('error'))
+    return ret.get('data')
 
-model_service = init_model_service_instance()
 
+args = parse_args()
 
-def get_model_service(model_name, model_version):
-    model_name = model_name.lower()
-    model_version = model_version.lower()
-    ins = model_service.get(f'{model_name}_{model_version}', None)
-    if ins is None:
-        raise ModelNotFoundError(message=f'Model {model_name} version {model_version} not found')
-    return ins
 
+def init_model_service_instance():
+    for i in range(args.instances_num):
+        p1, p2 = multiprocessing.Pipe()
+        status = multiprocessing.Value('i', -1)
+        workers_status.append(status)
+        LOGGER.info("start worker %s", i)
+        multiprocessing.Process(target=worker_main_loop, args=(args, p2, status)
+                                ).start()
+        workers_pool.put(p1)
+
+
+# model_service = init_model_service_instance()
+
+
+# def get_model_service(model_name, model_version):
+#     model_name = model_name.lower()
+#     model_version = model_version.lower()
+#     ins = model_service.get(f'{model_name}_{model_version}', None)
+#     if ins is None:
+#         raise ModelNotFoundError(message=f'Model {model_name} version {model_version} not found')
+#     return ins
 
 def is_all_model_ready():
-    if len(model_service) == 0:
-        return False
-    for k, instance in model_service.items():
-        if not instance.ready:
+    for stat in workers_status:
+        if stat.value != 0:
             return False
 
     return True
 
 
+# def is_all_model_ready():
+# if len(model_service) == 0:
+#     return False
+# for k, instance in model_service.items():
+#     if not instance.ready:
+#         return False
+
+# return True
+
+
 @app.before_request
 def add_request_id():
     # 记录请求开始时间
     g.start = time.time()
 
     forwarded_for = request.headers.get('X-Forwarded-For')
     LOGGER.debug('X-Forwarded-For:{}'.format(forwarded_for))
@@ -115,16 +180,30 @@
         else:
             request_id = str(uuid.uuid4())
         setattr(g, 'request_id', request_id)
     except Exception as e:
         logging.error(str(e))
 
 
+@app.before_request
+def limiter():
+    if request.path == '/health/live' or request.path == '/health/ready':
+        return
+
+    ok = semaphore.acquire(blocking=True, timeout=1)
+    g.is_limited = not ok
+    if not ok:
+        return {'error': '请求过于频繁，请稍后再试'}, 429, {'Content-Type': 'application/json'}
+
+
 @app.after_request
 def after_request(response):
+    if hasattr(g, 'is_limited') and not g.is_limited:
+        semaphore.release()
+
     try:
         extra = {
             # 'id': str(uuid.uuid4()),
             'http_method': request.method,
             'endpoint': request.endpoint,
             'url_path': request.path,
             'url_query': request.query_string.decode('utf-8'),
@@ -175,18 +254,18 @@
     ret = {
         'id': request_id,
         'model_name': model_name,
         'model_version': model_version,
         'parameters': {}
     }
 
-    instance = get_model_service(model_name, model_version)
+    # instance = get_model_service(model_name, model_version)
 
     try:
-        res = instance.inference(req.get('parameters', {}), context={})
+        res = model_inference(model_name, model_version, req.get('parameters', {}), ctx)
     except Exception as e:
         LOGGER.error('Algorithm crashed!')
         LOGGER.error(traceback.format_exc())
         raise ModelPredictError(message=str(e))
 
     ret['parameters'] = res
     return json.dumps(ret, ensure_ascii=False), 200, {
```

### Comparing `taichu-serve-1.0.11/model_service/common.py` & `taichu-serve-2.0.0/taichu_serve/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import threading
 import time
 import uuid
 
 import grpc
 
-from error_code import ModelPredictError, ModelNotFoundError
+from taichu_serve.error_code import ModelPredictError, ModelNotFoundError
 
 Local = threading.local()
 logger = logging.getLogger(__name__)
 
 
 def grpc_interceptor(func):
     @functools.wraps(func)
```

### Comparing `taichu-serve-1.0.11/model_service/error_code.py` & `taichu-serve-2.0.0/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_predict_v2.proto\x12\x0ctaichu_infer\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x93\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x42\n\x06inputs\x18\x04 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x12\x43\n\x07outputs\x18\x05 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xbe\x03\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x43\n\nparameters\x18\x04 \x03(\x0b\x32/.taichu_infer.ModelInferRequest.ParametersEntry\x1a\xdb\x01\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12^\n\nparameters\x18\x02 \x03(\x0b\x32J.taichu_infer.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\xe2\x01\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x44\n\nparameters\x18\x04 \x03(\x0b\x32\x30.taichu_infer.ModelInferResponse.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\x80\x01\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0bint64_param\x18\x02 \x01(\x03H\x00\x12\x15\n\x0b\x66loat_param\x18\x03 \x01(\x02H\x00\x12\x16\n\x0cstring_param\x18\x04 \x01(\tH\x00\x42\x12\n\x10parameter_choice2\xfd\x04\n\x14GRPCInferenceService\x12Q\n\nServerLive\x12\x1f.taichu_infer.ServerLiveRequest\x1a .taichu_infer.ServerLiveResponse\"\x00\x12T\n\x0bServerReady\x12 .taichu_infer.ServerReadyRequest\x1a!.taichu_infer.ServerReadyResponse\"\x00\x12Q\n\nModelReady\x12\x1f.taichu_infer.ModelReadyRequest\x1a .taichu_infer.ModelReadyResponse\"\x00\x12]\n\x0eServerMetadata\x12#.taichu_infer.ServerMetadataRequest\x1a$.taichu_infer.ServerMetadataResponse\"\x00\x12Z\n\rModelMetadata\x12\".taichu_infer.ModelMetadataRequest\x1a#.taichu_infer.ModelMetadataResponse\"\x00\x12Q\n\nModelInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00\x12[\n\x10ModelStreamInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00(\x01\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_predict_v2.proto\x12\x0ctaichu_infer\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x93\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x42\n\x06inputs\x18\x04 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x12\x43\n\x07outputs\x18\x05 \x03(\x0b\x32\x32.taichu_infer.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xbe\x03\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x43\n\nparameters\x18\x04 \x03(\x0b\x32/.taichu_infer.ModelInferRequest.ParametersEntry\x1a\xdb\x01\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12^\n\nparameters\x18\x02 \x03(\x0b\x32J.taichu_infer.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"\xe2\x01\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x44\n\nparameters\x18\x04 \x03(\x0b\x32\x30.taichu_infer.ModelInferResponse.ParametersEntry\x1aO\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.taichu_infer.InferParameter:\x02\x38\x01\"i\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x66loat_param\x18\x02 \x01(\x02H\x00\x12\x16\n\x0cstring_param\x18\x03 \x01(\tH\x00\x42\x12\n\x10parameter_choice2\xfd\x04\n\x14GRPCInferenceService\x12Q\n\nServerLive\x12\x1f.taichu_infer.ServerLiveRequest\x1a .taichu_infer.ServerLiveResponse\"\x00\x12T\n\x0bServerReady\x12 .taichu_infer.ServerReadyRequest\x1a!.taichu_infer.ServerReadyResponse\"\x00\x12Q\n\nModelReady\x12\x1f.taichu_infer.ModelReadyRequest\x1a .taichu_infer.ModelReadyResponse\"\x00\x12]\n\x0eServerMetadata\x12#.taichu_infer.ServerMetadataRequest\x1a$.taichu_infer.ServerMetadataResponse\"\x00\x12Z\n\rModelMetadata\x12\".taichu_infer.ModelMetadataRequest\x1a#.taichu_infer.ModelMetadataResponse\"\x00\x12Q\n\nModelInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00\x12[\n\x10ModelStreamInfer\x12\x1f.taichu_infer.ModelInferRequest\x1a .taichu_infer.ModelInferResponse\"\x00(\x01\x30\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_predict_v2_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _MODELINFERREQUEST_INFERREQUESTEDOUTPUTTENSOR_PARAMETERSENTRY._options = None
@@ -56,12 +56,12 @@
   _MODELINFERREQUEST_INFERREQUESTEDOUTPUTTENSOR_PARAMETERSENTRY._serialized_end=1046
   _MODELINFERREQUEST_PARAMETERSENTRY._serialized_start=967
   _MODELINFERREQUEST_PARAMETERSENTRY._serialized_end=1046
   _MODELINFERRESPONSE._serialized_start=1130
   _MODELINFERRESPONSE._serialized_end=1356
   _MODELINFERRESPONSE_PARAMETERSENTRY._serialized_start=967
   _MODELINFERRESPONSE_PARAMETERSENTRY._serialized_end=1046
-  _INFERPARAMETER._serialized_start=1359
-  _INFERPARAMETER._serialized_end=1487
-  _GRPCINFERENCESERVICE._serialized_start=1490
-  _GRPCINFERENCESERVICE._serialized_end=2127
+  _INFERPARAMETER._serialized_start=1358
+  _INFERPARAMETER._serialized_end=1463
+  _GRPCINFERENCESERVICE._serialized_start=1466
+  _GRPCINFERENCESERVICE._serialized_end=2103
 # @@protoc_insertion_point(module_scope)
```

### Comparing `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import grpc_predict_v2_pb2 as grpc__predict__v2__pb2
+import taichu_serve.grpc_predict_v2_pb2 as grpc__predict__v2__pb2
 
 
 class GRPCInferenceServiceStub(object):
     """Inference Server GRPC endpoints.
     """
 
     def __init__(self, channel):
```

### Comparing `taichu-serve-1.0.11/model_service/log.py` & `taichu-serve-2.0.0/taichu_serve/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import sys
 from typing import Optional
 
 from flask import request, g
-from common import Local
+from taichu_serve.common import Local
 
 class JsonFormatter(logging.Formatter):
 
     def __init__(
             self,
             fmt: Optional[str] = "%(asctime)s",
             datefmt: Optional[str] = None,
```

### Comparing `taichu-serve-1.0.11/model_service/model_service.py` & `taichu-serve-2.0.0/taichu_serve/model_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import traceback
 from abc import ABCMeta, abstractmethod
 import time
 
 logger = logging.getLogger(__name__)
 
 
-class ModelService(object):
+class BaseModelService(object):
     '''ModelService wraps up all preprocessing, inference and postprocessing
     functions used by model service. It is defined in a flexible manner to
     be easily extended to support different frameworks.
     '''
     __metaclass__ = ABCMeta
 
     def __init__(self, model_path):
@@ -58,15 +58,15 @@
         -------
         Dict
             Model service signiture.
         '''
         pass
 
 
-class SingleNodeService(ModelService):
+class SingleNodeService(BaseModelService):
     '''SingleNodeModel defines abstraction for model service which loads a
     single model.
     '''
 
     def __init__(self, model_path):
         super(SingleNodeService, self).__init__(model_path)
         self._ready = False
```

### Comparing `taichu-serve-1.0.11/setup.py` & `taichu-serve-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from datetime import date
 import sys
 from setuptools import setup, find_packages
 # pylint: disable = relative-import
-import model_service
+import taichu_serve
 
 pkgs = find_packages()
 
 if __name__ == '__main__':
     name = 'taichu-serve'
 
-    requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
+    requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gevent', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='1.0.11',
+        version='2.0.0',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
         entry_points={
-            'console_scripts': ['taichu-serve = model_service.command:infer_server_start']
+            'console_scripts': ['taichu_serve = model_service.command:infer_server_start']
         },
         include_package_data=True,
         # license='Apache License Version 2.0'
     )
```

