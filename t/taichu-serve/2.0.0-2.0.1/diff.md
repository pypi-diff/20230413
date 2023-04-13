# Comparing `tmp/taichu-serve-2.0.0.tar.gz` & `tmp/taichu-serve-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.0.tar", last modified: Thu Apr 13 09:34:05 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.1.tar", last modified: Thu Apr 13 11:28:21 2023, max compression
```

## Comparing `taichu-serve-2.0.0.tar` & `taichu-serve-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409543 taichu-serve-2.0.0/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 09:34:05.409395 taichu-serve-2.0.0/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-13 09:34:05.409588 taichu-serve-2.0.0/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:33:23.000000 taichu-serve-2.0.0/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.408188 taichu-serve-2.0.0/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3325 2023-04-13 09:12:09.000000 taichu-serve-2.0.0/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)    10809 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     2077 2023-04-13 09:34:02.000000 taichu-serve-2.0.0/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-2.0.0/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3800 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2103 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409227 taichu-serve-2.0.0/taichu_serve/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.0/taichu_serve/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     5233 2023-04-13 09:13:03.000000 taichu-serve-2.0.0/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.0/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     1908 2023-04-13 06:27:18.000000 taichu-serve-2.0.0/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 09:34:05.409087 taichu-serve-2.0.0/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      587 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       56 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-13 09:34:05.000000 taichu-serve-2.0.0/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 11:28:21.083966 taichu-serve-2.0.1/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 11:28:21.083828 taichu-serve-2.0.1/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-13 11:28:21.084010 taichu-serve-2.0.1/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-13 11:28:17.000000 taichu-serve-2.0.1/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 11:28:21.082664 taichu-serve-2.0.1/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3325 2023-04-13 09:12:09.000000 taichu-serve-2.0.1/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)    10854 2023-04-13 11:14:36.000000 taichu-serve-2.0.1/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     2176 2023-04-13 11:16:26.000000 taichu-serve-2.0.1/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.1/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-2.0.1/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.1/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.1/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3800 2023-04-13 09:06:46.000000 taichu-serve-2.0.1/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2103 2023-04-13 09:06:46.000000 taichu-serve-2.0.1/taichu_serve/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 11:28:21.083653 taichu-serve-2.0.1/taichu_serve/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.1/taichu_serve/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     5233 2023-04-13 09:13:03.000000 taichu-serve-2.0.1/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.1/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     1908 2023-04-13 06:27:18.000000 taichu-serve-2.0.1/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-13 11:28:21.083518 taichu-serve-2.0.1/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      587 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       73 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       56 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-13 11:28:21.000000 taichu-serve-2.0.1/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.0/setup.py` & `taichu-serve-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gevent', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='2.0.0',
+        version='2.0.1',
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
-            'console_scripts': ['taichu_serve = model_service.command:infer_server_start']
+            'console_scripts': ['taichu_serve = taichu_serve.command:infer_server_start']
         },
         include_package_data=True,
         # license='Apache License Version 2.0'
     )
```

### Comparing `taichu-serve-2.0.0/taichu_serve/__init__.py` & `taichu-serve-2.0.1/taichu_serve/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/app.py` & `taichu-serve-2.0.1/taichu_serve/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from taichu_serve.ratelimiter import semaphore
 
 init_logger()
 
 app = Flask("aa")
 
 from taichu_serve.error_code import ModelNotFoundError, ModelPredictError
+from taichu_serve import Service
 
 LOGGER = logging.getLogger(__name__)
 
-from taichu_serve.model_server import SingleNodeService
 import multiprocessing
 
 workers_pool = multiprocessing.Queue()
 workers_status = []
 
 
 def worker_main_loop(args, pipe, status):
@@ -49,30 +49,30 @@
     model_service_file = args.service_file
 
     print(
         "model_path={} \n model_service_file={} "
         .format(model_path, model_service_file))
 
     module = load_service(os.path.join(model_path, model_service_file)
-                          ) if model_service_file else SingleNodeService
+                          ) if model_service_file else Service
     classes = [cls[1] for cls in inspect.getmembers(module, inspect.isclass)]
 
