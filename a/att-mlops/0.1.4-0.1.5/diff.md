# Comparing `tmp/att_mlops-0.1.4.tar.gz` & `tmp/att_mlops-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "att_mlops-0.1.4.tar", max compression
+gzip compressed data, was "att_mlops-0.1.5.tar", max compression
```

## Comparing `att_mlops-0.1.4.tar` & `att_mlops-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-13 11:26:00.699032 att_mlops-0.1.4/README.md
--rw-r--r--   0        0        0      327 2023-04-13 12:44:15.849856 att_mlops-0.1.4/att_mlops/__init__.py
--rw-r--r--   0        0        0   843827 2023-04-13 12:01:19.144433 att_mlops-0.1.4/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     4633 2023-04-13 14:18:12.366906 att_mlops-0.1.4/att_mlops/mlflow_registrator.py
--rw-r--r--   0        0        0     1733 2023-04-13 13:11:31.344564 att_mlops-0.1.4/att_mlops/mlops_connector.py
--rw-r--r--   0        0        0    13614 2023-04-13 13:10:46.520581 att_mlops-0.1.4/att_mlops/mlops_deployer.py
--rw-r--r--   0        0        0      439 2023-04-13 14:18:47.354909 att_mlops-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 att_mlops-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-13 11:26:00.699032 att_mlops-0.1.5/README.md
+-rw-r--r--   0        0        0        1 2023-04-13 14:47:32.082481 att_mlops-0.1.5/att_mlops/__init__.py
+-rw-r--r--   0        0        0   843827 2023-04-13 12:01:19.144433 att_mlops-0.1.5/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     4633 2023-04-13 14:18:12.366906 att_mlops-0.1.5/att_mlops/mlflow_registrator.py
+-rw-r--r--   0        0        0     1733 2023-04-13 13:11:31.344564 att_mlops-0.1.5/att_mlops/mlops_connector.py
+-rw-r--r--   0        0        0    13614 2023-04-13 13:10:46.520581 att_mlops-0.1.5/att_mlops/mlops_deployer.py
+-rw-r--r--   0        0        0      439 2023-04-13 14:48:09.890457 att_mlops-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 att_mlops-0.1.5/PKG-INFO
```

### Comparing `att_mlops-0.1.4/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl` & `att_mlops-0.1.5/att_mlops/h2o_mlops_client-0.60.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `att_mlops-0.1.4/att_mlops/mlflow_registrator.py` & `att_mlops-0.1.5/att_mlops/mlflow_registrator.py`

 * *Files identical despite different names*

### Comparing `att_mlops-0.1.4/att_mlops/mlops_connector.py` & `att_mlops-0.1.5/att_mlops/mlops_connector.py`

 * *Files identical despite different names*

### Comparing `att_mlops-0.1.4/att_mlops/mlops_deployer.py` & `att_mlops-0.1.5/att_mlops/mlops_deployer.py`

 * *Files identical despite different names*

