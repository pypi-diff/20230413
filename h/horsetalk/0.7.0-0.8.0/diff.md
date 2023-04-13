# Comparing `tmp/horsetalk-0.7.0.tar.gz` & `tmp/horsetalk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.7.0.tar", max compression
+gzip compressed data, was "horsetalk-0.8.0.tar", max compression
```

## Comparing `horsetalk-0.7.0.tar` & `horsetalk-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1502 2023-04-12 22:25:58.873087 horsetalk-0.7.0/horsetalk/__init__.py
--rw-r--r--   0        0        0      244 2023-04-13 16:39:46.099964 horsetalk-0.7.0/horsetalk/age_category.py
--rw-r--r--   0        0        0      428 2023-04-09 18:32:25.935876 horsetalk-0.7.0/horsetalk/aw_going_description.py
--rw-r--r--   0        0        0      289 2023-04-13 16:39:46.099964 horsetalk-0.7.0/horsetalk/breed.py
--rw-r--r--   0        0        0      514 2023-04-13 16:41:40.705711 horsetalk-0.7.0/horsetalk/coat_colour.py
--rw-r--r--   0        0        0      287 2023-04-13 16:41:40.706685 horsetalk-0.7.0/horsetalk/dirt_going_description.py
--rw-r--r--   0        0        0     1187 2023-04-13 16:41:40.706685 horsetalk-0.7.0/horsetalk/disaster.py
--rw-r--r--   0        0        0      378 2023-04-13 16:39:46.100963 horsetalk-0.7.0/horsetalk/finishing_position.py
--rw-r--r--   0        0        0      223 2023-04-13 16:39:46.100963 horsetalk-0.7.0/horsetalk/form_break.py
--rw-r--r--   0        0        0     1426 2023-04-13 17:01:43.367227 horsetalk-0.7.0/horsetalk/form_figures.py
--rw-r--r--   0        0        0     2566 2023-04-13 16:41:13.817125 horsetalk-0.7.0/horsetalk/gender.py
--rw-r--r--   0        0        0      544 2023-04-13 16:39:46.101964 horsetalk-0.7.0/horsetalk/headgear.py
--rw-r--r--   0        0        0     4549 2023-04-13 17:01:43.386995 horsetalk-0.7.0/horsetalk/horse_age.py
--rw-r--r--   0        0        0      291 2023-04-13 16:39:46.101964 horsetalk-0.7.0/horsetalk/horse_experience_level.py
--rw-r--r--   0        0        0     1148 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/horse_height.py
--rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.7.0/horsetalk/horselength.py
--rw-r--r--   0        0        0      390 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/jockey_experience_level.py
--rw-r--r--   0        0        0      480 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/obstacle.py
--rw-r--r--   0        0        0      529 2023-04-13 16:39:41.041691 horsetalk-0.7.0/horsetalk/parsing_enum.py
--rw-r--r--   0        0        0      420 2023-04-13 16:39:46.103964 horsetalk-0.7.0/horsetalk/race_designation.py
--rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.7.0/horsetalk/race_distance.py
--rw-r--r--   0        0        0     2636 2023-04-13 17:01:43.407145 horsetalk-0.7.0/horsetalk/race_title.py
--rw-r--r--   0        0        0      372 2023-04-13 16:39:46.103964 horsetalk-0.7.0/horsetalk/racing_code.py
--rw-r--r--   0        0        0      258 2023-04-13 16:39:46.105966 horsetalk-0.7.0/horsetalk/sex.py
--rw-r--r--   0        0        0      288 2023-04-13 16:39:46.105966 horsetalk-0.7.0/horsetalk/surface.py
--rw-r--r--   0        0        0      839 2023-04-09 18:35:29.091069 horsetalk-0.7.0/horsetalk/turf_going_description.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.7.0/LICENSE
--rw-r--r--   0        0        0      723 2023-04-13 17:01:43.424654 horsetalk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.7.0/README.md
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1551 2023-04-13 18:31:02.457919 horsetalk-0.8.0/horsetalk/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-13 18:30:57.122742 horsetalk-0.8.0/horsetalk/age_category.py
+-rw-r--r--   0        0        0      428 2023-04-09 18:32:25.935876 horsetalk-0.8.0/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      289 2023-04-13 18:30:57.122742 horsetalk-0.8.0/horsetalk/breed.py
+-rw-r--r--   0        0        0      514 2023-04-13 16:41:40.705711 horsetalk-0.8.0/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      287 2023-04-13 16:41:40.706685 horsetalk-0.8.0/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0     1187 2023-04-13 18:30:57.123742 horsetalk-0.8.0/horsetalk/disaster.py
+-rw-r--r--   0        0        0      378 2023-04-13 18:30:57.123742 horsetalk-0.8.0/horsetalk/finishing_position.py
+-rw-r--r--   0        0        0      223 2023-04-13 18:30:57.124742 horsetalk-0.8.0/horsetalk/form_break.py
+-rw-r--r--   0        0        0     1426 2023-04-13 18:30:57.124742 horsetalk-0.8.0/horsetalk/form_figures.py
+-rw-r--r--   0        0        0     2566 2023-04-13 18:30:57.124742 horsetalk-0.8.0/horsetalk/gender.py
+-rw-r--r--   0        0        0      544 2023-04-13 18:30:57.125741 horsetalk-0.8.0/horsetalk/headgear.py
+-rw-r--r--   0        0        0     4549 2023-04-13 18:30:57.125741 horsetalk-0.8.0/horsetalk/horse_age.py
+-rw-r--r--   0        0        0      291 2023-04-13 18:30:57.125741 horsetalk-0.8.0/horsetalk/horse_experience_level.py
+-rw-r--r--   0        0        0     1148 2023-04-13 18:30:57.125741 horsetalk-0.8.0/horsetalk/horse_height.py
+-rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.8.0/horsetalk/horselength.py
+-rw-r--r--   0        0        0      390 2023-04-13 18:30:57.127246 horsetalk-0.8.0/horsetalk/jockey_experience_level.py
+-rw-r--r--   0        0        0      490 2023-04-13 18:31:02.420404 horsetalk-0.8.0/horsetalk/jump_category.py
+-rw-r--r--   0        0        0      362 2023-04-13 18:31:02.440405 horsetalk-0.8.0/horsetalk/obstacle_style.py
+-rw-r--r--   0        0        0      529 2023-04-13 16:39:41.041691 horsetalk-0.8.0/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      420 2023-04-13 18:30:57.128251 horsetalk-0.8.0/horsetalk/race_designation.py
+-rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.8.0/horsetalk/race_distance.py
+-rw-r--r--   0        0        0     2735 2023-04-13 18:31:02.421404 horsetalk-0.8.0/horsetalk/race_title.py
+-rw-r--r--   0        0        0      372 2023-04-13 18:30:57.128251 horsetalk-0.8.0/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      258 2023-04-13 18:30:57.129251 horsetalk-0.8.0/horsetalk/sex.py
+-rw-r--r--   0        0        0      288 2023-04-13 18:30:57.129251 horsetalk-0.8.0/horsetalk/surface.py
+-rw-r--r--   0        0        0      839 2023-04-09 18:35:29.091069 horsetalk-0.8.0/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.8.0/LICENSE
+-rw-r--r--   0        0        0      723 2023-04-13 18:31:07.401839 horsetalk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.8.0/README.md
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.8.0/PKG-INFO
```

### Comparing `horsetalk-0.7.0/horsetalk/__init__.py` & `horsetalk-0.8.0/horsetalk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .form_break import FormBreak
 from .form_figures import FormFigures
 from .gender import Gender
 from .headgear import Headgear
 from .horse_age import HorseAge
 from .horse_height import HorseHeight
 from .horselength import Horselength
