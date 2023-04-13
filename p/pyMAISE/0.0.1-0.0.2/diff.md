# Comparing `tmp/pyMAISE-0.0.1.tar.gz` & `tmp/pyMAISE-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMAISE-0.0.1.tar", last modified: Sun Apr  9 22:51:32 2023, max compression
+gzip compressed data, was "pyMAISE-0.0.2.tar", last modified: Thu Apr 13 19:34:57 2023, max compression
```

## Comparing `pyMAISE-0.0.1.tar` & `pyMAISE-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-09 22:51:32.944392 pyMAISE-0.0.1/
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      383 2023-04-09 22:51:32.944392 pyMAISE-0.0.1/PKG-INFO
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     1600 2023-04-05 20:52:35.000000 pyMAISE-0.0.1/README.md
-drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-09 22:51:32.924392 pyMAISE-0.0.1/pyMAISE/
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      190 2023-01-18 23:43:11.000000 pyMAISE-0.0.1/pyMAISE/__init__.py
-drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-09 22:51:32.934392 pyMAISE-0.0.1/pyMAISE/data/
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)       24 2023-02-02 00:06:37.000000 pyMAISE-0.0.1/pyMAISE/data/__init__.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      823 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/_handler.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)   112703 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/crx.csv
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    44733 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/fp_inp.csv
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    17186 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/fp_out.csv
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)   150964 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/heat.csv
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)   408727 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/data/powery.csv
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    94965 2023-02-14 16:40:25.000000 pyMAISE-0.0.1/pyMAISE/data/xs.csv
-drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-09 22:51:32.934392 pyMAISE-0.0.1/pyMAISE/methods/
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      320 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/methods/__init__.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     4235 2023-01-19 03:06:46.000000 pyMAISE-0.0.1/pyMAISE/methods/_dtree.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2889 2023-02-02 00:06:37.000000 pyMAISE-0.0.1/pyMAISE/methods/_kneighbors.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2665 2023-01-18 23:43:11.000000 pyMAISE-0.0.1/pyMAISE/methods/_lasso.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     1654 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/methods/_linear.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    17862 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/methods/_nn.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    26143 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/methods/_nn_wrapper.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     5416 2023-03-16 19:45:31.000000 pyMAISE-0.0.1/pyMAISE/methods/_rforest.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2963 2023-02-02 00:06:37.000000 pyMAISE-0.0.1/pyMAISE/methods/_svr.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    13096 2023-04-05 20:52:35.000000 pyMAISE-0.0.1/pyMAISE/postprocessing.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     5898 2023-04-05 17:07:39.000000 pyMAISE-0.0.1/pyMAISE/preprocessing.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2814 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/settings.py
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)    11757 2023-03-30 23:31:52.000000 pyMAISE-0.0.1/pyMAISE/tuning.py
-drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-09 22:51:32.934392 pyMAISE-0.0.1/pyMAISE.egg-info/
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      383 2023-04-09 22:51:32.000000 pyMAISE-0.0.1/pyMAISE.egg-info/PKG-INFO
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      710 2023-04-09 22:51:32.000000 pyMAISE-0.0.1/pyMAISE.egg-info/SOURCES.txt
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)        1 2023-04-09 22:51:32.000000 pyMAISE-0.0.1/pyMAISE.egg-info/dependency_links.txt
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      125 2023-04-09 22:51:32.000000 pyMAISE-0.0.1/pyMAISE.egg-info/requires.txt
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)        8 2023-04-09 22:51:32.000000 pyMAISE-0.0.1/pyMAISE.egg-info/top_level.txt
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)       38 2023-04-09 22:51:32.944392 pyMAISE-0.0.1/setup.cfg
--rw-r--r--   0 myerspat  (1000) myerspat  (1000)      826 2023-04-09 22:50:18.000000 pyMAISE-0.0.1/setup.py
+drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-13 19:34:57.782293 pyMAISE-0.0.2/
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      383 2023-04-13 19:34:57.782293 pyMAISE-0.0.2/PKG-INFO
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     1600 2023-04-05 20:52:35.000000 pyMAISE-0.0.2/README.md
+drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-13 19:34:57.762293 pyMAISE-0.0.2/pyMAISE/
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      190 2023-01-18 23:43:11.000000 pyMAISE-0.0.2/pyMAISE/__init__.py
+drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-13 19:34:57.772293 pyMAISE-0.0.2/pyMAISE/data/
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)       24 2023-02-02 00:06:37.000000 pyMAISE-0.0.2/pyMAISE/data/__init__.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      987 2023-04-13 19:28:50.000000 pyMAISE-0.0.2/pyMAISE/data/_handler.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)   112703 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/data/crx.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    44733 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/data/fp_inp.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    17186 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/data/fp_out.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)   150964 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/data/heat.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)   408727 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/data/powery.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    80790 2023-04-13 19:28:50.000000 pyMAISE-0.0.2/pyMAISE/data/rea_inputs.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    42314 2023-04-13 19:28:50.000000 pyMAISE-0.0.2/pyMAISE/data/rea_outputs.csv
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    94965 2023-02-14 16:40:25.000000 pyMAISE-0.0.2/pyMAISE/data/xs.csv
+drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-13 19:34:57.782293 pyMAISE-0.0.2/pyMAISE/methods/
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      320 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/methods/__init__.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     4235 2023-01-19 03:06:46.000000 pyMAISE-0.0.2/pyMAISE/methods/_dtree.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2889 2023-02-02 00:06:37.000000 pyMAISE-0.0.2/pyMAISE/methods/_kneighbors.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2665 2023-01-18 23:43:11.000000 pyMAISE-0.0.2/pyMAISE/methods/_lasso.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     1654 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/methods/_linear.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    17862 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/methods/_nn.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    26143 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/methods/_nn_wrapper.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     5416 2023-03-16 19:45:31.000000 pyMAISE-0.0.2/pyMAISE/methods/_rforest.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2963 2023-02-02 00:06:37.000000 pyMAISE-0.0.2/pyMAISE/methods/_svr.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    13096 2023-04-05 20:52:35.000000 pyMAISE-0.0.2/pyMAISE/postprocessing.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     5898 2023-04-05 17:07:39.000000 pyMAISE-0.0.2/pyMAISE/preprocessing.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)     2814 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/settings.py
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)    11757 2023-03-30 23:31:52.000000 pyMAISE-0.0.2/pyMAISE/tuning.py
+drwxr-xr-x   0 myerspat  (1000) myerspat  (1000)        0 2023-04-13 19:34:57.772293 pyMAISE-0.0.2/pyMAISE.egg-info/
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      383 2023-04-13 19:34:57.000000 pyMAISE-0.0.2/pyMAISE.egg-info/PKG-INFO
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      767 2023-04-13 19:34:57.000000 pyMAISE-0.0.2/pyMAISE.egg-info/SOURCES.txt
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)        1 2023-04-13 19:34:57.000000 pyMAISE-0.0.2/pyMAISE.egg-info/dependency_links.txt
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      125 2023-04-13 19:34:57.000000 pyMAISE-0.0.2/pyMAISE.egg-info/requires.txt
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)        8 2023-04-13 19:34:57.000000 pyMAISE-0.0.2/pyMAISE.egg-info/top_level.txt
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)       38 2023-04-13 19:34:57.782293 pyMAISE-0.0.2/setup.cfg
+-rw-r--r--   0 myerspat  (1000) myerspat  (1000)      826 2023-04-13 19:34:05.000000 pyMAISE-0.0.2/setup.py
```

### Comparing `pyMAISE-0.0.1/README.md` & `pyMAISE-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/_handler.py` & `pyMAISE-0.0.2/pyMAISE/data/_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,7 +24,13 @@
         [get_full_path("data/fp_inp.csv"), get_full_path("data/fp_out.csv")]
     )
 
 
 # Load benchmark fuel centerline temperature data
 def load_heat():
     return PreProcesser(get_full_path("data/heat.csv"), slice(0, -1), slice(-1, None))
