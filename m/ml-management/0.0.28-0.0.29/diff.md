# Comparing `tmp/ml-management-0.0.28.tar.gz` & `tmp/ml-management-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml-management-0.0.28.tar", last modified: Fri Mar 31 09:57:55 2023, max compression
+gzip compressed data, was "ml-management-0.0.29.tar", last modified: Thu Apr 13 06:27:53 2023, max compression
```

## Comparing `ml-management-0.0.28.tar` & `ml-management-0.0.29.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.098219 ml-management-0.0.28/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       18 2022-11-15 15:35:02.000000 ml-management-0.0.28/MANIFEST.in
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.28/ML_management/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/dataset/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1298 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/dataset/Dataset.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      190 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/dataset/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      330 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/dataset/datamodel.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/dataset/dummy_dataset/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      560 2023-03-14 13:05:09.000000 ml-management-0.0.28/ML_management/dataset/dummy_dataset/DummyDataset.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/dataset/dummy_dataset/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/dataset/s3_dataset/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    10399 2023-03-14 13:05:19.000000 ml-management-0.0.28/ML_management/dataset/s3_dataset/S3Dataset.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/dataset/s3_dataset/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/mlmanagement/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      581 2022-09-29 11:08:30.000000 ml-management-0.0.28/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3392 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     5054 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    11679 2023-03-30 13:46:32.000000 ml-management-0.0.28/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     7642 2023-03-30 13:46:32.000000 ml-management-0.0.28/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2986 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/mlmanagement/server_mlmanager_exceptions.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.094219 ml-management-0.0.28/ML_management/models/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      930 2022-12-12 14:54:32.000000 ml-management-0.0.28/ML_management/models/RetrainableModel.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      824 2022-10-17 21:23:47.000000 ml-management-0.0.28/ML_management/models/TrainableModel.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.28/ML_management/models/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      238 2023-01-13 09:22:49.000000 ml-management-0.0.28/ML_management/models/action_type.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      360 2023-01-13 09:22:49.000000 ml-management-0.0.28/ML_management/models/function_name_to_tag.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2430 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/models/model_pattern.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.098219 ml-management-0.0.28/ML_management/registry/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     7552 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/registry/RegistryManager.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.28/ML_management/registry/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2483 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/registry/exceptions.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.098219 ml-management-0.0.28/ML_management/tests/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/tests/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3361 2022-12-07 10:58:45.000000 ml-management-0.0.28/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     9508 2023-03-13 16:12:20.000000 ml-management-0.0.28/ML_management/tests/test_s3_dataset.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      367 2023-03-31 09:57:55.098219 ml-management-0.0.28/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       56 2022-08-01 13:04:47.000000 ml-management-0.0.28/README.md
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        7 2023-03-31 09:57:39.000000 ml-management-0.0.28/VERSION
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-03-31 09:57:55.098219 ml-management-0.0.28/ml_management.egg-info/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      367 2023-03-31 09:57:55.000000 ml-management-0.0.28/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1290 2023-03-31 09:57:55.000000 ml-management-0.0.28/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        1 2023-03-31 09:57:55.000000 ml-management-0.0.28/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      111 2023-03-31 09:57:55.000000 ml-management-0.0.28/ml_management.egg-info/requires.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       14 2023-03-31 09:57:55.000000 ml-management-0.0.28/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       38 2023-03-31 09:57:55.098219 ml-management-0.0.28/setup.cfg
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1062 2023-01-31 14:29:00.000000 ml-management-0.0.28/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/
+-rw-rw-r--   0 user      (1001) user      (1001)       18 2023-02-14 12:40:10.000000 ml-management-0.0.29/MANIFEST.in
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/dataset/
+-rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/Dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)      190 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      330 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/datamodel.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/dataset/dummy_dataset/
+-rw-rw-r--   0 user      (1001) user      (1001)      560 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/dummy_dataset/DummyDataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/dummy_dataset/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/dataset/s3_dataset/
+-rw-rw-r--   0 user      (1001) user      (1001)    10399 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/dataset/s3_dataset/S3Dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/s3_dataset/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/mlmanagement/
+-rw-rw-r--   0 user      (1001) user      (1001)      581 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3392 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 user      (1001) user      (1001)     5054 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 user      (1001) user      (1001)    11679 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 user      (1001) user      (1001)     7792 2023-04-04 08:32:07.000000 ml-management-0.0.29/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2986 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/server_mlmanager_exceptions.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/models/
+-rw-rw-r--   0 user      (1001) user      (1001)      930 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/RetrainableModel.py
+-rw-rw-r--   0 user      (1001) user      (1001)      824 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/TrainableModel.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      238 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/action_type.py
+-rw-rw-r--   0 user      (1001) user      (1001)      360 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/function_name_to_tag.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2430 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/models/model_pattern.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/registry/
+-rw-rw-r--   0 user      (1001) user      (1001)     7552 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/registry/RegistryManager.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/registry/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2483 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/registry/exceptions.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/tests/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/tests/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3361 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 user      (1001) user      (1001)     9508 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/tests/test_s3_dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)      367 2023-04-13 06:27:53.669418 ml-management-0.0.29/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       56 2023-02-14 12:40:10.000000 ml-management-0.0.29/README.md
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-04-13 06:25:51.000000 ml-management-0.0.29/VERSION
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ml_management.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      367 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)     1290 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)      111 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       14 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-13 06:27:53.669418 ml-management-0.0.29/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     1062 2023-02-14 12:40:10.000000 ml-management-0.0.29/setup.py
```

### Comparing `ml-management-0.0.28/ML_management/dataset/Dataset.py` & `ml-management-0.0.29/ML_management/dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/dataset/dummy_dataset/DummyDataset.py` & `ml-management-0.0.29/ML_management/dataset/dummy_dataset/DummyDataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/dataset/s3_dataset/S3Dataset.py` & `ml-management-0.0.29/ML_management/dataset/s3_dataset/S3Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.29/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.29/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.29/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.29/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.29/ML_management/mlmanagement/mlmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,17 @@
     }
     files = {
         "mlflow_request": json.dumps(mlflow_request),
         "model_zip": ("filename", model_file, "multipart/form-data"),
     }
 
     multipart = MultipartEncoder(fields=files)
