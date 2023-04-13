# Comparing `tmp/mountainsort5-0.1.4.tar.gz` & `tmp/mountainsort5-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort5-0.1.4.tar", last modified: Thu Apr 13 19:09:17 2023, max compression
+gzip compressed data, was "mountainsort5-0.1.5.tar", last modified: Thu Apr 13 19:18:22 2023, max compression
```

## Comparing `mountainsort5-0.1.4.tar` & `mountainsort5-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.685837 mountainsort5-0.1.4/mountainsort5/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.689837 mountainsort5-0.1.4/mountainsort5/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/SnippetClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/branch_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/compute_pca_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/compute_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/detect_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/extract_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_block_recording_for_scheme3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_sampled_recording_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_times_labels_from_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/remove_duplicate_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/mountainsort5/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme1SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme2SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme3SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.689837 mountainsort5-0.1.4/mountainsort5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/SnippetClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/branch_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/compute_pca_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/compute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/detect_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/extract_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_block_recording_for_scheme3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_sampled_recording_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_times_labels_from_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/remove_duplicate_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme1SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme2SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme3SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme3.py
```

### Comparing `mountainsort5-0.1.4/LICENSE` & `mountainsort5-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/PKG-INFO` & `mountainsort5-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.4
+Version: 0.1.5
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/magland/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mountainsort5-0.1.4/README.md` & `mountainsort5-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/SnippetClassifier.py` & `mountainsort5-0.1.5/mountainsort5/core/SnippetClassifier.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/branch_cluster.py` & `mountainsort5-0.1.5/mountainsort5/core/branch_cluster.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/detect_spikes.py` & `mountainsort5-0.1.5/mountainsort5/core/detect_spikes.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/extract_snippets.py` & `mountainsort5-0.1.5/mountainsort5/core/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/get_block_recording_for_scheme3.py` & `mountainsort5-0.1.5/mountainsort5/core/get_block_recording_for_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/get_sampled_recording_for_training.py` & `mountainsort5-0.1.5/mountainsort5/core/get_sampled_recording_for_training.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/get_times_labels_from_sorting.py` & `mountainsort5-0.1.5/mountainsort5/core/get_times_labels_from_sorting.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/core/remove_duplicate_events.py` & `mountainsort5-0.1.5/mountainsort5/core/remove_duplicate_events.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/Scheme1SortingParameters.py` & `mountainsort5-0.1.5/mountainsort5/schemes/Scheme1SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/Scheme2SortingParameters.py` & `mountainsort5-0.1.5/mountainsort5/schemes/Scheme2SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/Scheme3SortingParameters.py` & `mountainsort5-0.1.5/mountainsort5/schemes/Scheme3SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme1.py` & `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme1.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,23 @@
     print('Offsetting times to peak')
     # Now we need to offset the times again so that the spike times correspond to actual peaks
     offsets_to_peak = determine_offsets_to_peak(templates, detect_sign=sorting_parameters.detect_sign, T1=sorting_parameters.snippet_T1)
     print('Offsets to peak:', offsets_to_peak)
     # This time we need to add the offset
     times = offset_times(times, offsets_to_peak, labels)
 
-    # TODO: make sure the times are not out of bounds now that we have offset them a couple times
+    # Now we need to make sure the times are in order, because we have offset them
+    sort_inds = np.argsort(times)
+    times = times[sort_inds]
+    labels = labels[sort_inds]
+
+    # also make sure none of the times are out of bounds now that we have offset them a couple times
+    inds_okay = np.where((times >= sorting_parameters.snippet_T1) & (times < N - sorting_parameters.snippet_T2))[0]
+    times = times[inds_okay]
+    labels = labels[inds_okay]
 
     print('Reordering units')
     # relabel so that units are ordered by channel
     # and we also put any labels that are not used at the end
     aa = peak_channel_indices
     for k in range(1, K + 1):
         inds = np.where(labels == k)[0]
```

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme2.py` & `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme2.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme3.py` & `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/mountainsort5.egg-info/PKG-INFO` & `mountainsort5-0.1.5/mountainsort5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.4
+Version: 0.1.5
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/magland/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mountainsort5-0.1.4/mountainsort5.egg-info/SOURCES.txt` & `mountainsort5-0.1.5/mountainsort5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/setup.py` & `mountainsort5-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 setup(
     name='mountainsort5',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/magland/mountainsort5",
```

### Comparing `mountainsort5-0.1.4/tests/test_core.py` & `mountainsort5-0.1.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/tests/test_scheme1.py` & `mountainsort5-0.1.5/tests/test_scheme1.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/tests/test_scheme2.py` & `mountainsort5-0.1.5/tests/test_scheme2.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.4/tests/test_scheme3.py` & `mountainsort5-0.1.5/tests/test_scheme3.py`

 * *Files identical despite different names*

