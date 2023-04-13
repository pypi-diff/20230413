# Comparing `tmp/terra_ai_datasets-1.1.2.tar.gz` & `tmp/terra_ai_datasets-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets-1.1.2.tar", last modified: Wed Apr 12 14:33:04 2023, max compression
+gzip compressed data, was "terra_ai_datasets-1.1.3.tar", last modified: Thu Apr 13 10:32:56 2023, max compression
```

## Comparing `terra_ai_datasets-1.1.2.tar` & `terra_ai_datasets-1.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.715731 terra_ai_datasets-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 14:33:04.715731 terra_ai_datasets-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:33:04.715731 terra_ai_datasets-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.711731 terra_ai_datasets-1.1.2/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.711731 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.711731 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/creation/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.711731 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 14:33:04.000000 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 14:33:04.000000 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:33:04.000000 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 14:33:04.000000 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 14:33:04.000000 terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:04.711731 terra_ai_datasets-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 14:32:53.000000 terra_ai_datasets-1.1.2/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.947657 terra_ai_datasets-1.1.3/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 10:32:56.000000 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-13 10:32:56.000000 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:32:56.000000 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 10:32:56.000000 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:32:56.000000 terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:56.951657 terra_ai_datasets-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 10:32:46.000000 terra_ai_datasets-1.1.3/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets-1.1.2/setup.py` & `terra_ai_datasets-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
```

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/create.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
 
 class ImageArray(Array):
 
     def create(self, source: str, parameters: ImageValidator):
 
         image = Image.open(source)
         array = np.asarray(image)
+        if array.ndim == 2:
+            array = np.stack([array, array, array], axis=-1)
         array = resize_frame(image_array=array,
                              target_shape=(parameters.height, parameters.width),
                              frame_mode=parameters.process)
         if parameters.network == ImageNetworkTypes.linear:
             array = array.reshape(np.prod(np.array(array.shape)))
 
         return array
```

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                         if self.preprocessing.get(col_name) and split == "train":
                             if put_data.type == LayerInputTypeChoice.Text:
                                 pass
                             elif put_data.type == LayerInputTypeChoice.Image and put_data.parameters.preprocessing == ImageScalers.terra_image_scaler:
                                 self.preprocessing[col_name].fit(sample_array)
                             else:
                                 self.preprocessing[col_name].partial_fit(sample_array.reshape(-1, 1))
-                        if not use_generator:
+                        if not use_generator or use_generator and put_data.type == LayerInputTypeChoice.Text:
                             col_array.append(
                                 sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                             )
 
                     if self.preprocessing.get(col_name) and split == "train":
                         if put_data.type == LayerInputTypeChoice.Text:
                             if put_data.parameters.preprocessing != TextProcessTypes.word_to_vec:
```

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/utils.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/utils.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/inputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/creation/visualize.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/creation/visualize.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets/load.py` & `terra_ai_datasets-1.1.3/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/terra_ai_datasets.egg-info/SOURCES.txt` & `terra_ai_datasets-1.1.3/terra_ai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/tests/test_classification.py` & `terra_ai_datasets-1.1.3/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/tests/test_regression.py` & `terra_ai_datasets-1.1.3/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/tests/test_segmentation.py` & `terra_ai_datasets-1.1.3/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.2/tests/test_timeseries.py` & `terra_ai_datasets-1.1.3/tests/test_timeseries.py`

 * *Files identical despite different names*