-    return requests.post(server_ml_api, data=multipart, headers={"Content-Type": multipart.content_type})
+    return requests.post(
+        server_ml_api, data=multipart, headers={"Content-Type": multipart.content_type}, auth=(os.getenv("login"), os.getenv("password"))
+    )
 
 
 def send_request_to_server(function_name, kwargs, extra_attrs, for_class):
     """
     Send request to server.
 
     Takes frame of mlflow func and extra_attr
@@ -149,15 +151,18 @@
     elif function_name == "load_model":
         return mlflow.pyfunc.load_model(**kwargs)
     elif function_name == "save_model":
         return mlflow.pyfunc.save_model(**kwargs)
     else:
         response = request(function_name, kwargs, extra_attrs, None, for_class)
 
-    decoded_result = cloudpickle.loads(response.content)
+    try:
+        decoded_result = cloudpickle.loads(response.content)
+    except Exception:
+        raise Exception(response.content.decode())
 
     # raise error if mlflow is supposed to raise error
     if isinstance(decoded_result, MlflowException):
         is_rest = decoded_result.json_kwargs.pop("isRest", False)
         if is_rest:
             created_json = {
                 "error_code": decoded_result.error_code,
```

### Comparing `ml-management-0.0.28/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.29/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/models/RetrainableModel.py` & `ml-management-0.0.29/ML_management/models/RetrainableModel.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/models/TrainableModel.py` & `ml-management-0.0.29/ML_management/models/TrainableModel.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/models/model_pattern.py` & `ml-management-0.0.29/ML_management/models/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/registry/RegistryManager.py` & `ml-management-0.0.29/ML_management/registry/RegistryManager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/registry/exceptions.py` & `ml-management-0.0.29/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.29/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.29/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.29/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.28/setup.py` & `ml-management-0.0.29/setup.py`

 * *Files identical despite different names*

