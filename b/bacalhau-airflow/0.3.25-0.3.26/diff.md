# Comparing `tmp/bacalhau_airflow-0.3.25.tar.gz` & `tmp/bacalhau_airflow-0.3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_airflow-0.3.25.tar", last modified: Tue Mar 21 22:36:57 2023, max compression
+gzip compressed data, was "bacalhau_airflow-0.3.26.tar", last modified: Thu Apr 13 13:07:49 2023, max compression
```

## Comparing `bacalhau_airflow-0.3.25.tar` & `bacalhau_airflow-0.3.26.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.993595 bacalhau_airflow-0.3.25/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10247 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/LICENSE
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      242 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8064 2023-03-21 22:36:56.993595 bacalhau_airflow-0.3.25/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7340 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.989595 bacalhau_airflow-0.3.25/bacalhau_airflow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      137 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/bacalhau_airflow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2246 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/bacalhau_airflow/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6574 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/bacalhau_airflow/operators.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.989595 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8064 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       17 2023-03-21 22:36:56.000000 bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/top_level.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.989595 bacalhau_airflow-0.3.25/docs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/Makefile
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.993595 bacalhau_airflow-0.3.25/docs/_static/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   658378 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/_static/airflow_01.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   661811 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/_static/airflow_02.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   803839 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/_static/airflow_03.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   682446 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/_static/airflow_04.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      522 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/bacalhau_airflow.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5087 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/conf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/index.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       85 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/modules.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       27 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/docs/readme.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2023-03-21 22:36:56.993595 bacalhau_airflow-0.3.25/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1338 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-21 22:36:56.993595 bacalhau_airflow-0.3.25/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/tests/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1622 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/tests/test_hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2583 2023-03-21 22:35:25.000000 bacalhau_airflow-0.3.25/tests/test_operators.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.126543 bacalhau_airflow-0.3.26/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10247 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/LICENSE
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      242 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7816 2023-04-13 13:07:49.126543 bacalhau_airflow-0.3.26/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7092 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.122543 bacalhau_airflow-0.3.26/bacalhau_airflow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      137 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/bacalhau_airflow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2246 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/bacalhau_airflow/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6574 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/bacalhau_airflow/operators.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.122543 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7816 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       17 2023-04-13 13:07:49.000000 bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/top_level.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.122543 bacalhau_airflow-0.3.26/docs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/Makefile
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.126543 bacalhau_airflow-0.3.26/docs/_static/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   658378 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/_static/airflow_01.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   661811 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/_static/airflow_02.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   803839 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/_static/airflow_03.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   682446 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/_static/airflow_04.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      522 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/bacalhau_airflow.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5087 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/conf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/index.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       85 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/modules.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       27 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/docs/readme.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2023-04-13 13:07:49.126543 bacalhau_airflow-0.3.26/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1338 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 13:07:49.126543 bacalhau_airflow-0.3.26/tests/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/tests/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1622 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/tests/test_hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2583 2023-04-13 13:06:21.000000 bacalhau_airflow-0.3.26/tests/test_operators.py
```

### Comparing `bacalhau_airflow-0.3.25/LICENSE` & `bacalhau_airflow-0.3.26/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/PKG-INFO` & `bacalhau_airflow-0.3.26/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau_airflow
-Version: 0.3.25
+Version: 0.3.26
 Summary: An Apache Airflow provider for Bacalhau.
 Home-page: https://github.com/filecoin-project/bacalhau/tree/main/integration/airflow
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 License: Apache Software License 2.0
 Keywords: bacalhau,airflow,provider
 Platform: UNKNOWN
