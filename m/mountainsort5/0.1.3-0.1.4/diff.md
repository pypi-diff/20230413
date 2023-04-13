# Comparing `tmp/mountainsort5-0.1.3.tar.gz` & `tmp/mountainsort5-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort5-0.1.3.tar", last modified: Tue Apr 11 19:16:36 2023, max compression
+gzip compressed data, was "mountainsort5-0.1.4.tar", last modified: Thu Apr 13 19:09:17 2023, max compression
```

## Comparing `mountainsort5-0.1.3.tar` & `mountainsort5-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.012350 mountainsort5-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/SnippetClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/cluster_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/compute_pca_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/compute_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/detect_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/extract_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_block_recording_for_scheme3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_sampled_recording_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_times_labels_from_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/pairwise_merge_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme1SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme2SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme3SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-11 19:16:35.000000 mountainsort5-0.1.3/mountainsort5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:16:36.012350 mountainsort5-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.685837 mountainsort5-0.1.4/mountainsort5/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.689837 mountainsort5-0.1.4/mountainsort5/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/SnippetClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/branch_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/compute_pca_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/compute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/detect_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/extract_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_block_recording_for_scheme3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_sampled_recording_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/get_times_labels_from_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/core/remove_duplicate_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/mountainsort5/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme1SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme2SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/Scheme3SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.689837 mountainsort5-0.1.4/mountainsort5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 19:09:17.000000 mountainsort5-0.1.4/mountainsort5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:17.693837 mountainsort5-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 19:08:11.000000 mountainsort5-0.1.4/tests/test_scheme3.py
```

### Comparing `mountainsort5-0.1.3/LICENSE` & `mountainsort5-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/PKG-INFO` & `mountainsort5-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.3
+Version: 0.1.4
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/magland/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mountainsort5-0.1.3/README.md` & `mountainsort5-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/core/SnippetClassifier.py` & `mountainsort5-0.1.4/mountainsort5/core/SnippetClassifier.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/core/detect_spikes.py` & `mountainsort5-0.1.4/mountainsort5/core/detect_spikes.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     adjacency = []
     for m in range(M):
         adjacency.append([])
         for m2 in range(M):
             dist0 = np.sqrt(np.sum((channel_locations[m] - channel_locations[m2]) ** 2))
             if (channel_radius is None) or (dist0 <= channel_radius):
                 adjacency[m].append(m2)
+    print('')
+    print(f'Adjacency for detect spikes with channel radius {channel_radius}')
+    print(adjacency)
+    print('')
     
     inds1, inds2 = np.nonzero(traces <= -detect_threshold)
     
     candidate_times = [[] for m in range(M)]
     candidate_values = [[] for m in range(M)]
     for i in range(len(inds1)):
         if inds1[i] >= margin_left and inds1[i] < N - margin_right:
```

### Comparing `mountainsort5-0.1.3/mountainsort5/core/extract_snippets.py` & `mountainsort5-0.1.4/mountainsort5/core/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/core/get_block_recording_for_scheme3.py` & `mountainsort5-0.1.4/mountainsort5/core/get_block_recording_for_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/core/get_sampled_recording_for_training.py` & `mountainsort5-0.1.4/mountainsort5/core/get_sampled_recording_for_training.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/core/get_times_labels_from_sorting.py` & `mountainsort5-0.1.4/mountainsort5/core/get_times_labels_from_sorting.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/schemes/Scheme1SortingParameters.py` & `mountainsort5-0.1.4/mountainsort5/schemes/Scheme1SortingParameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,24 @@
     - detect_channel_radius: the radius (in units of channel locations) for exluding nearby channels from detection
     - detect_time_radius_msec: the radius (in msec) for excluding nearby events from detection
     - detect_sign: the sign of the threshold for detection (1, -1, or 0)
     - snippet_T1: the number of timepoints before the event to include in the snippet
     - snippet_T2: the number of timepoints after the event to include in the snippet
     - snippet_mask_radius: the radius (in units of channel locations) for making a snippet around the central channel
     - npca_per_branch: the number of PCA components to compute for each branch of clustering
