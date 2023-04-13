# Comparing `tmp/pyroundtrip-2.0.0.tar.gz` & `tmp/pyroundtrip-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroundtrip-2.0.0.tar", last modified: Wed Apr 12 19:48:54 2023, max compression
+gzip compressed data, was "dist/pyroundtrip-2.0.1.tar", last modified: Thu Apr 13 21:22:57 2023, max compression
```

## Comparing `pyroundtrip-2.0.0.tar` & `pyroundtrip-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-12 19:48:54.000000 pyroundtrip-2.0.0/
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1068 2023-04-12 19:32:18.000000 pyroundtrip-2.0.0/LICENSE
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1547 2023-04-12 19:48:54.000000 pyroundtrip-2.0.0/PKG-INFO
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1119 2023-04-11 18:45:46.000000 pyroundtrip-2.0.0/README.md
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-12 19:48:53.000000 pyroundtrip-2.0.0/pyroundtrip/
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      216 2023-04-11 18:52:12.000000 pyroundtrip-2.0.0/pyroundtrip/__init__.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       69 2023-04-11 19:06:15.000000 pyroundtrip-2.0.0/pyroundtrip/__main__.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     5130 2023-04-12 18:18:59.000000 pyroundtrip-2.0.0/pyroundtrip/cli.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    10122 2023-04-11 18:47:43.000000 pyroundtrip-2.0.0/pyroundtrip/model.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    76306 2023-04-12 18:20:07.000000 pyroundtrip-2.0.0/pyroundtrip/roundtrip.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    27480 2023-04-12 18:17:21.000000 pyroundtrip-2.0.0/pyroundtrip/util.py
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-12 19:48:53.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1547 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/PKG-INFO
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      371 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/SOURCES.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)        1 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/dependency_links.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       51 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/entry_points.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       54 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/requires.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       12 2023-04-12 19:48:52.000000 pyroundtrip-2.0.0/pyroundtrip.egg-info/top_level.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       38 2023-04-12 19:48:54.000000 pyroundtrip-2.0.0/setup.cfg
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1882 2023-04-12 19:48:23.000000 pyroundtrip-2.0.0/setup.py
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-13 21:22:57.000000 pyroundtrip-2.0.1/
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1068 2023-04-12 19:32:18.000000 pyroundtrip-2.0.1/LICENSE
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1547 2023-04-13 21:22:57.000000 pyroundtrip-2.0.1/PKG-INFO
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1119 2023-04-11 18:45:46.000000 pyroundtrip-2.0.1/README.md
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-13 21:22:57.000000 pyroundtrip-2.0.1/pyroundtrip/
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      248 2023-04-13 21:21:44.000000 pyroundtrip-2.0.1/pyroundtrip/__init__.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       69 2023-04-11 19:06:15.000000 pyroundtrip-2.0.1/pyroundtrip/__main__.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     5130 2023-04-12 18:18:59.000000 pyroundtrip-2.0.1/pyroundtrip/cli.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    10122 2023-04-11 18:47:43.000000 pyroundtrip-2.0.1/pyroundtrip/model.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    76306 2023-04-12 18:20:07.000000 pyroundtrip-2.0.1/pyroundtrip/roundtrip.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    27480 2023-04-12 18:17:21.000000 pyroundtrip-2.0.1/pyroundtrip/util.py
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-04-13 21:22:57.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1547 2023-04-13 21:22:55.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/PKG-INFO
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      371 2023-04-13 21:22:56.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/SOURCES.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)        1 2023-04-13 21:22:55.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/dependency_links.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       51 2023-04-13 21:22:56.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/entry_points.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       54 2023-04-13 21:22:56.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/requires.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       12 2023-04-13 21:22:56.000000 pyroundtrip-2.0.1/pyroundtrip.egg-info/top_level.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       38 2023-04-13 21:22:57.000000 pyroundtrip-2.0.1/setup.cfg
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1882 2023-04-13 21:21:54.000000 pyroundtrip-2.0.1/setup.py
```

### Comparing `pyroundtrip-2.0.0/LICENSE` & `pyroundtrip-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/PKG-INFO` & `pyroundtrip-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroundtrip
-Version: 2.0.0
+Version: 2.0.1
 Summary: Roundtrip: density estimation with deep generative neural networks
 Home-page: https://github.com/kimmo1019/Roundtrip
 Author: Qiao Liu
 Author-email: liuqiao@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroundtrip-2.0.0/README.md` & `pyroundtrip-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/pyroundtrip/cli.py` & `pyroundtrip-2.0.1/pyroundtrip/cli.py`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/pyroundtrip/model.py` & `pyroundtrip-2.0.1/pyroundtrip/model.py`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/pyroundtrip/roundtrip.py` & `pyroundtrip-2.0.1/pyroundtrip/roundtrip.py`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/pyroundtrip/util.py` & `pyroundtrip-2.0.1/pyroundtrip/util.py`

 * *Files identical despite different names*

### Comparing `pyroundtrip-2.0.0/pyroundtrip.egg-info/PKG-INFO` & `pyroundtrip-2.0.1/pyroundtrip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroundtrip
-Version: 2.0.0
+Version: 2.0.1
 Summary: Roundtrip: density estimation with deep generative neural networks
 Home-page: https://github.com/kimmo1019/Roundtrip
 Author: Qiao Liu
 Author-email: liuqiao@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroundtrip-2.0.0/setup.py` & `pyroundtrip-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pyroundtrip", 
-    version="2.0.0",
+    version="2.0.1",
     author="Qiao Liu",
     author_email="liuqiao@stanford.edu",
     description="Roundtrip: density estimation with deep generative neural networks",
     long_description="Density estimation is one of the fundamental problems in both statistics and machine learning. In this study, we propose Roundtrip, a computational framework for general-purpose density estimation based on deep generative neural networks. Roundtrip retains the generative power of deep generative models, such as generative adversarial networks (GANs) while it also provides estimates of density values, thus supporting both data generation and density estimation. Unlike previous neural density estimators that put stringent conditions on the transformation from the latent space to the data space, Roundtrip enables the use of much more general mappings where target density is modeled by learning a manifold induced from a base density (e.g., Gaussian distribution). Roundtrip provides a statistical framework for GAN models where an explicit evaluation of density values is feasible. In numerical experiments, Roundtrip exceeds state-of-the-art performance in a diverse range of density estimation tasks. Roundtrip is freely available at https://github.com/kimmo1019/Roundtrip.",
     long_description_content_type="text/markdown",
     url="https://github.com/kimmo1019/Roundtrip",
     packages=setuptools.find_packages(),
```