-    # assert len(classes) >= 1, \
-    #     'No valid python class derived from Base Model Service is in module file: %s' % \
-    #     model_service_file
+    assert len(classes) > 0, "There should be one user defined service derived from ModelService."
+
 
     class_defs = list(
         filter(
-            lambda c: issubclass(c, SingleNodeService) and len(
+            lambda c: issubclass(c, Service) and len(
                 c.__subclasses__()) == 0, classes))
 
     # if len(class_defs) != 1:
     #     raise Exception(
     #         'There should be one user defined service derived from ModelService.'
     #     )
+    assert len(class_defs) > 0, "There should be one user defined service derived from ModelService."
 
     for c in class_defs:
         LOGGER.info("class_defs: %s", c.__name__)
         instance = c(model_path)
         # threading.Thread(target=instance.warmup).start()
         instance.warmup()
         dict_model_service[f'{str(c.__name__).lower()}_{instance.model_version.lower()}'] = instance
@@ -185,15 +185,16 @@
 
 
 @app.before_request
 def limiter():
     if request.path == '/health/live' or request.path == '/health/ready':
         return
 
-    ok = semaphore.acquire(blocking=True, timeout=1)
+    ok = semaphore.acquire(blocking=False)
+    LOGGER.info('semaphore.acquire:{}'.format(ok))
     g.is_limited = not ok
     if not ok:
         return {'error': '请求过于频繁，请稍后再试'}, 429, {'Content-Type': 'application/json'}
 
 
 @app.after_request
 def after_request(response):
```

### Comparing `taichu-serve-2.0.0/taichu_serve/command.py` & `taichu-serve-2.0.1/taichu_serve/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # coding: utf-8
 import logging
 from concurrent import futures
 
 import grpc
-from gevent import pywsgi
 
 from taichu_serve.grpc_predict_v2_pb2_grpc import add_GRPCInferenceServiceServicer_to_server
 from taichu_serve.app import app, init_model_service_instance
 from taichu_serve.error_code import ModelNotFoundError
 from taichu_serve.grpc_server import GrpcModelService
 from taichu_serve.ratelimiter import semaphore
 from taichu_serve.settings import parse_args
 
-
 LOGGER = logging.getLogger(__name__)
 
 
 class GrpcServerInterceptor(grpc.ServerInterceptor):
     def intercept_service(self, continuation, handler_call_details):
         try:
             LOGGER.info("grpc request: %s", handler_call_details)
@@ -47,11 +45,17 @@
                          interceptors=[GrpcServerInterceptor()])
 
     add_GRPCInferenceServiceServicer_to_server(GrpcModelService(), server)
     server.add_insecure_port(f'[::]:{args.grpc_port}')
 
     server.start()
     LOGGER.info("grpc server start at port %s", args.grpc_port)
-    # server.wait_for_termination()
-    server = pywsgi.WSGIServer(('0.0.0.0', args.http_port), app)
-    server.serve_forever()
+    from gevent.pywsgi import WSGIServer
+
+    # http_server = WSGIServer(("0.0.0.0", args.http_port), app)
+    # LOGGER.info("http server start at port %s", args.http_port)
+    #
+    # http_server.serve_forever()
+
+    app.run("0.0.0.0", args.http_port)
+
     return app
```

### Comparing `taichu-serve-2.0.0/taichu_serve/common.py` & `taichu-serve-2.0.1/taichu_serve/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/error_code.py` & `taichu-serve-2.0.1/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.1/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.1/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/grpc_server.py` & `taichu-serve-2.0.1/taichu_serve/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/log.py` & `taichu-serve-2.0.1/taichu_serve/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/model_server.py` & `taichu-serve-2.0.1/taichu_serve/model_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve/settings.py` & `taichu-serve-2.0.1/taichu_serve/settings.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.0/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.1/taichu_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

