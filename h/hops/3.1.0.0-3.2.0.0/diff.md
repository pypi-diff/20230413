# Comparing `tmp/hops-3.1.0.0.tar.gz` & `tmp/hops-3.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hops-3.1.0.0.tar", last modified: Thu Dec 22 18:23:59 2022, max compression
+gzip compressed data, was "dist/hops-3.2.0.0.tar", last modified: Thu Apr 13 09:39:39 2023, max compression
```

## Comparing `hops-3.1.0.0.tar` & `hops-3.2.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1795 2022-12-22 18:23:48.000000 hops-3.1.0.0/setup.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    14054 2022-12-22 18:23:48.000000 hops-3.1.0.0/README.rst
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       80 2022-12-22 18:23:59.000000 hops-3.1.0.0/setup.cfg
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops.egg-info/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1338 2022-12-22 18:23:58.000000 hops-3.1.0.0/hops.egg-info/SOURCES.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        5 2022-12-22 18:23:58.000000 hops-3.1.0.0/hops.egg-info/top_level.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2022-12-22 18:23:58.000000 hops-3.1.0.0/hops.egg-info/PKG-INFO
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      314 2022-12-22 18:23:58.000000 hops-3.1.0.0/hops.egg-info/requires.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        1 2022-12-22 18:23:58.000000 hops-3.1.0.0/hops.egg-info/dependency_links.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2022-12-22 18:23:59.000000 hops-3.1.0.0/PKG-INFO
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3529 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/user.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17399 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/dataset.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3011 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/elasticsearch.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    26643 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/constants.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6851 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/kafka.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    31914 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/hdfs.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4608 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/pandas_helper.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6372 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/project.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5896 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/tensorboard.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1098 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/hive.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6902 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/numpy_helper.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7511 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/jobs.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    25975 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3549 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/devices.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops/experiment_impl/
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops/experiment_impl/distribute/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      229 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/mirrored_reservation_client.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     8320 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/mirrored_reservation.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5611 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/parameter_server.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5035 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/mirrored.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      245 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/parameter_server_client.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     9753 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops/experiment_impl/util/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/util/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    27081 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/util/experiment_utils.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5546 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/launcher.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/__init__.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:59.000000 hops-3.1.0.0/hops/experiment_impl/parallel/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/parallel/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6171 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/parallel/random_search.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    22222 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/parallel/differential_evolution.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4463 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/experiment_impl/parallel/grid_search.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      169 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7717 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/tls.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17320 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/model.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    38651 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/serving.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      727 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/service_discovery.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      773 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/featurestore.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5313 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/secret.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      470 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/exceptions.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    20187 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/util.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5596 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/credentials_provider.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       24 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/version.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5732 2022-12-22 18:23:48.000000 hops-3.1.0.0/hops/xattr.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1795 2023-04-13 09:39:35.000000 hops-3.2.0.0/setup.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    14054 2023-04-13 09:39:35.000000 hops-3.2.0.0/README.rst
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       80 2023-04-13 09:39:39.000000 hops-3.2.0.0/setup.cfg
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1338 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        5 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/top_level.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/PKG-INFO
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      314 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/requires.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        1 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-04-13 09:39:39.000000 hops-3.2.0.0/PKG-INFO
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3529 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/user.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17399 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/dataset.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3011 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/elasticsearch.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    26643 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/constants.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6851 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/kafka.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    31914 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/hdfs.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4608 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/pandas_helper.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6372 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/project.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5896 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/tensorboard.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1098 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/hive.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6902 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/numpy_helper.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7511 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/jobs.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    25975 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3549 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/devices.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/distribute/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      229 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation_client.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     8320 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5611 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5035 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      245 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_client.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     9753 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/util/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/util/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    27081 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/util/experiment_utils.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5546 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/launcher.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/__init__.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/parallel/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6171 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/random_search.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    22222 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/differential_evolution.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4463 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/grid_search.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      169 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7717 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/tls.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17320 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/model.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    38651 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/serving.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      727 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/service_discovery.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      773 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/featurestore.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5313 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/secret.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      470 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/exceptions.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    20187 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/util.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5596 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/credentials_provider.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       24 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/version.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5732 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/xattr.py
```

### Comparing `hops-3.1.0.0/setup.py` & `hops-3.2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/README.rst` & `hops-3.2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops.egg-info/SOURCES.txt` & `hops-3.2.0.0/hops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops.egg-info/PKG-INFO` & `hops-3.2.0.0/hops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hops
-Version: 3.1.0.0
+Version: 3.2.0.0
 Summary: Client library for interacting with Hopsworks, a full-stack platform for scale-out data science.
 Home-page: https://github.com/logicalclocks/hops-util-py
 Author: Robin Andersson
 Author-email: robin.eric.andersson@gmail.com
 License: Apache License 2.0
-Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.1.0.0.tar.gz
+Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.2.0.0.tar.gz
 Description: ============
         hops-util-py
         ============
         
         |Downloads| |PypiStatus| |PythonVersions|
         
         `hops-util-py` is a helper library for Hops that facilitates development by hiding the complexity of running applications, discovering services and interacting with HopsFS.
```

### Comparing `hops-3.1.0.0/PKG-INFO` & `hops-3.2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hops
-Version: 3.1.0.0
+Version: 3.2.0.0
 Summary: Client library for interacting with Hopsworks, a full-stack platform for scale-out data science.
 Home-page: https://github.com/logicalclocks/hops-util-py
 Author: Robin Andersson
 Author-email: robin.eric.andersson@gmail.com
 License: Apache License 2.0
-Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.1.0.0.tar.gz
+Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.2.0.0.tar.gz
 Description: ============
         hops-util-py
         ============
         
         |Downloads| |PypiStatus| |PythonVersions|
         
         `hops-util-py` is a helper library for Hops that facilitates development by hiding the complexity of running applications, discovering services and interacting with HopsFS.
```

### Comparing `hops-3.1.0.0/hops/user.py` & `hops-3.2.0.0/hops/user.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/dataset.py` & `hops-3.2.0.0/hops/dataset.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/elasticsearch.py` & `hops-3.2.0.0/hops/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/constants.py` & `hops-3.2.0.0/hops/constants.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/kafka.py` & `hops-3.2.0.0/hops/kafka.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/hdfs.py` & `hops-3.2.0.0/hops/hdfs.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/pandas_helper.py` & `hops-3.2.0.0/hops/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/project.py` & `hops-3.2.0.0/hops/project.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/tensorboard.py` & `hops-3.2.0.0/hops/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/hive.py` & `hops-3.2.0.0/hops/hive.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/numpy_helper.py` & `hops-3.2.0.0/hops/numpy_helper.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/jobs.py` & `hops-3.2.0.0/hops/jobs.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment.py` & `hops-3.2.0.0/hops/experiment.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/devices.py` & `hops-3.2.0.0/hops/devices.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/distribute/mirrored_reservation.py` & `hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/distribute/parameter_server.py` & `hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/distribute/mirrored.py` & `hops-3.2.0.0/hops/experiment_impl/distribute/mirrored.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py` & `hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/util/experiment_utils.py` & `hops-3.2.0.0/hops/experiment_impl/util/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/launcher.py` & `hops-3.2.0.0/hops/experiment_impl/launcher.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/parallel/random_search.py` & `hops-3.2.0.0/hops/experiment_impl/parallel/random_search.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/parallel/differential_evolution.py` & `hops-3.2.0.0/hops/experiment_impl/parallel/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/experiment_impl/parallel/grid_search.py` & `hops-3.2.0.0/hops/experiment_impl/parallel/grid_search.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/tls.py` & `hops-3.2.0.0/hops/tls.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/model.py` & `hops-3.2.0.0/hops/model.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/serving.py` & `hops-3.2.0.0/hops/serving.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/service_discovery.py` & `hops-3.2.0.0/hops/service_discovery.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/featurestore.py` & `hops-3.2.0.0/hops/featurestore.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/secret.py` & `hops-3.2.0.0/hops/secret.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/util.py` & `hops-3.2.0.0/hops/util.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/credentials_provider.py` & `hops-3.2.0.0/hops/credentials_provider.py`

 * *Files identical despite different names*

### Comparing `hops-3.1.0.0/hops/xattr.py` & `hops-3.2.0.0/hops/xattr.py`

 * *Files identical despite different names*

