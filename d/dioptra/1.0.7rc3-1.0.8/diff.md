# Comparing `tmp/dioptra-1.0.7rc3.tar.gz` & `tmp/dioptra-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptra-1.0.7rc3.tar", last modified: Sun Apr  9 23:54:38 2023, max compression
+gzip compressed data, was "dioptra-1.0.8.tar", last modified: Thu Apr 13 03:55:52 2023, max compression
```

## Comparing `dioptra-1.0.7rc3.tar` & `dioptra-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.695961 dioptra-1.0.7rc3/dioptra/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/inference_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/tf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/tf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5495 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/tf/tf_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6689 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/torch/torch_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/lake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/datasets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/lake/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/torch/object_store_datasets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27205 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/miners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2848 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/activation_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/base_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3230 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/coreset_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/entropy_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3208 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/knn_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/random_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/variance_miner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.251623 dioptra-1.0.8/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-13 03:55:51.000000 dioptra-1.0.8/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 03:55:52.247623 dioptra-1.0.8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-13 03:55:51.000000 dioptra-1.0.8/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/inference_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/tf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/tf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/tf/tf_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/inference/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6900 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/inference/torch/torch_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/lake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/datasets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/lake/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/torch/object_store_datasets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28545 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/lake/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra/miners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2848 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/activation_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4032 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/base_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3230 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/coreset_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/entropy_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3208 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/knn_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/random_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-13 03:55:51.000000 dioptra-1.0.8/dioptra/miners/variance_miner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 03:55:52.247623 dioptra-1.0.8/dioptra.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-13 03:55:52.000000 dioptra-1.0.8/dioptra.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 03:55:52.251623 dioptra-1.0.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-13 03:55:51.000000 dioptra-1.0.8/setup.py
```

### Comparing `dioptra-1.0.7rc3/LICENSE.md` & `dioptra-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/PKG-INFO` & `dioptra-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.7rc3
+Version: 1.0.8
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.7rc3/README.md` & `dioptra-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/inference/inference_runner.py` & `dioptra-1.0.8/dioptra/inference/inference_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/inference/tf/tf_runner.py` & `dioptra-1.0.8/dioptra/inference/tf/tf_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,45 @@
             model_name = None,
             datapoint_ids = [],
             embeddings_layers=[],
             logits_layer=None,
             class_names=[],
             datapoints_metadata=None,
             dataset_metadata=None,
-            mc_dropout_samples=0):
+            mc_dropout_samples=0,
+            channel_last=False,):
         """
         Utility to perform model inference on a dataset and extract layers needed for AL.
 
         Parameters:
             model: model to be used to inference
             model_name: the name of the model
             model_type: the type of the model use. Can be CLASSIFICATION or SEGMENTATION
             datapoint_ids: alist of datapoints to update with the predictions. Should be in the same order as the dataset.
             embeddings_layers: an array of layer names that should be used as embeddings
             logits_layer: the name of the logit layer (pre softmax) to be used for AL
             class_names: the class names corresponding to each logit. Indexes should match the logit layer
             datapoints_metadata: a list of dioptra style datapoints metadata to be added to teh datapoints. The indexes in this list should match the indexes in the dataset
             dataset_metadata: a dioptra style dataset metadata to be added to the dataset
+            channel_last: if the model expects the data to be in channel last format
         """
 
         super().__init__()
 
         self.model = model
         self.model_name = model_name
         self.datapoint_ids = datapoint_ids
         self.embeddings_layers = embeddings_layers
         self.logits_layer = logits_layer
         self.class_names = class_names
         self.datapoints_metadata = datapoints_metadata
         self.dataset_metadata = dataset_metadata
         self.model_type = model_type
         self.mc_dropout_samples = mc_dropout_samples
+        self.channel_last = channel_last
 
         input_layer = model.inputs
         if input_layer is None:
             input_layer = model.layers[0].inputs
 
         output_layers = {}
 
@@ -58,15 +61,15 @@
             inputs=input_layer,
             outputs=output_layers)
 
     def _get_layer_by_name(self, name):
         split = name.split('.')
         current_layer = self.model
         for part in split:
-            if re.match('\[[0-9]+\]', part):
+            if re.match('\[[0-9-]+\]', part):
                 index = int(part.replace('[', '').replace(']', ''))
                 current_layer = current_layer.layers[index]
             else:
                 current_layer = current_layer.get_layer(part)
         return current_layer
 
 
