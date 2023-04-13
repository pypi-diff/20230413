# Comparing `tmp/tensorflow-wavelets-1.0.8.tar.gz` & `tmp/tensorflow-wavelets-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\My Drive\Colab Notebooks\tensorflow-wavelets\dist\tmphxx8l0x2\tensorflow-wavelets-1.0.8.tar", last modified: Sat Sep 11 20:48:57 2021, max compression
+gzip compressed data, was "G:\My Drive\Colab Notebooks\tensorflow-wavelets\dist\tmp8kbsvtx1\tensorflow-wavelets-1.0.9.tar", last modified: Sat Sep 11 22:01:23 2021, max compression
```

## Comparing `tensorflow-wavelets-1.0.8.tar` & `tensorflow-wavelets-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/
--rw-rw-rw-   0        0        0     1083 2021-09-11 17:32:54.000000 tensorflow-wavelets-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      888 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      279 2021-09-11 19:32:39.000000 tensorflow-wavelets-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      879 2021-09-11 20:47:47.000000 tensorflow-wavelets-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DMWT/
--rw-rw-rw-   0        0        0     4646 2021-09-11 18:05:49.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DMWT/DMWT.py
--rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DMWT/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DTCWT/
--rw-rw-rw-   0        0        0     8585 2021-09-11 18:06:24.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DTCWT/DTCWT.py
--rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DTCWT/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DWT/
--rw-rw-rw-   0        0        0    12154 2021-09-11 18:07:27.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DWT/DWT.py
--rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DWT/__init__.py
--rw-rw-rw-   0        0        0        0 2021-09-11 19:26:50.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/__init__.py
--rw-rw-rw-   0        0        0        0 2021-09-11 19:27:43.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/
--rw-rw-rw-   0        0        0      888 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2021-09-11 20:48:57.000000 tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/
+-rw-rw-rw-   0        0        0     1083 2021-09-11 17:32:54.000000 tensorflow-wavelets-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1051 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2021-09-11 21:59:38.000000 tensorflow-wavelets-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      879 2021-09-11 21:59:44.000000 tensorflow-wavelets-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DMWT/
+-rw-rw-rw-   0        0        0     4646 2021-09-11 18:05:49.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DMWT/DMWT.py
+-rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DMWT/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DTCWT/
+-rw-rw-rw-   0        0        0     8585 2021-09-11 18:06:24.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DTCWT/DTCWT.py
+-rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DTCWT/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DWT/
+-rw-rw-rw-   0        0        0    12154 2021-09-11 18:07:27.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DWT/DWT.py
+-rw-rw-rw-   0        0        0        0 2021-09-11 18:39:57.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DWT/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-09-11 19:26:50.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-09-11 19:27:43.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/
+-rw-rw-rw-   0        0        0     1051 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2021-09-11 22:01:23.000000 tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/top_level.txt
```

### Comparing `tensorflow-wavelets-1.0.8/LICENSE` & `tensorflow-wavelets-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-wavelets-1.0.8/PKG-INFO` & `tensorflow-wavelets-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: tensorflow-wavelets
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tensorflow wavelet Layers
 Home-page: https://https://github.com/Timorleiderman/tensorflow-wavelets
 Author: Timor Leiderman
 Author-email: Timorleiderman@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Timorleiderman/tensorflow-wavelets/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# tensorflow-wavelets
-Multi Wavelets Transform Neural Networks Layer
-Duel Tree Complex Wavelets Transform Layer
-Discrete Wavelets Transform Layer
+tensorflow-wavelets is an implementation of
+- *Multi Wavelets Transform Neural Networks Layer*
+- *Duel Tree Complex Wavelets Transform Layer*
+- *Discrete Wavelets Transform Layer*
 
+## Installation
+
+```
+pip install tensorflow-wavelets
+```
 # Usage
-import tensorflow_wavelets.Layers.DWT
-import tensorflow_wavelets.Layers.DTCWT
-import tensorflow_wavelets.Layers.DMWT
+```
+import tensorflow_wavelets.Layers.DWT as DWT
+import tensorflow_wavelets.Layers.DTCWT as DTCWT
+import tensorflow_wavelets.Layers.DMWT as DMWT
+```
+
+**Free Software, Hell Yeah!**
```

### Comparing `tensorflow-wavelets-1.0.8/setup.py` & `tensorflow-wavelets-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tensorflow-wavelets",
-    version="1.0.8",
+    version="1.0.9",
     author="Timor Leiderman",
     author_email="Timorleiderman@gmail.com",
     description="Tensorflow wavelet Layers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://https://github.com/Timorleiderman/tensorflow-wavelets",
     project_urls={
```

### Comparing `tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DMWT/DMWT.py` & `tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DMWT/DMWT.py`

 * *Files identical despite different names*

### Comparing `tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DTCWT/DTCWT.py` & `tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DTCWT/DTCWT.py`

 * *Files identical despite different names*

### Comparing `tensorflow-wavelets-1.0.8/src/tensorflow_wavelets/Layers/DWT/DWT.py` & `tensorflow-wavelets-1.0.9/src/tensorflow_wavelets/Layers/DWT/DWT.py`

 * *Files identical despite different names*

### Comparing `tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/PKG-INFO` & `tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: tensorflow-wavelets
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tensorflow wavelet Layers
 Home-page: https://https://github.com/Timorleiderman/tensorflow-wavelets
 Author: Timor Leiderman
 Author-email: Timorleiderman@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Timorleiderman/tensorflow-wavelets/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# tensorflow-wavelets
-Multi Wavelets Transform Neural Networks Layer
-Duel Tree Complex Wavelets Transform Layer
-Discrete Wavelets Transform Layer
+tensorflow-wavelets is an implementation of
+- *Multi Wavelets Transform Neural Networks Layer*
+- *Duel Tree Complex Wavelets Transform Layer*
+- *Discrete Wavelets Transform Layer*
 
+## Installation
+
+```
+pip install tensorflow-wavelets
+```
 # Usage
-import tensorflow_wavelets.Layers.DWT
-import tensorflow_wavelets.Layers.DTCWT
-import tensorflow_wavelets.Layers.DMWT
+```
+import tensorflow_wavelets.Layers.DWT as DWT
+import tensorflow_wavelets.Layers.DTCWT as DTCWT
+import tensorflow_wavelets.Layers.DMWT as DMWT
+```
+
+**Free Software, Hell Yeah!**
```

### Comparing `tensorflow-wavelets-1.0.8/src/tensorflow_wavelets.egg-info/SOURCES.txt` & `tensorflow-wavelets-1.0.9/src/tensorflow_wavelets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

