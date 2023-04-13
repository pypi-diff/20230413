# Comparing `tmp/czmlpy-0.8.0.tar.gz` & `tmp/czmlpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czmlpy-0.8.0.tar", last modified: Thu Jan 12 02:24:22 2023, max compression
+gzip compressed data, was "czmlpy-0.9.0.tar", last modified: Thu Apr 13 09:24:09 2023, max compression
```

## Comparing `czmlpy-0.8.0.tar` & `czmlpy-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 02:24:22.218399 czmlpy-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-01-11 23:13:31.000000 czmlpy-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-11 23:57:29.000000 czmlpy-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4540 2023-01-12 02:24:22.218399 czmlpy-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3300 2023-01-12 02:22:22.000000 czmlpy-0.8.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1393 2023-01-12 02:24:22.218399 czmlpy-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       53 2023-01-11 23:52:23.000000 czmlpy-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 02:24:22.208399 czmlpy-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 02:24:22.208399 czmlpy-0.8.0/src/czmlpy/
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-12 00:10:45.000000 czmlpy-0.8.0/src/czmlpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/base.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/common.py
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/constants.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/core.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 02:24:22.218399 czmlpy-0.8.0/src/czmlpy/examples/
--rw-r--r--   0 root         (0) root         (0)       49 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49567 2023-01-11 23:41:37.000000 czmlpy-0.8.0/src/czmlpy/examples/simple.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/properties.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/py.typed
--rw-r--r--   0 root         (0) root         (0)    11494 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/types.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/utils.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-01-11 23:13:31.000000 czmlpy-0.8.0/src/czmlpy/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 02:24:22.218399 czmlpy-0.8.0/src/czmlpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4540 2023-01-12 02:24:21.000000 czmlpy-0.8.0/src/czmlpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      545 2023-01-12 02:24:22.000000 czmlpy-0.8.0/src/czmlpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 02:24:21.000000 czmlpy-0.8.0/src/czmlpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 23:53:47.000000 czmlpy-0.8.0/src/czmlpy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-12 02:24:22.000000 czmlpy-0.8.0/src/czmlpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-12 02:24:22.000000 czmlpy-0.8.0/src/czmlpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.543566 czmlpy-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-01-11 23:13:31.000000 czmlpy-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-11 23:57:29.000000 czmlpy-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-04-13 09:24:09.543566 czmlpy-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-01-12 02:22:22.000000 czmlpy-0.9.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-04-13 09:24:09.543566 czmlpy-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       53 2023-03-08 21:51:20.000000 czmlpy-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.533565 czmlpy-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.543566 czmlpy-0.9.0/src/czmlpy/
+-rw-r--r--   0 root         (0) root         (0)      144 2023-03-08 21:51:21.000000 czmlpy-0.9.0/src/czmlpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/base.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-03-28 11:43:34.000000 czmlpy-0.9.0/src/czmlpy/common.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-03-08 21:50:53.000000 czmlpy-0.9.0/src/czmlpy/core.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.543566 czmlpy-0.9.0/src/czmlpy/examples/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49567 2023-01-11 23:41:37.000000 czmlpy-0.9.0/src/czmlpy/examples/simple.py
+-rw-r--r--   0 root         (0) root         (0)    28356 2023-03-30 20:22:32.000000 czmlpy-0.9.0/src/czmlpy/properties.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/py.typed
+-rw-r--r--   0 root         (0) root         (0)    11494 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/types.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-01-11 23:13:31.000000 czmlpy-0.9.0/src/czmlpy/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.543566 czmlpy-0.9.0/src/czmlpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-04-13 09:24:09.000000 czmlpy-0.9.0/src/czmlpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-13 09:24:09.000000 czmlpy-0.9.0/src/czmlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:24:09.000000 czmlpy-0.9.0/src/czmlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 23:53:47.000000 czmlpy-0.9.0/src/czmlpy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-13 09:24:09.000000 czmlpy-0.9.0/src/czmlpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 09:24:09.000000 czmlpy-0.9.0/src/czmlpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:24:09.543566 czmlpy-0.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-01-11 23:41:39.000000 czmlpy-0.9.0/tests/test_core.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-01-11 23:41:40.000000 czmlpy-0.9.0/tests/test_document.py
+-rw-r--r--   0 root         (0) root         (0)      787 2023-01-11 23:41:41.000000 czmlpy-0.9.0/tests/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)    15167 2023-01-11 23:41:42.000000 czmlpy-0.9.0/tests/test_packet.py
+-rw-r--r--   0 root         (0) root         (0)    16752 2023-01-11 23:41:44.000000 czmlpy-0.9.0/tests/test_properties.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-01-11 23:41:45.000000 czmlpy-0.9.0/tests/test_rectangle_image.py
+-rw-r--r--   0 root         (0) root         (0)     5725 2023-01-11 23:41:48.000000 czmlpy-0.9.0/tests/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-01-11 23:41:58.000000 czmlpy-0.9.0/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-01-11 23:42:05.000000 czmlpy-0.9.0/tests/test_widget.py
```

### Comparing `czmlpy-0.8.0/LICENSE` & `czmlpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/PKG-INFO` & `czmlpy-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czmlpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python 3 library to write CZML
 Home-page: https://github.com/mixxen/czmlpy
 Download-URL: https://github.com/mixxen/czmlpy
 Author: Juan Luis Cano Rodríguez
 Author-email: hello@juanlu.space
 License: MIT
 Project-URL: Source, https://github.com/mixxen/czmlpy
