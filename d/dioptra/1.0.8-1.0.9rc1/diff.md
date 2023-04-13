# Comparing `tmp/dioptra-1.0.8.tar.gz` & `tmp/dioptra-1.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptra-1.0.8.tar", last modified: Thu Apr 13 03:55:52 2023, max compression
+gzip compressed data, was "dioptra-1.0.9rc1.tar", last modified: Thu Apr 13 04:32:02 2023, max compression
```

## Comparing `dioptra-1.0.8.tar` & `dioptra-1.0.9rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.251623 dioptra-1.0.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-13 03:55:51.000000 dioptra-1.0.8/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 03:55:52.247623 dioptra-1.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-13 03:55:51.000000 dioptra-1.0.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/inference_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/tf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/tf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/tf/tf_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6900 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/torch/torch_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/lake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/datasets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/lake/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/torch/object_store_datasets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28545 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/miners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2848 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/activation_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4032 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/base_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3230 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/coreset_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/entropy_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3208 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/knn_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/random_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/variance_miner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 03:55:52.251623 dioptra-1.0.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-13 03:55:51.000000 dioptra-1.0.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/inference_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/tf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/tf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/tf/tf_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6900 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/torch/torch_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/lake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8352 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/datasets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/lake/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/torch/object_store_datasets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29031 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/miners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/activation_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4382 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/base_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3533 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/coreset_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2105 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/entropy_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/knn_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/random_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/variance_miner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/setup.py
```

### Comparing `dioptra-1.0.8/LICENSE.md` & `dioptra-1.0.9rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/PKG-INFO` & `dioptra-1.0.9rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.8
+Version: 1.0.9rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.8/README.md` & `dioptra-1.0.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/dioptra/inference/inference_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/inference_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/dioptra/inference/tf/tf_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/tf/tf_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/dioptra/inference/torch/torch_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/torch/torch_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/dioptra/lake/datasets.py` & `dioptra-1.0.9rc1/dioptra/lake/datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,36 +17,39 @@
         my_dataset = Dataset()
         my_dataset.dataset_id = metadata['uuid']
         my_dataset.dataset_name = metadata['display_name']
         dataset_list.append(my_dataset)
 
     return dataset_list
 
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 class Dataset():
 
     def __init__(self):
 
         api_key = os.environ.get('DIOPTRA_API_KEY', None)
         if api_key is None:
             raise RuntimeError('DIOPTRA_API_KEY env var is not set')
 
         self.api_key = api_key
-        self.app_endpoint = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
         self.dataset_id = None
         self.dataset_name = None
 
     def get_from_uuid(self, uuid):
         """
         Retreive a dataset using its uuid
 
         Parameters:
             uuid: uuid of the dataset
         """
         try:
