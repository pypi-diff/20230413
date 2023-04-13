# Comparing `tmp/simunetcore-0.0.8.tar.gz` & `tmp/simunetcore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simunetcore-0.0.8.tar", last modified: Thu Dec  1 06:32:20 2022, max compression
+gzip compressed data, was "simunetcore-0.0.9.tar", last modified: Thu Dec  1 06:59:57 2022, max compression
```

## Comparing `simunetcore-0.0.8.tar` & `simunetcore-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 06:32:20.948772 simunetcore-0.0.8/
--rw-rw-rw-   0        0        0     1109 2022-11-10 10:48:35.000000 simunetcore-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      510 2022-12-01 06:32:20.947776 simunetcore-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-11-10 10:59:38.000000 simunetcore-0.0.8/README.md
--rw-rw-rw-   0        0        0      699 2022-12-01 06:32:06.000000 simunetcore-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-01 06:32:20.948772 simunetcore-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-01 06:32:20.937801 simunetcore-0.0.8/simunetcore/
--rw-rw-rw-   0        0        0      762 2022-12-01 06:32:04.000000 simunetcore-0.0.8/simunetcore/__init__.py
--rw-rw-rw-   0        0        0     4726 2022-11-11 06:26:30.000000 simunetcore-0.0.8/simunetcore/aws.py
--rw-rw-rw-   0        0        0     3038 2022-01-18 08:22:35.000000 simunetcore-0.0.8/simunetcore/exception.py
--rw-rw-rw-   0        0        0     1732 2022-11-29 06:36:16.000000 simunetcore-0.0.8/simunetcore/factory.py
--rw-rw-rw-   0        0        0     7911 2022-11-11 06:17:53.000000 simunetcore-0.0.8/simunetcore/invoker.py
--rw-rw-rw-   0        0        0     2151 2022-11-10 11:29:46.000000 simunetcore-0.0.8/simunetcore/logger.py
--rw-rw-rw-   0        0        0     8936 2022-11-10 11:29:47.000000 simunetcore-0.0.8/simunetcore/model.py
--rw-rw-rw-   0        0        0     7463 2022-11-10 11:29:47.000000 simunetcore-0.0.8/simunetcore/mqtt.py
--rw-rw-rw-   0        0        0     6155 2022-11-14 11:29:06.000000 simunetcore-0.0.8/simunetcore/plot.py
--rw-rw-rw-   0        0        0     2762 2022-11-29 06:11:24.000000 simunetcore-0.0.8/simunetcore/rest.py
--rw-rw-rw-   0        0        0     6245 2022-11-10 11:29:49.000000 simunetcore-0.0.8/simunetcore/serializer.py
--rw-rw-rw-   0        0        0     2185 2022-11-08 08:33:52.000000 simunetcore-0.0.8/simunetcore/utils.py
--rw-rw-rw-   0        0        0    29076 2022-12-01 06:31:17.000000 simunetcore-0.0.8/simunetcore/waveform.py
-drwxrwxrwx   0        0        0        0 2022-12-01 06:32:20.945778 simunetcore-0.0.8/simunetcore.egg-info/
--rw-rw-rw-   0        0        0      510 2022-12-01 06:32:20.000000 simunetcore-0.0.8/simunetcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2022-12-01 06:32:20.000000 simunetcore-0.0.8/simunetcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 06:32:20.000000 simunetcore-0.0.8/simunetcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-12-01 06:32:20.000000 simunetcore-0.0.8/simunetcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-01 06:32:20.000000 simunetcore-0.0.8/simunetcore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-01 06:59:57.871847 simunetcore-0.0.9/
+-rw-rw-rw-   0        0        0     1109 2022-11-10 10:48:35.000000 simunetcore-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      510 2022-12-01 06:59:57.871847 simunetcore-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-11-10 10:59:38.000000 simunetcore-0.0.9/README.md
+-rw-rw-rw-   0        0        0      699 2022-12-01 06:59:47.000000 simunetcore-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-12-01 06:59:57.871847 simunetcore-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-12-01 06:59:57.863868 simunetcore-0.0.9/simunetcore/
+-rw-rw-rw-   0        0        0      762 2022-12-01 06:59:46.000000 simunetcore-0.0.9/simunetcore/__init__.py
+-rw-rw-rw-   0        0        0     4726 2022-11-11 06:26:30.000000 simunetcore-0.0.9/simunetcore/aws.py
+-rw-rw-rw-   0        0        0     3038 2022-01-18 08:22:35.000000 simunetcore-0.0.9/simunetcore/exception.py
+-rw-rw-rw-   0        0        0     1732 2022-11-29 06:36:16.000000 simunetcore-0.0.9/simunetcore/factory.py
+-rw-rw-rw-   0        0        0     7911 2022-11-11 06:17:53.000000 simunetcore-0.0.9/simunetcore/invoker.py
+-rw-rw-rw-   0        0        0     2151 2022-11-10 11:29:46.000000 simunetcore-0.0.9/simunetcore/logger.py
+-rw-rw-rw-   0        0        0     8936 2022-11-10 11:29:47.000000 simunetcore-0.0.9/simunetcore/model.py
+-rw-rw-rw-   0        0        0     7463 2022-11-10 11:29:47.000000 simunetcore-0.0.9/simunetcore/mqtt.py
+-rw-rw-rw-   0        0        0     6155 2022-11-14 11:29:06.000000 simunetcore-0.0.9/simunetcore/plot.py
+-rw-rw-rw-   0        0        0     2762 2022-11-29 06:11:24.000000 simunetcore-0.0.9/simunetcore/rest.py
+-rw-rw-rw-   0        0        0     6245 2022-11-10 11:29:49.000000 simunetcore-0.0.9/simunetcore/serializer.py
+-rw-rw-rw-   0        0        0     2185 2022-11-08 08:33:52.000000 simunetcore-0.0.9/simunetcore/utils.py
+-rw-rw-rw-   0        0        0    29286 2022-12-01 06:59:04.000000 simunetcore-0.0.9/simunetcore/waveform.py
+drwxrwxrwx   0        0        0        0 2022-12-01 06:59:57.869852 simunetcore-0.0.9/simunetcore.egg-info/
+-rw-rw-rw-   0        0        0      510 2022-12-01 06:59:57.000000 simunetcore-0.0.9/simunetcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2022-12-01 06:59:57.000000 simunetcore-0.0.9/simunetcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-01 06:59:57.000000 simunetcore-0.0.9/simunetcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2022-12-01 06:59:57.000000 simunetcore-0.0.9/simunetcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-12-01 06:59:57.000000 simunetcore-0.0.9/simunetcore.egg-info/top_level.txt
```

### Comparing `simunetcore-0.0.8/LICENSE` & `simunetcore-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/pyproject.toml` & `simunetcore-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simunetcore"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Thorsten Wack", email="thorsten.wack@umsicht.fraunhofer.de" },
 ]
 description = "Co simulation package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simunetcore-0.0.8/simunetcore/__init__.py` & `simunetcore-0.0.9/simunetcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from simunetcore.mqtt import MQTTModel
 from simunetcore.aws import AWSModel
 from simunetcore.waveform import Waveform
 from simunetcore.factory import Factory
 
 __all__ = ["Serializer", "Model", "RESTModel", "MQTTModel", "AWSModel", "Waveform", "Factory"]
 __title__ = "simunetcore"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __license__ = "MIT License"
 __copyright__ = "core simunet team and contributors".format(datetime.date.today().year)
 
 # Set default logging handler to avoid "No handler found" warnings.
 import logging
 from logging import NullHandler
