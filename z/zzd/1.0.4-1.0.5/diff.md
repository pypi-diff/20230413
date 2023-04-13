# Comparing `tmp/zzd-1.0.4.tar.gz` & `tmp/zzd-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzd-1.0.4.tar", last modified: Sun Mar 19 11:03:07 2023, max compression
+gzip compressed data, was "zzd-1.0.5.tar", last modified: Thu Apr 13 09:12:25 2023, max compression
```

## Comparing `zzd-1.0.4.tar` & `zzd-1.0.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.781128 zzd-1.0.4/
--rw-r--r--   0 v         (1003) v         (1003)     1077 2022-07-08 07:33:48.000000 zzd-1.0.4/LICENSE
--rw-rw-r--   0 v         (1003) v         (1003)      418 2023-03-19 11:03:07.781128 zzd-1.0.4/PKG-INFO
--rw-r--r--   0 v         (1003) v         (1003)       45 2023-02-21 13:15:51.000000 zzd-1.0.4/README.md
--rw-rw-r--   0 v         (1003) v         (1003)       38 2023-03-19 11:03:07.781128 zzd-1.0.4/setup.cfg
--rw-r--r--   0 v         (1003) v         (1003)      580 2023-03-19 11:03:04.000000 zzd-1.0.4/setup.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.777128 zzd-1.0.4/zzd/
--rw-r--r--   0 v         (1003) v         (1003)       87 2022-10-27 08:38:38.000000 zzd-1.0.4/zzd/__init__.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.777128 zzd-1.0.4/zzd/feature_encode/
--rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-25 10:53:48.000000 zzd-1.0.4/zzd/feature_encode/__init__.py
--rw-r--r--   0 v         (1003) v         (1003)      916 2022-06-14 05:03:52.000000 zzd-1.0.4/zzd/feature_encode/ac.py
--rw-r--r--   0 v         (1003) v         (1003)      410 2022-06-14 05:04:43.000000 zzd-1.0.4/zzd/feature_encode/cksaap.py
--rw-rw-r--   0 v         (1003) v         (1003)      666 2022-06-14 05:04:15.000000 zzd-1.0.4/zzd/feature_encode/ct.py
--rw-r--r--   0 v         (1003) v         (1003)      356 2022-06-14 05:04:07.000000 zzd-1.0.4/zzd/feature_encode/dpc.py
--rw-r--r--   0 v         (1003) v         (1003)      238 2023-02-16 07:58:22.000000 zzd-1.0.4/zzd/feature_encode/encodes.py
--rw-rw-r--   0 v         (1003) v         (1003)      539 2022-05-26 11:32:25.000000 zzd-1.0.4/zzd/feature_encode/onehot.py
--rw-r--r--   0 v         (1003) v         (1003)     8246 2022-06-23 11:08:32.000000 zzd-1.0.4/zzd/feature_encode/pdb2graph.py
--rw-r--r--   0 v         (1003) v         (1003)     8639 2022-07-10 06:26:11.000000 zzd-1.0.4/zzd/feature_encode/pdb2graph_rd2.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.777128 zzd-1.0.4/zzd/methods/
--rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-24 18:43:17.000000 zzd-1.0.4/zzd/methods/ddi.py
--rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-24 18:43:23.000000 zzd-1.0.4/zzd/methods/dmi.py
--rw-rw-r--   0 v         (1003) v         (1003)     5762 2022-05-25 11:02:00.000000 zzd-1.0.4/zzd/methods/interolog.py
--rw-rw-r--   0 v         (1003) v         (1003)      103 2022-05-25 13:23:30.000000 zzd-1.0.4/zzd/methods/ppi.py
--rw-rw-r--   0 v         (1003) v         (1003)     1499 2022-05-26 08:58:40.000000 zzd-1.0.4/zzd/methods/ppi_bayesian.py
--rw-rw-r--   0 v         (1003) v         (1003)      129 2022-05-28 08:20:44.000000 zzd-1.0.4/zzd/methods/ppi_ddi.py
--rw-rw-r--   0 v         (1003) v         (1003)     5802 2022-05-28 08:15:09.000000 zzd-1.0.4/zzd/methods/ppi_interolog.py
--rw-rw-r--   0 v         (1003) v         (1003)     1528 2022-05-26 08:45:30.000000 zzd-1.0.4/zzd/methods/ppi_knn.py
--rw-rw-r--   0 v         (1003) v         (1003)     1484 2022-05-26 08:57:59.000000 zzd-1.0.4/zzd/methods/ppi_logistic.py
--rw-rw-r--   0 v         (1003) v         (1003)     2852 2022-06-14 06:53:08.000000 zzd-1.0.4/zzd/methods/ppi_randomforest.py
--rw-rw-r--   0 v         (1003) v         (1003)     1536 2022-05-26 08:59:16.000000 zzd-1.0.4/zzd/methods/ppi_svm.py
--rw-rw-r--   0 v         (1003) v         (1003)     1541 2022-05-26 08:59:28.000000 zzd-1.0.4/zzd/methods/ppi_xgboost.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.777128 zzd-1.0.4/zzd/models/
--rw-rw-r--   0 v         (1003) v         (1003)     1701 2022-05-16 11:30:17.000000 zzd-1.0.4/zzd/models/tf_cnn.py
--rw-rw-r--   0 v         (1003) v         (1003)     3384 2022-05-26 13:47:40.000000 zzd-1.0.4/zzd/models/torch_cnn.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.781128 zzd-1.0.4/zzd/utils/
--rw-r--r--   0 v         (1003) v         (1003)       67 2022-05-25 10:16:08.000000 zzd-1.0.4/zzd/utils/__init__.py
--rw-r--r--   0 v         (1003) v         (1003)     4936 2023-03-19 09:06:08.000000 zzd-1.0.4/zzd/utils/assess.py
--rw-r--r--   0 v         (1003) v         (1003)        0 2022-05-10 13:14:15.000000 zzd-1.0.4/zzd/utils/curve_train_hist.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.781128 zzd-1.0.4/zzd/utils/pdb/
--rw-rw-r--   0 v         (1003) v         (1003)        0 2022-06-09 07:27:50.000000 zzd-1.0.4/zzd/utils/pdb/__init__.py
--rw-rw-r--   0 v         (1003) v         (1003)     2493 2022-06-09 07:58:17.000000 zzd-1.0.4/zzd/utils/pdb/get_Ca_distance.py
--rw-rw-r--   0 v         (1003) v         (1003)      590 2022-06-09 08:14:38.000000 zzd-1.0.4/zzd/utils/pdb/get_sasa.py
--rw-rw-r--   0 v         (1003) v         (1003)     1146 2022-06-09 07:36:14.000000 zzd-1.0.4/zzd/utils/pdb/get_sec_struct.py
--rw-r--r--   0 v         (1003) v         (1003)     5198 2023-03-19 10:51:42.000000 zzd-1.0.4/zzd/utils/prc.py
--rw-r--r--   0 v         (1003) v         (1003)     5982 2023-03-19 07:47:45.000000 zzd-1.0.4/zzd/utils/roc.py
-drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-03-19 11:03:07.777128 zzd-1.0.4/zzd.egg-info/
--rw-r--r--   0 v         (1003) v         (1003)      418 2023-03-19 11:03:07.000000 zzd-1.0.4/zzd.egg-info/PKG-INFO
--rw-r--r--   0 v         (1003) v         (1003)      976 2023-03-19 11:03:07.000000 zzd-1.0.4/zzd.egg-info/SOURCES.txt
--rw-r--r--   0 v         (1003) v         (1003)        1 2023-03-19 11:03:07.000000 zzd-1.0.4/zzd.egg-info/dependency_links.txt
--rw-r--r--   0 v         (1003) v         (1003)        4 2023-03-19 11:03:07.000000 zzd-1.0.4/zzd.egg-info/top_level.txt
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/
+-rw-r--r--   0 v         (1003) v         (1003)     1077 2022-07-08 07:33:48.000000 zzd-1.0.5/LICENSE
+-rw-rw-r--   0 v         (1003) v         (1003)      418 2023-04-13 09:12:25.356592 zzd-1.0.5/PKG-INFO
+-rw-r--r--   0 v         (1003) v         (1003)       45 2023-02-21 13:15:51.000000 zzd-1.0.5/README.md
+-rw-rw-r--   0 v         (1003) v         (1003)       38 2023-04-13 09:12:25.356592 zzd-1.0.5/setup.cfg
+-rw-r--r--   0 v         (1003) v         (1003)      580 2023-04-13 09:12:16.000000 zzd-1.0.5/setup.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/
+-rw-r--r--   0 v         (1003) v         (1003)       87 2022-10-27 08:38:38.000000 zzd-1.0.5/zzd/__init__.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/feature_encode/
+-rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-25 10:53:48.000000 zzd-1.0.5/zzd/feature_encode/__init__.py
+-rw-r--r--   0 v         (1003) v         (1003)      916 2022-06-14 05:03:52.000000 zzd-1.0.5/zzd/feature_encode/ac.py
+-rw-r--r--   0 v         (1003) v         (1003)      410 2022-06-14 05:04:43.000000 zzd-1.0.5/zzd/feature_encode/cksaap.py
+-rw-rw-r--   0 v         (1003) v         (1003)      666 2022-06-14 05:04:15.000000 zzd-1.0.5/zzd/feature_encode/ct.py
+-rw-r--r--   0 v         (1003) v         (1003)      356 2022-06-14 05:04:07.000000 zzd-1.0.5/zzd/feature_encode/dpc.py
+-rw-r--r--   0 v         (1003) v         (1003)      238 2023-02-16 07:58:22.000000 zzd-1.0.5/zzd/feature_encode/encodes.py
+-rw-rw-r--   0 v         (1003) v         (1003)      539 2022-05-26 11:32:25.000000 zzd-1.0.5/zzd/feature_encode/onehot.py
+-rw-r--r--   0 v         (1003) v         (1003)     8246 2022-06-23 11:08:32.000000 zzd-1.0.5/zzd/feature_encode/pdb2graph.py
+-rw-r--r--   0 v         (1003) v         (1003)     8639 2022-07-10 06:26:11.000000 zzd-1.0.5/zzd/feature_encode/pdb2graph_rd2.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/methods/
+-rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-24 18:43:17.000000 zzd-1.0.5/zzd/methods/ddi.py
+-rw-rw-r--   0 v         (1003) v         (1003)        0 2022-05-24 18:43:23.000000 zzd-1.0.5/zzd/methods/dmi.py
+-rw-rw-r--   0 v         (1003) v         (1003)     5762 2022-05-25 11:02:00.000000 zzd-1.0.5/zzd/methods/interolog.py
+-rw-rw-r--   0 v         (1003) v         (1003)      103 2022-05-25 13:23:30.000000 zzd-1.0.5/zzd/methods/ppi.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1499 2022-05-26 08:58:40.000000 zzd-1.0.5/zzd/methods/ppi_bayesian.py
+-rw-rw-r--   0 v         (1003) v         (1003)      129 2022-05-28 08:20:44.000000 zzd-1.0.5/zzd/methods/ppi_ddi.py
+-rw-rw-r--   0 v         (1003) v         (1003)     5802 2022-05-28 08:15:09.000000 zzd-1.0.5/zzd/methods/ppi_interolog.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1528 2022-05-26 08:45:30.000000 zzd-1.0.5/zzd/methods/ppi_knn.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1484 2022-05-26 08:57:59.000000 zzd-1.0.5/zzd/methods/ppi_logistic.py
+-rw-rw-r--   0 v         (1003) v         (1003)     2852 2022-06-14 06:53:08.000000 zzd-1.0.5/zzd/methods/ppi_randomforest.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1536 2022-05-26 08:59:16.000000 zzd-1.0.5/zzd/methods/ppi_svm.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1541 2022-05-26 08:59:28.000000 zzd-1.0.5/zzd/methods/ppi_xgboost.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/models/
+-rw-rw-r--   0 v         (1003) v         (1003)     1701 2022-05-16 11:30:17.000000 zzd-1.0.5/zzd/models/tf_cnn.py
+-rw-rw-r--   0 v         (1003) v         (1003)     3384 2022-05-26 13:47:40.000000 zzd-1.0.5/zzd/models/torch_cnn.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/utils/
+-rw-r--r--   0 v         (1003) v         (1003)       67 2022-05-25 10:16:08.000000 zzd-1.0.5/zzd/utils/__init__.py
+-rw-r--r--   0 v         (1003) v         (1003)     4936 2023-03-19 09:06:08.000000 zzd-1.0.5/zzd/utils/assess.py
+-rw-r--r--   0 v         (1003) v         (1003)        0 2022-05-10 13:14:15.000000 zzd-1.0.5/zzd/utils/curve_train_hist.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd/utils/pdb/
+-rw-rw-r--   0 v         (1003) v         (1003)        0 2022-06-09 07:27:50.000000 zzd-1.0.5/zzd/utils/pdb/__init__.py
+-rw-rw-r--   0 v         (1003) v         (1003)     2493 2022-06-09 07:58:17.000000 zzd-1.0.5/zzd/utils/pdb/get_Ca_distance.py
+-rw-rw-r--   0 v         (1003) v         (1003)      590 2022-06-09 08:14:38.000000 zzd-1.0.5/zzd/utils/pdb/get_sasa.py
+-rw-rw-r--   0 v         (1003) v         (1003)     1146 2022-06-09 07:36:14.000000 zzd-1.0.5/zzd/utils/pdb/get_sec_struct.py
+-rw-r--r--   0 v         (1003) v         (1003)     5198 2023-03-19 10:51:42.000000 zzd-1.0.5/zzd/utils/prc.py
+-rw-r--r--   0 v         (1003) v         (1003)     5982 2023-03-19 07:47:45.000000 zzd-1.0.5/zzd/utils/roc.py
+-rw-rw-r--   0 v         (1003) v         (1003)      258 2023-04-13 09:11:05.000000 zzd-1.0.5/zzd/utils/seq.py
+drwxrwxr-x   0 v         (1003) v         (1003)        0 2023-04-13 09:12:25.356592 zzd-1.0.5/zzd.egg-info/
+-rw-r--r--   0 v         (1003) v         (1003)      418 2023-04-13 09:12:25.000000 zzd-1.0.5/zzd.egg-info/PKG-INFO
+-rw-r--r--   0 v         (1003) v         (1003)      993 2023-04-13 09:12:25.000000 zzd-1.0.5/zzd.egg-info/SOURCES.txt
+-rw-r--r--   0 v         (1003) v         (1003)        1 2023-04-13 09:12:25.000000 zzd-1.0.5/zzd.egg-info/dependency_links.txt
+-rw-r--r--   0 v         (1003) v         (1003)        4 2023-04-13 09:12:25.000000 zzd-1.0.5/zzd.egg-info/top_level.txt
```

### Comparing `zzd-1.0.4/LICENSE` & `zzd-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/setup.py` & `zzd-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zzd",
-    version="1.0.4",
+    version="1.0.5",
     author="ChenPing L", 
 	author_email="1965770446@qq.com",
     description="some tools", 
 	long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miderxi/zzd_lib",
     packages=setuptools.find_packages(),
