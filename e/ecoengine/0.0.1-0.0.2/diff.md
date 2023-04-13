# Comparing `tmp/ecoengine-0.0.1.tar.gz` & `tmp/ecoengine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.1.tar", last modified: Fri Apr  7 19:27:09 2023, max compression
+gzip compressed data, was "ecoengine-0.0.2.tar", last modified: Thu Apr 13 18:02:44 2023, max compression
```

## Comparing `ecoengine-0.0.1.tar` & `ecoengine-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.171819 ecoengine-0.0.1/
--rw-rw-rw-   0        0        0       59 2023-03-28 23:58:57.000000 ecoengine-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3644 2023-04-07 19:27:09.461223 ecoengine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3121 2023-04-07 19:26:25.000000 ecoengine-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      767 2023-04-07 19:27:09.554728 ecoengine-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-07 19:19:56.000000 ecoengine-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.299819 ecoengine-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.583819 ecoengine-0.0.1/src/ecoengine/
--rw-rw-rw-   0        0        0      938 2023-03-28 22:19:23.000000 ecoengine-0.0.1/src/ecoengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.403819 ecoengine-0.0.1/src/ecoengine/constants/
--rw-rw-rw-   0        0        0      457 2023-04-06 22:07:52.000000 ecoengine-0.0.1/src/ecoengine/constants/Constants.py
--rw-rw-rw-   0        0        0        0 2023-03-28 21:35:58.000000 ecoengine-0.0.1/src/ecoengine/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.455819 ecoengine-0.0.1/src/ecoengine/data/
--rw-rw-rw-   0        0        0        0 2023-03-28 23:03:59.000000 ecoengine-0.0.1/src/ecoengine/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.515819 ecoengine-0.0.1/src/ecoengine/data/load_shapes/
--rw-rw-rw-   0        0        0        0 2023-03-28 23:41:15.000000 ecoengine-0.0.1/src/ecoengine/data/load_shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.583819 ecoengine-0.0.1/src/ecoengine/engine/
--rw-rw-rw-   0        0        0     6895 2023-04-07 19:18:10.000000 ecoengine-0.0.1/src/ecoengine/engine/BuildingCreator.py
--rw-rw-rw-   0        0        0     7512 2023-04-07 17:59:25.000000 ecoengine-0.0.1/src/ecoengine/engine/EcosizerEngine.py
--rw-rw-rw-   0        0        0     2924 2023-04-07 19:18:05.000000 ecoengine-0.0.1/src/ecoengine/engine/SystemCreator.py
--rw-rw-rw-   0        0        0      917 2023-04-03 17:54:51.000000 ecoengine-0.0.1/src/ecoengine/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.623820 ecoengine-0.0.1/src/ecoengine/objects/
--rw-rw-rw-   0        0        0     9778 2023-04-07 19:17:33.000000 ecoengine-0.0.1/src/ecoengine/objects/Building.py
--rw-rw-rw-   0        0        0    24147 2023-04-07 19:17:41.000000 ecoengine-0.0.1/src/ecoengine/objects/SystemConfig.py
--rw-rw-rw-   0        0        0      965 2023-03-29 00:14:15.000000 ecoengine-0.0.1/src/ecoengine/objects/__init__.py
--rw-rw-rw-   0        0        0     3065 2023-04-07 19:08:24.000000 ecoengine-0.0.1/src/ecoengine/objects/systemConfigUtils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.671820 ecoengine-0.0.1/src/ecoengine/objects/systems/
--rw-rw-rw-   0        0        0     3563 2023-04-07 19:13:12.000000 ecoengine-0.0.1/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-rw-rw-   0        0        0    16890 2023-04-07 19:13:04.000000 ecoengine-0.0.1/src/ecoengine/objects/systems/SwingTank.py
--rw-rw-rw-   0        0        0        0 2023-03-28 21:35:43.000000 ecoengine-0.0.1/src/ecoengine/objects/systems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:27:04.359819 ecoengine-0.0.1/src/ecoengine.egg-info/
--rw-rw-rw-   0        0        0     3644 2023-04-07 19:27:03.000000 ecoengine-0.0.1/src/ecoengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      846 2023-04-07 19:27:04.000000 ecoengine-0.0.1/src/ecoengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:27:03.000000 ecoengine-0.0.1/src/ecoengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-07 19:27:03.000000 ecoengine-0.0.1/src/ecoengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-07 19:27:03.000000 ecoengine-0.0.1/src/ecoengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:44.214301 ecoengine-0.0.2/
+-rw-rw-rw-   0        0        0       59 2023-03-28 23:58:57.000000 ecoengine-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-04-13 18:02:44.280187 ecoengine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      767 2023-04-13 18:02:44.481451 ecoengine-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:33.502282 ecoengine-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:35.882286 ecoengine-0.0.2/src/ecoengine/
+-rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:38.918292 ecoengine-0.0.2/src/ecoengine/constants/
+-rw-rw-rw-   0        0        0      457 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/constants/Constants.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:39.282292 ecoengine-0.0.2/src/ecoengine/data/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:39.658293 ecoengine-0.0.2/src/ecoengine/data/load_shapes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/data/load_shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:41.082296 ecoengine-0.0.2/src/ecoengine/engine/
+-rw-rw-rw-   0        0        0     6879 2023-04-13 17:58:46.000000 ecoengine-0.0.2/src/ecoengine/engine/BuildingCreator.py
+-rw-rw-rw-   0        0        0     7508 2023-04-13 17:57:47.000000 ecoengine-0.0.2/src/ecoengine/engine/EcosizerEngine.py
+-rw-rw-rw-   0        0        0     2924 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/engine/SystemCreator.py
+-rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:42.682299 ecoengine-0.0.2/src/ecoengine/objects/
+-rw-rw-rw-   0        0        0     9746 2023-04-13 17:58:54.000000 ecoengine-0.0.2/src/ecoengine/objects/Building.py
+-rw-rw-rw-   0        0        0    23618 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/SystemConfig.py
+-rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/__init__.py
+-rw-rw-rw-   0        0        0     2948 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systemConfigUtils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:43.870301 ecoengine-0.0.2/src/ecoengine/objects/systems/
+-rw-rw-rw-   0        0        0     3509 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-rw-rw-   0        0        0    16890 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/SwingTank.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:02:38.202290 ecoengine-0.0.2/src/ecoengine.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2023-04-13 18:02:33.000000 ecoengine-0.0.2/src/ecoengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 18:02:32.000000 ecoengine-0.0.2/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.1/PKG-INFO` & `ecoengine-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -110,15 +110,23 @@
 2. navigate to docs directory and run:
 
 
 	$ make html
 
 ### Updating version on pypi
 
-1. Update the version number in setup.cfg
-2. Run the following commands from the project root directory:
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
 
 	$ python -m build