-from .obstacle import Obstacle
+from .jump_category import JumpCategory
+from .obstacle_style import ObstacleStyle
 from .race_designation import RaceDesignation
 from .race_distance import RaceDistance
 from .race_title import RaceTitle
 from .racing_code import RacingCode
 from .sex import Sex
 from .surface import Surface
 from .turf_going_description import TurfGoingDescription
@@ -36,17 +37,17 @@
     "Gender",
     "Headgear",
     "HorseAge",
     "HorseHeight",
     "Horselength",
     "HorseExperienceLevel",
     "JockeyExperienceLevel",
-    "Obstacle",
+    "JumpCategory",
+    "ObstacleStyle",
     "RaceDesignation",
     "RaceDistance",
-    "RaceExperienceStatus",
     "RaceTitle",
     "RacingCode",
     "Sex",
     "Surface",
     "TurfGoingDescription",
 ]
```

### Comparing `horsetalk-0.7.0/horsetalk/coat_colour.py` & `horsetalk-0.8.0/horsetalk/coat_colour.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/disaster.py` & `horsetalk-0.8.0/horsetalk/disaster.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/form_figures.py` & `horsetalk-0.8.0/horsetalk/form_figures.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/gender.py` & `horsetalk-0.8.0/horsetalk/gender.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/headgear.py` & `horsetalk-0.8.0/horsetalk/headgear.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/horse_age.py` & `horsetalk-0.8.0/horsetalk/horse_age.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/horse_height.py` & `horsetalk-0.8.0/horsetalk/horse_height.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/horselength.py` & `horsetalk-0.8.0/horsetalk/horselength.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/parsing_enum.py` & `horsetalk-0.8.0/horsetalk/parsing_enum.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/race_distance.py` & `horsetalk-0.8.0/horsetalk/race_distance.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/horsetalk/race_title.py` & `horsetalk-0.8.0/horsetalk/race_title.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from typing import List, Type
 from .age_category import AgeCategory
 from .horse_experience_level import HorseExperienceLevel
 from .gender import Gender
