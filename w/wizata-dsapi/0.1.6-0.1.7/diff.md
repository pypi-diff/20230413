# Comparing `tmp/wizata-dsapi-0.1.6.tar.gz` & `tmp/wizata-dsapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.6.tar", last modified: Thu Apr 13 17:48:42 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.7.tar", last modified: Thu Apr 13 17:52:17 2023, max compression
```

## Comparing `wizata-dsapi-0.1.6.tar` & `wizata-dsapi-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:48:42.729821 wizata-dsapi-0.1.6/
--rw-rw-rw-   0        0        0    11556 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      246 2023-04-13 17:48:42.729308 wizata-dsapi-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-13 17:48:42.730301 wizata-dsapi-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:48:42.697487 wizata-dsapi-0.1.6/wizata_dsapi/
--rw-rw-rw-   0        0        0      732 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.6/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-24 09:46:21.000000 wizata-dsapi-0.1.6/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.6/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     1856 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.6/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-21 09:56:23.000000 wizata-dsapi-0.1.6/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    13455 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.6/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3555 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.6/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     5447 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.6/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.6/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0     2136 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.6/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0     9756 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.6/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     6914 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.6/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0      392 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.6/wizata_dsapi/sql_dto.py
--rw-rw-rw-   0        0        0     3563 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.6/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0      952 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.6/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2235 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.6/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.6/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    33193 2023-04-07 15:57:41.000000 wizata-dsapi-0.1.6/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:48:42.727321 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      246 2023-04-13 17:48:42.000000 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-04-13 17:48:42.000000 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:48:42.000000 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-04-13 17:48:42.000000 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 17:48:42.000000 wizata-dsapi-0.1.6/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 17:52:17.929968 wizata-dsapi-0.1.7/
+-rw-rw-rw-   0        0        0    11556 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      246 2023-04-13 17:52:17.928967 wizata-dsapi-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:52:17.930461 wizata-dsapi-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-04-13 17:52:15.000000 wizata-dsapi-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:52:17.901490 wizata-dsapi-0.1.7/wizata_dsapi/
+-rw-rw-rw-   0        0        0      756 2023-04-13 17:52:10.000000 wizata-dsapi-0.1.7/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-24 09:46:21.000000 wizata-dsapi-0.1.7/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.7/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     1856 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.7/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-21 09:56:23.000000 wizata-dsapi-0.1.7/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    13455 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.7/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3555 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.7/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     5447 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.7/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.7/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0     2136 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.7/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0     9756 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.7/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     6914 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.7/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0      392 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.7/wizata_dsapi/sql_dto.py
+-rw-rw-rw-   0        0        0     3563 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.7/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0      952 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.7/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2235 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.7/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.7/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    33193 2023-04-07 15:57:41.000000 wizata-dsapi-0.1.7/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:52:17.926982 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-04-13 17:52:17.000000 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-04-13 17:52:17.000000 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:52:17.000000 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-04-13 17:52:17.000000 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 17:52:17.000000 wizata-dsapi-0.1.7/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.6/LICENSE.txt` & `wizata-dsapi-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/setup.py` & `wizata-dsapi-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.6',
+    version='0.1.7',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.7/wizata_dsapi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .ds_dataframe import DSDataFrame
 from .script import Script
 from .template import Template
 from .twinregistration import TwinRegistration
 
 # Sql Entities (Dto)
 from .sql_dto import SqlDto
+from .twin import Twin
 
 # Api
 from .wizata_dsapi_client import api
 from .wizata_dsapi_client import WizataDSAPIClient
 from .dataframe_toolkit import df_to_json, df_to_csv, df_from_json, df_from_csv
 from .model_toolkit import predict
```

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.7/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.7/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.7/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.7/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.7/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.7/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.7/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.7/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.7/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/request.py` & `wizata-dsapi-0.1.7/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/script.py` & `wizata-dsapi-0.1.7/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/template.py` & `wizata-dsapi-0.1.7/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.7/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.7/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.7/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.7/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.6/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.7/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