+
+# Rod ejection accident data
+def load_rea():
+    return PreProcesser(
+        [get_full_path("data/rea_inputs.csv"), get_full_path("data/rea_outputs.csv")],
+    )
```

### Comparing `pyMAISE-0.0.1/pyMAISE/data/crx.csv` & `pyMAISE-0.0.2/pyMAISE/data/crx.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/fp_inp.csv` & `pyMAISE-0.0.2/pyMAISE/data/fp_inp.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/fp_out.csv` & `pyMAISE-0.0.2/pyMAISE/data/fp_out.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/heat.csv` & `pyMAISE-0.0.2/pyMAISE/data/heat.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/powery.csv` & `pyMAISE-0.0.2/pyMAISE/data/powery.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/data/xs.csv` & `pyMAISE-0.0.2/pyMAISE/data/xs.csv`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_dtree.py` & `pyMAISE-0.0.2/pyMAISE/methods/_dtree.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_kneighbors.py` & `pyMAISE-0.0.2/pyMAISE/methods/_kneighbors.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_lasso.py` & `pyMAISE-0.0.2/pyMAISE/methods/_lasso.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_linear.py` & `pyMAISE-0.0.2/pyMAISE/methods/_linear.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_nn.py` & `pyMAISE-0.0.2/pyMAISE/methods/_nn.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_nn_wrapper.py` & `pyMAISE-0.0.2/pyMAISE/methods/_nn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_rforest.py` & `pyMAISE-0.0.2/pyMAISE/methods/_rforest.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/methods/_svr.py` & `pyMAISE-0.0.2/pyMAISE/methods/_svr.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/postprocessing.py` & `pyMAISE-0.0.2/pyMAISE/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/preprocessing.py` & `pyMAISE-0.0.2/pyMAISE/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/settings.py` & `pyMAISE-0.0.2/pyMAISE/settings.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE/tuning.py` & `pyMAISE-0.0.2/pyMAISE/tuning.py`

 * *Files identical despite different names*

### Comparing `pyMAISE-0.0.1/pyMAISE.egg-info/SOURCES.txt` & `pyMAISE-0.0.2/pyMAISE.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 pyMAISE/data/__init__.py
 pyMAISE/data/_handler.py
 pyMAISE/data/crx.csv
 pyMAISE/data/fp_inp.csv
 pyMAISE/data/fp_out.csv
 pyMAISE/data/heat.csv
 pyMAISE/data/powery.csv
+pyMAISE/data/rea_inputs.csv
+pyMAISE/data/rea_outputs.csv
 pyMAISE/data/xs.csv
 pyMAISE/methods/__init__.py
 pyMAISE/methods/_dtree.py
 pyMAISE/methods/_kneighbors.py
 pyMAISE/methods/_lasso.py
 pyMAISE/methods/_linear.py
 pyMAISE/methods/_nn.py
```

### Comparing `pyMAISE-0.0.1/setup.py` & `pyMAISE-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Michigan Artificial Intelligance Standard Environment"
 LONG_DESCRIPTION = "Machine learning and artificial intelligance benchmarking library for nuclear engineering applications."
 
 setup(
     name="pyMAISE",
     version=VERSION,
     description=DESCRIPTION,
```

