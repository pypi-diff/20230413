# Comparing `tmp/supervision-0.5.1.tar.gz` & `tmp/supervision-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.5.1.tar", last modified: Wed Apr 12 15:56:20 2023, max compression
+gzip compressed data, was "supervision-0.5.2.tar", last modified: Thu Apr 13 08:57:26 2023, max compression
```

## Comparing `supervision-0.5.1.tar` & `supervision-0.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.654640 supervision-0.5.1/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.5.1/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-12 15:56:20.654505 supervision-0.5.1/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.5.1/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-12 15:56:20.654689 supervision-0.5.1/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.5.1/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.646462 supervision-0.5.1/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)      876 2023-04-12 15:51:15.000000 supervision-0.5.1/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.648033 supervision-0.5.1/supervision/annotation/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-05 15:18:58.000000 supervision-0.5.1/supervision/annotation/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3279 2023-04-05 15:18:58.000000 supervision-0.5.1/supervision/annotation/voc.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.649601 supervision-0.5.1/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.1/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6166 2023-04-10 21:52:53.000000 supervision-0.5.1/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    14776 2023-04-11 11:49:26.000000 supervision-0.5.1/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7159 2023-03-23 11:05:51.000000 supervision-0.5.1/supervision/detection/line_counter.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.650094 supervision-0.5.1/supervision/detection/tools/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.5.1/supervision/detection/tools/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5058 2023-04-10 21:52:53.000000 supervision-0.5.1/supervision/detection/tools/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5527 2023-04-10 21:52:53.000000 supervision-0.5.1/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.651046 supervision-0.5.1/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.1/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.5.1/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.5.1/supervision/draw/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.651827 supervision-0.5.1/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.1/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.5.1/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.5.1/supervision/geometry/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.652244 supervision-0.5.1/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.1/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.5.1/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.5.1/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.647715 supervision-0.5.1/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-12 15:56:20.000000 supervision-0.5.1/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     1007 2023-04-12 15:56:20.000000 supervision-0.5.1/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-12 15:56:20.000000 supervision-0.5.1/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-12 15:56:20.000000 supervision-0.5.1/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-12 15:56:20.000000 supervision-0.5.1/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.652519 supervision-0.5.1/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.1/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.653115 supervision-0.5.1/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.1/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.5.1/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     4916 2023-03-14 12:33:54.000000 supervision-0.5.1/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.653607 supervision-0.5.1/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.1/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.5.1/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-12 15:56:20.654115 supervision-0.5.1/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.1/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.5.1/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.829212 supervision-0.5.2/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.5.2/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-13 08:57:26.829055 supervision-0.5.2/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.5.2/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-13 08:57:26.829270 supervision-0.5.2/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.5.2/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.823825 supervision-0.5.2/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)      876 2023-04-13 08:56:47.000000 supervision-0.5.2/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.824981 supervision-0.5.2/supervision/annotation/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-05 15:18:58.000000 supervision-0.5.2/supervision/annotation/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3279 2023-04-05 15:18:58.000000 supervision-0.5.2/supervision/annotation/voc.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.825698 supervision-0.5.2/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6166 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    14744 2023-04-13 08:56:47.000000 supervision-0.5.2/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7162 2023-04-13 08:46:01.000000 supervision-0.5.2/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.825971 supervision-0.5.2/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5058 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5527 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.826380 supervision-0.5.2/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.5.2/supervision/draw/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.826779 supervision-0.5.2/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.2/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/geometry/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827054 supervision-0.5.2/supervision/notebook/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/supervision/notebook/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/notebook/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.824705 supervision-0.5.2/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1007 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827198 supervision-0.5.2/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827782 supervision-0.5.2/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.2/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.5.2/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     4916 2023-03-14 12:33:54.000000 supervision-0.5.2/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.828265 supervision-0.5.2/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.5.2/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.828685 supervision-0.5.2/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.2/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.5.2/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.5.1/LICENSE.md` & `supervision-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/PKG-INFO` & `supervision-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.5.1 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.5.2 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.5.1/README.md` & `supervision-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/setup.py` & `supervision-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/__init__.py` & `supervision-0.5.2/supervision/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 from supervision.annotation.voc import detections_to_voc_xml
 from supervision.detection.annotate import BoxAnnotator, MaskAnnotator
 from supervision.detection.core import Detections
 from supervision.detection.line_counter import LineZone, LineZoneAnnotator
 from supervision.detection.tools.polygon_zone import PolygonZone, PolygonZoneAnnotator
 from supervision.detection.utils import generate_2d_mask, mask_to_xyxy
```

### Comparing `supervision-0.5.1/supervision/annotation/voc.py` & `supervision-0.5.2/supervision/annotation/voc.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/detection/annotate.py` & `supervision-0.5.2/supervision/detection/annotate.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/detection/core.py` & `supervision-0.5.2/supervision/detection/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,17 +315,15 @@
 
     def __getitem__(self, index: np.ndarray) -> Detections:
         if isinstance(index, np.ndarray) and (
             index.dtype == bool or index.dtype == int
         ):
             return Detections(
                 xyxy=self.xyxy[index],
-                mask=self.mask[index]
-                if self.mask is not None
-                else None,
+                mask=self.mask[index] if self.mask is not None else None,
                 confidence=self.confidence[index]
                 if self.confidence is not None
                 else None,
                 class_id=self.class_id[index] if self.class_id is not None else None,
                 tracker_id=self.tracker_id[index]
                 if self.tracker_id is not None
                 else None,
```

### Comparing `supervision-0.5.1/supervision/detection/line_counter.py` & `supervision-0.5.2/supervision/detection/line_counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
         Update the in_count and out_count for the detections that cross the line.
 
         Attributes:
             detections (Detections): The detections for which to update the counts.
 
         """
-        for xyxy, confidence, class_id, tracker_id in detections:
+        for xyxy, _, confidence, class_id, tracker_id in detections:
             # handle detections with no tracker_id
             if tracker_id is None:
                 continue
 
             # we check if all four anchors of bbox are on the same side of vector
             x1, y1, x2, y2 = xyxy
             anchors = [
```

### Comparing `supervision-0.5.1/supervision/detection/tools/polygon_zone.py` & `supervision-0.5.2/supervision/detection/tools/polygon_zone.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/detection/utils.py` & `supervision-0.5.2/supervision/detection/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/draw/color.py` & `supervision-0.5.2/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/draw/utils.py` & `supervision-0.5.2/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/geometry/core.py` & `supervision-0.5.2/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/geometry/utils.py` & `supervision-0.5.2/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/notebook/utils.py` & `supervision-0.5.2/supervision/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision/video.py` & `supervision-0.5.2/supervision/video.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/supervision.egg-info/PKG-INFO` & `supervision-0.5.2/supervision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.5.1 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.5.2 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.5.1/supervision.egg-info/SOURCES.txt` & `supervision-0.5.2/supervision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/test/detection/test_core.py` & `supervision-0.5.2/test/detection/test_core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/test/detection/test_utils.py` & `supervision-0.5.2/test/detection/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/test/draw/test_color.py` & `supervision-0.5.2/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.1/test/geometry/test_dataclasses.py` & `supervision-0.5.2/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

