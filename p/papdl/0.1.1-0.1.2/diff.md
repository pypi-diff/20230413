# Comparing `tmp/papdl-0.1.1.tar.gz` & `tmp/papdl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papdl-0.1.1.tar", max compression
+gzip compressed data, was "papdl-0.1.2.tar", max compression
```

## Comparing `papdl-0.1.1.tar` & `papdl-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0        0 2022-11-11 10:47:23.544741 papdl-0.1.1/README.md
--rw-r--r--   0        0        0     1061 2023-03-21 15:03:13.719915 papdl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.1/src/papdl/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.1/src/papdl/backend/__init__.py
--rw-r--r--   0        0        0     4352 2023-03-14 14:05:54.816808 papdl-0.1.1/src/papdl/backend/_api_benchmark.py
--rw-r--r--   0        0        0     7490 2023-03-16 13:30:58.518090 papdl-0.1.1/src/papdl/backend/_api_deploy.py
--rw-r--r--   0        0        0     1860 2023-03-13 14:29:35.763942 papdl-0.1.1/src/papdl/backend/_api_iperf.py
--rw-r--r--   0        0        0     5476 2023-03-13 14:29:28.819841 papdl-0.1.1/src/papdl/backend/_api_registry.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.1/src/papdl/backend/_api_slice.py
--rw-r--r--   0        0        0     5428 2023-03-13 22:06:58.467846 papdl-0.1.1/src/papdl/backend/api.py
--rw-r--r--   0        0        0     6043 2023-03-14 15:45:11.300911 papdl-0.1.1/src/papdl/backend/api_common.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.197294 papdl-0.1.1/src/papdl/backend/certificates/.stub
--rw-r--r--   0        0        0     3421 2023-03-16 14:57:00.351272 papdl-0.1.1/src/papdl/backend/common.py
--rw-r--r--   0        0        0      678 2023-03-13 18:53:09.022005 papdl-0.1.1/src/papdl/backend/containers/Benchmarker/Dockerfile
--rw-r--r--   0        0        0     7120 2023-03-16 14:57:00.351272 papdl-0.1.1/src/papdl/backend/containers/Benchmarker/app/server.py
--rw-r--r--   0        0        0       83 2023-03-15 22:25:18.188731 papdl-0.1.1/src/papdl/backend/containers/Benchmarker/requirements.txt
--rw-r--r--   0        0        0      654 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/Dockerfile
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/__init__.py
--rw-r--r--   0        0        0      586 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/configure.py
--rw-r--r--   0        0        0      133 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/iss_message.proto
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/proto/__init__.py
--rw-r--r--   0        0        0     3439 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/proto/iss_message_pb2.py
--rw-r--r--   0        0        0     8875 2023-03-16 14:57:00.351272 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/server.py
--rw-r--r--   0        0        0     1708 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/wsc.py
--rw-r--r--   0        0        0       83 2023-03-14 01:19:58.405982 papdl-0.1.1/src/papdl/backend/containers/Orchestrator/requirements.txt
--rw-r--r--   0        0        0      727 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Slice/Dockerfile
--rw-r--r--   0        0        0      144 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Slice/app/iss_message.proto
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Slice/app/proto/__init__.py
--rw-r--r--   0        0        0     3439 2023-03-04 02:54:49.201294 papdl-0.1.1/src/papdl/backend/containers/Slice/app/proto/iss_message_pb2.py
--rw-r--r--   0        0        0     4435 2023-03-16 14:57:00.351272 papdl-0.1.1/src/papdl/backend/containers/Slice/app/server.py
--rw-r--r--   0        0        0       65 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/backend/containers/Slice/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/backend/registry_volume/.stub
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/benchmark/__init__.py
--rw-r--r--   0        0        0     2910 2023-03-13 22:13:53.228885 papdl-0.1.1/src/papdl/benchmark/benchmark.py
--rw-r--r--   0        0        0     2449 2023-03-16 00:16:39.355022 papdl-0.1.1/src/papdl/benchmark/main.py
--rw-r--r--   0        0        0      205 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/benchmark/network_statistics.csv
--rw-r--r--   0        0        0    16278 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/benchmark/temp.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/clean/__init__.py
--rw-r--r--   0        0        0     2726 2023-03-14 13:57:41.259652 papdl-0.1.1/src/papdl/clean/main.py
--rw-r--r--   0        0        0      517 2023-03-04 13:48:39.786023 papdl-0.1.1/src/papdl/cli.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/configure/__init__.py
--rw-r--r--   0        0        0    20440 2023-03-20 21:29:37.314023 papdl-0.1.1/src/papdl/configure/configure.py
--rw-r--r--   0        0        0     1852 2023-03-18 21:57:44.692440 papdl-0.1.1/src/papdl/configure/main.py
--rw-r--r--   0        0        0     1397 2023-03-15 18:59:16.018428 papdl-0.1.1/src/papdl/deploy/deploy.py
--rw-r--r--   0        0        0      837 2023-03-14 05:06:57.818554 papdl-0.1.1/src/papdl/deploy/main.py
--rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.1/src/papdl/slice/__init__.py
--rw-r--r--   0        0        0     1045 2023-03-14 05:05:40.213508 papdl-0.1.1/src/papdl/slice/main.py
--rw-r--r--   0        0        0     3496 2023-03-14 16:21:02.317805 papdl-0.1.1/src/papdl/slice/slice.py
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 papdl-0.1.1/setup.py
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 papdl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5820 2023-04-13 15:17:01.829502 papdl-0.1.2/README.md
+-rw-r--r--   0        0        0     1076 2023-04-13 15:19:47.324965 papdl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.2/src/papdl/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.2/src/papdl/backend/__init__.py
+-rw-r--r--   0        0        0     4352 2023-03-14 14:05:54.816808 papdl-0.1.2/src/papdl/backend/_api_benchmark.py
+-rw-r--r--   0        0        0     7490 2023-03-16 13:30:58.518090 papdl-0.1.2/src/papdl/backend/_api_deploy.py
+-rw-r--r--   0        0        0     1860 2023-03-13 14:29:35.763942 papdl-0.1.2/src/papdl/backend/_api_iperf.py
+-rw-r--r--   0        0        0     5476 2023-03-13 14:29:28.819841 papdl-0.1.2/src/papdl/backend/_api_registry.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.193294 papdl-0.1.2/src/papdl/backend/_api_slice.py
+-rw-r--r--   0        0        0     5428 2023-03-13 22:06:58.467846 papdl-0.1.2/src/papdl/backend/api.py
+-rw-r--r--   0        0        0     6043 2023-03-14 15:45:11.300911 papdl-0.1.2/src/papdl/backend/api_common.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.197294 papdl-0.1.2/src/papdl/backend/certificates/.stub
+-rw-r--r--   0        0        0     3421 2023-03-26 15:53:14.979024 papdl-0.1.2/src/papdl/backend/common.py
+-rw-r--r--   0        0        0      678 2023-03-29 00:14:03.755820 papdl-0.1.2/src/papdl/backend/containers/Benchmarker/Dockerfile
+-rw-r--r--   0        0        0     8469 2023-04-06 09:01:32.407038 papdl-0.1.2/src/papdl/backend/containers/Benchmarker/app/server.py
+-rw-r--r--   0        0        0       83 2023-03-15 22:25:18.188731 papdl-0.1.2/src/papdl/backend/containers/Benchmarker/requirements.txt
+-rw-r--r--   0        0        0      654 2023-03-26 21:46:16.116270 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/Dockerfile
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/__init__.py
+-rw-r--r--   0        0        0      586 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/configure.py
+-rw-r--r--   0        0        0      133 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/iss_message.proto
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/proto/__init__.py
+-rw-r--r--   0        0        0     3439 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/proto/iss_message_pb2.py
+-rw-r--r--   0        0        0     7342 2023-03-26 23:47:32.267154 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/server.py
+-rw-r--r--   0        0        0     1708 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/wsc.py
+-rw-r--r--   0        0        0       87 2023-03-26 09:22:31.250097 papdl-0.1.2/src/papdl/backend/containers/Orchestrator/requirements.txt
+-rw-r--r--   0        0        0      727 2023-03-29 00:14:33.456225 papdl-0.1.2/src/papdl/backend/containers/Slice/Dockerfile
+-rw-r--r--   0        0        0      144 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Slice/app/iss_message.proto
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Slice/app/proto/__init__.py
+-rw-r--r--   0        0        0     3439 2023-03-04 02:54:49.201294 papdl-0.1.2/src/papdl/backend/containers/Slice/app/proto/iss_message_pb2.py
+-rw-r--r--   0        0        0     4359 2023-04-06 12:25:14.536544 papdl-0.1.2/src/papdl/backend/containers/Slice/app/server.py
+-rw-r--r--   0        0        0       69 2023-03-26 09:22:27.426045 papdl-0.1.2/src/papdl/backend/containers/Slice/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/backend/registry_volume/.stub
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/benchmark/__init__.py
+-rw-r--r--   0        0        0     2910 2023-03-13 22:13:53.228885 papdl-0.1.2/src/papdl/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2447 2023-03-28 20:04:54.106521 papdl-0.1.2/src/papdl/benchmark/main.py
+-rw-r--r--   0        0        0      205 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/benchmark/network_statistics.csv
+-rw-r--r--   0        0        0    16278 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/benchmark/temp.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/clean/__init__.py
+-rw-r--r--   0        0        0     2726 2023-03-14 13:57:41.259652 papdl-0.1.2/src/papdl/clean/main.py
+-rw-r--r--   0        0        0      517 2023-03-04 13:48:39.786023 papdl-0.1.2/src/papdl/cli.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/configure/__init__.py
+-rw-r--r--   0        0        0    23701 2023-03-29 17:48:19.413548 papdl-0.1.2/src/papdl/configure/configure.py
+-rw-r--r--   0        0        0     1852 2023-03-22 15:26:17.080320 papdl-0.1.2/src/papdl/configure/main.py
+-rw-r--r--   0        0        0     1397 2023-03-15 18:59:16.018428 papdl-0.1.2/src/papdl/deploy/deploy.py
+-rw-r--r--   0        0        0      843 2023-04-06 09:02:00.806964 papdl-0.1.2/src/papdl/deploy/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:54:49.205294 papdl-0.1.2/src/papdl/slice/__init__.py
+-rw-r--r--   0        0        0     1045 2023-03-14 05:05:40.213508 papdl-0.1.2/src/papdl/slice/main.py
+-rw-r--r--   0        0        0     3442 2023-04-06 09:02:10.662938 papdl-0.1.2/src/papdl/slice/slice.py
+-rw-r--r--   0        0        0     8223 1970-01-01 00:00:00.000000 papdl-0.1.2/setup.py
+-rw-r--r--   0        0        0     7655 1970-01-01 00:00:00.000000 papdl-0.1.2/PKG-INFO
```

### Comparing `papdl-0.1.1/pyproject.toml` & `papdl-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "papdl"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Tamim Azmain <maat1@st-andrews.ac.uk>"]
 readme = "README.md"
 packages = [{include = "papdl", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -38,14 +38,15 @@
 coloredlogs = "^15.0.1"
 dill = "^0.3.6"
 asyncstdlib = "^3.10.5"
 pympler = "^1.0.1"
 memory-profiler = "^0.61.0"
 filprofiler = "^2023.3.0"
 tabulate = "^0.9.0"
+lz4 = "^4.3.2"
 
 [tool.poetry.scripts]
 papdl = "papdl.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `papdl-0.1.1/src/papdl/backend/_api_benchmark.py` & `papdl-0.1.2/src/papdl/backend/_api_benchmark.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/_api_deploy.py` & `papdl-0.1.2/src/papdl/backend/_api_deploy.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/_api_iperf.py` & `papdl-0.1.2/src/papdl/backend/_api_iperf.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/_api_registry.py` & `papdl-0.1.2/src/papdl/backend/_api_registry.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/api.py` & `papdl-0.1.2/src/papdl/backend/api.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/api_common.py` & `papdl-0.1.2/src/papdl/backend/api_common.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/common.py` & `papdl-0.1.2/src/papdl/backend/common.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Benchmarker/Dockerfile` & `papdl-0.1.2/src/papdl/backend/containers/Benchmarker/Dockerfile`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # USER ${local_user}
 
 ENV PATH="/home/${local_user}/.local/bin:${PATH}"
 
 RUN mkdir /home/${local_user}/model
 RUN mkdir /home/${local_user}/app
 WORKDIR /home/${local_user}/app
-COPY models /home/${local_user}/models
 RUN chmod 777 /home/${local_user}/app
 
-ADD app /home/${local_user}/app
-
 # FORWARD INPUT
 EXPOSE 8765
 
 COPY requirements.txt requirements.txt
 
 RUN pip install --user --upgrade pip
-RUN pip install --user --no-cache-dir -r requirements.txt
+RUN pip install --user --no-cache-dir -r requirements.txt
+
+ADD app /home/${local_user}/app
+COPY models /home/${local_user}/models
```

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Benchmarker/app/server.py` & `papdl-0.1.2/src/papdl/backend/containers/Benchmarker/app/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,78 +23,91 @@
     model_test_batch_size: int
     bandwidth_test_duration_sec: int
     latency_test_count: int
     free_memory_multiplier:float
 
 config: Config
 
-INPUT_MULTIPLIER = 10
-# def load_benchmark_configs()->Config:
-#     # TODO: read from environment variables
-#     global config
-#     config = Config(
-#         model_test_batch_size=100,
-#         model_test_number_of_repeats=100,
-#         bandwidth_test_duration_sec=1,
-#         latency_test_count=1000,
-#         free_memory_multiplier = 0.5)
+INPUT_MULTIPLIER = 6
+
 
 def load_benchmark_configs()->Config:
     global config
     config = Config(
         model_test_batch_size=int(environ.get("MODEL_TEST_BATCH_SIZE")),
         model_test_number_of_repeats=int(environ.get("MODEL_TEST_NUMBER_OF_REPEATS")),
         bandwidth_test_duration_sec=int(environ.get("BANDWIDTH_TEST_DURATION_SEC")),
         latency_test_count=int(environ.get("LATENCY_TEST_COUNT")),
         free_memory_multiplier=float(environ.get("FREE_MEMORY_MULTIPLIER"))
     )
-    
 
 def isDebug()->bool:
     return int(environ.get("DEBUG")) == 1
 
 
 
 def get_available_memory():
     return psutil.virtual_memory().free
 
-# https://gist.github.com/jamesmishra/34bac09176bc07b1f0c33886e4b19dc7
-def memory_usage(model, *, batch_size: int):
+def model_memory_usage(model, *, batch_size:int):
     default_dtype = tf.keras.backend.floatx()
     shapes_mem_count = 0
     internal_model_mem_count = 0
     for layer in model.layers:
         if isinstance(layer, tf.keras.Model):
-            internal_model_mem_count += memory_usage(
+            internal_model_mem_count += model_memory_usage(
                 layer, batch_size=batch_size
             )
         single_layer_mem = tf.as_dtype(layer.dtype or default_dtype).size
         out_shape = layer.output_shape
         if isinstance(out_shape, list):
             out_shape = out_shape[0]
         for s in out_shape:
             if s is None:
                 continue
             single_layer_mem *= s
-        shapes_mem_count += single_layer_mem
+        shapes_mem_count += single_layer_mem 
 
     trainable_count = sum(
         [tf.keras.backend.count_params(p) for p in model.trainable_weights]
     )
     non_trainable_count = sum(
         [tf.keras.backend.count_params(p) for p in model.non_trainable_weights]
     )
+    return trainable_count + non_trainable_count
 
-    total_memory = (
-        batch_size * shapes_mem_count * INPUT_MULTIPLIER
+def hidden_layer_input_usage(model, *, batch_size: int):
+    default_dtype = tf.keras.backend.floatx()
+    shapes_mem_count = 0
+    internal_model_mem_count = 0
+    for layer in model.layers:
+        if isinstance(layer, tf.keras.Model):
+            internal_model_mem_count += hidden_layer_input_usage(
+                layer, batch_size=batch_size
+            )
+        single_layer_mem = tf.as_dtype(layer.dtype or default_dtype).size
+        out_shape = layer.output_shape
+        if isinstance(out_shape, list):
+            out_shape = out_shape[0]
+        for s in out_shape:
+            if s is None:
+                continue
+            single_layer_mem *= s
+        shapes_mem_count += single_layer_mem
+    
+    return (
+        batch_size * shapes_mem_count
         + internal_model_mem_count
-        # + trainable_count
-        # + non_trainable_count
     )
-    return total_memory
+
+def get_input_memory_multiplier(dimensions):
+    return np.prod(np.array(dimensions)) * INPUT_MULTIPLIER
+
+def total_memory_usage(model,dimensions, *, batch_size:int):
+    return model_memory_usage(model,batch_size=batch_size) + hidden_layer_input_usage(model,batch_size=batch_size) + get_input_memory_multiplier(dimensions)
 
 def load_network_benchmark_ips() -> List[str]:
     target_networks = environ.get("PAPDL_WORKERS").split(" ")
     print(target_networks,flush=True)
     return target_networks
 
 def get_available_memory():
@@ -129,83 +142,106 @@
                 "rtt_max_ms": r_ping.rtt_max_ms
             }
         }
         print(result[ip],flush=True)
         del client
     return result
 
+    
 def single_model_benchmark(args:Dict):
     mp = args["mp"]
     fmm = args["fmm"]
     mtbs = args["mtbs"]
+    mtnor = args["mtnor"]
     
-
     free_memory = get_available_memory()
     model:tf.keras.Model = load_model(mp)
-    model_memory_usage = memory_usage(model=model,batch_size=config["model_test_batch_size"])
     model_name = model.name
     dimensions = (mtbs,) + model.input_shape[1:]
-    print(f"Loaded model : {model_name} from path: {mp} with input_dims: {dimensions}",flush=True)
+    total = total_memory_usage(model=model,dimensions=dimensions, batch_size=mtbs)
+    print(f"Loaded model: {model_name} from path: {mp} with input_dims: {dimensions}",flush=True)
     
-    if(model_memory_usage > free_memory * fmm):
-        print(f"Skipping benchmarking as memory threshold {model_memory_usage} has been met {free_memory}.",flush=True)
+    if(total > free_memory * fmm):
+        print(f"Skipping benchmarking as memory threshold {total} has met {free_memory}.",flush=True)
+
         result = {}
+
         result["benchmark_size"] = float("inf")
         result["benchmark_time"] = float("inf")
-        result["benchmark_memory_usage"] = model_memory_usage
+
+        result["benchmark_model_memory_usage"] = model_memory_usage(model,batch_size=mtbs)
+        result["benchmark_hidden_and_input_memory_usage"] = hidden_layer_input_usage(model,batch_size=mtbs)
+        result["benchmark_input_memory_multiplier"] = get_input_memory_multiplier(dimensions)
         result["model_name"] = model_name
+
         del model
         tf.compat.v1.reset_default_graph()
         gc.collect()
         return result
-
-    print(f"Running benchmarking as memory threshold {free_memory} has not been met for model {model_memory_usage}")
+        
+    print(f"Running benchmarking as memory threshold {free_memory} has not been met for mode {total}")
     sample_input = np.random.random_sample(dimensions)
     start = time()
-    for i in range(mtbs):
+    for i in range(mtnor):
         tmp_out = model(sample_input,training=False)
         del tmp_out
         gc.collect()
     end = time()
-    
-    output:np.array = model(sample_input,training = False)
-    # file_name = f"fsize_{str(uuid.uuid4())}"
-    # np.save(file_name,"output")
-    
-    # size = stat(f"{file_name}.npy").st_size
+    output:np.ndarray = model(sample_input,training=False)
     size = asizeof(output)
+
     result = {}
+
     result["benchmark_size"] = size
     result["benchmark_time"] = (end - start) / mtbs
-    result["benchmark_memory_usage"] = model_memory_usage
+
+    result["benchmark_model_memory_usage"] = model_memory_usage(model,batch_size=mtbs)
+    result["benchmark_hidden_and_input_memory_usage"] = hidden_layer_input_usage(model,batch_size=mtbs)
+    result["benchmark_input_memory_multiplier"] = get_input_memory_multiplier(dimensions)
+
     result["model_name"] = model_name
 
     del model
     del output
     del sample_input
     tf.compat.v1.reset_default_graph()
+    gc.collect()
     return result
     
 
 
 def benchmark_models(model_paths=model_paths):
     global config
     result = {}
     with contextlib.closing(Pool(1)) as po:
         pool_args = []
         for mp in model_paths:
-            pool_args.append({"mp":mp, "fmm":config["free_memory_multiplier"], "mtbs": config["model_test_batch_size"]})
+            pool_args.append(
+                {
+                    "mp":mp, 
+                    "fmm":config["free_memory_multiplier"], 
+                    "mtbs": config["model_test_batch_size"],
+                    "mtnor": config["model_test_number_of_repeats"]
+                }
+            )
 
         pool_result = po.map_async(single_model_benchmark, pool_args)
         completed_pool_results = pool_result.get()
         for r in completed_pool_results:
             result[r["model_name"]] = {}
+
             result[r["model_name"]]["benchmark_size"] = r["benchmark_size"]
+
             result[r["model_name"]]["benchmark_time"] = r["benchmark_time"]
-            result[r["model_name"]]["benchmark_memory_usage"] = r["benchmark_memory_usage"]
+
+            result[r["model_name"]]["benchmark_model_memory_usage"] = r["benchmark_model_memory_usage"]
+
+            result[r["model_name"]]["benchmark_hidden_and_input_memory_usage"] = r["benchmark_hidden_and_input_memory_usage"]
+
+            result[r["model_name"]]["benchmark_input_memory_multiplier"] = r["benchmark_input_memory_multiplier"]
     return result
         
 
 load_benchmark_configs()
 print(f"Loaded config: {config}",flush=True)
 benchmark_result = {"free_memory": get_available_memory()}
 benchmark_result["network_performance"] = benchmark_network(papdl_workers=papdl_workers)
```

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Orchestrator/Dockerfile` & `papdl-0.1.2/src/papdl/backend/containers/Orchestrator/Dockerfile`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 USER ${local_user}
 ENV PATH="/home/${local_user}/.local/bin:${PATH}"
 
 RUN mkdir /home/${local_user}/app
 WORKDIR /home/${local_user}/app
 
-ADD app /home/${local_user}/app
 
 # FORWARD INPUT
 EXPOSE 8765
 
 COPY requirements.txt requirements.txt
 RUN pip install --user --upgrade pip
-RUN pip install --user --no-cache-dir -r requirements.txt
+RUN pip install --user --no-cache-dir -r requirements.txt
+ADD app /home/${local_user}/app
```

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/configure.py` & `papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/configure.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/proto/iss_message_pb2.py` & `papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/proto/iss_message_pb2.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/server.py` & `papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 import logging
 import asyncio
 import traceback
 from asyncio import Future
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = '3'
 import uuid
 import requests
-from sanic.log import logger
 import aiohttp
 import uproot
 from time import time_ns
 import asyncstdlib as asynclib
+import lz4.frame
+from sanic.log import logger
 
 from websockets.legacy.client import Connect
 
 from sanic import Request,Websocket,Sanic
 from sanic import response
 
 
@@ -74,109 +75,68 @@
 app.config.RESPONSE_TIMEOUT = sys.maxsize
 
 # request_response_map:Dict[str,Future] = {}
 # rrm_lock = asyncio.Lock()
 @app.websocket("/predict")
 async def record_response(request:Request,ws:Websocket):
     async for data in ws:
+        logger.info("RECEIVED PREDICT!")
         requestId:str
         try:
-            buff = io.BytesIO()
-            buff.write(data)
-            buff.seek(0)
-            uproot_buff = uproot.open(buff)
-            requestId = str(uproot_buff["requestId"])
-            output = uproot_buff["data"]["array"].array(library="np")
+            decompressed_buff = io.BytesIO()
+            decompressed_buff.write(lz4.frame.decompress(data))
+            decompressed_buff.seek(0)
+            requestId = decompressed_buff.read(36).decode("utf-8")
+            logger.info("DECOMPRESSED!")
+            logger.info(requestId)
+            # data = np.load(decompressed_buff)
+            # logger.info("LOADED!")
+            # logger.info(data.shape)
             async with app.ctx.rrm_lock:
-                app.ctx.request_response_map[requestId].set_result(output)
+                app.ctx.request_response_map[requestId].set_result(decompressed_buff.read())
         except Exception as e:
             logger.error(traceback.format_exc())
             async with app.ctx.rrm_lock:
                 app.ctx.request_response_map[requestId].set_exception(e)
 
 @app.post("/input")
 async def make_prediction(request:Request):
+    logger.info("INPUT REQUEST!")
     try:
         request_buff = io.BytesIO()
         request_buff.write(request.body)
         request_buff.seek(0)
         array:np.ndarray = np.load(request_buff)
         expected_input_dims = app.ctx.input_dims
 
         if len(expected_input_dims) + 1 != len(array.shape) or array.shape[1:] != expected_input_dims:
             raise ValueError()
         
         send_buff = io.BytesIO()
-        uproot_buff = uproot.recreate(send_buff)
         request_id = str(uuid.uuid4())
-        uproot_buff["requestId"] = request_id
-        uproot_buff["data"] = {"array":array}
+        send_buff.write(bytes(request_id,"utf-8"))
+        send_buff.write(request.body)
         send_buff.seek(0)
+        
+        
         loop = asyncio.get_running_loop()
         response_future = loop.create_future()
         async with app.ctx.rrm_lock:
             app.ctx.request_response_map[request_id] = response_future
-        await app.ctx.forward_connection.send(uproot_buff)
+        await app.ctx.forward_connection.send(lz4.frame.compress(send_buff.read()))
+        logger.info("WAITING!")
         await response_future
-        
-        response_buff = io.BytesIO()
-        np.save(response_buff,response_future.result())
-        response_buff.seek(0)
-        return response.raw(body=response_buff,status=HTTPStatus.OK)
+        return response.raw(body=response_future.result(), status = HTTPStatus.OK)
     except ValueError as e:
+        logger.error(traceback.format_exc())
         return response.raw(body="Input dimensions does not match the model",status=HTTPStatus.BAD_REQUEST)
     except Exception as e:
+        logger.error(traceback.format_exc())
         return response.json(body=e,status=HTTPStatus.INTERNAL_SERVER_ERROR)
 
-@app.post("/benchmark")
-async def benchmark_performance(request:Request):
-    try:
-        input_shape = app.ctx.input_dims
-        batch_size = int(request.json["batch_size"])
-        iterations = int(request.json["iterations"])
-
-        dimensions = (batch_size,) + input_shape
-        
-        loop = asyncio.get_running_loop()
-        benchmark_results = [(
-            str(uuid.uuid4()), 
-            np.random.random_sample(dimensions),
-            loop.create_future()
-            ) for i in range(iterations)]
-
-        req_id:str
-        sample:np.ndarray
-        duration_fut:asyncio.Future
-        async for i,(req_id, sample, duration_fut) in asynclib.enumerate(benchmark_results):
-            buff = io.BytesIO()
-            uproot_buff = uproot.recreate(buff)
-            uproot_buff["requestId"] = req_id
-            uproot_buff["data"] = {"array":sample}
-            buff.seek(0)
-            _loop = asyncio.get_running_loop()
-            response_future = _loop.create_future()
-            async with app.ctx.rrm_lock:
-                app.ctx.request_response_map[req_id] = response_future
-
-            begin = time_ns()
-            await app.ctx.forward_connection.send(buff)
-            await response_future
-            end = time_ns()
-            duration_fut.set_result(end - begin)
-        
-        durations_completed = []
-        for br in benchmark_results:
-            await br[2]
-            durations_completed.append(br[2].result())
-
-        return response.json(body=durations_completed,status=HTTPStatus.OK)
-    except KeyError as e:
-        return response.text("Bad request. Missing batch_size or iterations arguments",status=HTTPStatus.BAD_REQUEST)
-    except Exception as e:
-        return response.text(body=traceback.format_exc(),status=HTTPStatus.INTERNAL_SERVER_ERROR)
     
 @app.get("/connect")
 async def connect_to_forward(request:Request):
     try:
         app.ctx.forward_connection:Connect = await ws_connect(f"{app.ctx.forward_url}/predict", max_size=sys.maxsize)
         logger.info(f"Successfly connected to forward_url: {app.ctx.forward_url}")
         return response.text("Successfully connected to  forward url",status=HTTPStatus.OK)
@@ -228,8 +188,8 @@
         return response.json(result,status=HTTPStatus.OK)
     except Exception:
         logger.error(traceback.format_exc())
         return response.text(body="Failed to fetch health check for one or more workers. Perhaps connections have not been established yet. Run http://\{orchestrator_ip\}:8765/activateworkers",status=HTTPStatus.BAD_REQUEST)
 
 
 if __name__ == "__main__":
-    app.run(host=CURR_HOST,port=8765,access_log=True)
+    app.run(host=CURR_HOST,port=8765,access_log=True,debug=True)
```

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Orchestrator/app/wsc.py` & `papdl-0.1.2/src/papdl/backend/containers/Orchestrator/app/wsc.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Slice/Dockerfile` & `papdl-0.1.2/src/papdl/backend/containers/Slice/Dockerfile`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 USER ${local_user}
 ENV PATH="/home/${local_user}/.local/bin:${PATH}"
 
 RUN mkdir /home/${local_user}/model
 RUN mkdir /home/${local_user}/app
 WORKDIR /home/${local_user}/app
 
-ADD app /home/${local_user}/app
 
 # FORWARD INPUT
 EXPOSE 8765
 
 COPY requirements.txt requirements.txt
 RUN pip install --user --upgrade pip
 RUN pip install --user --no-cache-dir -r requirements.txt
+ADD app /home/${local_user}/app
 COPY model /home/${local_user}/model
```

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Slice/app/proto/iss_message_pb2.py` & `papdl-0.1.2/src/papdl/backend/containers/Slice/app/proto/iss_message_pb2.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/backend/containers/Slice/app/server.py` & `papdl-0.1.2/src/papdl/backend/containers/Slice/app/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import sys
 from time import sleep
 import os
 import json
+import lz4.frame
 
 
 from websockets.client import connect as ws_connect
 from websockets.server import serve as ws_serve
 from websockets.datastructures import Headers,HeadersLike
 from http import HTTPStatus
 
@@ -16,15 +17,14 @@
 import logging
 import asyncio
 from keras.models import load_model
 from keras import Model
 import getpass
 import traceback
 import uproot
-import gc
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = '3'
 
 def isDebug()->bool:
     return int(os.environ.get("DEBUG")) == 1
 
 
@@ -62,29 +62,28 @@
 
 print("UPROOT SERIALIZATION")
 
 async def forward(websocket):
     async for data in websocket:
         try:
             input_buff = io.BytesIO()
-            input_buff.write(data)
+            input_buff.write(lz4.frame.decompress(data))
             input_buff.seek(0)
 
-            input_uproot_buff = uproot.open(input_buff)
-            model_input = input_uproot_buff["data"]["array"].array(library="np")
-            model_output = model.predict(model_input)
-            
-            output_buff = io.BytesIO()
-            output_uproot_buff = uproot.recreate(output_buff)
-            output_uproot_buff["data"] = {"array":model_output}
-            output_uproot_buff["requestId"] = str(input_uproot_buff["requestId"])
+            requestId = input_buff.read(36).decode("utf-8")
+            model_output = model.predict(np.load(input_buff))
 
+            output_buff = io.BytesIO()
+            output_buff.write(bytes(requestId,"utf-8"))
+            np.save(output_buff, model_output)
             output_buff.seek(0)
-            await forward_connection.send(output_buff)
-            gc.collect()
+
+            print("SENDING!",flush=True)
+            await forward_connection.send(lz4.frame.compress(output_buff.read()))
+            print("SENT!",flush=True)
         except:
             logger.error("Caught Exception! Dropping input...")
             logger.error(traceback.format_exc())
 
 async def process_request(path:str,request_headers:Headers)->Optional[Tuple[HTTPStatus,HeadersLike,bytes]]:
     global forward_connection
     global forward_url
```

### Comparing `papdl-0.1.1/src/papdl/benchmark/benchmark.py` & `papdl-0.1.2/src/papdl/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/benchmark/main.py` & `papdl-0.1.2/src/papdl/benchmark/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 @click.argument("sliced_model_path")
 @click.option("-n","--project_name",type=str,default="debug")
 @click.option("-o","--output",type=str)
 @click.option("-i","--service_idle_detection",type=int,default=6000)
 @click.option("-s","--startup_timeout",type=int,default=6000)
 
 @click.option("-b","--model_test_batch_size",type=int,default=1)
-@click.option("-r","--model_test_number_of_repeats",type=int,default=100)
+@click.option("-r","--model_test_number_of_repeats",type=int,default=10)
 @click.option("-d","--bandwidth_test_duration_sec",type=int,default=1)
-@click.option("-l","--latency_test_count",type=int,default=1000)
-@click.option("-m","--free_memory_multiplier",type=float,default=0.9)
+@click.option("-l","--latency_test_count",type=int,default=100)
+@click.option("-m","--free_memory_multiplier",type=float,default=0.8)
 #TODO: search constraints
 def benchmark(
     sliced_model_path:str,
     project_name:str,
     output:str,
     service_idle_detection:int,
     startup_timeout:int,
```

### Comparing `papdl-0.1.1/src/papdl/benchmark/temp.py` & `papdl-0.1.2/src/papdl/benchmark/temp.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/clean/main.py` & `papdl-0.1.2/src/papdl/clean/main.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/cli.py` & `papdl-0.1.2/src/papdl/cli.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/configure/configure.py` & `papdl-0.1.2/src/papdl/configure/configure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from logging import Logger
 from typing import NamedTuple, List, Dict, TypedDict, Union, Tuple, MutableSet
 from json import loads, dumps
 import heapq
 import keras
-from ..backend.common import PapdlException,BenchmarkPreferences
+from ..backend.common import PapdlException, BenchmarkPreferences
 import logging
 import re
 from tabulate import tabulate
+from tqdm import tqdm
+import math
+import pickle
+import psutil
+import gc
+from time import sleep
 
 
 class Layer():
-    def __init__(self, name,memory_usage):
+    def __init__(self, name, model_memory_usage, hidden_memory_usage, io_memory_usage):
         self.name = name
-        self.memory_usage = memory_usage
+        self.model_memory_usage = model_memory_usage
+        self.hidden_memory_usage = hidden_memory_usage
+        self.io_memory_usage = io_memory_usage
 
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, other: "Layer"):
         if other is None:
             return False
@@ -25,15 +33,15 @@
         return other.name == self.name
 
     def __str__(self):
         return self.name
 
 
 class Worker():
-    def __init__(self, name,free_memory):
+    def __init__(self, name, free_memory):
         self.name = name
         self.free_memory = free_memory
 
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, other: "Worker"):
@@ -44,120 +52,145 @@
         return other.name == self.name
 
     def __str__(self):
         return self.name
 
 
 class SearchConstraints():
-    def __init__(self,layer_must_be_in_device:Dict[Layer,Worker],layer_must_not_be_in_device:Dict[Layer,Worker]):
-        self.layer_must_be_in_device:Dict[Layer,Worker] = layer_must_be_in_device
-        self.layer_must_not_be_in_device:Dict[Layer,Worker] = layer_must_not_be_in_device
-    
+    def __init__(self, layer_must_be_in_device: Dict[Layer, Worker], layer_must_not_be_in_device: Dict[Layer, Worker]):
+        self.layer_must_be_in_device: Dict[Layer,
+                                           Worker] = layer_must_be_in_device
+        self.layer_must_not_be_in_device: Dict[Layer,
+                                               Worker] = layer_must_not_be_in_device
+
     @staticmethod
-    def parse_match(match:str)->Dict[str,List[str]]:
+    def parse_match(match: str) -> Dict[str, List[str]]:
         result = {}
         if match is not None:
             conditions = match.split(",")
             for key_val in conditions:
                 split_key_val = key_val.split(":")
                 key = split_key_val[0].strip()
                 val = split_key_val[1].strip()
                 result[key] = val
         return result
-    
-    def __getitem__(self,item):
+
+    def __getitem__(self, item):
         if item == "layer_must_be_in_device":
             return self.layer_must_be_in_device
         if item == "layer_must_not_be_in_device":
             return self.layer_must_not_be_in_device
         raise KeyError
-    
+
     def __str__(self):
         return f"must={self.layer_must_be_in_device},mustnot={self.layer_must_not_be_in_device}"
-    
+
     @staticmethod
-    def coarsce_type(dict_to_coersce:Dict[str,str])->Dict[Layer,Worker]:
-        result:Dict[Layer,Worker] = {}
-        for layer_str,worker_str in dict_to_coersce.items():
-            result[Layer(name=layer_str,memory_usage=None)] = Worker(name=worker_str,free_memory=None)
+    def coarsce_type(dict_to_coersce: Dict[str, str]) -> Dict[Layer, Worker]:
+        result: Dict[Layer, Worker] = {}
+        for layer_str, worker_str in dict_to_coersce.items():
+            result[Layer(name=layer_str, model_memory_usage=None,hidden_memory_usage=None,io_memory_usage=None)] = Worker(
+                name=worker_str, free_memory=None)
         return result
-    
+
     @staticmethod
-    def parse_from_str(input_str:str):
+    def parse_from_str(input_str: str):
         try:
-            must_str = re.search(r"(?<=must=\{)(\w|\s|:|,)+(?=\})",input_str)
-            mustnot_str = re.search(r"(?<=mustnot=\{)(\w|\s|:|,)+(?=\})",input_str)
-            
-            layer_must_be_in_device:Dict[Layer,Worker] = {}
-            if(must_str is not None):
-                layer_must_be_in_device_str_dict = SearchConstraints.parse_match(must_str.group())
-                layer_must_be_in_device = SearchConstraints.coarsce_type(layer_must_be_in_device_str_dict)
-            
-            layer_must_not_be_in_device:Dict[Layer,Worker] = {}
-            if(mustnot_str is not None):
-                layer_must_not_be_in_device_str_dict = SearchConstraints.parse_match(mustnot_str.group())
-                layer_must_not_be_in_device = SearchConstraints.coarsce_type(layer_must_not_be_in_device_str_dict)
-            
-            return SearchConstraints(layer_must_be_in_device=layer_must_be_in_device,layer_must_not_be_in_device=layer_must_not_be_in_device)
-                
+            must_str = re.search(r"(?<=must=\{)(\w|\s|:|,)+(?=\})", input_str)
+            mustnot_str = re.search(
+                r"(?<=mustnot=\{)(\w|\s|:|,)+(?=\})", input_str)
+
+            layer_must_be_in_device: Dict[Layer, Worker] = {}
+            if (must_str is not None):
+                layer_must_be_in_device_str_dict = SearchConstraints.parse_match(
+                    must_str.group())
+                layer_must_be_in_device = SearchConstraints.coarsce_type(
+                    layer_must_be_in_device_str_dict)
+
+            layer_must_not_be_in_device: Dict[Layer, Worker] = {}
+            if (mustnot_str is not None):
+                layer_must_not_be_in_device_str_dict = SearchConstraints.parse_match(
+                    mustnot_str.group())
+                layer_must_not_be_in_device = SearchConstraints.coarsce_type(
+                    layer_must_not_be_in_device_str_dict)
+
+            return SearchConstraints(layer_must_be_in_device=layer_must_be_in_device, layer_must_not_be_in_device=layer_must_not_be_in_device)
+
         except Exception as e:
             raise ValueError
 
 
 class SliceBlock(NamedTuple):
     layers: List[Layer]
     slice_index: Tuple[int, int]
     device: Worker
-    model:keras.models.Model
+    model: keras.models.Model
 
 
 class Configuration(TypedDict):
     slices: List[Layer]
     blocks: List[SliceBlock]
     devices: List[Worker]
     constraints: SearchConstraints
-    source_device:Worker
+    source_device: Worker
     input_shape: Tuple[int]
-    benchmark_preferences:BenchmarkPreferences
-    penalty:float
-    
+    benchmark_preferences: BenchmarkPreferences
+    penalty: float
+
+
 class ConfigurationPreferences(TypedDict):
     logger: logging.Logger
-    search_constraints:SearchConstraints
-
+    search_constraints: SearchConstraints
 
 
 class Configurer():
 
     def __init__(self, logger: Logger):
         self.logger = logger
-    
-    def tabulated_print(self,configuration:Configuration):
-        slice_blocks:List[SliceBlock]  = configuration["blocks"]
-        
+
+    def tabulated_print(self, configuration: Configuration):
+        slice_blocks: List[SliceBlock] = configuration["blocks"]
+        # print(slice_blocks)
+
         table = []
-        table.append(["Slice Indices","Device","Intermediary Memory Usage (MB)"])
-        sb:SliceBlock
+        table.append(["Slice Indices", "Device", "Device Free Memory (MB)", "Model Memory Usage (MB)",
+                     "Hidden Layer Memory Usage (MB)", "IO Memory Usage (MB)"])
+        sb: SliceBlock
         for sb in slice_blocks:
-            table.append([str(sb.slice_index),sb.device.name,sum([l.memory_usage/1000/1000 for l in sb.layers])])
-        self.logger.info(tabulate(table,headers="firstrow",tablefmt="outline"))
+            table.append(
+                [str(sb.slice_index),
+                 sb.device.name,
+                 sb.device.free_memory / 1_000_000 * configuration["benchmark_preferences"]["free_memory_multiplier"],
+                 sum([
+                     l.model_memory_usage
+                     for l in sb.layers
+                 ]) / 1_000_000,
+                 sum([
+                     l.hidden_memory_usage
+                     for l in sb.layers
+                 ]) / 1_000_000,
+                 sb.layers[0].io_memory_usage / 1_000_000
+                 ]
+            )
+        self.logger.info(
+            "\n" + tabulate(table, headers="firstrow", tablefmt="outline"))
         self.logger.info(f"PENALTY: {configuration['penalty']}")
 
     class DecisionNode():
         def __init__(self,
                      model: Layer = None,
                      device: Worker = None,
                      paths: List["Configurer.Path"] = []):
             self.model: Layer = model
             self.device: Worker = device
             self.paths: List[Configurer.Path] = paths
 
         def __lt__(self, other):
             return False
-
+        
         def __hash__(self) -> int:
             if self.model is None:
                 return hash("NULL" + "-" + self.device.name)
             else:
                 return hash(self.model.name + "-" + self.device.name)
 
         def __eq__(self, other: "Configurer.DecisionNode") -> bool:
@@ -192,113 +225,149 @@
             return f"<NODE model:{model_name} device:{self.device.name} children=[\n{self.__str_children()}]>"
 
         def __str__(self) -> str:
             model_name = "NULL" if self.model is None else self.model.name
             return f"<NODE model:{model_name} device:{self.device.name}>"
 
     class Path():
-        def __init__(self,node:"Configurer.DecisionNode",penalty:float):
+        def __init__(self, node: "Configurer.DecisionNode", penalty: float):
             self.node = node
             self.penalty = penalty
-        
-        def __eq__ (self, other:"Configurer.Path"):
-            return isinstance(other,Configurer.Path) and other.penalty == self.penalty
-        
-        def __lt__ (self, other:"Configurer.Path"):
-            return isinstance(other,Configurer.Path) and other.penalty < self.penalty
-    
+
+        def __eq__(self, other: "Configurer.Path"):
+            return isinstance(other, Configurer.Path) and other.penalty == self.penalty
+
+        def __lt__(self, other: "Configurer.Path"):
+            return isinstance(other, Configurer.Path) and other.penalty < self.penalty
 
     class OptimalPath(NamedTuple):
         path: List["Configurer.DecisionNode"]
         penalty: float
 
     class SearchStatus(NamedTuple):
         total_distance: float
         path: "Configurer.Path"
 
-    def __valid_path(path: List[DecisionNode], constraints: SearchConstraints,benchmark_pref:BenchmarkPreferences):
+    def __valid_path(path: List[DecisionNode], constraints: SearchConstraints, benchmark_pref: BenchmarkPreferences):
         node: Configurer.DecisionNode
         for node in path:
             for model, device in constraints["layer_must_be_in_device"].items(
             ):
                 if model == node.model and device != node.device:
                     return False
 
         node: Configurer.DecisionNode
         for node in path:
-            for model, device in constraints["layer_must_not_be_in_device"].items(
-            ):
+            for model, device in constraints["layer_must_not_be_in_device"].items():
                 if model == node.model and device == node.device:
                     return False
-                
+
         node: Configurer.DecisionNode
-        node_memory_usage:Dict[Worker,int] = {}
+        worker_memory_usage: Dict[Worker, int] = {}
+        prevNode = path[0]
         for node in path:
-            if node.device not in node_memory_usage.keys():
-                node_memory_usage[node.device] = 0
+            if node.device not in worker_memory_usage.keys():
+                worker_memory_usage[node.device] = 0
             if node.model is None:
                 continue
-            node_memory_usage[node.device]+=node.model.memory_usage
-            
-            for worker,nmu in node_memory_usage.items():
-                if nmu > worker.free_memory * benchmark_pref["free_memory_multiplier"]:
+            worker_memory_usage[node.device] += node.model.model_memory_usage + \
+                node.model.hidden_memory_usage
+
+            if node.device != prevNode:
+                worker_memory_usage[node.device] += node.model.io_memory_usage
+                prevNode = node.device
+
+            for worker, memory_usage in worker_memory_usage.items():
+                if memory_usage > worker.free_memory * benchmark_pref["free_memory_multiplier"]:
                     return False
         return True
 
+    def __jumps(path: List[DecisionNode]):
+        jump_count = 0
+        prev_device: Worker = path[0].device
+        n: Configurer.DecisionNode
+        for n in path[1:]:
+            if n.device != prev_device:
+                jump_count += 1
+                prev_device = n.device
+
+        return jump_count
+
+    def __free_memory_variance(path: List[DecisionNode]):
+        node: Configurer.DecisionNode
+        worker_memory_usage: Dict[Worker, int] = {}
+
+        prevDevice:Worker = path[0].device
+        for node in path:
+            if node.device not in worker_memory_usage.keys():
+                worker_memory_usage[node.device] = 0
+            if node.model is None:
+                continue
+            worker_memory_usage[node.device] += node.model.model_memory_usage + node.model.hidden_memory_usage
+            if(prevDevice != node.device):
+                worker_memory_usage[node.device] += node.model.io_memory_usage
+                
+
+        average = [memory_usage / worker.free_memory for worker,
+                   memory_usage in worker_memory_usage.items()]
+
+        variance = sum([
+            (memory_usage / worker.free_memory - avg)
+            for avg, (worker, memory_usage)
+            in zip(
+                average,
+                worker_memory_usage.items())
+        ]) / len(worker_memory_usage)
+        return variance
+
     def __find_shortest_loop(
         start_node: DecisionNode,
         constraints: SearchConstraints,
-        benchmark_pref: BenchmarkPreferences
+        benchmark_pref: BenchmarkPreferences,
+        depth: int,
+        width: int
     ) -> Union[OptimalPath, None]:
-        # visited = {start_node: [start_node]}
-        # queue = [(0,Configurer.Path(node=start_node, penalty=0))]
-        # while queue:
-        #     total_penalty, path = heapq.heappop(queue)
-        #     current_node = path.node
-        #     for child_path in current_node.paths:
-        #         child_node = child_path.node
-        #         if child_node not in visited:
-        #             new_path = visited[current_node] + [child_node]
-        #             if Configurer.__valid_path(
-        #                 path = new_path,
-        #                 constraints=constraints,
-        #                 benchmark_pref=benchmark_pref
-        #             ):
-        #                 visited[child_node] = new_path
-        #                 new_penalty = total_penalty + child_path.penalty
-        #                 heapq.heappush(queue, (new_penalty, Configurer.Path(node=child_node, penalty=new_penalty)))
-        #             elif child_node == start_node and len(visited[current_node]) > 1:
-        #                 return Configurer.OptimalPath(
-        #                     path = visited[current_node] + [start_node], penalty=child_path.penalty
-        #                 )
-        # return None
         visited = set()
         queue = [(0, start_node, [], visited)]
-        while queue:
-            penalty:float
-            current_node:Configurer.DecisionNode
-            traversed_nodes:List[Configurer.DecisionNode]
-            visited:MutableSet
-            
-            penalty, current_node, traversed_nodes, visited = heapq.heappop(queue)
-            # print("PENALTY", penalty, "CURRENT_NODE", str(current_node), "TRAVERSED NODES", [str(n) for n in traversed_nodes], "VISITED NODES", [ str(n) for n in visited])
-            # print("="*20)
-            
-            if current_node in visited and current_node == start_node:
-                return Configurer.OptimalPath(path=traversed_nodes,penalty=penalty)
-
-            if current_node not in visited:
-                visited.add(current_node)
-                traversed_nodes = traversed_nodes + [current_node]
-
-                for p in current_node.paths:
-                    new_penalty = penalty + p.penalty
-                    new_path = traversed_nodes + [p.node]
-                    if Configurer.__valid_path(new_path,constraints,benchmark_pref) and new_penalty != float('inf'):
-                        heapq.heappush(queue, (new_penalty, p.node,traversed_nodes,visited.copy()))
+        frontier_depth = 1
+        with tqdm(total=depth + 2) as pbar:
+            while queue:
+                penalty, current_node, traversed_nodes, visited = heapq.heappop(
+                    queue)
+                
+
+                if current_node in visited and current_node == start_node:
+                    pbar.update(1)
+                    return Configurer.OptimalPath(path=traversed_nodes + [current_node], penalty=penalty)
+
+                if current_node not in visited:
+                    visited.add(current_node)
+                    traversed_nodes = traversed_nodes + [current_node]
+
+                    for p in current_node.paths:
+                        new_penalty = penalty + p.penalty
+                        new_path = traversed_nodes + [p.node]
+
+
+                        if Configurer.__valid_path(new_path, constraints, benchmark_pref) and new_penalty != float('inf'):
+                            heapq.heappush(
+                                queue, (new_penalty, p.node, traversed_nodes, visited.copy()))
+                            
+                        else:
+                            pass
+
+                        if len(new_path) > frontier_depth:
+                            pbar.update(1)
+                            frontier_depth = len(new_path)
+                        
+                        # if psutil.virtual_memory().free >> 30 <= 1:
+                        #     queue = queue[:len(queue)//2]
+                        #     heapq.heapify(queue)
+                        #     gc.collect()
+                # print("=====")
         return None
 
     def __calculate_performance_penalty(
             benchmark_result: Dict,
             destination: Worker,
             model: Layer) -> float:
         return benchmark_result[destination.name]["model_performance"][model.name]["benchmark_time"]
@@ -306,15 +375,15 @@
     def __calculate_network_penalty(
         benchmark_result: Dict,
         source: Worker,
         destination: Worker,
         filesize_to_send: int
     ) -> float:
         stats = benchmark_result[source.name]["network_performance"][destination.name]
-        latency = stats["latency"]["rtt_avg_ms"] / 1000
+        latency = stats["latency"]["rtt_avg_ms"] / 1000 # Get in seconds
         bandwidth = stats["bandwidth"]["sent_bps"]
         return (latency + (filesize_to_send / bandwidth))
 
     def __calculate_network_penalty_from_model(
         benchmark_result: Dict,
         source: Worker,
         destination: Worker,
@@ -422,101 +491,125 @@
                     models_left=models_left[1:],
                     currNode=nextNode,
                     source_device=source_device,
                     devices=devices,
                     input_size=input_size
                 )
 
-    def __fetch_model_from_nodes(nodes:List[DecisionNode],models:List[keras.models.Model])->List[keras.models.Model]:
-        result:List[keras.models.Model] = []
+    def __fetch_model_from_nodes(nodes: List[DecisionNode], models: List[keras.models.Model]) -> List[keras.models.Model]:
+        result: List[keras.models.Model] = []
+        # jprint([
+        # j    n.model.name
+        # j    for n in nodes
+        # j    if (n.model is not None)
+        # j    else None])
+        # print([m.name for m in models])
         for n in nodes:
-            search = [m for m in models if m.name == n.model.name]
+            search = [
+                m for m in models if n.model is not None and m.name == n.model.name]
             if len(search) != 1:
-                raise PapdlException("Model names in benchmark.json does not match model names for the ones used for benchmarking. Rerun benchmarking process...")
+                raise PapdlException(
+                    "Model names in benchmark.json does not match model names for the ones used for benchmarking. Rerun benchmarking process...")
             result.append(search[0])
         return result
-    
-    def __merge_models(models:List[keras.models.Model])->keras.models.Model:
+
+    def __merge_models(models: List[keras.models.Model]) -> keras.models.Model:
         result_model = keras.models.Sequential()
         for model in models:
             result_model.add(model)
         result_model.build()
         return result_model
-        
-        
+
     def __generate_blocks(
         op: OptimalPath,
         models: List[keras.models.Model]
     ) -> List[SliceBlock]:
         l = 1
         r = 2
         slices: List[SliceBlock] = []
         while r < len(op.path):
-            
+            # print((l,r,slices))
             if op.path[r].device != op.path[l].device:
                 nodes_slice = op.path[l:r]
                 s = SliceBlock(
                     layers=[
                         n.model
                         for n in nodes_slice
                     ],
-                    slice_index=(l, r),
+                    slice_index=(l-1, r-1),
                     device=op.path[l].device,
                     model=Configurer.__merge_models(
-                        Configurer.__fetch_model_from_nodes(nodes_slice,models)
+                        Configurer.__fetch_model_from_nodes(
+                            nodes_slice, models)
                     )
                 )
                 slices.append(s)
                 l = r
             r += 1
 
         if len(slices) == 0:
             return [
                 SliceBlock(
-                    layers=[n.model for n in op.path],
-                    slice_index=(0, len(op.path)),
-                    device=op.path[0].device,
+                    layers=[n.model for n in op.path if n.model is not None],
+                    slice_index=(0, len(op.path)-1),
+                    device=op.path[1].device,
                     model=Configurer.__merge_models(
-                        Configurer.__fetch_model_from_nodes(op.path)
+                        Configurer.__fetch_model_from_nodes(
+                            [n for n in op.path if n.model is not None], models)
                     )
                 )
             ]
 
         return slices
 
     def parse_from_benchmark(
         self,
         benchmark_result: Dict,
         source_device: Union[Worker, str],
         input_size: int,
         search_constraints: SearchConstraints,
-        model_list:List[keras.models.Model],
-        benchmark_pref:BenchmarkPreferences
+        model_list: List[keras.models.Model],
+        benchmark_pref: BenchmarkPreferences
     ) -> Configuration:
         devices: List[Worker] = [
-            Worker(k,benchmark_result[k]["free_memory"]) for k in list(
+            Worker(k, benchmark_result[k]["free_memory"]) for k in list(
                 benchmark_result.keys())]
+        
+        
 
+        self.logger.debug("Benchmark Result")
+        self.logger.debug(benchmark_result)
         sd: Worker = None
         if isinstance(source_device, Worker):
             sd = source_device
         if isinstance(source_device, str):
-            sd = Worker(name=source_device,free_memory=benchmark_result[source_device]["free_memory"])
+            sd = Worker(
+                name=source_device, free_memory=benchmark_result[source_device]["free_memory"])
 
         models: List[Layer] = []
-        def model_total_ordering(k:str):
+
+        def model_total_ordering(k: str):
             _split = k.split("_")
             if len(_split) == 1:
                 return 0
             else:
                 return int(_split[1])
-        sorted_models = sorted(list(benchmark_result[sd.name]["model_performance"].keys()),key=model_total_ordering)
+        sorted_models = sorted(list(
+            benchmark_result[sd.name]["model_performance"].keys()), key=model_total_ordering)
         for m_key in sorted_models:
             model_dict = benchmark_result[sd.name]["model_performance"][m_key]
-            models.append(Layer(name=m_key,memory_usage=model_dict["benchmark_memory_usage"]))
+            models.append(
+                Layer(
+                    name=m_key,
+                    model_memory_usage=model_dict["benchmark_model_memory_usage"],
+                    hidden_memory_usage=model_dict["benchmark_hidden_and_input_memory_usage"],
+                    io_memory_usage=model_dict["benchmark_input_memory_multiplier"]
+                )
+            )
+        # self.tabulated_print_devices(devices,benchmark_pref)
 
         global visited_node_map
 
         visited_node_map = {}
 
         head = Configurer.DecisionNode(
             model=None,
@@ -527,34 +620,50 @@
             models_left=models,
             currNode=head,
             source_device=sd,
             devices=devices,
             input_size=input_size
         )
 
-        self.logger.info(f"Searching path with benchmark preferences: {benchmark_pref} and search preferences: {search_constraints}")
+        self.logger.info(
+            f"Searching path with benchmark preferences: {benchmark_pref} and search preferences: {search_constraints}")
+        depth = len(models)
+        width = len(devices)
+
         shortest_loop = Configurer.__find_shortest_loop(
             start_node=head,
             constraints=search_constraints,
-            benchmark_pref=benchmark_pref
+            benchmark_pref=benchmark_pref,
+            depth=depth,
+            width=width
         )
+        
+        # [print((n.device.name, n.model.name if n.model is not None else None)) for n in shortest_loop.path]
+        
+
+        # shortest_loop = None
+
+        # with open("shortest_loop_cache.pickle","rb") as f:
+        #     shortest_loop = pickle.load(f)
+
         if shortest_loop is None:
             self.logger.error("No path found with the provided constraints")
             exit(1)
 
-        blocks = Configurer.__generate_blocks(shortest_loop,model_list)
+        # print([f"model:{n.model} device:{n.device}" for n in shortest_loop.path])
+        blocks = Configurer.__generate_blocks(shortest_loop, model_list)
+
+        # print([b.device.name for b in blocks])
 
-        print([b.device.name for b in blocks])
-        
         input_shape = blocks[0].model.input_shape[1:]
 
         config = Configuration(
             slices=models,
             blocks=blocks,
             devices=devices,
             constraints=search_constraints,
             source_device=sd,
             input_shape=input_shape,
             benchmark_preferences=benchmark_pref,
             penalty=shortest_loop.penalty
         )
-        return config
+        return config
```

### Comparing `papdl-0.1.1/src/papdl/configure/main.py` & `papdl-0.1.2/src/papdl/configure/main.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/deploy/deploy.py` & `papdl-0.1.2/src/papdl/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/deploy/main.py` & `papdl-0.1.2/src/papdl/deploy/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 ):
     try:
         logger = prepare_logger(logging.DEBUG)
         logging.info("Deploying models...")
         configuration:Configuration = None
         with open(configuration_path,"rb") as f:
             configuration = pickle.load(f)
-        print(configuration["blocks"])
+        logger.info(configuration["blocks"])
         deploy_configuration(configuration,debug)
     except Exception:
         logger.error(traceback.format_exc())
         exit(1)
```

### Comparing `papdl-0.1.1/src/papdl/slice/main.py` & `papdl-0.1.2/src/papdl/slice/main.py`

 * *Files identical despite different names*

### Comparing `papdl-0.1.1/src/papdl/slice/slice.py` & `papdl-0.1.2/src/papdl/slice/slice.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
             prev_layers.append(node.inbound_layers)
 
     pl_outs = []
     for pl in prev_layers:
         pl_outs.extend([get_output_of_layer(
             pl, new_input, starting_layer_name)])
 
-    print(type(layer),type(pl_outs[0]),type(pl_outs))
     out = layer(pl_outs[0] if len(pl_outs) == 1 else pl_outs)
     layer_outputs[layer.name] = out
     return out
 
 
 # Returns a submodel for a specified input and output layer
 def get_model(input_layer: int, output_layer: int):
```