@@ -22,15 +22,14 @@
 
 This is `bacalhau-airflow`, a Python package that integrates [Bacalhau](https://github.com/bacalhau-project/bacalhau) with [Apache Airflow](https://github.com/apache/airflow).
 The benefit is two fold.
 First, thanks to this package you can now write complex pipelines for Bacalhau.
 For instance, jobs can communicate their output's CIDs to downstream jobs, that can use those as inputs.
 Second, Apache Airflow provides a solid solution to reliably orchestrate your DAGs.
 
-> :warning: You may try this out using a local devstack until https://github.com/bacalhau-project/bacalhau/issues/2038 has been fixed. Please set the following environment variables `AIRFLOW_VAR_BACALHAU_API_HOST`, `AIRFLOW_VAR_BACALHAU_API_PORT`.
 
 ## Features
 
 - Create Airflow tasks that run on Bacalhau (via custom operator!)
 - Support for sharded jobs: output shards can be passed downstream (via [XComs](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/xcoms.html))
 - Coming soon...
     - Lineage (see [OpenLineage proof-of-concept integration here](https://github.com/enricorotundo/bacalhau-airflow-provider))
```

### Comparing `bacalhau_airflow-0.3.25/README.md` & `bacalhau_airflow-0.3.26/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 This is `bacalhau-airflow`, a Python package that integrates [Bacalhau](https://github.com/bacalhau-project/bacalhau) with [Apache Airflow](https://github.com/apache/airflow).
 The benefit is two fold.
 First, thanks to this package you can now write complex pipelines for Bacalhau.
 For instance, jobs can communicate their output's CIDs to downstream jobs, that can use those as inputs.
 Second, Apache Airflow provides a solid solution to reliably orchestrate your DAGs.
 
-> :warning: You may try this out using a local devstack until https://github.com/bacalhau-project/bacalhau/issues/2038 has been fixed. Please set the following environment variables `AIRFLOW_VAR_BACALHAU_API_HOST`, `AIRFLOW_VAR_BACALHAU_API_PORT`.
 
 ## Features
 
 - Create Airflow tasks that run on Bacalhau (via custom operator!)
 - Support for sharded jobs: output shards can be passed downstream (via [XComs](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/xcoms.html))
 - Coming soon...
     - Lineage (see [OpenLineage proof-of-concept integration here](https://github.com/enricorotundo/bacalhau-airflow-provider))
```

### Comparing `bacalhau_airflow-0.3.25/bacalhau_airflow/hooks.py` & `bacalhau_airflow-0.3.26/bacalhau_airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/bacalhau_airflow/operators.py` & `bacalhau_airflow-0.3.26/bacalhau_airflow/operators.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/PKG-INFO` & `bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-airflow
-Version: 0.3.25
+Version: 0.3.26
 Summary: An Apache Airflow provider for Bacalhau.
 Home-page: https://github.com/filecoin-project/bacalhau/tree/main/integration/airflow
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 License: Apache Software License 2.0
 Keywords: bacalhau,airflow,provider
 Platform: UNKNOWN
@@ -22,15 +22,14 @@
 
 This is `bacalhau-airflow`, a Python package that integrates [Bacalhau](https://github.com/bacalhau-project/bacalhau) with [Apache Airflow](https://github.com/apache/airflow).
 The benefit is two fold.
 First, thanks to this package you can now write complex pipelines for Bacalhau.
 For instance, jobs can communicate their output's CIDs to downstream jobs, that can use those as inputs.
 Second, Apache Airflow provides a solid solution to reliably orchestrate your DAGs.
 
-> :warning: You may try this out using a local devstack until https://github.com/bacalhau-project/bacalhau/issues/2038 has been fixed. Please set the following environment variables `AIRFLOW_VAR_BACALHAU_API_HOST`, `AIRFLOW_VAR_BACALHAU_API_PORT`.
 
 ## Features
 
 - Create Airflow tasks that run on Bacalhau (via custom operator!)
 - Support for sharded jobs: output shards can be passed downstream (via [XComs](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/xcoms.html))
 - Coming soon...
     - Lineage (see [OpenLineage proof-of-concept integration here](https://github.com/enricorotundo/bacalhau-airflow-provider))
```

### Comparing `bacalhau_airflow-0.3.25/bacalhau_airflow.egg-info/SOURCES.txt` & `bacalhau_airflow-0.3.26/bacalhau_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/Makefile` & `bacalhau_airflow-0.3.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/_static/airflow_01.png` & `bacalhau_airflow-0.3.26/docs/_static/airflow_01.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/_static/airflow_02.png` & `bacalhau_airflow-0.3.26/docs/_static/airflow_02.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/_static/airflow_03.png` & `bacalhau_airflow-0.3.26/docs/_static/airflow_03.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/_static/airflow_04.png` & `bacalhau_airflow-0.3.26/docs/_static/airflow_04.png`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/bacalhau_airflow.rst` & `bacalhau_airflow-0.3.26/docs/bacalhau_airflow.rst`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/conf.py` & `bacalhau_airflow-0.3.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/docs/index.rst` & `bacalhau_airflow-0.3.26/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/setup.py` & `bacalhau_airflow-0.3.26/setup.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/tests/test_hooks.py` & `bacalhau_airflow-0.3.26/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `bacalhau_airflow-0.3.25/tests/test_operators.py` & `bacalhau_airflow-0.3.26/tests/test_operators.py`

 * *Files identical despite different names*

