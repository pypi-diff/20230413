# Comparing `tmp/atlasofsmoothspaces-1.0.6.tar.gz` & `tmp/atlasofsmoothspaces-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.6.tar", last modified: Wed Apr 12 10:22:53 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.7.tar", last modified: Thu Apr 13 19:01:21 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.6.tar` & `atlasofsmoothspaces-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)    12118 2023-04-12 10:15:05.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-12 10:22:51.000000 atlasofsmoothspaces-1.0.6/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.334562 atlasofsmoothspaces-1.0.7/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)    12951 2023-04-13 18:59:47.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-13 19:01:21.334562 atlasofsmoothspaces-1.0.7/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-13 19:00:31.000000 atlasofsmoothspaces-1.0.7/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/main.py` & `atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     """
     MU = (XMAX - XMIN) / 2
     ALPHA = np.log((1-BETA) / BETA) / MU
     return YMIN + (YMAX-  YMIN) / (1 + np.exp((-1)* ALPHA * (x - MU)))
 
 
 class SmoothnessBase():
+    """It creates instances that can deal with smoothness.
+    In particular it takes new values and calculates the smoothness of them.
+    It is agnostic to the source of the data.
+    """
 
     
     def __init__(self, 
         cacheLength: int,
         derivativeDegree: int,
         alpha: float or list[float]):
 
@@ -46,14 +50,15 @@
                 raise Exception("There need to be as many values of alpha as there are degrees of derivatives!")
             self.__alphaIsList = True
             self.alpha = np.array(alpha)
         else:
             self.__alphaIsList = False
             self.alpha = alpha
         
+        ## lastUpdateTime is in milliseconds
         self.lastUpdateTime = time.time()*1000.0
                 
 
 
     def _addNewDerivative(self, newValue: float, newDelta: float):
         """add a value to the derivatives array
 
@@ -86,19 +91,30 @@
             if (self.smoothnessMeasures[measure]["isCalibrated"]):
                 self.smoothnessMeasures[measure]["calibratedSignal"] = sigmoid(
                     x=self.smoothnessMeasures[measure]["raw"], 
                     **self.smoothnessMeasures[measure]["calibration"])
         
         
 
-    def addNewValue(self, newValue: float, newDelta: float=None):
+    def addNewValue(self, newValue: float, newDelta: float=None, newTime: float=None):
         
-        newTime = time.time()*1000.0
-        if newDelta is None:
-            newDelta = newTime - self.lastUpdateTime
+        currentTime = time.time()*1000.0
+        if newDelta is None and newTime is None:
+            newDelta = currentTime - self.lastUpdateTime
+            newTime = currentTime
+        elif newDelta is None and newTime is not None:
+            currentTime = newTime 
+            newDelta = currentTime - self.lastUpdateTime
+        elif newDelta is not None and newTime is None:
+            currentTime = self.lastUpdateTime + newDelta
+        else:
+            raise Exception("Cant have both new Delta and new Time")
+
+
+
             
         self._addNewDelta(newDelta)
         newDerivatives = self._addNewDerivative(newValue, newDelta)
         self._addNewSmoothness(newDerivatives)
         self._updateSmoothnessMeasures()
 
         self.lastUpdateTime = newTime
@@ -221,18 +237,22 @@
         if smoothnessType in self.data:
             del self.data[smoothnessType] 
             del self.cacheLengths[smoothnessType] 
             del self.derivativeDegrees[smoothnessType] 
             del self.alphas[smoothnessType]     
 
 
-    def addNewValues(self, channelData: dict[int, float], returnSmoothness: bool = False):
+    def addNewValues(self, 
+                     channelData: dict[int, float],
+                     newTime: float = None, 
+                     newDelta: float = None, 
+                     returnSmoothness: bool = False):
         for smoothnessType in self.data.keys():
             newValue = self.conversion(smoothnessType, channelData)
-            self.data[smoothnessType].addNewValue(newValue)
+            self.data[smoothnessType].addNewValue(newValue, newTime=newTime, newDelta=newDelta)
         if returnSmoothness:
             return self.getSmoothnessMeasure()
         
 
     def getSmoothnessMeasure(self, smoothnessMeasure=None):
         smoothnessMeasure = (self.currentDefaultSmoothnessMeasure if smoothnessMeasure is None else smoothnessMeasure)
         return  {
```

### Comparing `atlasofsmoothspaces-1.0.6/setup.py` & `atlasofsmoothspaces-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.6' 
+VERSION = '1.0.7' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

