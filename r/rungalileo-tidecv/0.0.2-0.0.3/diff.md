# Comparing `tmp/rungalileo-tidecv-0.0.2.tar.gz` & `tmp/rungalileo-tidecv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rungalileo-tidecv-0.0.2.tar", last modified: Wed Apr  5 13:34:56 2023, max compression
+gzip compressed data, was "rungalileo-tidecv-0.0.3.tar", last modified: Thu Apr 13 16:50:35 2023, max compression
```

## Comparing `rungalileo-tidecv-0.0.2.tar` & `rungalileo-tidecv-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-05 13:34:56.396375 rungalileo-tidecv-0.0.2/
--rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.2/LICENSE
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-05 13:34:56.396045 rungalileo-tidecv-0.0.2/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.2/README.md
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-05 13:34:56.371301 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-05 13:34:56.000000 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)      434 2023-04-05 13:34:56.000000 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/SOURCES.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-04-05 13:34:56.000000 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/dependency_links.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-04-05 13:34:56.000000 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/requires.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-04-05 13:34:56.000000 rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/top_level.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-04-05 13:34:56.396492 rungalileo-tidecv-0.0.2/setup.cfg
--rw-r--r--   0 benepstein   (501) staff       (20)     1099 2023-04-05 13:34:35.000000 rungalileo-tidecv-0.0.2/setup.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-05 13:34:56.393484 rungalileo-tidecv-0.0.2/tidecv/
--rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/__init__.py
--rw-r--r--   0 benepstein   (501) staff       (20)    10968 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/ap.py
--rw-r--r--   0 benepstein   (501) staff       (20)     4717 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/data.py
--rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/datasets.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-05 13:34:56.395498 rungalileo-tidecv-0.0.2/tidecv/errors/
--rw-r--r--   0 benepstein   (501) staff       (20)     2927 2023-04-05 13:33:29.000000 rungalileo-tidecv-0.0.2/tidecv/errors/error.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3049 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/errors/main_errors.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.2/tidecv/errors/qualifiers.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.2/tidecv/functions.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.2/tidecv/plotting.py
--rw-r--r--   0 benepstein   (501) staff       (20)    26949 2023-04-05 13:33:53.000000 rungalileo-tidecv-0.0.2/tidecv/quantify.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.556410 rungalileo-tidecv-0.0.3/
+-rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/LICENSE
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-13 16:50:35.556048 rungalileo-tidecv-0.0.3/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/README.md
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.544806 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)      434 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/SOURCES.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/dependency_links.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/requires.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/top_level.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-04-13 16:50:35.556575 rungalileo-tidecv-0.0.3/setup.cfg
+-rw-r--r--   0 benepstein   (501) staff       (20)     1214 2023-04-13 15:04:15.000000 rungalileo-tidecv-0.0.3/setup.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.551152 rungalileo-tidecv-0.0.3/tidecv/
+-rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-04-13 14:59:03.000000 rungalileo-tidecv-0.0.3/tidecv/__init__.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    10968 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/ap.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     4733 2023-04-13 14:56:12.000000 rungalileo-tidecv-0.0.3/tidecv/data.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/datasets.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.554985 rungalileo-tidecv-0.0.3/tidecv/errors/
+-rw-r--r--   0 benepstein   (501) staff       (20)     2927 2023-04-05 13:33:29.000000 rungalileo-tidecv-0.0.3/tidecv/errors/error.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3081 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.3/tidecv/errors/main_errors.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/tidecv/errors/qualifiers.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/functions.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/tidecv/plotting.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    27034 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.3/tidecv/quantify.py
```

### Comparing `rungalileo-tidecv-0.0.2/LICENSE` & `rungalileo-tidecv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/PKG-INFO` & `rungalileo-tidecv-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.2
+Version: 0.0.3
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.2/README.md` & `rungalileo-tidecv-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/rungalileo_tidecv.egg-info/PKG-INFO` & `rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.2
+Version: 0.0.3
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.2/setup.py` & `rungalileo-tidecv-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pathlib
 from setuptools import setup
+import json
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding="utf8")
+with open("tidecv/__init__.py") as f:
+    VERSION = json.loads(f.readlines()[0].split("=")[1].strip())
 
 # This call to setup() does all the work
 setup(
     name="rungalileo-tidecv",
-    version="0.0.2",
+    version=VERSION,
     description="A General Toolbox for Identifying ObjectDetection Errors",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/rungalileo/tide",
     author="Galileo",
     author_email="galileo@rungalileo.io",
     license="MIT",
```

### Comparing `rungalileo-tidecv-0.0.2/tidecv/ap.py` & `rungalileo-tidecv-0.0.3/tidecv/ap.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/data.py` & `rungalileo-tidecv-0.0.3/tidecv/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 
     def add_image(self, id: int, name: str):
         """Register an image name/path with an image ID."""
         self.images[id]["name"] = name
 
     def get(self, image_id: int):
         """Collects all the annotations / detections for that particular image."""
-        return [self.annotations[x] for x in self.images[image_id]["anns"]]
+        return [self.annotations[x] for x in self.images.get(image_id, {}).get("anns", [])]
```

### Comparing `rungalileo-tidecv-0.0.2/tidecv/datasets.py` & `rungalileo-tidecv-0.0.3/tidecv/datasets.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/errors/error.py` & `rungalileo-tidecv-0.0.3/tidecv/errors/error.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/errors/main_errors.py` & `rungalileo-tidecv-0.0.3/tidecv/errors/main_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,17 @@
 
     description = (
         "Error caused when a prediction would have been marked positive "
         + "if it had the correct class and was localized better."
     )
     short_name = "ClsLoc"
 
-    def __init__(self, pred: dict):
+    def __init__(self, pred: dict, gt: dict):
         self.pred = pred
+        self.gt = gt
 
     def fix(self):
         return None
 
 
 class MissedError(Error):
```

### Comparing `rungalileo-tidecv-0.0.2/tidecv/errors/qualifiers.py` & `rungalileo-tidecv-0.0.3/tidecv/errors/qualifiers.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/functions.py` & `rungalileo-tidecv-0.0.3/tidecv/functions.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/plotting.py` & `rungalileo-tidecv-0.0.3/tidecv/plotting.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.2/tidecv/quantify.py` & `rungalileo-tidecv-0.0.3/tidecv/quantify.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self.run_errors = run_errors
 
         self._run()
 
     def _run(self):
         """And awaaay we go"""
 
-        for image in self.gt.images:
+        for image in set(self.gt.images).union(self.preds.images):
             x = self.preds.get(image)
             y = self.gt.get(image)
 
             # These classes are ignored for the whole image and not in the ground truth, so
             # we can safely just remove these detections from the predictions at the start.
             # However, since ignored detections are still used for error calculations, we have to keep them.
             if not self.run_errors:
@@ -299,15 +299,16 @@
                     # This should have been marked as background
                     self._add_error(BackgroundError(pred))
                     continue
 
                 # A base case to catch uncaught errors
                 # self._add_error(OtherError(pred))
                 # idx is already representing the gt box with highest overlap
-                self._add_error(ClassBoxError(pred))
+                self._add_error(ClassBoxError(pred, ex.gt[idx]))
+                pred["info"]["iou"] = iou
 
         for truth in gt:
             # If the GT wasn't used in matching, meaning it's some kind of false negative
             if not truth["ignore"] and not truth["used"]:
                 self.ap_data.push_false_negative(truth["class"], truth["_id"])
 
                 if self.run_errors:
```