@@ -125,15 +128,16 @@
         return [{
             **({
                 'prediction': _format_prediction(
                     logits=logits,
                     embeddings=embeddings,
                     task_type=self.model_type,
                     model_name=self.model_name,
-                    class_names=self.class_names
+                    class_names=self.class_names,
+                    channel_last=self.channel_last
                 )
                } if logits is not None or embeddings is not None else {}
             ),
             **({'id': datapoint_id} if datapoint_id is not None else {}),
             **(self.datapoints_metadata[record_global_idx] \
                if self.datapoints_metadata and len(self.datapoints_metadata) > record_global_idx else {}
             ),
```

### Comparing `dioptra-1.0.7rc3/dioptra/inference/torch/torch_runner.py` & `dioptra-1.0.8/dioptra/inference/torch/torch_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
             embeddings_layers=[],
             logits_layer=None,
             class_names=[],
             datapoints_metadata=None,
             dataset_metadata=None,
             data_transform=None,
             mc_dropout_samples=0,
+            channel_last=False,
             device='cpu'):
         """
         Utility to perform model inference on a dataset and extract layers needed for AL.
 
         Parameters:
             model: model to be used to inference
             model_name: the name of the model
@@ -29,14 +30,15 @@
             embeddings_layers: an array of layer names that should be used as embeddings
             logits_layer: the name of the logit layer (pre softmax) to be used for AL
             class_names: the class names corresponding to each logit. Indexes should match the logit layer
             datapoints_metadata: a list of dioptra style datapoints metadata to be added to teh datapoints. The indexes in this list should match the indexes in the dataset
             dataset_metadata: a dioptra style dataset metadata to be added to the dataset
             data_transform: a transform function that will be called before the model is called. Should only return the data, without the groundtruth
             device: the devide to be use to perform the inference
+            channel_last: if the model expects the data to be in channel last format
         """
 
         super().__init__()
 
         self.model = model
         self.model_name = model_name
         self.datapoint_ids = datapoint_ids
@@ -45,27 +47,28 @@
         self.class_names = class_names
         self.datapoints_metadata = datapoints_metadata
         self.dataset_metadata = dataset_metadata
         self.data_transform = data_transform
         self.device = device
         self.model_type = model_type
         self.mc_dropout_samples = mc_dropout_samples
+        self.channel_last = channel_last
 
         self.activation = {}
 
         for my_layer_name in embeddings_layers + [logits_layer]:
             if my_layer_name is not None:
                 my_layer = self._get_layer_by_name(my_layer_name)
                 my_layer.register_forward_hook(self._get_activation(my_layer_name))
 
     def _get_layer_by_name(self, name):
         split = name.split('.')
         current_layer = self.model
         for part in split:
-            if re.match('\[[0-9]+\]', part):
+            if re.match('\[[0-9-]+\]', part):
                 index = int(part.replace('[', '').replace(']', ''))
                 current_layer = current_layer[index]
             else:
                 current_layer = getattr(current_layer, part)
         return current_layer
 
     def _get_activation(self, name):
@@ -150,15 +153,16 @@
         return [{
             **({
                 'prediction': _format_prediction(
                     logits=logits,
                     embeddings=embeddings,
                     task_type=self.model_type,
                     model_name=self.model_name,
-                    class_names=self.class_names
+                    class_names=self.class_names,
+                    channel_last=self.channel_last
                 )
                } if logits is not None or embeddings is not None else {}
             ),
             **({'id': datapoint_id} if datapoint_id is not None else {}),
             **(self.datapoints_metadata[record_global_idx] \
                if self.datapoints_metadata and len(self.datapoints_metadata) > record_global_idx else {}
             ),
```

### Comparing `dioptra-1.0.7rc3/dioptra/lake/datasets.py` & `dioptra-1.0.8/dioptra/lake/datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/lake/torch/object_store_datasets.py` & `dioptra-1.0.8/dioptra/lake/torch/object_store_datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/lake/utils.py` & `dioptra-1.0.8/dioptra/lake/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -553,37 +553,66 @@
         return {
             'task_type': task_type,
             'segmentation_class_mask': gt_array,
             **({'class_names': class_names} if class_names is not None else {}),
             **({'id': groundtruth_id} if groundtruth_id is not None else {})
         }
 
-def _format_prediction(logits, embeddings, task_type, model_name, class_names=None, prediction_id=None):
+def _format_prediction(
+        logits, embeddings, task_type, model_name,
+        class_names=None, prediction_id=None, channel_last=False):
     """
     Utility formatting the prediction field.
 
     Parameters:
         logits: the prediction logits (before softmax)
         embeddings: a dictionary containing the embeddings by layer names, or a single embeddings vector.
         task_type: the type of gt. Supported types CLASSIFICATION, SEGMENTATION
-        class_names: a list of class names. If the groundtruth contains indexes, it will be used to convert them to names
+        class_names: a list of class names.
+            If the groundtruth contains indexes, it will be used to convert them to names
         prediction_id: the id of the prediction to be updated
+        channel_last: if the logits and embeddings are in channel last format
     """
     if getattr(logits, 'numpy', None) is not None: # dealing with Tensorflow Tensors
         logits = logits.numpy()
 
-    if not isinstance(logits, np.ndarray):
-        logits = np.array(logits)
-    logits = logits.astype(np.float16).tolist()
+    if logits is not None:
+        if not isinstance(logits, np.ndarray):
+            logits = np.array(logits)
+        logits = logits.astype(np.float16)
+
+        if channel_last:
+            logits = np.moveaxis(logits, -1, 0)
+
+        logits = logits.tolist()
+
+    if embeddings is not None and len(embeddings) > 0:
+        if isinstance(embeddings, dict):
+            embeddings = {}
+            for k, v in embeddings.items():
+                if getattr(v, 'numpy', None) is not None: # dealing with Tensorflow Tensors
+                    v = v.numpy()
+                if not isinstance(v, np.ndarray):
+                    v = np.array(v)
+                embeddings[k] = v.astype(np.float16).tolist() if not channel_last \
+                    else np.moveaxis(v.astype(np.float16), -1, 0).tolist()
+        else:
+            if getattr(embeddings, 'numpy', None) is not None: # dealing with Tensorflow Tensors
+                embeddings = embeddings.numpy()
+            if not isinstance(embeddings, np.ndarray):
+                embeddings = np.array(embeddings)
+
+            embeddings = embeddings.astype(np.float16).tolist() if not channel_last \
+                    else np.moveaxis(embeddings.astype(np.float16), -1, 0).tolist()
 
     if task_type in ['CLASSIFICATION', 'SEGMENTATION']:
         return {
             'task_type': task_type,
-            'logits': logits,
-            'embeddings': embeddings,
+            **({'embeddings': embeddings} if embeddings is not None and len(embeddings) > 0 else {}),
+            **({'logits': logits} if logits is not None else {}),
             'model_name': model_name,
             **({'class_names': class_names} if class_names is not None else {}),
             **({'id': prediction_id} if prediction_id is not None else {})
         }
 
 def _resolve_mc_drop_out_predictions(predictions):
     return {
```

### Comparing `dioptra-1.0.7rc3/dioptra/miners/activation_miner.py` & `dioptra-1.0.8/dioptra/miners/activation_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/miners/base_miner.py` & `dioptra-1.0.8/dioptra/miners/base_miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,22 @@
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             })
             r.raise_for_status()
             response_json = r.json()
             task = response_json['task']
             status = task['status']
-
             if status == 'SUCCESS':
+
                 results =  task['result']
                 # TODO: remove this.
+                if results is None:
+                    results = []
                 if len(results) == 0 and retry_on_empty_success:
-                    time.sleep(2)
+                    time.sleep(10)
                     return self.get_results(retry_on_empty_success=False)
                 else:
                     return results
 
             elif status == 'FAILURE' or status == 'REVOKED':
                 raise RuntimeError('Miner failed')
             else:
```

### Comparing `dioptra-1.0.7rc3/dioptra/miners/coreset_miner.py` & `dioptra-1.0.8/dioptra/miners/coreset_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/miners/entropy_miner.py` & `dioptra-1.0.8/dioptra/miners/entropy_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/miners/knn_miner.py` & `dioptra-1.0.8/dioptra/miners/knn_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/miners/random_miner.py` & `dioptra-1.0.8/dioptra/miners/random_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra/miners/variance_miner.py` & `dioptra-1.0.8/dioptra/miners/variance_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/dioptra.egg-info/PKG-INFO` & `dioptra-1.0.8/dioptra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.7rc3
+Version: 1.0.8
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.7rc3/dioptra.egg-info/SOURCES.txt` & `dioptra-1.0.8/dioptra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc3/setup.py` & `dioptra-1.0.8/setup.py`

 * *Files identical despite different names*