+
 	$ python -m twine upload dist/*
 
 ### Contact Information
 To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.1/README.md` & `ecoengine-0.0.2/src/ecoengine.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: ecoengine
+Version: 0.0.2
+Summary: A software for sizing Heat Pump Water Heaters for buildings
+Home-page: https://ecosizer.ecotope.com/sizer/
+Author: Nolan
+Author-email: nolan@ecotope.com
+Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
 # EcosizerEngine
 
 ### Requirements:
 
 This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
 
 ### Using the package in scripts:
@@ -96,15 +110,23 @@
 2. navigate to docs directory and run:
 
 
 	$ make html
 
 ### Updating version on pypi
 
-1. Update the version number in setup.cfg
-2. Run the following commands from the project root directory:
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
 
 	$ python -m build
+
 	$ python -m twine upload dist/*
 
 ### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.1/setup.cfg` & `ecoengine-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 656e 6769 6e65 0d0a 7665   = ecoengine..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 310d 0a61  rsion = 0.0.1..a
+00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a61  rsion = 0.0.2..a
 00000030: 7574 686f 7220 3d20 4e6f 6c61 6e0d 0a61  uthor = Nolan..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 6e6f  uthor_email = no
 00000050: 6c61 6e40 6563 6f74 6f70 652e 636f 6d0d  lan@ecotope.com.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 6f66 7477 6172 6520 666f 7220 7369   software for si
 00000080: 7a69 6e67 2048 6561 7420 5075 6d70 2057  zing Heat Pump W
 00000090: 6174 6572 2048 6561 7465 7273 2066 6f72  ater Heaters for
```

### Comparing `ecoengine-0.0.1/src/ecoengine/__init__.py` & `ecoengine-0.0.2/src/ecoengine/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-""" 
-	EcosizerEngine
-    Copyright (C) 2023  Ecotope Inc.
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-
-__all__ = ['EcosizerEngine', 'createBuilding', 'createSystem']
-from .engine.EcosizerEngine import *
-from .engine.BuildingCreator import createBuilding
+""" 
+	EcosizerEngine
+    Copyright (C) 2023  Ecotope Inc.
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+
+__all__ = ['EcosizerEngine', 'createBuilding', 'createSystem']
+from .engine.EcosizerEngine import *
+from .engine.BuildingCreator import createBuilding
 from .engine.SystemCreator import createSystem
```

### Comparing `ecoengine-0.0.1/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.2/src/ecoengine/engine/BuildingCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ecoengine.objects.Building import *
 import numpy as np
 
 def createBuilding(incomingT_F, magnitudeStat, supplyT_F, buildingType, loadshape = None, avgLoadshape = None,
-                    returnT_F = 0, flow_rate = 0, gpdpp = 0, nBR = None, nApt = 0, Wapt = 0, standardGPD = None):
+                    returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, nApt = 0, Wapt = 0, standardGPD = None):
     
     """
     Initializes the building in which the HPWH system will be sized for
 
     Attributes
     ----------
     incomingT_F : float 
@@ -19,15 +19,15 @@
         a string indicating the type of building we are sizing for (e.g. "multi_family", "office_building", etc.)
     loadShape : ndarray
         defaults to design load shape for building type.
     avgLoadShape : ndarray
         defaults to average load shape for building type.
     returnT_F : float 
         The water temperature returning from the recirculation loop. [°F]
-    flow_rate : float 
+    flowRate : float 
         The pump flow rate of the recirculation loop. (GPM)
     gpdpp : float
         The volume of water in gallons at 120F each person uses per dat.[°F]
     nBR : array_like
         A list of the number of units by size in the order 0 bedroom units,
         1 bedroom units, 2 bedroom units, 3 bedroom units, 4 bedroom units,
         5 bedroom units.
@@ -51,16 +51,16 @@
         else:
             if not isinstance(magnitudeStat, list) or len(buildingType) != len(magnitudeStat):
                 raise Exception("Missing values for multi-use building. Collected " + str(len(buildingType)) + " building types but collected " + 
                                 ("1" if not isinstance(magnitudeStat, list) else str(len(magnitudeStat)))+ " magnitude varriables")
             building_list = []
             for i in range(len(buildingType)):
                 building_list.append(createBuilding(incomingT_F, magnitudeStat[i], supplyT_F, buildingType[i], loadshape, avgLoadshape,
-                        returnT_F, flow_rate, gpdpp, nBR, nApt, Wapt))
-            return MultiUse(building_list, incomingT_F, supplyT_F, returnT_F, flow_rate)
+                        returnT_F, flowRate, gpdpp, nBR, nApt, Wapt))
+            return MultiUse(building_list, incomingT_F, supplyT_F, returnT_F, flowRate)
     
     #only one building type so there should only be one magnitude statistic 
     if isinstance(magnitudeStat, list):
         if len(magnitudeStat) == 1:
             magnitudeStat = magnitudeStat[0]
         else:
             raise Exception("Missing values for multi-use building. Collected 1 building type but collected " + str(len(magnitudeStat)) + " magnitude varriables")
@@ -79,37 +79,37 @@
         checkLoadShape(avgLoadshape)
 
     loadshape = np.array(loadshape) # TODO - this changes values of loadshape a bit, show this to scott
     avgLoadshape = np.array(avgLoadshape) # TODO - this changes values of loadshape a bit, show this to scott
 
     match buildingType:
         case 'apartment':
-            return Apartment(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return Apartment(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'elementary_school':
-            return ElementarySchool(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return ElementarySchool(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'food_service_a':
-            return FoodServiceA(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return FoodServiceA(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'food_service_b':
-            return FoodServiceB(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return FoodServiceB(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'junior_high':
-            return JuniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return JuniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'mens_dorm':
-            return MensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return MensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'motel':
-            return Motel(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return Motel(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'nursing_home':
-            return NursingHome(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return NursingHome(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'office_building':
-            return OfficeBuilding(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return OfficeBuilding(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'senior_high':
-            return SeniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return SeniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'womens_dorm':
-            return WomensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+            return WomensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         case 'multi_family':
-            return MultiFamily(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate, gpdpp, nBR, nApt, Wapt, standardGPD)
+            return MultiFamily(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, gpdpp, nBR, nApt, Wapt, standardGPD)
         case _:
             raise Exception("Unrecognized building type.")
         
 def getLoadShape(file_name, shape = 'Stream'):
     if shape != 'Stream' and shape != 'Stream_Avg':
         raise Exception("Mapping key not found for loadshapes, valid keys are: 'Stream', or 'Stream_Avg'")
     try:
```

### Comparing `ecoengine-0.0.1/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.2/src/ecoengine/engine/EcosizerEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         defaults to average load shape for building type.
     loadShiftSchedule : array_like
         List or array of 0's and 1's for don't run and run respectively. Used for load shifting
     loadShiftPercent: float
         Percentage of days the load shift will be met
     returnT_F : float 
         The water temperature returning from the recirculation loop. [°F]
-    flow_rate : float 
+    flowRate : float 
         The pump flow rate of the recirculation loop. (GPM)
     gpdpp : float
         The volume of water in gallons at 120F each person uses per dat.[°F]
     nBR : array_like
         A list of the number of units by size in the order 0 bedroom units,
         1 bedroom units, 2 bedroom units, 3 bedroom units, 4 bedroom units,
         5 bedroom units.
@@ -66,26 +66,26 @@
         Maximum hours per day the temperature maintenance equipment can run
     standardGPD : string
         indicates whether to use a standard gpdpp specification for multi-family buildings. Set to None if not using a standard gpdpp.
     """
 
     def __init__(self, incomingT_F, magnitudeStat, supplyT_F, storageT_F, percentUseable, aquaFract, 
                             schematic, buildingType, loadshape = None, avgLoadshape = None, loadShiftSchedule = None, loadShiftPercent = 1,
-                            returnT_F = 0, flow_rate = 0, gpdpp = 0, nBR = None, safetyTM = 1.75,
+                            returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, safetyTM = 1.75,
                             defrostFactor = 1, compRuntime_hr = 16, nApt = 0, Wapt = 0, doLoadShift = False,
                             setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333, standardGPD = None):
         
         building = createBuilding(  incomingT_F     = incomingT_F,
                                     magnitudeStat   = magnitudeStat, 
                                     supplyT_F       = supplyT_F, 
                                     buildingType    = buildingType,
                                     loadshape       = loadshape,
                                     avgLoadshape    = avgLoadshape,
                                     returnT_F       = returnT_F, 
-                                    flow_rate       = flow_rate,
+                                    flowRate       = flowRate,
                                     gpdpp           = gpdpp,
                                     nBR             = nBR,
                                     nApt            = nApt,
                                     Wapt            = Wapt,
                                     standardGPD     = standardGPD
         )
```

### Comparing `ecoengine-0.0.1/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.2/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.1/src/ecoengine/objects/Building.py` & `ecoengine-0.0.2/src/ecoengine/objects/Building.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import json
 import numpy as np
 
 from ecoengine.constants.Constants import *
 
 class Building:
-    def __init__(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         
-        self._checkParams(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        self._checkParams(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
         self.loadshape = loadshape
         self.avgLoadshape = avgLoadshape
         self.incomingT_F = incomingT_F
         self.supplyT_F = supplyT_F
-        self.recirc_loss = (supplyT_F - returnT_F) * flow_rate * rhoCp * 60. #BTU/HR
+        self.recirc_loss = (supplyT_F - returnT_F) * flowRate * rhoCp * 60. #BTU/HR
 
-    def _checkParams(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def _checkParams(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         if not isinstance(loadshape, np.ndarray) or len(loadshape) != 24:
             raise Exception("Error: Loadshape must be a list of length 24.")
         if sum(loadshape) > 1 + 1e-3 or sum(loadshape) < 1 - 1e-3:
             raise Exception("Error:  Sum of the loadshape does not equal 1 but "+str(sum(loadshape))+".")
         if any(x < 0 for x in loadshape):
             raise Exception("Error:  Can not have negative load shape values in loadshape.")
         if not isinstance(avgLoadshape, np.ndarray) or len(avgLoadshape) != 24:
@@ -32,76 +32,76 @@
             raise Exception("Error: Supply temp must be a number.")
         if not (isinstance(returnT_F, int) or isinstance(returnT_F, float)):
             raise Exception("Error: Return temp must be a number.")
         if supplyT_F <= returnT_F:
             raise Exception("Error: Supply temp must be higher than return temp.")
         if not (isinstance(incomingT_F, int) or isinstance(incomingT_F, float)):
             raise Exception("Error: City water temp must be a number.")
-        if not (isinstance(flow_rate, int) or isinstance(flow_rate, float)):
+        if not (isinstance(flowRate, int) or isinstance(flowRate, float)):
             raise Exception("Error: Flow rate must be a number.")
         if not hasattr(self, 'magnitude'):
             raise Exception("Magnitude has not been set.")
 
 class MensDorm(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_students * 18.9 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class WomensDorm(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_students * 16.4 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class Motel(Building):
-    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_units * 28.8 # ASHREA GPD per unit
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class NursingHome(Building):
-    def __init__(self, n_beds, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_beds, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_beds * 20.1 # ASHREA GPD per bed
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class OfficeBuilding(Building):
-    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_people * 1.11 # ASHREA GPD per person
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class FoodServiceA(Building):
-    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_meals * 11.032 # ASHREA GPD per meal
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class FoodServiceB(Building):
-    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_meals * 6.288 # ASHREA GPD per meal
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class Apartment(Building):
-    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_units * 42.8 # ASHREA GPD per unit
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class ElementarySchool(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_students * 1.081 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class JuniorHigh(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_students * 3.27 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
 
 class SeniorHigh(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
         self.magnitude = n_students * 3.02 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
     
 class MultiFamily(Building):
-    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate, gpdpp, nBR, nApt, Wapt, standardGPD):
+    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, gpdpp, nBR, nApt, Wapt, standardGPD):
         # check inputs
         if not (isinstance(nApt, int)):
             raise Exception("Error: Number of apartments must be an integer.")
         if not (isinstance(Wapt, int)):
             raise Exception("Error: WATTs per apt must be an integer.")
         if standardGPD is None:
             if not (isinstance(gpdpp, int) or isinstance(gpdpp, float)):
@@ -127,21 +127,21 @@
                     else:
                         gpdpp = dataDict['gpdpp'][standardGPD][0]
             else:
                 raise Exception("Error: standardGPD must be a String of one of the following values: " + str(possibleStandardGPDs))
             
         self.magnitude = gpdpp * n_people # gpdpp * number_of_people
 
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         # recalculate recirc_loss with different method if applicable
         if(nApt > 0 and Wapt > 0):
             self.recirc_loss = nApt * Wapt * W_TO_BTUHR
 
 class MultiUse(Building):
-    def __init__(self, building_list, incomingT_F, supplyT_F, returnT_F, flow_rate):
+    def __init__(self, building_list, incomingT_F, supplyT_F, returnT_F, flowRate):
         # Generates building with loadshape that is combination of multiple loadshapes, one for each use section of the building. Each loadshape is multiplied
         # by the magnitude of that use section of the multi-use building, then all added together and divided by the total magnitude for the whole building
 
         total_magnitude = building_list[0].magnitude
         total_loadshape = [j * building_list[0].magnitude for j in building_list[0].loadshape]
         total_avg_loadshape = [j * building_list[0].magnitude for j in building_list[0].avgLoadshape]
 
@@ -155,8 +155,8 @@
         total_loadshape = [j / total_magnitude for j in total_loadshape]
         total_avg_loadshape = [j / total_magnitude for j in total_avg_loadshape]
         total_loadshape = np.array(total_loadshape)
         total_avg_loadshape = np.array(total_avg_loadshape)
 
         self.magnitude = total_magnitude
 
-        super().__init__(total_loadshape, total_avg_loadshape, incomingT_F, supplyT_F, returnT_F, flow_rate)
+        super().__init__(total_loadshape, total_avg_loadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
```

### Comparing `ecoengine-0.0.1/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.2/src/ecoengine/objects/SystemConfig.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,529 +1,529 @@
-from ecoengine.constants.Constants import *
-from .Building import Building
-import numpy as np
-from scipy.stats import norm #lognorm
-from plotly.graph_objs import Figure, Scatter
-from plotly.offline import plot
-from .systemConfigUtils import roundList, mixVolume, hrToMinList, getPeakIndices, checkLiqudWater, checkHeatHours
-
-class SystemConfig:
-    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
-        # check inputs. LoadShiftSchedule not checked because it is checked elsewhere
-        self._checkInputs(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent)
-        
-        self.doLoadShift = doLoadShift
-        self.building = building        
-        # self.totalHWLoad = self.building.magnitude
-        self.storageT_F = storageT_F
-        self.defrostFactor = defrostFactor
-        self.percentUseable = percentUseable
-        self.compRuntime_hr = compRuntime_hr
-        self.aquaFract = aquaFract
-
-        if doLoadShift and not loadShiftSchedule is None:
-            self._setLoadShift(loadShiftSchedule, loadShiftPercent)
-        else:
-            self.loadShiftSchedule = [1] * 24
-            self.fract_total_vol = 1 # fraction of total volume for for load shifting, or 1 if no load shifting
-
-        #Check if need to increase sizing to meet lower runtimes for load shift
-        self.maxDayRun_hr = min(self.compRuntime_hr, sum(self.loadShiftSchedule))
-
-        #size system
-        self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr)
-        self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, self.effSwingFract )
-
-    def _checkInputs(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent):
-        if not isinstance(building, Building):
-            raise Exception("Error: Building is not valid.")
-        if not (isinstance(storageT_F, int) or isinstance(storageT_F, float)) or not checkLiqudWater(storageT_F):
-            raise Exception('Invalid input given for Storage temp, it must be between 32 and 212F.')
-        if not (isinstance(defrostFactor, int) or isinstance(defrostFactor, float)) or defrostFactor < 0 or defrostFactor > 1:
-            raise Exception("Invalid input given for Defrost Factor, must be a number between 0 and 1.")
-        if not (isinstance(percentUseable, int) or isinstance(percentUseable, float)) or percentUseable > 1 or percentUseable < 0:
-            raise Exception("Invalid input given for percentUseable, must be a number between 0 and 1.")
-        if not isinstance(compRuntime_hr, int) or compRuntime_hr <= 0 or compRuntime_hr > 24:
-            raise Exception("Invalid input given for compRuntime_hr, must be an integer between 0 and 24.")
-        if not (isinstance(aquaFract, int) or isinstance(aquaFract, float)) or aquaFract > 1 or aquaFract <= 0:
-            raise Exception("Invalid input given for aquaFract must, be a number between 0 and 1.")
-        if not (isinstance(loadShiftPercent, int) or isinstance(loadShiftPercent, float)) or loadShiftPercent > 1 or loadShiftPercent < 0:
-            raise Exception("Invalid input given for loadShiftPercent, must be a number between 0 and 1.")
-        if not isinstance(doLoadShift, bool):
-            raise Exception("Invalid input given for doLoadShift, must be a boolean.")
-
-    def getSizingResults(self):
-        """
-        Returns the minimum primary volume and heating capacity sizing results. Implimented seperatly in Temp Maintenence systems.
-
-        Returns
-        -------
-        list
-            self.PVol_G_atStorageT, self.PCap_kBTUhr
-        """
-        return [self.PVol_G_atStorageT, self.PCap_kBTUhr]
-
-    def simulate(self, initPV=None, initST=None, Pcapacity=None, Pvolume=None):
-        """
-        Implimented seperatly for Swink Tank systems 
-        Inputs
-        ------
-        initPV : float
-            Primary volume at start of the simulation
-        initST : float
-            Primary Swing tank at start of the simulation. Not used in this instance of the function
-        Pcapacity : float
-            The primary heating capacity in kBTUhr to use for the simulation,
-            default is the sized system
-        Pvolume : float
-            The primary storage volume in gallons to  to use for the simulation,
-            default is the sized system
-        
-        Returns
-        -------
-        list [ pV, G_hw, D_hw, prun ]
-        pV : list 
-            Volume of HW in the tank with time at the strorage temperature.
-        G_hw : list 
-            The generation of HW with time at the supply temperature
-        D_hw : list 
-            The hot water demand with time at the tsupply temperature
-        prun : list 
-            The actual output in gallons of the HPWH with time
-        """
-
-        G_hw, D_hw, V0, Vtrig, pV, pheating = self._getInitialSimulationValues(Pcapacity, Pvolume)
-
-        hw_outSwing = [0] * (len(G_hw))
-        hw_outSwing[0] = D_hw[0]
-        prun = [0] * (len(G_hw))
-
-        if initPV:
-            pV[0] = initPV
-
-        # Run the "simulation"
-        for i in range(1, len(G_hw)):
-            mixedDHW = mixVolume(D_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
-            mixedGHW = mixVolume(G_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
-            pheating, pV[i], prun[i] = self.runOnePrimaryStep(pheating, V0, Vtrig, pV[i-1], mixedDHW, mixedGHW)
-
-        return [roundList(pV, 3),
-                roundList(G_hw, 3),
-                roundList(D_hw, 3),
-                roundList(prun, 3)]
-
-    def _getInitialSimulationValues(self, Pcapacity=None, Pvolume=None):
-        """
-        Returns initialized arrays needed for 3-day simulation
-
-        Parameters
-        ----------
-        Pcapacity : float
-            The primary heating capacity in kBTUhr to use for the simulation,
-            default is the sized system
-        Pvolume : float
-            The primary storage volume in gallons to  to use for the simulation,
-            default is the sized system
-
-        Returns
-        -------
-        list [ G_hw, D_hw, V0, V, run, pheating ]
-        G_hw : list
-            The generation of HW with time at the supply temperature
-        D_hw : list
-            The hot water demand with time at the tsupply temperature
-        V0 : float
-            The storage volume of the primary system at the storage temperature
-        Vtrig : float
-            The remaining volume of the primary storage volume when heating is
-            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho?
-        pV : list 
-            Volume of HW in the tank with time at the strorage temperature. Initialized to array of 0s with pV[0] set to V0
-        pheating : boolean 
-            set to false. Simulation starts with a full tank so primary heating starts off
-        """
-        if not Pcapacity:
-            Pcapacity =  self.PCap_kBTUhr
-
-        if not Pvolume:
-            Pvolume =  self.PVol_G_atStorageT
-
-        loadShapeN = self.building.loadshape
-        if self.doLoadShift:
-            loadShapeN = self.building.avgLoadshape
-
-        # Get the generation rate from the primary capacity
-        G_hw = 1000 * Pcapacity / rhoCp / (self.building.supplyT_F - self.building.incomingT_F) \
-               * self.defrostFactor * np.tile(self.loadShiftSchedule,3)
-        
-        # Define the use of DHW with the normalized load shape
-        D_hw = self.building.magnitude * self.fract_total_vol * np.tile(loadShapeN, 3)
-
-        # To per minute from per hour
-        G_hw = np.array(hrToMinList(G_hw)) / 60
-        D_hw = np.array(hrToMinList(D_hw)) / 60
-
-        # Init the "simulation"
-        V0 = np.ceil(Pvolume * self.percentUseable)
-        Vtrig = np.ceil(Pvolume * (1 - self.aquaFract)) + 1 # To prevent negatives with any of that rounding math.
-        pV = [V0] + [0] * (len(G_hw) - 1)
-
-        pheating = False
-
-        return G_hw, D_hw, V0, Vtrig, pV, pheating
-    
-    def _setLoadShift(self, loadShiftSchedule, loadShiftPercent=1):
-        """
-        Sets the load shifting schedule from input loadShiftSchedule
-
-        Parameters
-        ----------
-        loadShiftSchedule : array_like
-            List or array of 0's and 1's for don't run and run.
-
-        loadShiftPercent : float
-            Percentile of days which need to be covered by load shifting
-
-        """
-        # Check
-        if len(loadShiftSchedule) != 24 : #TODO ensure loadShiftSchedule is valid and add load up
-            raise Exception("loadshift is not of length 24 but instead has length of "+str(len(loadShiftSchedule))+".")
-        if sum(loadShiftSchedule) == 0 :
-            raise Exception("When using Load shift the HPWH's must run for at least 1 hour each day.")
-        if loadShiftPercent < 0.25 :
-            raise Exception("Load shift only available for above 25 percent of days.")
-        if loadShiftPercent > 1 :
-            raise Exception("Cannot load shift for more than 100 percent of days")
-
-        self.loadShiftSchedule = loadShiftSchedule
-        self.loadshift = np.array(loadShiftSchedule, dtype = float)# Coerce to numpy array of data type float
-
-        # adjust for loadShiftPercent
-        if loadShiftPercent == 1: # meaing 100% of days covered by load shift
-            self.fract_total_vol = 1
-        else:
-            # calculate fraction total hot water required to meet load shift days
-            fract = norm_mean + norm_std * norm.ppf(loadShiftPercent) #TODO norm_mean and std are currently from multi-family, need other types eventually. For now, loadshifting will only be available for multi-family
-            self.fract_total_vol = fract if fract <= 1. else 1.
-        
-        self.doLoadShift = True
-
-    # SwingTank has it's own implimentation
-    def _primaryHeatHrs2kBTUHR(self, heathours, effSwingVolFract=1):
-        """
-        Converts from hours of heating in a day to heating capacity.
-
-        Implimented seperatly in Swing Tank systems
-
-        Parameters
-        ----------
-        heathours : float or numpy.ndarray
-            The number of hours primary heating equipment can run.
-
-        effSwingVolFract : float or numpy.ndarray
-            The fractional adjustment to the total hot water load for the
-            primary system. Only used in a swing tank system.
-
-        Returns
-        -------
-        heatCap
-            The heating capacity in [btu/hr].
-        """
-        checkHeatHours(heathours)
-        heatCap = self.building.magnitude / heathours * rhoCp * \
-            (self.building.supplyT_F - self.building.incomingT_F) / self.defrostFactor /1000.
-        return heatCap
-    
-    def sizePrimaryTankVolume(self, heatHrs):
-        """
-        Calculates the primary storage using the Ecotope sizing methodology
-
-        Parameters
-        ----------
-        heatHrs : float
-            The number of hours primary heating equipment can run in a day.
-        
-        Raises
-        ------
-        ValueError: aquastat fraction is too low.
-        ValueError: The minimum aquastat fraction is greater than 1.
-
-        Returns
-        -------
-        totalVolMax : float
-            The total storage volume in gallons adjusted to the storage tempreature
-        effMixFract : float
-            The fractional adjustment to the total hot water load for the
-            primary system. Only used in a swing tank system.
-        
-        """
-        if heatHrs <= 0 or heatHrs > 24:
-            raise Exception("Heat hours is not within 1 - 24 hours")
-        # Fraction used for adjusting swing tank volume.
-        effMixFract = 1.
-
-        # Running vol
-        runningVol_G, effMixFract = self._calcRunningVol(heatHrs, np.ones(24), self.building.loadshape, effMixFract)
-
-        # If doing load shift, solve for the runningVol_G and take the larger volume
-        if self.doLoadShift:
-            LSrunningVol_G = 0
-            LSeffMixFract = 0
-            # calculate loadshift sizing with avg loadshape (see page 19 of methodology documentation)
-            LSrunningVol_G, LSeffMixFract = self._calcRunningVol(heatHrs, self.loadShiftSchedule, self.building.avgLoadshape, LSeffMixFract)
-            LSrunningVol_G *= self.fract_total_vol
-
-            # Get total volume from max of primary method or load shift method
-            if LSrunningVol_G > runningVol_G:
-                runningVol_G = LSrunningVol_G
-                effMixFract = LSeffMixFract
-
-        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G)
-
-        # Check the Cycling Volume ############################################
-        cyclingVol_G = totalVolAtStorage * (self.aquaFract - (1 - self.percentUseable))
-        minRunVol_G = pCompMinimumRunTime * (self.building.magnitude * effMixFract / heatHrs) # (generation rate - no usage)
-
-        if minRunVol_G > cyclingVol_G:
-            min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
-            if min_AF < 1:
-                raise ValueError("01", "The aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
-            raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
-
-        # Return the temperature adjusted total volume ########################
-        return totalVolAtStorage, effMixFract
-    
-    def _calcRunningVol(self, heatHrs, onOffArr, loadshape, effMixFract = 0):
-        """
-        Function to find the running volume for the hot water storage tank, which
-        is needed for calculating the total volume for primary sizing and in the event of load shift sizing
-        represents the entire volume.
-
-        Implimented seperatly for Swing Tank systems
-
-        Parameters
-        ----------
-        heatHrs : float
-            The number of hours primary heating equipment can run in a day.
-        onOffArr : ndarray
-            array of 1/0's where 1's allow heat pump to run and 0's dissallow. of length 24.
-        loadshape : ndarray
-            normalized array of length 24 representing the daily loadshape for this calculation.
-        effMixFract: Int
-            unused value in this instance of the function. Used in Swing Tank implimentation
-
-        Raises
-        ------
-        Exception: Error if oversizeing system.
-
-        Returns
-        -------
-        runV_G : float
-            The running volume in gallons
-        effMixFract: int
-            returns same value from parameter. Needed for Swing Tank implimentation. Not actually used in this function instance 
-        """          
-        genrate = np.tile(onOffArr,2) / heatHrs #hourly
-        diffN = genrate - np.tile(loadshape,2) #hourly
-        diffInd = getPeakIndices(diffN[0:24]) #Days repeat so just get first day!
-        diffN *= self.building.magnitude
-        # Get the running volume ##############################################
-        if len(diffInd) == 0:
-            #TODO but what if it is undersized? Also can this ever be hit? users currently do not have power to change num hours from interface
-            raise Exception("ERROR ID 03","The heating rate is greater than the peak volume the system is oversized! Try increasing the hours the heat pump runs in a day",)
-        runV_G = 0
-        for peakInd in diffInd:
-            #Get the rest of the day from the start of the peak
-            diffCum = np.cumsum(diffN[peakInd:])  #hourly
-            runV_G = max(runV_G, -min(diffCum[diffCum<0.])) #Minimum value less than 0 or 0.
-
-        return runV_G, effMixFract
-    
-    def _getTotalVolAtStorage(self, runningVol_G):
-        """
-        Calculates the maximum primary storage using the Ecotope sizing methodology. Swing Tanks implement sperately
-
-        Parameters
-        ----------
-        runningVol_G : float
-            The running volume in gallons
-
-        Returns
-        -------
-        totalVolMax : float
-            The total storage volume in gallons adjusted to the storage tempreature
-        
-        """
-        return mixVolume(runningVol_G, self.storageT_F, self.building.incomingT_F, self.building.supplyT_F) / (1-self.aquaFract)
-    
-    def primaryCurve(self):
-        """
-        Sizes the primary system curve. Will catch the point at which the aquatstat
-        fraction is too small for system and cuts the return arrays to match cutoff point.
-
-        Returns
-        -------
-        volN : array
-            Array of volume in the tank at each hour.
-
-        primaryHeatHrs2kBTUHR : array
-            Array of heating capacity in kBTU/hr
-            
-        heatHours : array
-            Array of running hours per day corresponding to primaryHeatHrs2kBTUHR
-            
-        recIndex : int
-            The index of the recommended heating rate. 
-        """
-        # Define the heating hours we'll check
-        delta = -0.25
-        maxHeatHours = 1/(max(self.building.loadshape))*1.001   
-        
-        arr1 = np.arange(24, self.maxDayRun_hr, delta)
-        recIndex = len(arr1)
-        heatHours = np.concatenate((arr1, np.arange(self.maxDayRun_hr, maxHeatHours, delta)))
-        
-        volN = np.zeros(len(heatHours))
-        effMixFract = np.ones(len(heatHours))
-        for i in range(0,len(heatHours)):
-            try:
-                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i])
-            except ValueError:
-                break
-        # Cut to the point the aquastat fraction was too small
-        volN        = volN[:i]
-        heatHours   = heatHours[:i]
-        effMixFract = effMixFract[:i]
-
-        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, effMixFract), heatHours, recIndex]
-
-    
-    def runOnePrimaryStep(self, pheating, V0, Vtrig, Vcurr, hw_out, hw_in):
-        """
-        Runs one step on the primary system. This changes the volume of the primary system
-        by assuming there is hot water removed at a volume of hw_out and hot water
-        generated or added at a volume of hw_in. This is assuming the system is perfectly
-        stratified and all of the hot water above the cold temperature is at the storage temperature.
-
-        Parameters
-        ----------
-        pheating : boolean
-            indicates whether system is heating at the beginning of this step
-        V0 : float
-            The storage volume of the primary system at the storage temperature
-        Vtrig : float
-            The remaining volume of the primary storage volume when heating is
-            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho? 
-        Vcurr : float
-            The primary volume at the timestep.
-        hw_out : float
-            The volume of DHW removed from the primary system, assumed that
-            100% of what of what is removed is replaced
-        hw_in : float
-            The volume of hot water generated in a time step
-
-        Returns
-        -------
-        pheating : boolean
-            Boolean indicating if the primary system is heating at the end of this step in the simulation 
-        Vnew : float
-            The new primary volume at the timestep.
-        did_run : float
-            The volume of hot water generated during the time step.
-
-        """
-        did_run = 0
-        Vnew = 0
-        if pheating:
-            Vnew = Vcurr + hw_in - hw_out # If heating, generate HW and lose HW
-            did_run = hw_in
-
-        else:  # Else not heating,
-            Vnew = Vcurr - hw_out # So lose HW
-            if Vnew < Vtrig: # If should heat
-                time_missed = (Vtrig - Vnew)/hw_out # Volume below turn on / rate of draw gives time below tigger
-                Vnew += hw_in * time_missed # Start heating
-                did_run = hw_in * time_missed
-                pheating = True
-
-        if Vnew > V0: # If overflow
-            time_over = (Vnew - V0) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
-            Vnew = V0 - hw_out * time_over # Make full with missing volume
-            did_run = hw_in * (1-time_over)
-            pheating = False # Stop heating
-
-        if Vnew < 0:
-           raise Exception("Primary storage ran out of Volume!")
-
-        return pheating, Vnew, did_run
-    
-    def plotStorageLoadSim(self, return_as_div=True):
-        """
-        Returns a plot of the of the simulation for the minimum sized primary
-        system as a div or plotly figure. Can plot the minute level simulation
-
-        Implimented seperatly for Swing Tank systems
-
-        Parameters
-        ----------
-        return_as_div
-            A logical on the output, as a div (true) or as a figure (false)
-
-        Returns
-        -------
-        div/fig
-            plot_div
-        """
-        [V, G_hw, D_hw, run] = self.simulate()
-
-        hrind_fromback = 24 # Look at the last 24 hours of the simulation not the whole thing
-        run = np.array(run[-(60*hrind_fromback):])*60
-        G_hw = np.array(G_hw[-(60*hrind_fromback):])*60
-        D_hw = np.array(D_hw[-(60*hrind_fromback):])*60
-        V = np.array(V[-(60*hrind_fromback):])
-
-        if any(i < 0 for i in V):
-            raise Exception("Primary storage ran out of Volume!")
-
-        fig = Figure()
-
-        # Do primary components
-        x_data = list(range(len(V)))
-
-        if self.doLoadShift:
-            ls_off = [int(not x)* max(V)*2 for x in G_hw]
-            fig.add_trace(Scatter(x=x_data, y=ls_off, name='Load Shift Off Period',
-                                  mode='lines', line_shape='hv',
-                                  opacity=0.5, marker_color='grey',
-                                  fill='tonexty'))
-
-        fig.add_trace(Scatter(x=x_data, y=V, name='Useful Storage Volume at Storage Temperature',
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='green'))
-        fig.add_trace(Scatter(x=x_data, y=run, name = "Hot Water Generation at Storage Temperature",
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='red'))
-        fig.add_trace(Scatter(x=x_data, y=D_hw, name='Hot Water Demand at Supply Temperature',
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='blue'))
-        fig.update_yaxes(range=[0, np.ceil(max(np.append(V,D_hw))/100)*100])
-
-        fig.update_layout(title="Hot Water Simulation",
-                          xaxis_title= "Minute of Day",
-                          yaxis_title="Gallons or\nGallons per Hour",
-                          width=900,
-                          height=700)
-
-        if return_as_div:
-            plot_div = plot(fig, output_type='div', show_link=False, link_text="",
-                        include_plotlyjs = False)
-            return plot_div
-        return fig
-    
-    
-class Primary(SystemConfig):
-    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
-        super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule)
-
+from ecoengine.constants.Constants import *
+from .Building import Building
+import numpy as np
+from scipy.stats import norm #lognorm
+from plotly.graph_objs import Figure, Scatter
+from plotly.offline import plot
+from .systemConfigUtils import roundList, mixVolume, hrToMinList, getPeakIndices, checkLiqudWater, checkHeatHours
+
+class SystemConfig:
+    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
+        # check inputs. LoadShiftSchedule not checked because it is checked elsewhere
+        self._checkInputs(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent)
+        
+        self.doLoadShift = doLoadShift
+        self.building = building        
+        # self.totalHWLoad = self.building.magnitude
+        self.storageT_F = storageT_F
+        self.defrostFactor = defrostFactor
+        self.percentUseable = percentUseable
+        self.compRuntime_hr = compRuntime_hr
+        self.aquaFract = aquaFract
+
+        if doLoadShift and not loadShiftSchedule is None:
+            self._setLoadShift(loadShiftSchedule, loadShiftPercent)
+        else:
+            self.loadShiftSchedule = [1] * 24
+            self.fract_total_vol = 1 # fraction of total volume for for load shifting, or 1 if no load shifting
+
+        #Check if need to increase sizing to meet lower runtimes for load shift
+        self.maxDayRun_hr = min(self.compRuntime_hr, sum(self.loadShiftSchedule))
+
+        #size system
+        self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr)
+        self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, self.effSwingFract )
+
+    def _checkInputs(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent):
+        if not isinstance(building, Building):
+            raise Exception("Error: Building is not valid.")
+        if not (isinstance(storageT_F, int) or isinstance(storageT_F, float)) or not checkLiqudWater(storageT_F):
+            raise Exception('Invalid input given for Storage temp, it must be between 32 and 212F.')
+        if not (isinstance(defrostFactor, int) or isinstance(defrostFactor, float)) or defrostFactor < 0 or defrostFactor > 1:
+            raise Exception("Invalid input given for Defrost Factor, must be a number between 0 and 1.")
+        if not (isinstance(percentUseable, int) or isinstance(percentUseable, float)) or percentUseable > 1 or percentUseable < 0:
+            raise Exception("Invalid input given for percentUseable, must be a number between 0 and 1.")
+        if not isinstance(compRuntime_hr, int) or compRuntime_hr <= 0 or compRuntime_hr > 24:
+            raise Exception("Invalid input given for compRuntime_hr, must be an integer between 0 and 24.")
+        if not (isinstance(aquaFract, int) or isinstance(aquaFract, float)) or aquaFract > 1 or aquaFract <= 0:
+            raise Exception("Invalid input given for aquaFract must, be a number between 0 and 1.")
+        if not (isinstance(loadShiftPercent, int) or isinstance(loadShiftPercent, float)) or loadShiftPercent > 1 or loadShiftPercent < 0:
+            raise Exception("Invalid input given for loadShiftPercent, must be a number between 0 and 1.")
+        if not isinstance(doLoadShift, bool):
+            raise Exception("Invalid input given for doLoadShift, must be a boolean.")
+
+    def getSizingResults(self):
+        """
+        Returns the minimum primary volume and heating capacity sizing results. Implimented seperatly in Temp Maintenence systems.
+
+        Returns
+        -------
+        list
+            self.PVol_G_atStorageT, self.PCap_kBTUhr
+        """
+        return [self.PVol_G_atStorageT, self.PCap_kBTUhr]
+
+    def simulate(self, initPV=None, initST=None, Pcapacity=None, Pvolume=None):
+        """
+        Implimented seperatly for Swink Tank systems 
+        Inputs
+        ------
+        initPV : float
+            Primary volume at start of the simulation
+        initST : float
+            Primary Swing tank at start of the simulation. Not used in this instance of the function
+        Pcapacity : float
+            The primary heating capacity in kBTUhr to use for the simulation,
+            default is the sized system
+        Pvolume : float
+            The primary storage volume in gallons to  to use for the simulation,
+            default is the sized system
+        
+        Returns
+        -------
+        list [ pV, G_hw, D_hw, prun ]
+        pV : list 
+            Volume of HW in the tank with time at the strorage temperature.
+        G_hw : list 
+            The generation of HW with time at the supply temperature
+        D_hw : list 
+            The hot water demand with time at the tsupply temperature
+        prun : list 
+            The actual output in gallons of the HPWH with time
+        """
+
+        G_hw, D_hw, V0, Vtrig, pV, pheating = self._getInitialSimulationValues(Pcapacity, Pvolume)
+
+        hw_outSwing = [0] * (len(G_hw))
+        hw_outSwing[0] = D_hw[0]
+        prun = [0] * (len(G_hw))
+
+        if initPV:
+            pV[0] = initPV
+
+        # Run the "simulation"
+        for i in range(1, len(G_hw)):
+            mixedDHW = mixVolume(D_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
+            mixedGHW = mixVolume(G_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
+            pheating, pV[i], prun[i] = self.runOnePrimaryStep(pheating, V0, Vtrig, pV[i-1], mixedDHW, mixedGHW)
+
+        return [roundList(pV, 3),
+                roundList(G_hw, 3),
+                roundList(D_hw, 3),
+                roundList(prun, 3)]
+
+    def _getInitialSimulationValues(self, Pcapacity=None, Pvolume=None):
+        """
+        Returns initialized arrays needed for 3-day simulation
+
+        Parameters
+        ----------
+        Pcapacity : float
+            The primary heating capacity in kBTUhr to use for the simulation,
+            default is the sized system
+        Pvolume : float
+            The primary storage volume in gallons to  to use for the simulation,
+            default is the sized system
+
+        Returns
+        -------
+        list [ G_hw, D_hw, V0, V, run, pheating ]
+        G_hw : list
+            The generation of HW with time at the supply temperature
+        D_hw : list
+            The hot water demand with time at the tsupply temperature
+        V0 : float
+            The storage volume of the primary system at the storage temperature
+        Vtrig : float
+            The remaining volume of the primary storage volume when heating is
+            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho?
+        pV : list 
+            Volume of HW in the tank with time at the strorage temperature. Initialized to array of 0s with pV[0] set to V0
+        pheating : boolean 
+            set to false. Simulation starts with a full tank so primary heating starts off
+        """
+        if not Pcapacity:
+            Pcapacity =  self.PCap_kBTUhr
+
+        if not Pvolume:
+            Pvolume =  self.PVol_G_atStorageT
+
+        loadShapeN = self.building.loadshape
+        if self.doLoadShift:
+            loadShapeN = self.building.avgLoadshape
+
+        # Get the generation rate from the primary capacity
+        G_hw = 1000 * Pcapacity / rhoCp / (self.building.supplyT_F - self.building.incomingT_F) \
+               * self.defrostFactor * np.tile(self.loadShiftSchedule,3)
+        
+        # Define the use of DHW with the normalized load shape
+        D_hw = self.building.magnitude * self.fract_total_vol * np.tile(loadShapeN, 3)
+
+        # To per minute from per hour
+        G_hw = np.array(hrToMinList(G_hw)) / 60
+        D_hw = np.array(hrToMinList(D_hw)) / 60
+
+        # Init the "simulation"
+        V0 = np.ceil(Pvolume * self.percentUseable)
+        Vtrig = np.ceil(Pvolume * (1 - self.aquaFract)) + 1 # To prevent negatives with any of that rounding math.
+        pV = [V0] + [0] * (len(G_hw) - 1)
+
+        pheating = False
+
+        return G_hw, D_hw, V0, Vtrig, pV, pheating
+    
+    def _setLoadShift(self, loadShiftSchedule, loadShiftPercent=1):
+        """
+        Sets the load shifting schedule from input loadShiftSchedule
+
+        Parameters
+        ----------
+        loadShiftSchedule : array_like
+            List or array of 0's and 1's for don't run and run.
+
+        loadShiftPercent : float
+            Percentile of days which need to be covered by load shifting
+
+        """
+        # Check
+        if len(loadShiftSchedule) != 24 : #TODO ensure loadShiftSchedule is valid and add load up
+            raise Exception("loadshift is not of length 24 but instead has length of "+str(len(loadShiftSchedule))+".")
+        if sum(loadShiftSchedule) == 0 :
+            raise Exception("When using Load shift the HPWH's must run for at least 1 hour each day.")
+        if loadShiftPercent < 0.25 :
+            raise Exception("Load shift only available for above 25 percent of days.")
+        if loadShiftPercent > 1 :
+            raise Exception("Cannot load shift for more than 100 percent of days")
+
+        self.loadShiftSchedule = loadShiftSchedule
+        self.loadshift = np.array(loadShiftSchedule, dtype = float)# Coerce to numpy array of data type float
+
+        # adjust for loadShiftPercent
+        if loadShiftPercent == 1: # meaing 100% of days covered by load shift
+            self.fract_total_vol = 1
+        else:
+            # calculate fraction total hot water required to meet load shift days
+            fract = norm_mean + norm_std * norm.ppf(loadShiftPercent) #TODO norm_mean and std are currently from multi-family, need other types eventually. For now, loadshifting will only be available for multi-family
+            self.fract_total_vol = fract if fract <= 1. else 1.
+        
+        self.doLoadShift = True
+
+    # SwingTank has it's own implimentation
+    def _primaryHeatHrs2kBTUHR(self, heathours, effSwingVolFract=1):
+        """
+        Converts from hours of heating in a day to heating capacity.
+
+        Implimented seperatly in Swing Tank systems
+
+        Parameters
+        ----------
+        heathours : float or numpy.ndarray
+            The number of hours primary heating equipment can run.
+
+        effSwingVolFract : float or numpy.ndarray
+            The fractional adjustment to the total hot water load for the
+            primary system. Only used in a swing tank system.
+
+        Returns
+        -------
+        heatCap
+            The heating capacity in [btu/hr].
+        """
+        checkHeatHours(heathours)
+        heatCap = self.building.magnitude / heathours * rhoCp * \
+            (self.building.supplyT_F - self.building.incomingT_F) / self.defrostFactor /1000.
+        return heatCap
+    
+    def sizePrimaryTankVolume(self, heatHrs):
+        """
+        Calculates the primary storage using the Ecotope sizing methodology
+
+        Parameters
+        ----------
+        heatHrs : float
+            The number of hours primary heating equipment can run in a day.
+        
+        Raises
+        ------
+        ValueError: aquastat fraction is too low.
+        ValueError: The minimum aquastat fraction is greater than 1.
+
+        Returns
+        -------
+        totalVolMax : float
+            The total storage volume in gallons adjusted to the storage tempreature
+        effMixFract : float
+            The fractional adjustment to the total hot water load for the
+            primary system. Only used in a swing tank system.
+        
+        """
+        if heatHrs <= 0 or heatHrs > 24:
+            raise Exception("Heat hours is not within 1 - 24 hours")
+        # Fraction used for adjusting swing tank volume.
+        effMixFract = 1.
+
+        # Running vol
+        runningVol_G, effMixFract = self._calcRunningVol(heatHrs, np.ones(24), self.building.loadshape, effMixFract)
+
+        # If doing load shift, solve for the runningVol_G and take the larger volume
+        if self.doLoadShift:
+            LSrunningVol_G = 0
+            LSeffMixFract = 0
+            # calculate loadshift sizing with avg loadshape (see page 19 of methodology documentation)
+            LSrunningVol_G, LSeffMixFract = self._calcRunningVol(heatHrs, self.loadShiftSchedule, self.building.avgLoadshape, LSeffMixFract)
+            LSrunningVol_G *= self.fract_total_vol
+
+            # Get total volume from max of primary method or load shift method
+            if LSrunningVol_G > runningVol_G:
+                runningVol_G = LSrunningVol_G
+                effMixFract = LSeffMixFract
+
+        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G)
+
+        # Check the Cycling Volume ############################################
+        cyclingVol_G = totalVolAtStorage * (self.aquaFract - (1 - self.percentUseable))
+        minRunVol_G = pCompMinimumRunTime * (self.building.magnitude * effMixFract / heatHrs) # (generation rate - no usage)
+
+        if minRunVol_G > cyclingVol_G:
+            min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
+            if min_AF < 1:
+                raise ValueError("01", "The aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
+            raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
+
+        # Return the temperature adjusted total volume ########################
+        return totalVolAtStorage, effMixFract
+    
+    def _calcRunningVol(self, heatHrs, onOffArr, loadshape, effMixFract = 0):
+        """
+        Function to find the running volume for the hot water storage tank, which
+        is needed for calculating the total volume for primary sizing and in the event of load shift sizing
+        represents the entire volume.
+
+        Implimented seperatly for Swing Tank systems
+
+        Parameters
+        ----------
+        heatHrs : float
+            The number of hours primary heating equipment can run in a day.
+        onOffArr : ndarray
+            array of 1/0's where 1's allow heat pump to run and 0's dissallow. of length 24.
+        loadshape : ndarray
+            normalized array of length 24 representing the daily loadshape for this calculation.
+        effMixFract: Int
+            unused value in this instance of the function. Used in Swing Tank implimentation
+
+        Raises
+        ------
+        Exception: Error if oversizeing system.
+
+        Returns
+        -------
+        runV_G : float
+            The running volume in gallons
+        effMixFract: int
+            returns same value from parameter. Needed for Swing Tank implimentation. Not actually used in this function instance 
+        """          
+        genrate = np.tile(onOffArr,2) / heatHrs #hourly
+        diffN = genrate - np.tile(loadshape,2) #hourly
+        diffInd = getPeakIndices(diffN[0:24]) #Days repeat so just get first day!
+        diffN *= self.building.magnitude
+        # Get the running volume ##############################################
+        if len(diffInd) == 0:
+            #TODO but what if it is undersized? Also can this ever be hit? users currently do not have power to change num hours from interface
+            raise Exception("ERROR ID 03","The heating rate is greater than the peak volume the system is oversized! Try increasing the hours the heat pump runs in a day",)
+        runV_G = 0
+        for peakInd in diffInd:
+            #Get the rest of the day from the start of the peak
+            diffCum = np.cumsum(diffN[peakInd:])  #hourly
+            runV_G = max(runV_G, -min(diffCum[diffCum<0.])) #Minimum value less than 0 or 0.
+
+        return runV_G, effMixFract
+    
+    def _getTotalVolAtStorage(self, runningVol_G):
+        """
+        Calculates the maximum primary storage using the Ecotope sizing methodology. Swing Tanks implement sperately
+
+        Parameters
+        ----------
+        runningVol_G : float
+            The running volume in gallons
+
+        Returns
+        -------
+        totalVolMax : float
+            The total storage volume in gallons adjusted to the storage tempreature
+        
+        """
+        return mixVolume(runningVol_G, self.storageT_F, self.building.incomingT_F, self.building.supplyT_F) / (1-self.aquaFract)
+    
+    def primaryCurve(self):
+        """
+        Sizes the primary system curve. Will catch the point at which the aquatstat
+        fraction is too small for system and cuts the return arrays to match cutoff point.
+
+        Returns
+        -------
+        volN : array
+            Array of volume in the tank at each hour.
+
+        primaryHeatHrs2kBTUHR : array
+            Array of heating capacity in kBTU/hr
+            
+        heatHours : array
+            Array of running hours per day corresponding to primaryHeatHrs2kBTUHR
+            
+        recIndex : int
+            The index of the recommended heating rate. 
+        """
+        # Define the heating hours we'll check
+        delta = -0.25
+        maxHeatHours = 1/(max(self.building.loadshape))*1.001   
+        
+        arr1 = np.arange(24, self.maxDayRun_hr, delta)
+        recIndex = len(arr1)
+        heatHours = np.concatenate((arr1, np.arange(self.maxDayRun_hr, maxHeatHours, delta)))
+        
+        volN = np.zeros(len(heatHours))
+        effMixFract = np.ones(len(heatHours))
+        for i in range(0,len(heatHours)):
+            try:
+                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i])
+            except ValueError:
+                break
+        # Cut to the point the aquastat fraction was too small
+        volN        = volN[:i]
+        heatHours   = heatHours[:i]
+        effMixFract = effMixFract[:i]
+
+        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, effMixFract), heatHours, recIndex]
+
+    
+    def runOnePrimaryStep(self, pheating, V0, Vtrig, Vcurr, hw_out, hw_in):
+        """
+        Runs one step on the primary system. This changes the volume of the primary system
+        by assuming there is hot water removed at a volume of hw_out and hot water
+        generated or added at a volume of hw_in. This is assuming the system is perfectly
+        stratified and all of the hot water above the cold temperature is at the storage temperature.
+
+        Parameters
+        ----------
+        pheating : boolean
+            indicates whether system is heating at the beginning of this step
+        V0 : float
+            The storage volume of the primary system at the storage temperature
+        Vtrig : float
+            The remaining volume of the primary storage volume when heating is
+            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho? 
+        Vcurr : float
+            The primary volume at the timestep.
+        hw_out : float
+            The volume of DHW removed from the primary system, assumed that
+            100% of what of what is removed is replaced
+        hw_in : float
+            The volume of hot water generated in a time step
+
+        Returns
+        -------
+        pheating : boolean
+            Boolean indicating if the primary system is heating at the end of this step in the simulation 
+        Vnew : float
+            The new primary volume at the timestep.
+        did_run : float
+            The volume of hot water generated during the time step.
+
+        """
+        did_run = 0
+        Vnew = 0
+        if pheating:
+            Vnew = Vcurr + hw_in - hw_out # If heating, generate HW and lose HW
+            did_run = hw_in
+
+        else:  # Else not heating,
+            Vnew = Vcurr - hw_out # So lose HW
+            if Vnew < Vtrig: # If should heat
+                time_missed = (Vtrig - Vnew)/hw_out # Volume below turn on / rate of draw gives time below tigger
+                Vnew += hw_in * time_missed # Start heating
+                did_run = hw_in * time_missed
+                pheating = True
+
+        if Vnew > V0: # If overflow
+            time_over = (Vnew - V0) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
+            Vnew = V0 - hw_out * time_over # Make full with missing volume
+            did_run = hw_in * (1-time_over)
+            pheating = False # Stop heating
+
+        if Vnew < 0:
+           raise Exception("Primary storage ran out of Volume!")
+
+        return pheating, Vnew, did_run
+    
+    def plotStorageLoadSim(self, return_as_div=True):
+        """
+        Returns a plot of the of the simulation for the minimum sized primary
+        system as a div or plotly figure. Can plot the minute level simulation
+
+        Implimented seperatly for Swing Tank systems
+
+        Parameters
+        ----------
+        return_as_div
+            A logical on the output, as a div (true) or as a figure (false)
+
+        Returns
+        -------
+        div/fig
+            plot_div
+        """
+        [V, G_hw, D_hw, run] = self.simulate()
+
+        hrind_fromback = 24 # Look at the last 24 hours of the simulation not the whole thing
+        run = np.array(run[-(60*hrind_fromback):])*60
+        G_hw = np.array(G_hw[-(60*hrind_fromback):])*60
+        D_hw = np.array(D_hw[-(60*hrind_fromback):])*60
+        V = np.array(V[-(60*hrind_fromback):])
+
+        if any(i < 0 for i in V):
+            raise Exception("Primary storage ran out of Volume!")
+
+        fig = Figure()
+
+        # Do primary components
+        x_data = list(range(len(V)))
+
+        if self.doLoadShift:
+            ls_off = [int(not x)* max(V)*2 for x in G_hw]
+            fig.add_trace(Scatter(x=x_data, y=ls_off, name='Load Shift Off Period',
+                                  mode='lines', line_shape='hv',
+                                  opacity=0.5, marker_color='grey',
+                                  fill='tonexty'))
+
+        fig.add_trace(Scatter(x=x_data, y=V, name='Useful Storage Volume at Storage Temperature',
+                              mode='lines', line_shape='hv',
+                              opacity=0.8, marker_color='green'))
+        fig.add_trace(Scatter(x=x_data, y=run, name = "Hot Water Generation at Storage Temperature",
+                              mode='lines', line_shape='hv',
+                              opacity=0.8, marker_color='red'))
+        fig.add_trace(Scatter(x=x_data, y=D_hw, name='Hot Water Demand at Supply Temperature',
+                              mode='lines', line_shape='hv',
+                              opacity=0.8, marker_color='blue'))
+        fig.update_yaxes(range=[0, np.ceil(max(np.append(V,D_hw))/100)*100])
+
+        fig.update_layout(title="Hot Water Simulation",
+                          xaxis_title= "Minute of Day",
+                          yaxis_title="Gallons or\nGallons per Hour",
+                          width=900,
+                          height=700)
+
+        if return_as_div:
+            plot_div = plot(fig, output_type='div', show_link=False, link_text="",
+                        include_plotlyjs = False)
+            return plot_div
+        return fig
+    
+    
+class Primary(SystemConfig):
+    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
+        super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+                 doLoadShift, loadShiftPercent, loadShiftSchedule)
+
```

### Comparing `ecoengine-0.0.1/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.2/src/ecoengine/objects/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-""" 
-	EcosizerEngine
-    Copyright (C) 2023  Ecotope Inc.
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-
-# __all__ = ['EcosizerEngine', 'createBuilding', 'createSystem']
-from .Building import *
-from .SystemConfig import *
-from .systemConfigUtils import *
-from .systems.ParallelLoopTank import *
+""" 
+	EcosizerEngine
+    Copyright (C) 2023  Ecotope Inc.
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+
+# __all__ = ['EcosizerEngine', 'createBuilding', 'createSystem']
+from .Building import *
+from .SystemConfig import *
+from .systemConfigUtils import *
+from .systems.ParallelLoopTank import *
 from .systems.SwingTank import *
```

### Comparing `ecoengine-0.0.1/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-0.0.2/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.1/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,118 @@
-Metadata-Version: 2.1
-Name: ecoengine
-Version: 0.0.1
-Summary: A software for sizing Heat Pump Water Heaters for buildings
-Home-page: https://ecosizer.ecotope.com/sizer/
-Author: Nolan
-Author-email: nolan@ecotope.com
-Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# EcosizerEngine
-
-### Requirements:
-
-This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
-
-### Using the package in scripts:
-
-1. Install the package with pip
-
-	$ pip install ecosizer-engine
-
-2. To import and use the tools in this package, add the following import statement to your script:
-
-	from ecosizer_engine_package import *
-
-You should now be able to use the features of EcosizerEngine in your script
-
-### Running locally in a container:
-First, clone the EcosizerEngine repo from github
-
-    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
-
-Depending on what type of environment you want to run the code in, please follow the appropriate steps.
-
-Steps for installing in a virtual environment:
-1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
-2. Run the following command:
-
-	$ pip install -e .
-
-This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
-This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
-
-Steps for installing using docker container:
-1. Navigate to the EcosizerEngine directory.
-2. Build container with docker file
-
-	$ docker build -t ecosizerengine:latest .
-
-3. Run docker container
-
-	$  docker run -it ecosizerengine bash
-
-4. When you are done messing about in the docker image, just type the command
-
-	$ exit
-
-or press ctrl+c then ctrl+d
-
-Steps for installing conda environment from the Anaconda prompt:
-1. Navigate to the EcosizerEngine directory.
-2. Create new environment from .yml file.
-
-
-	$ conda env create --file EcosizerEngine.yml
-
-If the environment creation doesn't work, make sure Anaconda is up-to-date with
-
-    $ conda update --all
-
-If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
-
-    $ conda create -n py311 python=3.11
-    $ conda activate py311
-    $ conda env create --file EcosizerEngine.yml
-
-3. Check that the environment was created
-
-
-	$ conda env list
-
-4. Activate the new environment
-
-
-	$ conda activate EcosizerEngine
-
-If an environment already exits it can be removed with:
-
-	$ conda remove --name EcosizerEngine --all
-
-
-All the available environment can be found with:
-
-	$ conda env list
-
-### Testing:
-From the parent directory, type
-
-	$ python -m pytest
-
-This will run all unit tests for the package
-
-### Updating Documentation:
-1. If not installed in environment: pip install sphinx and numpydocs
-2. navigate to docs directory and run:
-
-
-	$ make html
-
-### Updating version on pypi
-
-1. Update the version number in setup.cfg
-2. Run the following commands from the project root directory:
-
-	$ python -m build
-	$ python -m twine upload dist/*
-
-### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+# EcosizerEngine
+
+### Requirements:
+
+This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
+
+### Using the package in scripts:
+
+1. Install the package with pip
+
+	$ pip install ecosizer-engine
+
+2. To import and use the tools in this package, add the following import statement to your script:
+
+	from ecosizer_engine_package import *
+
+You should now be able to use the features of EcosizerEngine in your script
+
+### Running locally in a container:
+First, clone the EcosizerEngine repo from github
+
+    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
+
+Depending on what type of environment you want to run the code in, please follow the appropriate steps.
+
+Steps for installing in a virtual environment:
+1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
+2. Run the following command:
+
+	$ pip install -e .
+
+This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
+This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
+
+Steps for installing using docker container:
+1. Navigate to the EcosizerEngine directory.
+2. Build container with docker file
+
+	$ docker build -t ecosizerengine:latest .
+
+3. Run docker container
+
+	$  docker run -it ecosizerengine bash
+
+4. When you are done messing about in the docker image, just type the command
+
+	$ exit
+
+or press ctrl+c then ctrl+d
+
+Steps for installing conda environment from the Anaconda prompt:
+1. Navigate to the EcosizerEngine directory.
+2. Create new environment from .yml file.
+
+
+	$ conda env create --file EcosizerEngine.yml
+
+If the environment creation doesn't work, make sure Anaconda is up-to-date with
+
+    $ conda update --all
+
+If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
+
+    $ conda create -n py311 python=3.11
+    $ conda activate py311
+    $ conda env create --file EcosizerEngine.yml
+
+3. Check that the environment was created
+
+
+	$ conda env list
+
+4. Activate the new environment
+
+
+	$ conda activate EcosizerEngine
+
+If an environment already exits it can be removed with:
+
+	$ conda remove --name EcosizerEngine --all
+
+
+All the available environment can be found with:
+
+	$ conda env list
+
+### Testing:
+From the parent directory, type
+
+	$ python -m pytest
+
+This will run all unit tests for the package
+
+### Updating Documentation:
+1. If not installed in environment: pip install sphinx and numpydocs
+2. navigate to docs directory and run:
+
+
+	$ make html
+
+### Updating version on pypi
+
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
+
+	$ python -m build
+
+	$ python -m twine upload dist/*
+
+### Contact Information
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.1/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.2/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

