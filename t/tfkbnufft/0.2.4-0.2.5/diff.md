# Comparing `tmp/tfkbnufft-0.2.4.tar.gz` & `tmp/tfkbnufft-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfkbnufft-0.2.4.tar", last modified: Fri Jul 23 15:29:38 2021, max compression
+gzip compressed data, was "tfkbnufft-0.2.5.tar", last modified: Thu Apr 13 08:32:31 2023, max compression
```

## Comparing `tfkbnufft-0.2.4.tar` & `tfkbnufft-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/kbmodule.py
--rw-r--r--   0 runner    (1001) docker     (121)    12827 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/kbnufft.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/mri/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/mri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5705 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/mri/dcomp_calc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/nufft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/nufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9036 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/nufft/fft_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9937 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/nufft/interp_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6899 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/nufft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/kbnufft_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/ndft_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/tests/nufft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/nufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6184 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/nufft/fft_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7485 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/nufft/interp_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-07-23 15:29:28.000000 tfkbnufft-0.2.4/tfkbnufft/utils/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 15:29:38.401592 tfkbnufft-0.2.4/tfkbnufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-23 15:29:38.000000 tfkbnufft-0.2.4/tfkbnufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.104227 tfkbnufft-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-13 08:32:31.104227 tfkbnufft-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:32:31.104227 tfkbnufft-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.100227 tfkbnufft-0.2.5/tfkbnufft/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/kbmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/kbnufft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.100227 tfkbnufft-0.2.5/tfkbnufft/mri/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/mri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/mri/dcomp_calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.100227 tfkbnufft-0.2.5/tfkbnufft/nufft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/nufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/nufft/fft_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/nufft/interp_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/nufft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.100227 tfkbnufft-0.2.5/tfkbnufft/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/kbnufft_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/ndft_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.104227 tfkbnufft-0.2.5/tfkbnufft/tests/nufft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/nufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/nufft/fft_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/nufft/interp_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.104227 tfkbnufft-0.2.5/tfkbnufft/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 08:32:19.000000 tfkbnufft-0.2.5/tfkbnufft/utils/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:32:31.100227 tfkbnufft-0.2.5/tfkbnufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:32:31.000000 tfkbnufft-0.2.5/tfkbnufft.egg-info/top_level.txt
```

### Comparing `tfkbnufft-0.2.4/LICENSE` & `tfkbnufft-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/PKG-INFO` & `tfkbnufft-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tfkbnufft
-Version: 0.2.4
+Version: 0.2.5
 Summary: A robust, easy-to-deploy non-uniform Fast Fourier Transform in TensorFlow.
 Home-page: https://github.com/zaccharieramzi/tfkbnufft
+Download-URL: https://github.com/zaccharieramzi/tfkbnufft
 Author: Zaccharie Ramzi
 Author-email: zaccharie.ramzi@inria.fr
 License: MIT
-Download-URL: https://github.com/zaccharieramzi/tfkbnufft
 Keywords: MRI,tensorflow
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -89,9 +88,7 @@
   title = {Torch KB-NUFFT},
   year = {2019},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mmuckley/torchkbnufft}}
 }
 ```
-
-
```

### Comparing `tfkbnufft-0.2.4/README.md` & `tfkbnufft-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/setup.py` & `tfkbnufft-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/__init__.py` & `tfkbnufft-0.2.5/tfkbnufft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Package info"""
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = 'Zaccharie Ramzi'
 __author_email__ = 'zaccharie.ramzi@inria.fr'
 __license__ = 'MIT'
 __homepage__ = 'https://github.com/zaccharieramzi/tfkbnufft'
 __docs__ = 'A robust, easy-to-deploy non-uniform Fast Fourier Transform in TensorFlow.'
 
 try:
```

### Comparing `tfkbnufft-0.2.4/tfkbnufft/kbmodule.py` & `tfkbnufft-0.2.5/tfkbnufft/kbmodule.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/kbnufft.py` & `tfkbnufft-0.2.5/tfkbnufft/kbnufft.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/mri/dcomp_calc.py` & `tfkbnufft-0.2.5/tfkbnufft/mri/dcomp_calc.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/nufft/fft_functions.py` & `tfkbnufft-0.2.5/tfkbnufft/nufft/fft_functions.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/nufft/interp_functions.py` & `tfkbnufft-0.2.5/tfkbnufft/nufft/interp_functions.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/nufft/utils.py` & `tfkbnufft-0.2.5/tfkbnufft/nufft/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # calculate interpolation coefficients using kb kernel
     def interp_coeff(om, npts, grdsz, alpha, order):
         gam = 2 * np.pi / grdsz
         interp_dist = om / gam - np.floor(om / gam - npts / 2)
         Jvec = np.reshape(np.array(range(1, npts + 1)), (1, npts))
         kern_in = -1 * Jvec + np.expand_dims(interp_dist, 1)
 
-        cur_coeff = np.zeros(shape=kern_in.shape, dtype=np.complex)
+        cur_coeff = np.zeros(shape=kern_in.shape, dtype=np.complex64)
         indices = abs(kern_in) < npts / 2
         bess_arg = np.sqrt(1 - (kern_in[indices] / (npts / 2))**2)
         denom = special.iv(order, alpha)
         cur_coeff[indices] = special.iv(order, alpha * bess_arg) / denom
         cur_coeff = np.real(cur_coeff)
 
         return cur_coeff, kern_in
```

### Comparing `tfkbnufft-0.2.4/tfkbnufft/tests/kbnufft_test.py` & `tfkbnufft-0.2.5/tfkbnufft/tests/kbnufft_test.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/tests/ndft_test.py` & `tfkbnufft-0.2.5/tfkbnufft/tests/ndft_test.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/tests/nufft/fft_functions_test.py` & `tfkbnufft-0.2.5/tfkbnufft/tests/nufft/fft_functions_test.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/tests/nufft/interp_functions_test.py` & `tfkbnufft-0.2.5/tfkbnufft/tests/nufft/interp_functions_test.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft/tests/utils.py` & `tfkbnufft-0.2.5/tfkbnufft/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tfkbnufft-0.2.4/tfkbnufft.egg-info/PKG-INFO` & `tfkbnufft-0.2.5/tfkbnufft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tfkbnufft
-Version: 0.2.4
+Version: 0.2.5
 Summary: A robust, easy-to-deploy non-uniform Fast Fourier Transform in TensorFlow.
 Home-page: https://github.com/zaccharieramzi/tfkbnufft
+Download-URL: https://github.com/zaccharieramzi/tfkbnufft
 Author: Zaccharie Ramzi
 Author-email: zaccharie.ramzi@inria.fr
 License: MIT
-Download-URL: https://github.com/zaccharieramzi/tfkbnufft
 Keywords: MRI,tensorflow
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -89,9 +88,7 @@
   title = {Torch KB-NUFFT},
   year = {2019},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mmuckley/torchkbnufft}}
 }
 ```
-
-
```

### Comparing `tfkbnufft-0.2.4/tfkbnufft.egg-info/SOURCES.txt` & `tfkbnufft-0.2.5/tfkbnufft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