```

### Comparing `czmlpy-0.8.0/README.rst` & `czmlpy-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/setup.cfg` & `czmlpy-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/base.py` & `czmlpy-0.9.0/src/czmlpy/base.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/common.py` & `czmlpy-0.9.0/src/czmlpy/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # noinspection PyPep8Naming
 from __future__ import annotations
 
 import datetime as dt
 
 import attr
 
-from .enums import InterpolationAlgorithms
+from .enums import InterpolationAlgorithms, ExtrapolationTypes
 
 
 @attr.s(str=False, frozen=True, kw_only=True)
 class Deletable:
     """A property whose value may be deleted."""
 
     delete: bool | None = attr.ib(default=None)
@@ -22,7 +22,9 @@
 
     The interpolation happens over provided time-tagged samples.
     """
 
     epoch: dt.datetime | None = attr.ib(default=None)
     interpolationAlgorithm: InterpolationAlgorithms | None = attr.ib(default=None)
     interpolationDegree: int | None = attr.ib(default=None)
+    forwardExtrapolationType: ExtrapolationTypes | None = attr.ib(default=None)
+    backwardExtrapolationType: ExtrapolationTypes | None = attr.ib(default=None)
```

### Comparing `czmlpy-0.8.0/src/czmlpy/core.py` & `czmlpy-0.9.0/src/czmlpy/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,19 @@
     path = attr.ib(default=None)
     point = attr.ib(default=None)
     polygon = attr.ib(default=None)
     polyline = attr.ib(default=None)
     rectangle = attr.ib(default=None)
     tileset = attr.ib(default=None)
     wall = attr.ib(default=None)
+    agi_conicSensor = attr.ib(default=None)
+    agi_customPatternSensor = attr.ib(default=None)
+    agi_rectangularSensor = attr.ib(default=None)
+    agi_fan = attr.ib(default=None)
+    agi_vector  = attr.ib(default=None)
 
 
 @attr.s(str=False, frozen=True)
 class Document(Sequence):
     """A CZML document, consisting on a list of packets."""
 
     @property
```

### Comparing `czmlpy-0.8.0/src/czmlpy/enums.py` & `czmlpy-0.9.0/src/czmlpy/enums.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/examples/simple.py` & `czmlpy-0.9.0/src/czmlpy/examples/simple.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/types.py` & `czmlpy-0.9.0/src/czmlpy/types.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/utils.py` & `czmlpy-0.9.0/src/czmlpy/utils.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy/widget.py` & `czmlpy-0.9.0/src/czmlpy/widget.py`

 * *Files identical despite different names*

### Comparing `czmlpy-0.8.0/src/czmlpy.egg-info/PKG-INFO` & `czmlpy-0.9.0/src/czmlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czmlpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python 3 library to write CZML
 Home-page: https://github.com/mixxen/czmlpy
 Download-URL: https://github.com/mixxen/czmlpy
 Author: Juan Luis Cano Rodríguez
 Author-email: hello@juanlu.space
 License: MIT
 Project-URL: Source, https://github.com/mixxen/czmlpy
```

### Comparing `czmlpy-0.8.0/src/czmlpy.egg-info/SOURCES.txt` & `czmlpy-0.9.0/src/czmlpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,8 +17,17 @@
 src/czmlpy.egg-info/PKG-INFO
 src/czmlpy.egg-info/SOURCES.txt
 src/czmlpy.egg-info/dependency_links.txt
 src/czmlpy.egg-info/not-zip-safe
 src/czmlpy.egg-info/requires.txt
 src/czmlpy.egg-info/top_level.txt
 src/czmlpy/examples/__init__.py
-src/czmlpy/examples/simple.py
+src/czmlpy/examples/simple.py
+tests/test_core.py
+tests/test_document.py
+tests/test_examples.py
+tests/test_packet.py
+tests/test_properties.py
+tests/test_rectangle_image.py
+tests/test_types.py
+tests/test_utils.py
+tests/test_widget.py
```