-    - pairwise_merge_step: whether to do the pairwise merge step
     """
     detect_threshold: float=5.5
     detect_channel_radius: Union[float, None]=None
     detect_time_radius_msec: float=0.5
     detect_sign: int=-1
     snippet_T1: int=20
     snippet_T2: int=20
     snippet_mask_radius: Union[float, None]=None
     npca_per_branch: int=12
-    pairwise_merge_step: bool=True
+    pairwise_merge_step: bool=False # deprecated
 
     def check_valid(self, *, M: int, N: int, sampling_frequency: float, channel_locations: npt.NDArray[np.float32]):
         """Internal function for checking validity of parameters"""
         assert channel_locations.shape[0] == M, 'Shape mismatch between traces and channel locations'
         D = channel_locations.shape[1]
         assert N >= self.snippet_T1 + self.snippet_T2
         if self.snippet_mask_radius is not None:
```

### Comparing `mountainsort5-0.1.3/mountainsort5/schemes/Scheme2SortingParameters.py` & `mountainsort5-0.1.4/mountainsort5/schemes/Scheme2SortingParameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     - phase1_detect_channel_radius: detect_channel_radius in phase 1
     - detect_channel_radius: detect_channel_radius in phase 2
     - phase1_detect_threshold: detect_threshold in phase 1
     - phase1_detect_time_radius_msec: detect_time_radius_msec in phase 1
     - detect_time_radius_msec: detect_time_radius_msec in phase 2
     - phase1_npca_per_branch: npca_per_branch in phase 1
-    - phase1_pairwise_merge_step: pairwise_merge_step in phase 1
     - detect_sign
     - detect_threshold: detect_threshold in phase 2
     - snippet_T1
     - snippet_T2
     - snippet_mask_radius
     - max_num_snippets_per_training_batch: the maximum number of snippets to use for training the classifier in each batch
     - classifier_npca: the number of principal components to use for each neighborhood classifier
@@ -29,15 +28,15 @@
     """
     phase1_detect_channel_radius: Union[float, None]
     detect_channel_radius: Union[float, None]
     phase1_detect_threshold: float=5.5
     phase1_detect_time_radius_msec: float=1.5
     detect_time_radius_msec: float=0.5
     phase1_npca_per_branch: int=12
-    phase1_pairwise_merge_step: bool=True
+    phase1_pairwise_merge_step: bool=False # deprecated
     detect_sign: int=-1
     detect_threshold: float=5.5
     snippet_T1: int=20
     snippet_T2: int=20
     snippet_mask_radius: Union[float, None]=None
     max_num_snippets_per_training_batch: int=200
     classifier_npca: Union[int, None]=None
```

### Comparing `mountainsort5-0.1.3/mountainsort5/schemes/Scheme3SortingParameters.py` & `mountainsort5-0.1.4/mountainsort5/schemes/Scheme3SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme1.py` & `mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme3.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,81 @@
-from typing import Union
+from typing import Dict, Union
 import numpy as np
-import math
+import numpy.typing as npt
 import spikeinterface as si
