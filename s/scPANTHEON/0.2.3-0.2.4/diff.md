# Comparing `tmp/scPANTHEON-0.2.3.tar.gz` & `tmp/scPANTHEON-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.2.3.tar", last modified: Wed Apr  5 05:30:17 2023, max compression
+gzip compressed data, was "scPANTHEON-0.2.4.tar", last modified: Thu Apr 13 11:05:40 2023, max compression
```

## Comparing `scPANTHEON-0.2.3.tar` & `scPANTHEON-0.2.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.769201 scPANTHEON-0.2.3/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-04-05 05:30:17.768698 scPANTHEON-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.729210 scPANTHEON-0.2.3/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-05 05:30:17.000000 scPANTHEON-0.2.3/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.738723 scPANTHEON-0.2.3/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.716127 scPANTHEON-0.2.3/scpantheon/extension/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.739725 scPANTHEON-0.2.3/scpantheon/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.742231 scPANTHEON-0.2.3/scpantheon/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.3/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.3/scpantheon/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.744238 scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.745498 scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/__pycache__/
--rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.746632 scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.749785 scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.750784 scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.754291 scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.755875 scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.758379 scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.759380 scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.762647 scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.764153 scPANTHEON-0.2.3/scpantheon/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2023-04-05 05:30:17.767195 scPANTHEON-0.2.3/scpantheon/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.3/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.3/scpantheon/extension/TOMAS/module.py
--rw-rw-rw-   0        0        0     1026 2023-04-05 05:30:01.000000 scPANTHEON-0.2.3/scpantheon/main.py
--rw-rw-rw-   0        0        0     5551 2023-04-05 05:25:57.000000 scPANTHEON-0.2.3/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/run.py
--rw-rw-rw-   0        0        0    59203 2023-04-05 05:26:39.000000 scPANTHEON-0.2.3/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.3/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-04-05 05:30:17.769201 scPANTHEON-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-05 05:29:51.000000 scPANTHEON-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.950222 scPANTHEON-0.2.4/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-04-13 11:05:40.949218 scPANTHEON-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.904047 scPANTHEON-0.2.4/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1676 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 11:05:40.000000 scPANTHEON-0.2.4/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.913632 scPANTHEON-0.2.4/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.889197 scPANTHEON-0.2.4/scpantheon/extension/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.915264 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.919311 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/
+-rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.4/scpantheon/extension/Change_Color/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.920314 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.922527 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/
+-rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.924042 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.927599 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.929695 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.932834 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
+-rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.934353 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.937463 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/
+-rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.939476 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.943067 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.944592 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:05:40.948213 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/
+-rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.4/scpantheon/extension/TOMAS/module.py
+-rw-rw-rw-   0        0        0     1026 2023-04-05 05:30:01.000000 scPANTHEON-0.2.4/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5551 2023-04-05 05:25:57.000000 scPANTHEON-0.2.4/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/run.py
+-rw-rw-rw-   0        0        0    59203 2023-04-05 05:26:39.000000 scPANTHEON-0.2.4/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.4/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:05:40.950222 scPANTHEON-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-04-13 11:05:25.000000 scPANTHEON-0.2.4/setup.py
```

### Comparing `scPANTHEON-0.2.3/scPANTHEON.egg-info/SOURCES.txt` & `scPANTHEON-0.2.4/scPANTHEON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Change_Color/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Change_Color/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Check_Histogram/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Check_Histogram/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Clustering_with_Scanpy/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Clustering_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Differential_Expression_Analysis/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Differential_Expression_Analysis/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Find_Marker_Gene/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Find_Marker_Gene/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/Preprocessing_with_Scanpy/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/Preprocessing_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/extension/TOMAS/module.py` & `scPANTHEON-0.2.4/scpantheon/extension/TOMAS/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/main.py` & `scPANTHEON-0.2.4/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/qt.py` & `scPANTHEON-0.2.4/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/source.py` & `scPANTHEON-0.2.4/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/scpantheon/transform.py` & `scPANTHEON-0.2.4/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.3/setup.py` & `scPANTHEON-0.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.2.3',#版本
+    version='0.2.4',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
-    install_requires=['bokeh==2.4.3','pandas','anndata==0.8.0','colorcet','scanpy','numpy','PyQt5==5.15.9','PyQtWebEngine==5.15.6'], # 依赖包,如果没有,可以不要
+    install_requires=['bokeh==2.4.3','pandas','anndata==0.8.0','colorcet','scanpy','numpy','PyQt5==5.15.9','PyQtWebEngine==5.15.6','appdirs==1.4.4'], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'],
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