```

### Comparing `simunetcore-0.0.8/simunetcore/aws.py` & `simunetcore-0.0.9/simunetcore/aws.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/exception.py` & `simunetcore-0.0.9/simunetcore/exception.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/factory.py` & `simunetcore-0.0.9/simunetcore/factory.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/invoker.py` & `simunetcore-0.0.9/simunetcore/invoker.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/logger.py` & `simunetcore-0.0.9/simunetcore/logger.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/model.py` & `simunetcore-0.0.9/simunetcore/model.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/mqtt.py` & `simunetcore-0.0.9/simunetcore/mqtt.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/plot.py` & `simunetcore-0.0.9/simunetcore/plot.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/rest.py` & `simunetcore-0.0.9/simunetcore/rest.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/serializer.py` & `simunetcore-0.0.9/simunetcore/serializer.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/utils.py` & `simunetcore-0.0.9/simunetcore/utils.py`

 * *Files identical despite different names*

### Comparing `simunetcore-0.0.8/simunetcore/waveform.py` & `simunetcore-0.0.9/simunetcore/waveform.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,17 +395,21 @@
         Raises
         ------
         `ComputeError` if something went wrong.
 
         """
 
         try:
-            # Get model and client from dictionary
+            # Get model from dictionary
             model = self.models[model_id]
-            kwargs = self.compute_kwargs[model_id] if model_id in self.compute_kwargs else {}
+            
+            # Get compute args for the model
+            kwargs = {} 
+            if model_id in self.compute_kwargs:
+                kwargs = self.compute_kwargs[model_id]
 
             # Perform computation
             if model.threadsafe:
                 model.compute(
                     simulation_id=self.simulation_id, 
                     model_id=model_id, 
                     **kwargs)
@@ -629,27 +633,28 @@
 
         # Call user callback function if provided
         if self.on_simulation_started != None:
             self.on_simulation_started(self)
 
         # print job properties
         if verbose:
-            msg = "Waveform '{}' using '{}' base steps.\n".format(self.simulation_id, step_type)
-            msg += "    t_start = {}\n".format(t_start)
-            msg += "    t_end = {}\n".format(t_end)
-            msg += "    frame_length = {}\n".format(frame_length)
-            msg += "    min_frame_length = {}\n".format(min_frame_length)
-            msg += "    max_frame_length = {}\n".format(max_frame_length)
-            msg += "    max_iter_frame  = {}\n".format(max_iter_frame)
-            msg += "    points_per_frame = {}\n".format(points_per_frame)
-            msg += "    max_iter  = {}\n".format(max_iter)
-            msg += "    iter_threshold = {}\n".format(iter_threshold)
-            msg += "    alpha  = {}\n".format(alpha)
-            msg += "    beta  = {}\n".format(beta)
-            msg += "    epsilon = {}".format(epsilon)
+            msg = "Starting '{}'\n".format(self.simulation_id)
+            msg += "    t_start = {:.3E}\n".format(self.t_start)
+            msg += "    t_end = {:.3E}\n".format(self.t_end)
+            msg += "    frame_length = {:.3E}\n".format(self.frame_length)
+            msg += "    min_frame_length = {:.3E}\n".format(self.min_frame_length)
+            msg += "    max_frame_length = {:.3E}\n".format(self.max_frame_length)
+            msg += "    max_iter_frame  = {:d}\n".format(self.max_iter_frame)
+            msg += "    points_per_frame = {:d}\n".format(self.points_per_frame)
+            msg += "    max_iter = {:d}\n".format(self.max_iter)
+            msg += "    iter_threshold = {:d}\n".format(self.iter_threshold)
+            msg += "    alpha = {:.3E}\n".format(self.alpha)
+            msg += "    beta = {:.3E}\n".format(self.beta)
+            msg += "    epsilon = {:.3E}\n".format(self.epsilon)
+            msg += "    base steps = {}".format(self.step_type)
             print(msg)
             
         # Prepare the frames list holding the results for each frame
         if len(self.frames) > 0:
             self.models = copy.deepcopy(self.frames[0])
             self.num_iter_all = 0
             self.num_iter_used = 0
```

