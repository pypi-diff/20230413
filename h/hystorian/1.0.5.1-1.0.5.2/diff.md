# Comparing `tmp/hystorian-1.0.5.1.tar.gz` & `tmp/hystorian-1.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hystorian-1.0.5.1.tar", last modified: Wed Dec 14 09:07:23 2022, max compression
+gzip compressed data, was "hystorian-1.0.5.2.tar", last modified: Thu Apr 13 07:28:53 2023, max compression
```

## Comparing `hystorian-1.0.5.1.tar` & `hystorian-1.0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2022-12-14 09:07:13.000000 hystorian-1.0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2022-12-14 09:07:13.000000 hystorian-1.0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/hystorian/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/hystorian/io/
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/ardf_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/csv_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/gsf_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/ibw_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/img_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/nanoscope_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/shg_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/sxm_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/io/xrdml_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/hystorian/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    39035 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/ndim.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   141486 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/hystorian/processing/twodim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/hystorian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-14 09:07:23.000000 hystorian-1.0.5.1/hystorian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2022-12-14 09:07:23.000000 hystorian-1.0.5.1/hystorian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 09:07:23.000000 hystorian-1.0.5.1/hystorian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-14 09:07:23.000000 hystorian-1.0.5.1/hystorian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-14 09:07:23.000000 hystorian-1.0.5.1/hystorian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 09:07:23.508948 hystorian-1.0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-14 09:07:14.000000 hystorian-1.0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:28:53.099486 hystorian-1.0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-13 07:28:43.000000 hystorian-1.0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-13 07:28:53.099486 hystorian-1.0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 07:28:43.000000 hystorian-1.0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:28:53.091486 hystorian-1.0.5.2/hystorian/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:28:53.095486 hystorian-1.0.5.2/hystorian/io/
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/ardf_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/csv_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/gsf_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/ibw_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/img_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/nanoscope_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/shg_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/sxm_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/io/xrdml_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:28:53.095486 hystorian-1.0.5.2/hystorian/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    39035 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/ndim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141524 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/hystorian/processing/twodim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:28:53.091486 hystorian-1.0.5.2/hystorian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-13 07:28:53.000000 hystorian-1.0.5.2/hystorian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-13 07:28:53.000000 hystorian-1.0.5.2/hystorian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:28:53.000000 hystorian-1.0.5.2/hystorian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 07:28:53.000000 hystorian-1.0.5.2/hystorian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 07:28:53.000000 hystorian-1.0.5.2/hystorian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:28:53.099486 hystorian-1.0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 07:28:44.000000 hystorian-1.0.5.2/setup.py
```

### Comparing `hystorian-1.0.5.1/LICENSE` & `hystorian-1.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/PKG-INFO` & `hystorian-1.0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hystorian
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: a generic materials science data analysis Python package built with processing traceability, reproducibility, and archival ability at its core.
 Home-page: https://gitlab.unige.ch/paruch-group/hystorian
 Author: Loïc Musy <loic.musy@unige.ch>, Ralph Bulanadi <ralph.bulanadi@unige.ch>
 Author-email: loic.musy@unige.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `hystorian-1.0.5.1/README.md` & `hystorian-1.0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/__init__.py` & `hystorian-1.0.5.2/hystorian/__init__.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/ardf_files.py` & `hystorian-1.0.5.2/hystorian/io/ardf_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/csv_files.py` & `hystorian-1.0.5.2/hystorian/io/csv_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/gsf_files.py` & `hystorian-1.0.5.2/hystorian/io/gsf_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/ibw_files.py` & `hystorian-1.0.5.2/hystorian/io/ibw_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/img_files.py` & `hystorian-1.0.5.2/hystorian/io/img_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/nanoscope_files.py` & `hystorian-1.0.5.2/hystorian/io/nanoscope_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/read_file.py` & `hystorian-1.0.5.2/hystorian/io/read_file.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/shg_files.py` & `hystorian-1.0.5.2/hystorian/io/shg_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/sxm_files.py` & `hystorian-1.0.5.2/hystorian/io/sxm_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/io/xrdml_files.py` & `hystorian-1.0.5.2/hystorian/io/xrdml_files.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/core.py` & `hystorian-1.0.5.2/hystorian/processing/core.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/deprecated.py` & `hystorian-1.0.5.2/hystorian/processing/deprecated.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/experimental.py` & `hystorian-1.0.5.2/hystorian/processing/experimental.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/ndim.py` & `hystorian-1.0.5.2/hystorian/processing/ndim.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/plot.py` & `hystorian-1.0.5.2/hystorian/processing/plot.py`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/hystorian/processing/twodim.py` & `hystorian-1.0.5.2/hystorian/processing/twodim.py`

 * *Files 0% similar despite different names*

```diff
@@ -947,23 +947,23 @@
     Returns
     -------
     best_guess : float
         final guess for best threshold
     """
     if old_diff is None:
         binary = image > old_guess
-        binary_filt = medfilt(binary, 3)
-        old_diff = np.sum(np.abs(binary_filt - binary))
+        binary_filt = ndimage.median_filter(binary, size=3)
+        old_diff = np.sum(np.abs(binary_filt ^ binary))
     if iterations > 0:
         new_guesses = [old_guess - thresh_range, old_guess + thresh_range]
         diffs = []
         for thresh in new_guesses:
             binary = image > thresh
-            binary_filt = medfilt(binary, 3)
-            diffs.append(np.sum(np.abs(binary_filt - binary)))
+            binary_filt = ndimage.median_filter(binary, size=3)
+            diffs.append(np.sum(np.abs(binary_filt ^ binary)))
         best_i = np.argmin(diffs)
         best_guess = threshold_noise(image, new_guesses[best_i], thresh_range / 2, iterations - 1,
                                      diffs[best_i])
     else:
         best_guess = old_guess
     return best_guess
```

### Comparing `hystorian-1.0.5.1/hystorian.egg-info/PKG-INFO` & `hystorian-1.0.5.2/hystorian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hystorian
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: a generic materials science data analysis Python package built with processing traceability, reproducibility, and archival ability at its core.
 Home-page: https://gitlab.unige.ch/paruch-group/hystorian
 Author: Loïc Musy <loic.musy@unige.ch>, Ralph Bulanadi <ralph.bulanadi@unige.ch>
 Author-email: loic.musy@unige.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `hystorian-1.0.5.1/hystorian.egg-info/SOURCES.txt` & `hystorian-1.0.5.2/hystorian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hystorian-1.0.5.1/setup.py` & `hystorian-1.0.5.2/setup.py`

 * *Files identical despite different names*

