# Comparing `tmp/metnet-4.1.8.tar.gz` & `tmp/metnet-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metnet-4.1.8.tar", last modified: Wed Nov 16 11:05:23 2022, max compression
+gzip compressed data, was "metnet-4.1.9.tar", last modified: Mon Feb 13 08:25:01 2023, max compression
```

## Comparing `metnet-4.1.8.tar` & `metnet-4.1.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 11:05:23.235072 metnet-4.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-11-16 11:05:04.000000 metnet-4.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-16 11:05:04.000000 metnet-4.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-11-16 11:05:23.235072 metnet-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-11-16 11:05:04.000000 metnet-4.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 11:05:23.231072 metnet-4.1.8/metnet/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 11:05:23.231072 metnet-4.1.8/metnet/layers/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/ConditionTime.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/ConditionWithTimeMetNet2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7852 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/ConvGRU.py
--rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/ConvLSTM.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/CoordConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/DilatedCondConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/DownSampler.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/LeadTimeConditioner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/TimeDistributed.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/layers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 11:05:23.231072 metnet-4.1.8/metnet/models/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/models/metnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    11460 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/models/metnet2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5735 2022-11-16 11:05:04.000000 metnet-4.1.8/metnet/models/metnet_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 11:05:23.231072 metnet-4.1.8/metnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-11-16 11:05:23.000000 metnet-4.1.8/metnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-11-16 11:05:23.000000 metnet-4.1.8/metnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 11:05:23.000000 metnet-4.1.8/metnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-16 11:05:23.000000 metnet-4.1.8/metnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-16 11:05:23.000000 metnet-4.1.8/metnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-16 11:05:04.000000 metnet-4.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 11:05:23.235072 metnet-4.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-16 11:05:06.000000 metnet-4.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-13 08:24:45.000000 metnet-4.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-13 08:24:45.000000 metnet-4.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-02-13 08:25:01.384585 metnet-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-02-13 08:24:45.000000 metnet-4.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/metnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/metnet/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/ConditionTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/ConditionWithTimeMetNet2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/ConvGRU.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/ConvLSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/CoordConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/DilatedCondConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/DownSampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/LeadTimeConditioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/TimeDistributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/layers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/metnet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/models/metnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/models/metnet2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-02-13 08:24:45.000000 metnet-4.1.9/metnet/models/metnet_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/metnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-02-13 08:25:01.000000 metnet-4.1.9/metnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-13 08:25:01.000000 metnet-4.1.9/metnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 08:25:01.000000 metnet-4.1.9/metnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-13 08:25:01.000000 metnet-4.1.9/metnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-13 08:25:01.000000 metnet-4.1.9/metnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-13 08:24:45.000000 metnet-4.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 08:25:01.388585 metnet-4.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-13 08:24:46.000000 metnet-4.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:25:01.384585 metnet-4.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-02-13 08:24:45.000000 metnet-4.1.9/tests/test_model.py
```

### Comparing `metnet-4.1.8/LICENSE` & `metnet-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/PKG-INFO` & `metnet-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metnet
-Version: 4.1.8
+Version: 4.1.9
 Summary: PyTorch MetNet Implementation
 Home-page: https://github.com/openclimatefix/metnet
 Author: Jacob Bieker
 Author-email: jacob@openclimatefix.org
 License: MIT License
 Keywords: artificial intelligence,deep learning,transformer,attention mechanism,metnet,forecasting,remote-sensing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metnet-4.1.8/README.md` & `metnet-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/ConditionTime.py` & `metnet-4.1.9/metnet/layers/ConditionTime.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/ConditionWithTimeMetNet2.py` & `metnet-4.1.9/metnet/layers/ConditionWithTimeMetNet2.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/ConvGRU.py` & `metnet-4.1.9/metnet/layers/ConvGRU.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/ConvLSTM.py` & `metnet-4.1.9/metnet/layers/ConvLSTM.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/CoordConv.py` & `metnet-4.1.9/metnet/layers/CoordConv.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/DilatedCondConv.py` & `metnet-4.1.9/metnet/layers/DilatedCondConv.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/DownSampler.py` & `metnet-4.1.9/metnet/layers/DownSampler.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/LeadTimeConditioner.py` & `metnet-4.1.9/metnet/layers/LeadTimeConditioner.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/Preprocessor.py` & `metnet-4.1.9/metnet/layers/Preprocessor.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/layers/TimeDistributed.py` & `metnet-4.1.9/metnet/layers/TimeDistributed.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/models/metnet.py` & `metnet-4.1.9/metnet/models/metnet.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/models/metnet2.py` & `metnet-4.1.9/metnet/models/metnet2.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet/models/metnet_pv.py` & `metnet-4.1.9/metnet/models/metnet_pv.py`

 * *Files identical despite different names*

### Comparing `metnet-4.1.8/metnet.egg-info/PKG-INFO` & `metnet-4.1.9/metnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metnet
-Version: 4.1.8
+Version: 4.1.9
 Summary: PyTorch MetNet Implementation
 Home-page: https://github.com/openclimatefix/metnet
 Author: Jacob Bieker
 Author-email: jacob@openclimatefix.org
 License: MIT License
 Keywords: artificial intelligence,deep learning,transformer,attention mechanism,metnet,forecasting,remote-sensing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metnet-4.1.8/metnet.egg-info/SOURCES.txt` & `metnet-4.1.9/metnet.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 metnet/layers/Preprocessor.py
 metnet/layers/TimeDistributed.py
 metnet/layers/__init__.py
 metnet/layers/utils.py
 metnet/models/__init__.py
 metnet/models/metnet.py
 metnet/models/metnet2.py
-metnet/models/metnet_pv.py
+metnet/models/metnet_pv.py
+tests/test_model.py
```

### Comparing `metnet-4.1.8/setup.py` & `metnet-4.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = Path(__file__).parent
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="metnet",
-    version="4.1.8",
+    version="4.1.9",
     packages=find_packages(),
     url="https://github.com/openclimatefix/metnet",
     license="MIT License",
     company="Open Climate Fix Ltd",
     author="Jacob Bieker",
     author_email="jacob@openclimatefix.org",
     description="PyTorch MetNet Implementation",
```