-from .obstacle import Obstacle
+from .jump_category import JumpCategory
 from .race_designation import RaceDesignation
 
 
 class RaceTitle:
     """
     A class for parsing a race title into its component parts.
 
@@ -32,27 +32,33 @@
 
         Returns:
             dict: A dictionary of component parts.
         """
         self = cls()
         self._words = title.split()
 
-        enums = [AgeCategory, HorseExperienceLevel, Gender, Obstacle, RaceDesignation]
+        enums = [
+            AgeCategory,
+            HorseExperienceLevel,
+            Gender,
+            JumpCategory,
+            RaceDesignation,
+        ]
         end_index = -1
         for i, word in enumerate(self._words):
             if any(getattr(enum, word, None) is not None for enum in enums):
                 end_index = i
                 break
         name = " ".join(self._words[:end_index])
 
         return {
             "age_category": self._lookup(AgeCategory),
             "horse_experience_level": self._lookup(HorseExperienceLevel),
             "gender": self._lookup(Gender, allow_multiple=True),
-            "obstacle": self._lookup(Obstacle),
+            "jump_category": self._lookup(JumpCategory),
             "race_designation": self._lookup(RaceDesignation),
             "name": name,
         }
 
     def _lookup(
         self, enum: Type[Enum], allow_multiple: bool = False
     ) -> List[Enum] | Enum | None:
```

### Comparing `horsetalk-0.7.0/horsetalk/turf_going_description.py` & `horsetalk-0.8.0/horsetalk/turf_going_description.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/LICENSE` & `horsetalk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.7.0/pyproject.toml` & `horsetalk-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.7.0"
+version = "0.8.0"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `horsetalk-0.7.0/PKG-INFO` & `horsetalk-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.7.0
+Version: 0.8.0
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

