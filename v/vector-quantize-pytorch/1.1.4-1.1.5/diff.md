# Comparing `tmp/vector_quantize_pytorch-1.1.4.tar.gz` & `tmp/vector_quantize_pytorch-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.1.4.tar", last modified: Wed Apr 12 20:09:51 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.1.5.tar", last modified: Thu Apr 13 20:21:35 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.1.4.tar` & `vector_quantize_pytorch-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.841647 vector_quantize_pytorch-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:09:51.841647 vector_quantize_pytorch-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-04-13 20:21:25.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:35.231237 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 20:21:35.000000 vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.1.4/LICENSE` & `vector_quantize_pytorch-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.4/PKG-INFO` & `vector_quantize_pytorch-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.1.4
+Version: 1.1.5
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.1.4/README.md` & `vector_quantize_pytorch-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.4/setup.py` & `vector_quantize_pytorch-1.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.1.4',
+  version = '1.1.5',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,29 @@
     def __init__(
         self,
         *,
         dim,
         codebook_size,
         codebook_dim,
         num_codebooks = 1,
+        norm = True,
         **kwargs
     ):
         super().__init__()
         self.num_codebooks = num_codebooks
 
         rand_projs = torch.empty(num_codebooks, dim, codebook_dim)
         nn.init.xavier_normal_(rand_projs)
 
         self.register_buffer('rand_projs', rand_projs)
 
         # in section 3 of https://arxiv.org/abs/2202.01855
         # "The input data is normalized to have 0 mean and standard deviation of 1 ... to prevent collapse"
 
-        self.norm = nn.LayerNorm(dim, elementwise_affine = False)
+        self.norm = nn.LayerNorm(dim, elementwise_affine = False) if norm else nn.Identity()
 
         self.vq = VectorQuantize(
             dim = codebook_dim * num_codebooks,
             heads = num_codebooks,
             codebook_size = codebook_size,
             use_cosine_sim = True,
             separate_codebook_per_head = True,
```

### Comparing `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.1.5/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.1.4
+Version: 1.1.5
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