-from .Scheme1SortingParameters import Scheme1SortingParameters
-from ..core.detect_spikes import detect_spikes
-from ..core.extract_snippets import extract_snippets
-from ..core.cluster_snippets import cluster_snippets
-from ..core.compute_templates import compute_templates
-from ..core.pairwise_merge_step import pairwise_merge_step
+from .Scheme3SortingParameters import Scheme3SortingParameters
+from .sorting_scheme2 import get_time_chunks
+from .sorting_scheme2 import sorting_scheme2, get_times_labels_from_sorting
+from ..core.get_block_recording_for_scheme3 import get_block_recording_for_scheme3
+from ..core.SnippetClassifier import SnippetClassifier
+from ..core.get_times_labels_from_sorting import get_times_labels_from_sorting
 
 
-def sorting_scheme1(
+def sorting_scheme3(
     recording: si.BaseRecording, *,
-    sorting_parameters: Scheme1SortingParameters
-):
-    """MountainSort 5 sorting scheme 1
+    sorting_parameters: Scheme3SortingParameters
+) -> si.BaseSorting:
+    """MountainSort 5 sorting scheme 3
 
     Args:
         recording (si.BaseRecording): SpikeInterface recording object
-        sorting_parameters (Scheme2SortingParameters): Sorting parameters
+        sorting_parameters (Scheme3SortingParameters): Sorting parameters
 
     Returns:
         si.BaseSorting: SpikeInterface sorting object
     """
 
     ###################################################################
     # Handle multi-segment recordings
     if recording.get_num_segments() > 1:
         print('Recording has multiple segments. Joining segments for sorting...')
         recording_joined = si.concatenate_recordings(recording_list=[recording])
-        sorting_joined = sorting_scheme1(recording_joined, sorting_parameters=sorting_parameters)
+        sorting_joined = sorting_scheme3(recording_joined, sorting_parameters=sorting_parameters)
         print('Splitting sorting into segments to match original multisegment recording...')
         sorting = si.split_sorting(sorting_joined, recording_joined)
         return sorting
     ###################################################################
 
     M = recording.get_num_channels()
     N = recording.get_num_frames()
     sampling_frequency = recording.sampling_frequency
-
     channel_locations = recording.get_channel_locations()
 
-    print(f'Number of channels: {M}')
-    print(f'Number of timepoints: {N}')
-    print(f'Sampling frequency: {sampling_frequency} Hz')
-    for m in range(M):
-        print(f'Channel {m}: {channel_locations[m]}')
-
     sorting_parameters.check_valid(M=M, N=N, sampling_frequency=sampling_frequency, channel_locations=channel_locations)
-    
-    print('Loading traces')
-    traces = recording.get_traces()
 
-    print('Detecting spikes')
-    time_radius = int(math.ceil(sorting_parameters.detect_time_radius_msec / 1000 * sampling_frequency))
-    times, channel_indices = detect_spikes(
-        traces=traces,
-        channel_locations=channel_locations,
-        time_radius=time_radius,
-        channel_radius=sorting_parameters.detect_channel_radius,
-        detect_threshold=sorting_parameters.detect_threshold,
-        detect_sign=sorting_parameters.detect_sign,
-        margin_left=sorting_parameters.snippet_T1,
-        margin_right=sorting_parameters.snippet_T2,
-        verbose=True
-    )
-
-    print(f'Extracting {len(times)} snippets')
-    snippets = extract_snippets( # L x T x M
-        traces=traces,
-        channel_locations=channel_locations,
-        mask_radius=sorting_parameters.snippet_mask_radius,
-        times=times,
-        channel_indices=channel_indices,
-        T1=sorting_parameters.snippet_T1,
-        T2=sorting_parameters.snippet_T2
-    )
-    L = snippets.shape[0]
-    T = snippets.shape[1]
-    assert snippets.shape[2] == M
-
-    print('Clustering snippets')
-    labels = cluster_snippets(
-        snippets=snippets,
-        npca_per_branch=sorting_parameters.npca_per_branch
-    )
-    K = int(np.max(labels))
-    print(f'Found {K} clusters')
-
-    print('Computing templates')
-    templates = compute_templates(snippets=snippets, labels=labels) # K x T x M
-    peak_channel_indices = [np.argmin(np.min(templates[i], axis=0)) for i in range(K)]
-
-    if sorting_parameters.pairwise_merge_step:
-        print('Pairwise merge step')
-        times, labels = pairwise_merge_step(
-            templates=templates,
-            snippets=snippets,
-            labels=labels,
-            times=times,
-            detect_sign=sorting_parameters.detect_sign,
-            unit_ids=np.arange(1, K + 1).astype(np.int32),
-            detect_time_radius=time_radius
-        )
+    block_size = int(sorting_parameters.block_duration_sec * sampling_frequency) # size of chunks in samples
+    blocks = get_time_chunks(recording.get_num_samples(), chunk_size=block_size, padding=1000)
 
-    print('Reordering units')
-    # relabel so that units are ordered by channel
-    # and we also put any labels that are not used at the end
-    aa = peak_channel_indices
-    for k in range(1, K + 1):
-        inds = np.where(labels == k)[0]
-        if len(inds) == 0:
-            aa[k - 1] = np.Inf
-    new_labels_mapping = np.argsort(np.argsort(aa)) + 1 # too tricky! my head aches right now
-    labels = new_labels_mapping[labels - 1]
+    times_list: list[npt.NDArray[np.int64]] = []
+    labels_list: list[npt.NDArray[np.int32]] = []
+    last_label_used = 0
+    previous_snippet_classifiers: Union[Dict[int, SnippetClassifier], None] = None
+    for i, chunk in enumerate(blocks):
+        print('')
+        print('=============================================')
+        print(f'Processing block {i + 1} of {len(blocks)}...')
+        subrecording = get_block_recording_for_scheme3(recording=recording, start_frame=chunk.start - chunk.padding_left, end_frame=chunk.end + chunk.padding_right)
+        subsorting, snippet_classifiers = sorting_scheme2(
+            subrecording,
+            sorting_parameters=sorting_parameters.block_sorting_parameters,
+            return_snippet_classifiers=True,
+            reference_snippet_classifiers=previous_snippet_classifiers,
+            label_offset=last_label_used
+        )
+        previous_snippet_classifiers = snippet_classifiers
+        times0, labels0 = get_times_labels_from_sorting(subsorting)
+        valid_inds = np.where((times0 >= chunk.padding_left) & (times0 < chunk.padding_left + (chunk.end - chunk.start)))[0]
+        times0: npt.NDArray[np.int32] = times0[valid_inds]
+        labels0: npt.NDArray[np.int32] = labels0[valid_inds]
+        times0 = times0.astype(np.int64) + chunk.start - np.int64(chunk.padding_left)
+        if len(labels0) > 0:
+            last_label_used = max(last_label_used, np.max(labels0))
+        times_list.append(times0)
+        labels_list.append(labels0)
     
-    sorting = si.NumpySorting.from_times_labels(times_list=[times], labels_list=[labels], sampling_frequency=sampling_frequency)
+    times_concat = np.concatenate(times_list)
+    labels_concat = np.concatenate(labels_list)
+
+    # Now create a new sorting object from the times and labels results
+    sorting2 = si.NumpySorting.from_times_labels([times_concat], [labels_concat], sampling_frequency=recording.sampling_frequency)
 
-    return sorting
+    return sorting2
```

### Comparing `mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme2.py` & `mountainsort5-0.1.4/mountainsort5/schemes/sorting_scheme2.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import spikeinterface as si
 from .Scheme2SortingParameters import Scheme2SortingParameters
 from .Scheme1SortingParameters import Scheme1SortingParameters
 from ..core.detect_spikes import detect_spikes
 from ..core.extract_snippets import extract_snippets, extract_snippets_in_channel_neighborhood
 from .sorting_scheme1 import sorting_scheme1
 from ..core.SnippetClassifier import SnippetClassifier
-from ..core.pairwise_merge_step import remove_duplicate_events
+from ..core.remove_duplicate_events import remove_duplicate_events
 from ..core.get_sampled_recording_for_training import get_sampled_recording_for_training
 from ..core.get_times_labels_from_sorting import get_times_labels_from_sorting
 
 
 def sorting_scheme2(
     recording: si.BaseRecording, *,
     sorting_parameters: Scheme2SortingParameters,
@@ -81,16 +81,15 @@
             detect_threshold=sorting_parameters.phase1_detect_threshold,
             detect_sign=sorting_parameters.detect_sign,
             detect_time_radius_msec=sorting_parameters.phase1_detect_time_radius_msec,
             detect_channel_radius=sorting_parameters.phase1_detect_channel_radius,
             snippet_mask_radius=sorting_parameters.snippet_mask_radius,
             snippet_T1=sorting_parameters.snippet_T1,
             snippet_T2=sorting_parameters.snippet_T2,
-            npca_per_branch=sorting_parameters.phase1_npca_per_branch,
-            pairwise_merge_step=sorting_parameters.phase1_pairwise_merge_step
+            npca_per_branch=sorting_parameters.phase1_npca_per_branch
         )
     )
     times, labels = get_times_labels_from_sorting(sorting1)
     K = np.max(labels) # number of clusters
     labels = labels + label_offset # used in scheme 3
 
     print('Loading training traces')
```

### Comparing `mountainsort5-0.1.3/mountainsort5.egg-info/PKG-INFO` & `mountainsort5-0.1.4/mountainsort5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.3
+Version: 0.1.4
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/magland/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mountainsort5-0.1.3/mountainsort5.egg-info/SOURCES.txt` & `mountainsort5-0.1.4/mountainsort5.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 mountainsort5.egg-info/PKG-INFO
 mountainsort5.egg-info/SOURCES.txt
 mountainsort5.egg-info/dependency_links.txt
 mountainsort5.egg-info/requires.txt
 mountainsort5.egg-info/top_level.txt
 mountainsort5/core/SnippetClassifier.py
 mountainsort5/core/__init__.py
-mountainsort5/core/cluster_snippets.py
+mountainsort5/core/branch_cluster.py
 mountainsort5/core/compute_pca_features.py
 mountainsort5/core/compute_templates.py
 mountainsort5/core/detect_spikes.py
 mountainsort5/core/extract_snippets.py
 mountainsort5/core/get_block_recording_for_scheme3.py
 mountainsort5/core/get_sampled_recording_for_training.py
 mountainsort5/core/get_times_labels_from_sorting.py
-mountainsort5/core/pairwise_merge_step.py
+mountainsort5/core/remove_duplicate_events.py
 mountainsort5/schemes/Scheme1SortingParameters.py
 mountainsort5/schemes/Scheme2SortingParameters.py
 mountainsort5/schemes/Scheme3SortingParameters.py
 mountainsort5/schemes/__init__.py
 mountainsort5/schemes/sorting_scheme1.py
 mountainsort5/schemes/sorting_scheme2.py
 mountainsort5/schemes/sorting_scheme3.py
```

### Comparing `mountainsort5-0.1.3/setup.py` & `mountainsort5-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 setup(
     name='mountainsort5',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/magland/mountainsort5",
```

### Comparing `mountainsort5-0.1.3/tests/test_core.py` & `mountainsort5-0.1.4/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import spikeinterface.extractors as se
 from mountainsort5.core.compute_pca_features import compute_pca_features
 from mountainsort5.core.compute_templates import compute_templates
 from mountainsort5.core.detect_spikes import detect_spikes
 from mountainsort5.core.extract_snippets import extract_snippets, extract_snippets_in_channel_neighborhood
 from mountainsort5.core.get_sampled_recording_for_training import get_sampled_recording_for_training
 from mountainsort5.core.get_block_recording_for_scheme3 import get_block_recording_for_scheme3
-from mountainsort5.core.cluster_snippets import cluster_snippets
-from mountainsort5.core.pairwise_merge_step import pairwise_merge_step
+from mountainsort5.core.branch_cluster import branch_cluster
 from mountainsort5.core.get_times_labels_from_sorting import get_times_labels_from_sorting
 
 
 def test_compute_pca_features():
     x = np.random.normal(size=(100, 20))
     features = compute_pca_features(x, npca=10)
     assert features.shape == (100, 10)
@@ -157,57 +156,31 @@
         end_frame=20 * recording.sampling_frequency
     )
     assert np.array_equal(
         recording.get_traces(start_frame=10 * recording.sampling_frequency, end_frame=20 * recording.sampling_frequency),
         recording2.get_traces()
     )
 
-def test_cluster_snippets():
+def test_branch_cluster():
     N = 1000
     L = 100
     M = 4
     T1 = 20
     T2 = 20
     traces = np.random.normal(size=(N, M))
     traces[500:] += 10 # offset this so we get more than one cluster (important for coverage of cluster_snippets)
     times = np.random.randint(T1, N - T2, size=(L,))
     snippets = extract_snippets(traces, times=times, channel_locations=None, mask_radius=None, channel_indices=None, T1=T1, T2=T2)
-    labels = cluster_snippets(
-        snippets,
+    labels = branch_cluster(
+        snippets.reshape((L, M * (T1 + T2))),
         npca_per_branch=10
     )
     assert np.min(labels) == 1
     assert len(labels) == L
 
-def test_pairwise_merge_step():
-    N = 1000
-    L = 100
-    M = 4
-    T1 = 20
-    T2 = 20
-    traces = np.random.normal(size=(N, M))
-    times = np.random.randint(T1, N - T2, size=(L,))
-    snippets = extract_snippets(traces, times=times, channel_locations=None, mask_radius=None, channel_indices=None, T1=T1, T2=T2)
-    labels = cluster_snippets(
-        snippets,
-        npca_per_branch=10
-    )
-    templates = compute_templates(snippets, labels)
-    new_times, new_labels = pairwise_merge_step(
-        snippets=snippets,
-        labels=labels,
-        templates=templates,
-        times=times,
-        detect_sign=-1,
-        unit_ids=np.unique(labels),
-        detect_time_radius=10
-    )
-    assert len(new_times) == len(new_labels)
-    assert len(new_times) <= len(times)
-
 def test_get_times_labels_from_sorting():
     recording, sorting = se.toy_example(duration=6, num_channels=4, num_units=10, sampling_frequency=30000, seed=0, num_segments=1)
     recording: si.BaseRecording = recording
     sorting: si.BaseSorting = sorting
 
     times, labels = get_times_labels_from_sorting(sorting)
     assert len(times) == len(labels)
```

### Comparing `mountainsort5-0.1.3/tests/test_scheme1.py` & `mountainsort5-0.1.4/tests/test_scheme1.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/tests/test_scheme2.py` & `mountainsort5-0.1.4/tests/test_scheme2.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.3/tests/test_scheme3.py` & `mountainsort5-0.1.4/tests/test_scheme3.py`

 * *Files identical despite different names*