```

### Comparing `zzd-1.0.4/zzd/feature_encode/ac.py` & `zzd-1.0.5/zzd/feature_encode/ac.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/feature_encode/ct.py` & `zzd-1.0.5/zzd/feature_encode/ct.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/feature_encode/onehot.py` & `zzd-1.0.5/zzd/feature_encode/onehot.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/feature_encode/pdb2graph.py` & `zzd-1.0.5/zzd/feature_encode/pdb2graph.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/feature_encode/pdb2graph_rd2.py` & `zzd-1.0.5/zzd/feature_encode/pdb2graph_rd2.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/interolog.py` & `zzd-1.0.5/zzd/methods/interolog.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_bayesian.py` & `zzd-1.0.5/zzd/methods/ppi_bayesian.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_interolog.py` & `zzd-1.0.5/zzd/methods/ppi_interolog.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_knn.py` & `zzd-1.0.5/zzd/methods/ppi_knn.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_logistic.py` & `zzd-1.0.5/zzd/methods/ppi_logistic.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_randomforest.py` & `zzd-1.0.5/zzd/methods/ppi_randomforest.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_svm.py` & `zzd-1.0.5/zzd/methods/ppi_svm.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/methods/ppi_xgboost.py` & `zzd-1.0.5/zzd/methods/ppi_xgboost.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/models/tf_cnn.py` & `zzd-1.0.5/zzd/models/tf_cnn.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/models/torch_cnn.py` & `zzd-1.0.5/zzd/models/torch_cnn.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/assess.py` & `zzd-1.0.5/zzd/utils/assess.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/pdb/get_Ca_distance.py` & `zzd-1.0.5/zzd/utils/pdb/get_Ca_distance.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/pdb/get_sasa.py` & `zzd-1.0.5/zzd/utils/pdb/get_sasa.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/pdb/get_sec_struct.py` & `zzd-1.0.5/zzd/utils/pdb/get_sec_struct.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/prc.py` & `zzd-1.0.5/zzd/utils/prc.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd/utils/roc.py` & `zzd-1.0.5/zzd/utils/roc.py`

 * *Files identical despite different names*

### Comparing `zzd-1.0.4/zzd.egg-info/SOURCES.txt` & `zzd-1.0.5/zzd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,11 +30,12 @@
 zzd/models/tf_cnn.py
 zzd/models/torch_cnn.py
 zzd/utils/__init__.py
 zzd/utils/assess.py
 zzd/utils/curve_train_hist.py
 zzd/utils/prc.py
 zzd/utils/roc.py
+zzd/utils/seq.py
 zzd/utils/pdb/__init__.py
 zzd/utils/pdb/get_Ca_distance.py
 zzd/utils/pdb/get_sasa.py
 zzd/utils/pdb/get_sec_struct.py
```

