# Comparing `tmp/histoprep-1.0.8.tar.gz` & `tmp/histoprep-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histoprep-1.0.8.tar", last modified: Wed Aug  3 07:19:53 2022, max compression
+gzip compressed data, was "histoprep-2.0.1.tar", max compression
```

## Comparing `histoprep-1.0.8.tar` & `histoprep-2.0.1.tar`

### file list

```diff
@@ -1,62 +1,26 @@
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.456726 histoprep-1.0.8/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     9009 2022-06-03 12:31:06.000000 histoprep-1.0.8/HistoPrep
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1064 2022-06-02 10:36:25.000000 histoprep-1.0.8/LICENSE
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     4238 2022-08-03 07:19:53.456726 histoprep-1.0.8/PKG-INFO
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3569 2022-06-02 10:39:59.000000 histoprep-1.0.8/README.md
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.152715 histoprep-1.0.8/histoprep/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      116 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/__init__.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.192717 histoprep-1.0.8/histoprep/_outliers/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)       49 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_outliers/__init__.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)    13228 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_outliers/_detect.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)    11204 2022-06-29 08:07:37.000000 histoprep-1.0.8/histoprep/_outliers/_visualize.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.232718 histoprep-1.0.8/histoprep/_reader/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)       72 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_reader/__init__.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.328721 histoprep-1.0.8/histoprep/_reader/_backend/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      340 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_reader/_backend/__init__.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      956 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_reader/_backend/_base.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3424 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_reader/_backend/_bioformats.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2540 2022-06-06 15:41:26.000000 histoprep-1.0.8/histoprep/_reader/_backend/_openslide.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2243 2022-06-06 10:41:42.000000 histoprep-1.0.8/histoprep/_reader/_backend/_pillow.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3018 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/_reader/_backend/_zeiss.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)    33715 2022-08-02 07:52:22.000000 histoprep-1.0.8/histoprep/_reader/_reader.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     9819 2022-06-06 15:53:41.000000 histoprep-1.0.8/histoprep/_reader/_utils.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)       22 2022-08-03 07:10:36.000000 histoprep-1.0.8/histoprep/_version.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.376723 histoprep-1.0.8/histoprep/functional/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      331 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/__init__.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     4888 2022-06-06 15:07:05.000000 histoprep-1.0.8/histoprep/functional/_coordinates.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     5669 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/_dearray.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2017 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/_functional.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     6304 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/_helpers.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)    11394 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/_preprocess.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2304 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/functional/_tissue.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.388723 histoprep-1.0.8/histoprep/helpers/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      264 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/__init__.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3288 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_files.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1399 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_io.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1727 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_javabridge.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     4778 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_metadata.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3163 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_multiprocess.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1348 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_time.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3750 2022-08-03 07:15:07.000000 histoprep-1.0.8/histoprep/helpers/_verbose.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2198 2022-06-02 10:36:25.000000 histoprep-1.0.8/histoprep/helpers/_visualize.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.176716 histoprep-1.0.8/histoprep.egg-info/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     4238 2022-08-03 07:19:53.000000 histoprep-1.0.8/histoprep.egg-info/PKG-INFO
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1442 2022-08-03 07:19:53.000000 histoprep-1.0.8/histoprep.egg-info/SOURCES.txt
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)        1 2022-08-03 07:19:53.000000 histoprep-1.0.8/histoprep.egg-info/dependency_links.txt
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      140 2022-08-03 07:19:53.000000 histoprep-1.0.8/histoprep.egg-info/requires.txt
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)       10 2022-08-03 07:19:53.000000 histoprep-1.0.8/histoprep.egg-info/top_level.txt
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)       38 2022-08-03 07:19:53.456726 histoprep-1.0.8/setup.cfg
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1273 2022-06-30 10:56:36.000000 histoprep-1.0.8/setup.py
-drwxrwx---   0 jpohjone (1251996) jpohjone (1251996)        0 2022-08-03 07:19:53.456726 histoprep-1.0.8/test/
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3104 2022-06-06 15:57:47.000000 histoprep-1.0.8/test/test_backends.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2586 2022-06-02 10:36:25.000000 histoprep-1.0.8/test/test_coordinates.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1353 2022-06-03 11:45:43.000000 histoprep-1.0.8/test/test_cutting.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)        0 2022-06-03 12:06:34.000000 histoprep-1.0.8/test/test_excecutable.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1016 2022-06-02 10:36:25.000000 histoprep-1.0.8/test/test_files.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     2222 2022-06-02 13:20:57.000000 histoprep-1.0.8/test/test_metadata.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1241 2022-06-02 10:36:25.000000 histoprep-1.0.8/test/test_multiprocess.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1531 2022-08-03 07:18:33.000000 histoprep-1.0.8/test/test_outliers.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     3431 2022-06-02 10:36:25.000000 histoprep-1.0.8/test/test_preprocess.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     1189 2022-08-03 07:13:36.000000 histoprep-1.0.8/test/test_progress_bar.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)     4654 2022-06-06 15:52:22.000000 histoprep-1.0.8/test/test_reader.py
--rw-rw----   0 jpohjone (1251996) jpohjone (1251996)      490 2022-06-02 10:36:25.000000 histoprep-1.0.8/test/test_time.py
+-rw-r--r--   0        0        0     1064 2023-02-21 10:11:24.560924 histoprep-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4498 2023-04-13 12:06:06.845518 histoprep-2.0.1/README.md
+-rw-r--r--   0        0        0      208 2023-04-12 16:08:51.730543 histoprep-2.0.1/histoprep/__init__.py
+-rw-r--r--   0        0        0    12824 2023-04-13 11:58:17.436440 histoprep-2.0.1/histoprep/_backend.py
+-rw-r--r--   0        0        0    12916 2023-04-13 11:57:10.830117 histoprep-2.0.1/histoprep/_cli.py
+-rw-r--r--   0        0        0     2632 2023-04-12 15:47:00.972683 histoprep-2.0.1/histoprep/_data.py
+-rw-r--r--   0        0        0    27360 2023-04-13 11:56:18.924307 histoprep-2.0.1/histoprep/_reader.py
+-rw-r--r--   0        0        0      907 2023-04-13 12:20:57.494642 histoprep-2.0.1/histoprep/functional/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-12 15:40:13.626407 histoprep-2.0.1/histoprep/functional/_check.py
+-rw-r--r--   0        0        0     1297 2023-04-12 16:23:34.711207 histoprep-2.0.1/histoprep/functional/_concurrent.py
+-rw-r--r--   0        0        0     5400 2023-04-12 15:45:03.944588 histoprep-2.0.1/histoprep/functional/_dearray.py
+-rw-r--r--   0        0        0     4305 2023-04-12 15:45:01.032486 histoprep-2.0.1/histoprep/functional/_draw.py
+-rw-r--r--   0        0        0     2641 2023-04-13 12:19:15.958972 histoprep-2.0.1/histoprep/functional/_images.py
+-rw-r--r--   0        0        0      410 2023-04-12 16:02:13.168518 histoprep-2.0.1/histoprep/functional/_level.py
+-rw-r--r--   0        0        0     1881 2023-04-13 12:19:50.132209 histoprep-2.0.1/histoprep/functional/_mean_std.py
+-rw-r--r--   0        0        0     5490 2023-04-13 12:20:09.164897 histoprep-2.0.1/histoprep/functional/_metrics.py
+-rw-r--r--   0        0        0     5476 2023-04-12 15:44:49.396078 histoprep-2.0.1/histoprep/functional/_normalize.py
+-rw-r--r--   0        0        0     8211 2023-04-13 12:21:53.940676 histoprep-2.0.1/histoprep/functional/_tiles.py
+-rw-r--r--   0        0        0     4766 2023-04-12 15:45:57.762471 histoprep-2.0.1/histoprep/functional/_tissue.py
+-rw-r--r--   0        0        0      421 2023-04-13 12:05:05.503101 histoprep-2.0.1/histoprep/utils/__init__.py
+-rw-r--r--   0        0        0     5870 2023-04-13 11:58:49.445556 histoprep-2.0.1/histoprep/utils/_normalize.py
+-rw-r--r--   0        0        0    12291 2023-04-13 12:16:52.593762 histoprep-2.0.1/histoprep/utils/_process.py
+-rw-r--r--   0        0        0     4891 2023-04-12 15:58:31.116776 histoprep-2.0.1/histoprep/utils/_torch.py
+-rw-r--r--   0        0        0      724 2023-04-13 12:23:06.887300 histoprep-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 histoprep-2.0.1/setup.py
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.1/PKG-INFO
```

### Comparing `histoprep-1.0.8/LICENSE` & `histoprep-2.0.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Jopo666
+Copyright (c) 2023 jopo666
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `histoprep-1.0.8/histoprep/functional/_dearray.py` & `histoprep-2.0.1/histoprep/functional/_dearray.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,142 @@
-import logging
-from typing import List, Tuple
+import warnings
 
 import cv2
-import numpy
+import numpy as np
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.metrics import silhouette_score
 
-__all__ = ["dearray"]
 
+def get_spot_coordinates(
+    spot_mask: np.ndarray,
+) -> dict[str, tuple[int, int, int, int]]:
+    """Dearray tissue microarray spots based on a spot mask.
 
-def dearray(
-    tissue_mask: numpy.ndarray,
-    kernel_size: int = 5,
-    iterations: int = 3,
-    min_area: float = 0.1,
-    max_area: float = 3.0,
-) -> Tuple[numpy.ndarray, Tuple[int, int, int, int], List[int]]:
-    """Detects TMA spots from an image and gives each spot a number starting
-    from the top-left corner.
+    Numbers each spot from top-left and takes into account missing spots etc in the
+    numbering.
 
     Args:
-        tissue_mask: Tissue mask.
-        kernel_size: Kernel size for dilate. Defaults to 5.
-        iterations: Dilate iterations. Defaults to 3.
-        min_area: Minimum area for a spot. Defaults to 0.1 and calculated with:
-            `median(areas) * min_area`
-        max_area_ Maximum area for a spot. Similar to `min_area`. Defaults to 3.0.
+        spot_mask: Tissue mask of TMA-slide, should only contain TMA spots an no
+            artifacts (see `F.clean_tissue_mask`).
+
+    Returns:
+        Dictionary of spot numbers and xywh-coordinates.
     """
-    # Dilate.
-    kernel = numpy.ones((kernel_size, kernel_size), numpy.uint8)
-    spot_mask = cv2.dilate(tissue_mask, kernel, iterations=iterations)
-    # Detect contours and get their areas.
-    contours, __ = cv2.findContours(spot_mask, cv2.RETR_CCOMP, cv2.CHAIN_APPROX_SIMPLE)
-    areas = numpy.array([cv2.contourArea(cnt) for cnt in contours])
-    # Define min and max values.
-    min_area = numpy.median(areas) * min_area
-    max_area = numpy.median(areas) * max_area
-    # Initialize new mask.
-    new_mask = numpy.zeros_like(spot_mask)
-    bboxes = []
-    centroids = []
-    for cnt in contours:
-        area = cv2.contourArea(cnt)
-        # Select only contours that fit into area range.
-        if not min_area < area < max_area:
-            continue
-        # Get bounding box.
-        bbox = cv2.boundingRect(cnt)
-        # Get centroid.
-        moments = cv2.moments(cnt)
-        centroid = (
-            int(moments["m10"] / moments["m00"]),
-            int(moments["m01"] / moments["m00"]),
-        )
-        # Draw to the new map.
-        cv2.drawContours(new_mask, [cnt], -1, 1, -1)
-        # Add bbox and centroid.
-        bboxes.append(bbox)
-        centroids.append(centroid)
+    # Detect contours and get their bboxes and centroids.
+    bboxes, centroids = _contour_bboxes_and_centroids(spot_mask)
+    if len(bboxes) == 0:
+        return {}
     # Detect possible rotation of the image based on centroids.
-    theta = get_theta(centroids)
-    # Rotate centroids.
-    centroids = rotate_coordinates(centroids, theta)
-    # Detect optimal number of rows and columns.
-    num_cols = get_optimal_cluster_size(centroids[:, 0])
-    num_rows = get_optimal_cluster_size(centroids[:, 1])
-    # Cluster each coordinate to column and row.
-    col_labels = hierachial_clustering(centroids[:, 0], n_clusters=num_cols)
-    row_labels = hierachial_clustering(centroids[:, 1], n_clusters=num_rows)
-    # Detect cluster means.
+    centroids = _rotate_coordinates(centroids, _detect_rotation(centroids))
+    # Detect optimal number of rows and columns and cluster each spot.
+    num_cols = _optimal_cluster_size(centroids[:, 0].reshape(-1, 1))
+    num_rows = _optimal_cluster_size(centroids[:, 1].reshape(-1, 1))
+    col_labels = _hierachial_clustering(
+        centroids[:, 0].reshape(-1, 1), n_clusters=num_cols
+    )
+    row_labels = _hierachial_clustering(
+        centroids[:, 1].reshape(-1, 1), n_clusters=num_rows
+    )
+    # Change label numbers to correct order (starting from top-left).
     x_means = [centroids[col_labels == i, 0].mean() for i in range(num_cols)]
     y_means = [centroids[row_labels == i, 1].mean() for i in range(num_rows)]
-    # Change label numbers to correct order (starting from top-left).
     for i in range(num_cols):
-        new_label = numpy.arange(num_cols)[numpy.argsort(x_means) == i]
+        new_label = np.arange(num_cols)[np.argsort(x_means) == i]
         col_labels[col_labels == i] = -new_label
     col_labels *= -1
     for i in range(num_rows):
-        new_label = numpy.arange(num_rows)[numpy.argsort(y_means) == i]
+        new_label = np.arange(num_rows)[np.argsort(y_means) == i]
         row_labels[row_labels == i] = -new_label
     row_labels *= -1
     # Collect numbers.
-    numbers = numpy.zeros(len(centroids)).astype("str")
-    i = 1
-    complain = False
+    numbers = np.zeros(len(centroids)).astype("str")
+    current_number = 1
+    same_spot_number = False
     for r in range(num_rows):
         for c in range(num_cols):
-            idx = [x == (c, r) for x in zip(col_labels, row_labels)]
-            if sum(idx) == 1:
-                numbers[idx] = i
-            elif sum(idx) > 1:
-                complain = True
-                numbers[idx] = [f"{i}_{ii}" for ii in range(sum(idx))]
-            i += 1
-    if complain:
-        logging.warning("Some spots were assigned the same number.")
-    # Return new mask, coords and numbers.
-    return new_mask, bboxes, numbers
+            matches = [x == (c, r) for x in zip(col_labels, row_labels)]
+            if sum(matches) == 1:
+                numbers[matches] = str(current_number)
+            elif sum(matches) > 1:
+                same_spot_number = True
+                numbers[matches] = [
+                    f"{current_number}-{version+1}" for version in range(sum(matches))
+                ]
+            current_number += 1
+    if same_spot_number:
+        warnings.warn("Some spots were assigned the same number.", stacklevel=1)
+    # Return bboxes and numbers.
+    return {f"spot_{k}": tuple(v) for k, v in zip(numbers, bboxes)}
+
+
+def _contour_bboxes_and_centroids(mask: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+    """Extract contour bounding boxes and centroids."""
+    contours, hierarchy = cv2.findContours(
+        mask, cv2.RETR_CCOMP, cv2.CHAIN_APPROX_SIMPLE
+    )
+    if len(contours) == 0:
+        return np.array([]), np.array([])
+    bboxes, centroids = [], []
+    for cnt, is_parent in zip(contours, hierarchy[0][:, -1] == -1):
+        # Skip non-parents and contours without area.
+        if not is_parent or cv2.contourArea(cnt) == 0:
+            continue
+        # Get bounding box.
+        bboxes.append(cv2.boundingRect(cnt))
+        # Get centroid.
+        moments = cv2.moments(cnt)
+        centroids.append(
+            (
+                int(moments["m10"] / moments["m00"]),
+                int(moments["m01"] / moments["m00"]),
+            )
+        )
+    return np.array(bboxes), np.array(centroids)
 
 
-def get_theta(centroids: numpy.ndarray) -> float:
+def _detect_rotation(centroids: np.ndarray) -> float:
     """Detect rotation from centroid coordinates and return angle in radians."""
     # Calculate angle between each centroid.
     n = len(centroids)
     thetas = []
     for r in range(n):
         for c in range(n):
             x1, y1 = centroids[r]
             x2, y2 = centroids[c]
-            thetas.append(numpy.rad2deg(numpy.arctan2(y2 - y1, x2 - x1)))
+            thetas.append(np.rad2deg(np.arctan2(y2 - y1, x2 - x1)))
     # We want deviations from 0 so divide corrections.
-    corrections = numpy.arange(0, 361, 45)
+    corrections = np.arange(0, 361, 45)
     for i, theta in enumerate(thetas):
-        sign = numpy.sign(theta)
-        idx = numpy.abs(numpy.abs(theta) - corrections).argmin()
+        sign = np.sign(theta)
+        idx = np.abs(np.abs(theta) - corrections).argmin()
         thetas[i] = theta - sign * corrections[idx]
     # Finally return most common angle.
-    values, counts = numpy.unique(numpy.round(thetas), return_counts=True)
+    values, counts = np.unique(np.round(thetas), return_counts=True)
     theta = values[counts.argmax()]
-    return numpy.radians(theta)
+    return np.radians(theta)
 
 
-def rotate_coordinates(coords: numpy.ndarray, theta: float) -> numpy.ndarray:
+def _rotate_coordinates(coords: np.ndarray, theta: float) -> np.ndarray:
     """Rotate coordinates with given theta."""
-    c, s = numpy.cos(theta), numpy.sin(theta)
-    R = numpy.array(((c, -s), (s, c)))
-    return coords @ R
+    c, s = np.cos(theta), np.sin(theta)
+    r_matrix = np.array(((c, -s), (s, c)))
+    return coords @ r_matrix
 
 
-def get_optimal_cluster_size(X: numpy.ndarray) -> int:
+def _optimal_cluster_size(data: np.ndarray) -> int:
     """Find optimal cluster size for dataset X."""
-    if len(X.shape) < 2:
-        X = X.reshape(-1, 1)
     sil = []
-    for n in range(2, X.shape[0]):
-        clust = AgglomerativeClustering(n_clusters=n, linkage="ward")
-        clust.fit(X)
-        sil.append(silhouette_score(X, clust.labels_))
-    return numpy.argmax(sil) + 2
+    if data.shape[0] <= 2:  # noqa
+        return 1
+    for n in range(2, data.shape[0]):
+        labels = _hierachial_clustering(data=data, n_clusters=n)
+        sil.append(silhouette_score(data, labels))
+    return np.argmax(sil) + 2
 
 
-def hierachial_clustering(
-    X: numpy.ndarray, n_clusters: int, linkage: str = "ward"
-) -> numpy.ndarray:
-    """Perform hierarchian clustering."""
-    if len(X.shape) < 2:
-        X = X.reshape(-1, 1)
-    clust = AgglomerativeClustering(n_clusters=n_clusters, linkage=linkage)
-    clust.fit(X)
+def _hierachial_clustering(data: np.ndarray, n_clusters: int) -> np.ndarray:
+    """Perform hierarchian clustering and get labels."""
+    if n_clusters == 1:
+        return np.zeros(data.shape[0], dtype=np.int32)
+    clust = AgglomerativeClustering(n_clusters=n_clusters, linkage="ward")
+    clust.fit(data)
     return clust.labels_
```

