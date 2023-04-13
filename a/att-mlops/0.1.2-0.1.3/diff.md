# Comparing `tmp/att_mlops-0.1.2.tar.gz` & `tmp/att_mlops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "att_mlops-0.1.2.tar", max compression
+gzip compressed data, was "att_mlops-0.1.3.tar", max compression
```

## Comparing `att_mlops-0.1.2.tar` & `att_mlops-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-13 11:26:00.699032 att_mlops-0.1.2/README.md
--rw-r--r--   0        0        0      327 2023-04-13 12:44:15.849856 att_mlops-0.1.2/att_mlops/__init__.py
--rw-r--r--   0        0        0   843827 2023-04-13 12:01:19.144433 att_mlops-0.1.2/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     4788 2023-04-13 11:30:56.086467 att_mlops-0.1.2/att_mlops/mlflow_registrator.py
--rw-r--r--   0        0        0     1804 2023-04-13 11:30:56.086467 att_mlops-0.1.2/att_mlops/mlops_connector.py
--rw-r--r--   0        0        0    13346 2023-04-13 12:47:47.301728 att_mlops-0.1.2/att_mlops/mlops_deployer.py
--rw-r--r--   0        0        0      439 2023-04-13 12:48:19.785708 att_mlops-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 att_mlops-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-13 11:26:00.699032 att_mlops-0.1.3/README.md
+-rw-r--r--   0        0        0      327 2023-04-13 12:44:15.849856 att_mlops-0.1.3/att_mlops/__init__.py
+-rw-r--r--   0        0        0   843827 2023-04-13 12:01:19.144433 att_mlops-0.1.3/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     4688 2023-04-13 13:12:24.112533 att_mlops-0.1.3/att_mlops/mlflow_registrator.py
+-rw-r--r--   0        0        0     1733 2023-04-13 13:11:31.344564 att_mlops-0.1.3/att_mlops/mlops_connector.py
+-rw-r--r--   0        0        0    13614 2023-04-13 13:10:46.520581 att_mlops-0.1.3/att_mlops/mlops_deployer.py
+-rw-r--r--   0        0        0      439 2023-04-13 13:13:00.728513 att_mlops-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 att_mlops-0.1.3/PKG-INFO
```

### Comparing `att_mlops-0.1.2/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl` & `att_mlops-0.1.3/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `att_mlops-0.1.2/att_mlops/mlflow_registrator.py` & `att_mlops-0.1.3/att_mlops/mlflow_registrator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-# Databricks notebook source
-# Databricks notebook source
 import os
 import mimetypes
 import time
 import json
-# import mlflow
-# from mlflow.types.schema import Schema
-# from mlflow.models import infer_signature
-# from mlflow.tracking import MlflowClient
+import mlflow
+from mlflow.types.schema import Schema
+from mlflow.models import infer_signature
+from mlflow.tracking import MlflowClient
 from typing import List
-# import h2o_mlops_client
-# import h2o_mlops_client as mlops
+import h2o_mlops_client
+import h2o_mlops_client as mlops
 
-
-# Databricks notebook source
 class ModelRegistrator:
     
     def __init__(self, experiment_name, model, model_name, framework, X_train, y_train, target, model_metrics=[], name=None, description=None, creator_user=None,
     business_unit_owner=None, location=None, key_model_parameters=None, set_experiment_path=None):
       self.experiment_name = experiment_name
       self.model = model
       self.model_name = model_name
```

### Comparing `att_mlops-0.1.2/att_mlops/mlops_connector.py` & `att_mlops-0.1.3/att_mlops/mlops_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# Databricks notebook source
-# Databricks notebook source
 import os
 import mimetypes
 import time
 import json
-# import mlflow
-# from mlflow.types.schema import Schema
-# from mlflow.models import infer_signature
-# from mlflow.tracking import MlflowClient
+import mlflow
+from mlflow.types.schema import Schema
+from mlflow.models import infer_signature
+from mlflow.tracking import MlflowClient
 from typing import List
-# import h2o_mlops_client
-# import h2o_mlops_client as mlops
-
+import h2o_mlops_client
+import h2o_mlops_client as mlops
 
 # Databricks notebook source
 class mlopsConnect:
   # initializer / instance attributes
   def __init__(self, REFRESH_TOKEN, 
               API_CLIENT_ID="hac-platform-public",
               TOKEN_ENDPOINT_URL=(
```

### Comparing `att_mlops-0.1.2/att_mlops/mlops_deployer.py` & `att_mlops-0.1.3/att_mlops/mlops_deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+import os
+import mimetypes
+import time
+import json
+import mlflow
+from mlflow.types.schema import Schema
+from mlflow.models import infer_signature
+from mlflow.tracking import MlflowClient
+from typing import List
+import h2o_mlops_client
+import h2o_mlops_client as mlops
 # Databricks notebook source
 class importModel:
     prj = mlops.StorageProject
 
     def __init__(self,mlops_client, 
                   project_name,
                   deployment_scale,
```