-            r = requests.get(f'{self.app_endpoint}/api/dataset/{uuid}', headers={
+            r = requests.get(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{uuid}', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
             print('There was an error retreiving a dataset ...')
             raise err
@@ -89,15 +92,15 @@
         Creates a dataset. Datasets are collections of datapoints that are version controled by Dioptra
 
         Parameters:
             name: name of the dataset
         """
 
         try:
-            r = requests.post(f'{self.app_endpoint}/api/dataset', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/dataset', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             }, json={
                 'displayName': name
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
@@ -111,15 +114,15 @@
         Commit the changes made to the dataset that are not committed
 
         Parameters:
             message: message of the commit
         """
 
         try:
-            r = requests.post(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/commit', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/commit', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             }, json={
                 'message': message
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
@@ -132,15 +135,15 @@
     def history(self):
         """
         Get the dataset commit history
 
         """
 
         try:
-            r = requests.get(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/versions', headers={
+            r = requests.get(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/versions', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
             print('There was an error fetching history for the dataset ...')
             raise err
@@ -154,15 +157,15 @@
         Parameters:
             fields: the list of fields to be downloaded.
                     By default all fields are returned, except embeddings & logits
 
         """
 
         try:
-            r = requests.get(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/datapoints', headers={
+            r = requests.get(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/datapoints', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
             print('There was an error downloading a dataset ...')
             raise err
@@ -175,15 +178,15 @@
         The datapoints will be uncommitted until a commit command is called
 
         Parameters:
             datapoint_ids: list of datapoint ids
         """
 
         try:
-            r = requests.post(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/add', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/add', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             }, json={
                 'datapointIds': datapoint_ids
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
@@ -196,15 +199,15 @@
         The datapoints will be uncommitted until a commit command is called unless the datapoints are aleady uncommitted
 
         Parameters:
             datapoint_ids: list of datapoint ids
         """
 
         try:
-            r = requests.post(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/remove', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/remove', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             }, json={
                 'datapointIds': datapoint_ids
             })
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
@@ -218,15 +221,15 @@
         This will delete the current uncommitted changes
 
         Parameters:
             commit_id: id of the commit to checkout
         """
 
         try:
-            r = requests.post(f'{self.app_endpoint}/api/dataset/{self.dataset_id}/checkout/{commit_id}', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}/checkout/{commit_id}', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
 
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
             print('There was an error checking out a dataset ...')
@@ -237,15 +240,15 @@
     def delete(self):
         """
         Delete the dataset. This is NOT reversible !!
 
         """
 
         try:
-            r = requests.delete(f'{self.app_endpoint}/api/dataset/{self.dataset_id}', headers={
+            r = requests.delete(f'{DIOPTRA_APP_ENDPOINT}/api/dataset/{self.dataset_id}', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
 
             r.raise_for_status()
         except requests.exceptions.RequestException as err:
             print('There was an error deleting a dataset ...')
```

### Comparing `dioptra-1.0.8/dioptra/lake/torch/object_store_datasets.py` & `dioptra-1.0.9rc1/dioptra/lake/torch/object_store_datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/dioptra/lake/utils.py` & `dioptra-1.0.9rc1/dioptra/lake/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 
 # TODO: figure out how to return status codes form lambda functions.
 # See the wip_return_error_code branch of the infrastructure repo.
 def _raise_for_apigateway_errormessage(response):
     if response is not None and 'errorMessage' in response:
         raise RuntimeError(response['errorMessage'])
 
+DIOPTRA_API_ENDPOINT = os.environ.get('DIOPTRA_API_ENDPOINT', 'https://api.dioptra.ai/events')
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 def query_dioptra_app(method, path, body=None):
     api_key = os.environ.get('DIOPTRA_API_KEY', None)
     if api_key is None:
         raise RuntimeError('DIOPTRA_API_KEY env var is not set')
 
-    app_endpoint = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
     r = None
     try:
-        r = getattr(requests, method.lower())(f'{app_endpoint}{path}', headers={
+        r = getattr(requests, method.lower())(f'{DIOPTRA_APP_ENDPOINT}{path}', verify=DIOPTRA_SSL_VERIFY, headers={
             'content-type': 'application/json',
             'x-api-key': api_key
         }, json=body)
         r.raise_for_status()
     except requests.exceptions.RequestException as err:
         if r is None:
             raise err
@@ -185,20 +189,19 @@
         records: array of dipotra style records. See teh doc for accepted formats
     """
 
     api_key = os.environ.get('DIOPTRA_API_KEY', None)
     if api_key is None:
         raise RuntimeError('DIOPTRA_API_KEY env var is not set')
 
-    api_endpoint = os.environ.get('DIOPTRA_API_ENDPOINT', 'https://api.dioptra.ai/events')
-
     try:
-        r = requests.post(api_endpoint, headers={
+        r = requests.post(DIOPTRA_API_ENDPOINT, verify=DIOPTRA_SSL_VERIFY, headers={
             'content-type': 'application/json',
-            'x-api-key': api_key
+            'x-api-key': api_key,
+            'host': 'api.dioptra.ai'
         }, json={
             'records': records
         })
         r.raise_for_status()
         response = r.json()
         _raise_for_apigateway_errormessage(response)
     except requests.exceptions.RequestException as err:
@@ -251,23 +254,23 @@
         object_name: name of the key in the bucket where the records are
     """
 
     api_key = os.environ.get('DIOPTRA_API_KEY', None)
     if api_key is None:
         raise RuntimeError('DIOPTRA_API_KEY env var is not set')
 
-    api_endpoint = os.environ.get('DIOPTRA_API_ENDPOINT', 'https://api.dioptra.ai/events')
     if storage_type == 's3':
         signed_url = _generate_s3_signed_url(bucket_name, object_name)
     elif storage_type == 'gs':
         signed_url = _generate_gs_signed_url(bucket_name, object_name)
     try:
-        r = requests.post(api_endpoint, headers={
+        r = requests.post(DIOPTRA_API_ENDPOINT, verify=DIOPTRA_SSL_VERIFY, headers={
             'content-type': 'application/json',
-            'x-api-key': api_key
+            'x-api-key': api_key,
+            'host': 'api.dioptra.ai'
         }, json={
             'url': signed_url,
             'offset': offset,
             'limit': limit
         } if disable_batching else {
             'urls': [signed_url]
         })
@@ -314,33 +317,32 @@
     if isinstance(upload_id, dict) and 'id' in upload_id:
         upload_id = upload_id['id']
 
     api_key = os.environ.get('DIOPTRA_API_KEY', None)
     if api_key is None:
         raise RuntimeError('DIOPTRA_API_KEY env var is not set')
 
-    app_endpoint = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
     sleepTimeSecs = 1
     totalSleepTimeSecs = 0
     try:
         while True:
             if totalSleepTimeSecs > 900:
                 raise RuntimeError('Timed out waiting for the upload to finish.')
 
-            r = requests.get(f'{app_endpoint}/api/ingestion/executions/{upload_id}', headers={
+            r = requests.get(f'{DIOPTRA_APP_ENDPOINT}/api/ingestion/executions/{upload_id}', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': api_key
             })
             r.raise_for_status()
             upload = r.json()
             if upload['status'] in ['SUCCEEDED']:
                 return upload
             elif upload['status'] in ['FAILED', 'TIMED_OUT', 'ABORTED']:
                 raise RuntimeError(
-                    f'Upload failed with status {upload["status"]}. See more information in the Dioptra UI: {app_endpoint}/settings/uploads/{upload_id}')
+                    f'Upload failed with status {upload["status"]}. See more information in the Dioptra UI: {DIOPTRA_APP_ENDPOINT}/settings/uploads/{upload_id}')
             else:
                 time.sleep(sleepTimeSecs)
                 totalSleepTimeSecs += sleepTimeSecs
                 sleepTimeSecs = min(sleepTimeSecs * 2, 60)
     except requests.exceptions.RequestException as err:
         print('There was an error waiting for the upload to finish ...')
         raise err
@@ -359,14 +361,17 @@
         raise err
 
     return response
 
 def _generate_gs_signed_url(bucket_name, object_name):
 
     cred_file = os.environ.get('GOOGLE_APPLICATION_CREDENTIALS', None)
+    if cred_file is None:
+        raise RuntimeError('GOOGLE_APPLICATION_CREDENTIALS env var is not set. See the documentation for more information: https://dioptra.gitbook.io/dioptra-doc/EIKhoPaxsbOt062jkPon/overview/lake-ml/configuring-object-stores')
+
     with open(cred_file, 'r') as f:
         credentials = json.load(f)
     gcs_client = storage.Client.from_service_account_info(credentials)
     bucket = gcs_client.get_bucket(bucket_name)
     blob = bucket.get_blob(object_name)
     try:
         response = blob.generate_signed_url(
```

### Comparing `dioptra-1.0.8/dioptra/miners/activation_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/activation_miner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+import os
 import requests
 from .base_miner import BaseMiner
 
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 class ActivationMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name=None,
             embeddings_field='embeddings',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
@@ -23,15 +28,15 @@
             select_desc: whether to order by dec or not
             skip_caching: whether to skip vector caching or not
 
         """
 
         super().__init__()
         try:
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'ACTIVATION',
                 'size': size,
```

### Comparing `dioptra-1.0.8/dioptra/miners/coreset_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/knn_miner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 import requests
 from .base_miner import BaseMiner
 
-class CoresetMiner(BaseMiner):
+import os
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
+class KNNMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name=None,
             embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
-        CoreSet miner
+        KNN miner
         Will perform a AL query based on CoreSet
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
             embeddings_field: embedding fields to run the analysis on. Could be 'embeddings'
+            metric: the metrics to be used to do KNN. Could be 'euclidian' or 'cosine'
             select_filters: dioptra style filters to select the data to be queried from
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
             select_reference_filters: dioptra style filters to select the data that is already in your training dataset
             select_reference_limit: like previous but for teh reference data
             select_reference_order_by: like previous but for teh reference data
             select_reference_desc: like previous but for teh reference data
             skip_caching: whether to skip vector caching or not
         """
 
         super().__init__()
         try:
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
-                'strategy': 'CORESET',
-                'size': size,
+                'strategy': 'NEAREST_NEIGHBORS',
                 'metric': metric,
+                'size': size,
                 'embeddings_field': embeddings_field,
                 'model_name': model_name,
                 'select': {
                     'filters': select_filters,
                     **({'limit': select_limit} if select_limit is not None else {}),
                     **({'order_by': select_order_by} if select_order_by is not None else {}),
                     **({'desc': select_desc} if select_desc is not None else {}),
                 },
-                **({'select_reference':
-                    {
-                        'filters': select_reference_filters,
-                        **({'limit': select_reference_limit} if select_reference_limit is not None else {}),
-                        **({'order_by': select_reference_order_by} if select_reference_order_by is not None else {}),
-                        **({'desc': select_reference_desc} if select_reference_desc is not None else {}),
-                    }
-                } if select_reference_filters is not None else {}),
+                'select_reference': {
+                    'filters': select_reference_filters,
+                    **({'limit': select_reference_limit} if select_reference_limit is not None else {}),
+                    **({'order_by': select_reference_order_by} if select_reference_order_by is not None else {}),
+                    **({'desc': select_reference_desc} if select_reference_desc is not None else {}),
+                },
                 'skip_caching': skip_caching
             })
             r.raise_for_status()
             self.miner_id = r.json()['miner_id']
             self.miner_name = display_name
         except requests.exceptions.RequestException as err:
             print('There was an error getting miner status...')
```

### Comparing `dioptra-1.0.8/dioptra/miners/entropy_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/entropy_miner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import requests
 from .base_miner import BaseMiner
 
+import os
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 class EntropyMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name=None,
             select_limit=None, select_order_by=None, select_desc=None):
         """
         Entropy miner
         Will perform a AL query based on Entropy
@@ -16,15 +21,15 @@
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
         """
 
         super().__init__()
         try:
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'ENTROPY',
                 'size': size,
```

### Comparing `dioptra-1.0.8/dioptra/miners/knn_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/coreset_miner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 import requests
 from .base_miner import BaseMiner
 
-class KNNMiner(BaseMiner):
+import os
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
+class CoresetMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name=None,
             embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
-        KNN miner
+        CoreSet miner
         Will perform a AL query based on CoreSet
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
             embeddings_field: embedding fields to run the analysis on. Could be 'embeddings'
-            metric: the metrics to be used to do KNN. Could be 'euclidian' or 'cosine'
             select_filters: dioptra style filters to select the data to be queried from
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
             select_reference_filters: dioptra style filters to select the data that is already in your training dataset
             select_reference_limit: like previous but for teh reference data
             select_reference_order_by: like previous but for teh reference data
             select_reference_desc: like previous but for teh reference data
             skip_caching: whether to skip vector caching or not
         """
 
         super().__init__()
         try:
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
-                'strategy': 'NEAREST_NEIGHBORS',
-                'metric': metric,
+                'strategy': 'CORESET',
                 'size': size,
+                'metric': metric,
                 'embeddings_field': embeddings_field,
                 'model_name': model_name,
                 'select': {
                     'filters': select_filters,
                     **({'limit': select_limit} if select_limit is not None else {}),
                     **({'order_by': select_order_by} if select_order_by is not None else {}),
                     **({'desc': select_desc} if select_desc is not None else {}),
                 },
-                'select_reference': {
-                    'filters': select_reference_filters,
-                    **({'limit': select_reference_limit} if select_reference_limit is not None else {}),
-                    **({'order_by': select_reference_order_by} if select_reference_order_by is not None else {}),
-                    **({'desc': select_reference_desc} if select_reference_desc is not None else {}),
-                },
+                **({'select_reference':
+                    {
+                        'filters': select_reference_filters,
+                        **({'limit': select_reference_limit} if select_reference_limit is not None else {}),
+                        **({'order_by': select_reference_order_by} if select_reference_order_by is not None else {}),
+                        **({'desc': select_reference_desc} if select_reference_desc is not None else {}),
+                    }
+                } if select_reference_filters is not None else {}),
                 'skip_caching': skip_caching
             })
             r.raise_for_status()
             self.miner_id = r.json()['miner_id']
             self.miner_name = display_name
         except requests.exceptions.RequestException as err:
             print('There was an error getting miner status...')
```

### Comparing `dioptra-1.0.8/dioptra/miners/random_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/random_miner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import requests
 from .base_miner import BaseMiner
 
+import os
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 class RandomMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters,
             select_limit=None, select_order_by=None, select_desc=None, model_name=None):
         """
         Random miner
         Will perform a random query
@@ -17,15 +22,15 @@
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
         """
 
         super().__init__()
         try:
 
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'RANDOM',
                 'size': size,
```

### Comparing `dioptra-1.0.8/dioptra/miners/variance_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/variance_miner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import requests
 from .base_miner import BaseMiner
 
+import os
+DIOPTRA_APP_ENDPOINT = os.environ.get('DIOPTRA_APP_ENDPOINT', 'https://app.dioptra.ai')
+# We ask for a definitive signal to disable but using the positive form is easier in code.
+DIOPTRA_SSL_VERIFY = not os.environ.get('DIOPTRA_SSL_NOVERIFY', 'False') == 'True'
+
 class VarianceMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters,
             select_limit=None, select_order_by=None, select_desc=None, model_name=None):
         """
         Variance miner
         Will perform a AL query based on Variance
@@ -15,15 +20,15 @@
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
         """
 
         super().__init__()
         try:
-            r = requests.post(f'{self.app_endpoint}/api/tasks/miners', headers={
+            r = requests.post(f'{DIOPTRA_APP_ENDPOINT}/api/tasks/miners', verify=DIOPTRA_SSL_VERIFY, headers={
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'VARIANCE',
                 'size': size,
```

### Comparing `dioptra-1.0.8/dioptra.egg-info/PKG-INFO` & `dioptra-1.0.9rc1/dioptra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.8
+Version: 1.0.9rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.8/dioptra.egg-info/SOURCES.txt` & `dioptra-1.0.9rc1/dioptra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.8/setup.py` & `dioptra-1.0.9rc1/setup.py`

 * *Files identical despite different names*

