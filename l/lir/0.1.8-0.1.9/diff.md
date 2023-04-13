# Comparing `tmp/lir-0.1.8.tar.gz` & `tmp/lir-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lir-0.1.8.tar", last modified: Thu Mar 17 10:07:40 2022, max compression
+gzip compressed data, was "lir-0.1.9.tar", last modified: Tue Mar 22 13:26:50 2022, max compression
```

## Comparing `lir-0.1.8.tar` & `lir-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 10:07:40.501591 lir-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11360 2022-03-17 10:07:01.000000 lir-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-03-17 10:07:40.501591 lir-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-03-17 10:07:01.000000 lir-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 10:07:40.501591 lir-0.1.8/lir/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-03-17 10:07:01.000000 lir-0.1.8/lir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10004 2022-03-17 10:07:01.000000 lir-0.1.8/lir/_plotting_new.py
--rw-r--r--   0 runner    (1001) docker     (121)    23845 2022-03-17 10:07:01.000000 lir-0.1.8/lir/_plotting_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-03-17 10:07:01.000000 lir-0.1.8/lir/bayeserror.py
--rw-r--r--   0 runner    (1001) docker     (121)    25703 2022-03-17 10:07:01.000000 lir-0.1.8/lir/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-03-17 10:07:01.000000 lir-0.1.8/lir/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-03-17 10:07:01.000000 lir-0.1.8/lir/ece.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-03-17 10:07:01.000000 lir-0.1.8/lir/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     7384 2022-03-17 10:07:01.000000 lir-0.1.8/lir/lr.py
--rw-r--r--   0 runner    (1001) docker     (121)    12444 2022-03-17 10:07:01.000000 lir-0.1.8/lir/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 10:07:40.501591 lir-0.1.8/lir/multiclass/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-03-17 10:07:01.000000 lir-0.1.8/lir/multiclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-03-17 10:07:01.000000 lir-0.1.8/lir/multiclass/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-03-17 10:07:01.000000 lir-0.1.8/lir/multiclass/lr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-03-17 10:07:01.000000 lir-0.1.8/lir/multiclass/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-17 10:07:01.000000 lir-0.1.8/lir/multiclass/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-17 10:07:01.000000 lir-0.1.8/lir/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-03-17 10:07:01.000000 lir-0.1.8/lir/regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     5528 2022-03-17 10:07:01.000000 lir-0.1.8/lir/transformers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-03-17 10:07:01.000000 lir-0.1.8/lir/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 10:07:40.501591 lir-0.1.8/lir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-03-17 10:07:40.000000 lir-0.1.8/lir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-03-17 10:07:40.000000 lir-0.1.8/lir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 10:07:40.000000 lir-0.1.8/lir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-17 10:07:40.000000 lir-0.1.8/lir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-17 10:07:40.000000 lir-0.1.8/lir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-17 10:07:40.505591 lir-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1002 2022-03-17 10:07:31.000000 lir-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 13:26:50.405973 lir-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11360 2022-03-22 13:26:01.000000 lir-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-03-22 13:26:50.405973 lir-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-03-22 13:26:01.000000 lir-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 13:26:50.405973 lir-0.1.9/lir/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-03-22 13:26:01.000000 lir-0.1.9/lir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10004 2022-03-22 13:26:01.000000 lir-0.1.9/lir/_plotting_new.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23845 2022-03-22 13:26:01.000000 lir-0.1.9/lir/_plotting_old.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-03-22 13:26:01.000000 lir-0.1.9/lir/bayeserror.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25703 2022-03-22 13:26:01.000000 lir-0.1.9/lir/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-03-22 13:26:01.000000 lir-0.1.9/lir/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-03-22 13:26:01.000000 lir-0.1.9/lir/ece.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-03-22 13:26:01.000000 lir-0.1.9/lir/generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7384 2022-03-22 13:26:01.000000 lir-0.1.9/lir/lr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12444 2022-03-22 13:26:01.000000 lir-0.1.9/lir/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 13:26:50.405973 lir-0.1.9/lir/multiclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-03-22 13:26:01.000000 lir-0.1.9/lir/multiclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-03-22 13:26:01.000000 lir-0.1.9/lir/multiclass/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-03-22 13:26:01.000000 lir-0.1.9/lir/multiclass/lr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-03-22 13:26:01.000000 lir-0.1.9/lir/multiclass/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-22 13:26:01.000000 lir-0.1.9/lir/multiclass/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-22 13:26:01.000000 lir-0.1.9/lir/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-03-22 13:26:01.000000 lir-0.1.9/lir/regression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-03-22 13:26:01.000000 lir-0.1.9/lir/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-03-22 13:26:01.000000 lir-0.1.9/lir/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 13:26:50.405973 lir-0.1.9/lir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-03-22 13:26:50.000000 lir-0.1.9/lir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-03-22 13:26:50.000000 lir-0.1.9/lir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-22 13:26:50.000000 lir-0.1.9/lir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-22 13:26:50.000000 lir-0.1.9/lir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-22 13:26:50.000000 lir-0.1.9/lir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-22 13:26:50.405973 lir-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1002 2022-03-22 13:26:39.000000 lir-0.1.9/setup.py
```

### Comparing `lir-0.1.8/LICENSE.txt` & `lir-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/PKG-INFO` & `lir-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lir
-Version: 0.1.8
+Version: 0.1.9
 Summary: scripts for calculating likelihood ratios
 Home-page: https://github.com/NetherlandsForensicInstitute/lir
 Author: Netherlands Forensic Institute
 Author-email: fbda@nfi.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lir-0.1.8/README.md` & `lir-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/__init__.py` & `lir-0.1.9/lir/__init__.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/_plotting_new.py` & `lir-0.1.9/lir/_plotting_new.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/_plotting_old.py` & `lir-0.1.9/lir/_plotting_old.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/bayeserror.py` & `lir-0.1.9/lir/bayeserror.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/calibration.py` & `lir-0.1.9/lir/calibration.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/data.py` & `lir-0.1.9/lir/data.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/ece.py` & `lir-0.1.9/lir/ece.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/generators.py` & `lir-0.1.9/lir/generators.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/lr.py` & `lir-0.1.9/lir/lr.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/metrics.py` & `lir-0.1.9/lir/metrics.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/multiclass/calibration.py` & `lir-0.1.9/lir/multiclass/calibration.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/multiclass/lr.py` & `lir-0.1.9/lir/multiclass/lr.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/multiclass/metrics.py` & `lir-0.1.9/lir/multiclass/metrics.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/regression.py` & `lir-0.1.9/lir/regression.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir/transformers.py` & `lir-0.1.9/lir/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     """
     def __init__(self):
         self.rank_functions = None
 
     def fit(self, X, y=None):
         assert len(X.shape) == 2
         ranks_X = rankdata(X, method='max', axis=0)/len(X)
+        # if a feature is a constant int value, interp1d returns nan -> convert to float
+        X = X.astype(float)
         self.rank_functions = [interp1d(X[:, i], ranks_X[:, i], bounds_error=False,
                                         fill_value=(0, 1)) for i in range(X.shape[1])]
         return self
 
     def transform(self, X):
         assert self.rank_functions, "transform() called before fit()"
         assert len(X.shape) == 2
```

### Comparing `lir-0.1.8/lir/util.py` & `lir-0.1.9/lir/util.py`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/lir.egg-info/PKG-INFO` & `lir-0.1.9/lir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lir
-Version: 0.1.8
+Version: 0.1.9
 Summary: scripts for calculating likelihood ratios
 Home-page: https://github.com/NetherlandsForensicInstitute/lir
 Author: Netherlands Forensic Institute
 Author-email: fbda@nfi.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lir-0.1.8/lir.egg-info/SOURCES.txt` & `lir-0.1.9/lir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lir-0.1.8/setup.py` & `lir-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 setup(
     name="lir",
-    version="0.1.8",
+    version="0.1.9",
     description="scripts for calculating likelihood ratios",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NetherlandsForensicInstitute/lir",
     author="Netherlands Forensic Institute",
     author_email="fbda@nfi.nl",
     packages=find_packages(),
```

