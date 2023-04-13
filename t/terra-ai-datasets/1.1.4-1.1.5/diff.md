# Comparing `tmp/terra_ai_datasets-1.1.4.tar.gz` & `tmp/terra_ai_datasets-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets-1.1.4.tar", last modified: Thu Apr 13 10:48:54 2023, max compression
+gzip compressed data, was "terra_ai_datasets-1.1.5.tar", last modified: Thu Apr 13 11:16:35 2023, max compression
```

## Comparing `terra_ai_datasets-1.1.4.tar` & `terra_ai_datasets-1.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.468944 terra_ai_datasets-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 10:48:54.468944 terra_ai_datasets-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:48:54.468944 terra_ai_datasets-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.460944 terra_ai_datasets-1.1.4/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.464944 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.464944 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/creation/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.460944 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 10:48:54.000000 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-13 10:48:54.000000 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:48:54.000000 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 10:48:54.000000 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:48:54.000000 terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:54.468944 terra_ai_datasets-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:48:44.000000 terra_ai_datasets-1.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-13 10:48:45.000000 terra_ai_datasets-1.1.4/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 10:48:45.000000 terra_ai_datasets-1.1.4/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 10:48:45.000000 terra_ai_datasets-1.1.4/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 10:48:45.000000 terra_ai_datasets-1.1.4/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.454140 terra_ai_datasets-1.1.5/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.454140 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 11:16:35.000000 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-13 11:16:35.000000 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:16:35.000000 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 11:16:35.000000 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:16:35.000000 terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:35.458140 terra_ai_datasets-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 11:16:22.000000 terra_ai_datasets-1.1.5/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets-1.1.4/setup.py` & `terra_ai_datasets-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
```

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/create.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/arrays.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/utils.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,27 +143,27 @@
         data_to_return.append(' '.join(words_list))
 
     return data_to_return
 
 
 def extract_image_data(folder_path: Path, parameters: Union[ImageValidator, SegmentationValidator]):
     image_samples = []
-    for image_path in folder_path.iterdir():
+    for image_path in sorted(folder_path.iterdir()):
         image_samples.append(image_path)
 
     return image_samples
 
 
 def extract_segmentation_data(folder_path: Path, parameters: SegmentationValidator):
     return extract_image_data(folder_path, parameters)
 
 
 def extract_text_data(folder_path: Path, parameters: TextValidator):
     text_samples = []
-    for text_path in folder_path.iterdir():
+    for text_path in sorted(folder_path.iterdir()):
         with open(text_path, 'r', encoding="utf-8") as text_file:
             text = ' '.join(text_to_word_sequence(
                 text_file.read().strip(), **{'lower': False, 'filters': parameters.filters, 'split': ' '})
             ).split()
         if parameters.mode == TextModeTypes.full:
             text_samples.append(' '.join(text[:parameters.max_words]))
         else:
@@ -173,15 +173,15 @@
                 if len(text_sample) < parameters.length:
                     break
     return text_samples
 
 
 def extract_audio_data(folder_path: Path, parameters: AudioValidator):
     audio_samples = []
-    for audio_path in folder_path.iterdir():
+    for audio_path in sorted(folder_path.iterdir()):
         if parameters.mode == TextModeTypes.full:
             audio_samples.append(';'.join([str(audio_path), f"0:{parameters.max_seconds}"]))
         else:
             duration = librosa.get_duration(path=str(audio_path))
             start_idx, stop_idx = 0, parameters.length
             audio_samples.append(';'.join([str(audio_path), f"{start_idx}:{stop_idx}"]))
             while stop_idx < duration:
```

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/inputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/creation/visualize.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/creation/visualize.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets/load.py` & `terra_ai_datasets-1.1.5/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/terra_ai_datasets.egg-info/SOURCES.txt` & `terra_ai_datasets-1.1.5/terra_ai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/tests/test_classification.py` & `terra_ai_datasets-1.1.5/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/tests/test_regression.py` & `terra_ai_datasets-1.1.5/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/tests/test_segmentation.py` & `terra_ai_datasets-1.1.5/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.4/tests/test_timeseries.py` & `terra_ai_datasets-1.1.5/tests/test_timeseries.py`

 * *Files identical despite different names*

