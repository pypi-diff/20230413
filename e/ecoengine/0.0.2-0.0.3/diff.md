# Comparing `tmp/ecoengine-0.0.2.tar.gz` & `tmp/ecoengine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.2.tar", last modified: Thu Apr 13 18:02:44 2023, max compression
+gzip compressed data, was "ecoengine-0.0.3.tar", last modified: Thu Apr 13 18:51:18 2023, max compression
```

## Comparing `ecoengine-0.0.2.tar` & `ecoengine-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:44.214301 ecoengine-0.0.2/
--rw-rw-rw-   0        0        0       59 2023-03-28 23:58:57.000000 ecoengine-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3815 2023-04-13 18:02:44.280187 ecoengine-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      767 2023-04-13 18:02:44.481451 ecoengine-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:33.502282 ecoengine-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:35.882286 ecoengine-0.0.2/src/ecoengine/
--rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:38.918292 ecoengine-0.0.2/src/ecoengine/constants/
--rw-rw-rw-   0        0        0      457 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/constants/Constants.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:39.282292 ecoengine-0.0.2/src/ecoengine/data/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:39.658293 ecoengine-0.0.2/src/ecoengine/data/load_shapes/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.2/src/ecoengine/data/load_shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:41.082296 ecoengine-0.0.2/src/ecoengine/engine/
--rw-rw-rw-   0        0        0     6879 2023-04-13 17:58:46.000000 ecoengine-0.0.2/src/ecoengine/engine/BuildingCreator.py
--rw-rw-rw-   0        0        0     7508 2023-04-13 17:57:47.000000 ecoengine-0.0.2/src/ecoengine/engine/EcosizerEngine.py
--rw-rw-rw-   0        0        0     2924 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/engine/SystemCreator.py
--rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:42.682299 ecoengine-0.0.2/src/ecoengine/objects/
--rw-rw-rw-   0        0        0     9746 2023-04-13 17:58:54.000000 ecoengine-0.0.2/src/ecoengine/objects/Building.py
--rw-rw-rw-   0        0        0    23618 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/SystemConfig.py
--rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/__init__.py
--rw-rw-rw-   0        0        0     2948 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systemConfigUtils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:43.870301 ecoengine-0.0.2/src/ecoengine/objects/systems/
--rw-rw-rw-   0        0        0     3509 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-rw-rw-   0        0        0    16890 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/SwingTank.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.2/src/ecoengine/objects/systems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:02:38.202290 ecoengine-0.0.2/src/ecoengine.egg-info/
--rw-rw-rw-   0        0        0     3815 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      846 2023-04-13 18:02:33.000000 ecoengine-0.0.2/src/ecoengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-13 18:02:31.000000 ecoengine-0.0.2/src/ecoengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 18:02:32.000000 ecoengine-0.0.2/src/ecoengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.924722 ecoengine-0.0.3/
+-rw-rw-rw-   0        0        0       45 2023-04-13 18:49:37.000000 ecoengine-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-04-13 18:51:18.954344 ecoengine-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      767 2023-04-13 18:51:18.997104 ecoengine-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:15.848715 ecoengine-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.292716 ecoengine-0.0.3/src/ecoengine/
+-rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.848717 ecoengine-0.0.3/src/ecoengine/constants/
+-rw-rw-rw-   0        0        0      457 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/constants/Constants.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.904718 ecoengine-0.0.3/src/ecoengine/data/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:17.872720 ecoengine-0.0.3/src/ecoengine/data/load_shapes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/apartment.json
+-rw-rw-rw-   0        0        0      971 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-rw-rw-   0        0        0     1127 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-rw-rw-   0        0        0     1272 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-rw-rw-   0        0        0     1240 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/junior_high.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/motel.json
+-rw-rw-rw-   0        0        0    47218 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/multi_family.json
+-rw-rw-rw-   0        0        0     1273 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-rw-rw-   0        0        0     1058 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/office_building.json
+-rw-rw-rw-   0        0        0     1120 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/senior_high.json
+-rw-rw-rw-   0        0        0     1219 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.124720 ecoengine-0.0.3/src/ecoengine/engine/
+-rw-rw-rw-   0        0        0     6879 2023-04-13 17:58:46.000000 ecoengine-0.0.3/src/ecoengine/engine/BuildingCreator.py
+-rw-rw-rw-   0        0        0     7508 2023-04-13 17:57:47.000000 ecoengine-0.0.3/src/ecoengine/engine/EcosizerEngine.py
+-rw-rw-rw-   0        0        0     2924 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/engine/SystemCreator.py
+-rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.604722 ecoengine-0.0.3/src/ecoengine/objects/
+-rw-rw-rw-   0        0        0     9746 2023-04-13 17:58:54.000000 ecoengine-0.0.3/src/ecoengine/objects/Building.py
+-rw-rw-rw-   0        0        0    23618 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/SystemConfig.py
+-rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/__init__.py
+-rw-rw-rw-   0        0        0     2948 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systemConfigUtils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.852722 ecoengine-0.0.3/src/ecoengine/objects/systems/
+-rw-rw-rw-   0        0        0     3509 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-rw-rw-   0        0        0    16890 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/SwingTank.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.684717 ecoengine-0.0.3/src/ecoengine.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1430 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.2/PKG-INFO` & `ecoengine-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.2/README.md` & `ecoengine-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/setup.cfg` & `ecoengine-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 656e 6769 6e65 0d0a 7665   = ecoengine..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a61  rsion = 0.0.2..a
+00000020: 7273 696f 6e20 3d20 302e 302e 330d 0a61  rsion = 0.0.3..a
 00000030: 7574 686f 7220 3d20 4e6f 6c61 6e0d 0a61  uthor = Nolan..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 6e6f  uthor_email = no
 00000050: 6c61 6e40 6563 6f74 6f70 652e 636f 6d0d  lan@ecotope.com.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 6f66 7477 6172 6520 666f 7220 7369   software for si
 00000080: 7a69 6e67 2048 6561 7420 5075 6d70 2057  zing Heat Pump W
 00000090: 6174 6572 2048 6561 7465 7273 2066 6f72  ater Heaters for
```

### Comparing `ecoengine-0.0.2/src/ecoengine/__init__.py` & `ecoengine-0.0.3/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.3/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.3/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.3/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.3/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/Building.py` & `ecoengine-0.0.3/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.3/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.3/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.3/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-0.0.3/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-0.0.3/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.2/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.3/src/ecoengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

