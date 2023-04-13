# Comparing `tmp/horsetalk-0.6.1.tar.gz` & `tmp/horsetalk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.6.1.tar", max compression
+gzip compressed data, was "horsetalk-0.7.0.tar", max compression
```

## Comparing `horsetalk-0.6.1.tar` & `horsetalk-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1502 2023-04-08 20:26:53.418399 horsetalk-0.6.1/horsetalk/__init__.py
--rw-r--r--   0        0        0      157 2023-04-08 16:43:51.100371 horsetalk-0.6.1/horsetalk/age_category.py
--rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.6.1/horsetalk/aw_going_description.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.6.1/horsetalk/breed.py
--rw-r--r--   0        0        0      514 2023-04-08 16:50:46.370436 horsetalk-0.6.1/horsetalk/coat_colour.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.6.1/horsetalk/dirt_going_description.py
--rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.6.1/horsetalk/disaster.py
--rw-r--r--   0        0        0      275 2023-04-08 18:27:27.925629 horsetalk-0.6.1/horsetalk/finishing_position.py
--rw-r--r--   0        0        0      138 2023-04-08 18:27:27.925629 horsetalk-0.6.1/horsetalk/form_break.py
--rw-r--r--   0        0        0      422 2023-04-08 16:50:46.371438 horsetalk-0.6.1/horsetalk/form_figures.py
--rw-r--r--   0        0        0      566 2023-04-08 16:43:51.100371 horsetalk-0.6.1/horsetalk/gender.py
--rw-r--r--   0        0        0      542 2023-04-08 16:50:46.371438 horsetalk-0.6.1/horsetalk/headgear.py
--rw-r--r--   0        0        0     2043 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horse_age.py
--rw-r--r--   0        0        0      205 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/horse_experience_level.py
--rw-r--r--   0        0        0     1146 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horse_height.py
--rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horselength.py
--rw-r--r--   0        0        0      303 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/jockey_experience_level.py
--rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.6.1/horsetalk/obstacle.py
--rw-r--r--   0        0        0      529 2023-04-08 20:26:58.137781 horsetalk-0.6.1/horsetalk/parsing_enum.py
--rw-r--r--   0        0        0      332 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/race_designation.py
--rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.6.1/horsetalk/race_distance.py
--rw-r--r--   0        0        0     2046 2023-04-08 16:50:46.373436 horsetalk-0.6.1/horsetalk/race_title.py
--rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.6.1/horsetalk/racing_code.py
--rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/sex.py
--rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/surface.py
--rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/turf_going_description.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.6.1/LICENSE
--rw-r--r--   0        0        0      723 2023-04-08 20:27:24.446544 horsetalk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.6.1/README.md
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1502 2023-04-12 22:25:58.873087 horsetalk-0.7.0/horsetalk/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-13 16:39:46.099964 horsetalk-0.7.0/horsetalk/age_category.py
+-rw-r--r--   0        0        0      428 2023-04-09 18:32:25.935876 horsetalk-0.7.0/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      289 2023-04-13 16:39:46.099964 horsetalk-0.7.0/horsetalk/breed.py
+-rw-r--r--   0        0        0      514 2023-04-13 16:41:40.705711 horsetalk-0.7.0/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      287 2023-04-13 16:41:40.706685 horsetalk-0.7.0/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0     1187 2023-04-13 16:41:40.706685 horsetalk-0.7.0/horsetalk/disaster.py
+-rw-r--r--   0        0        0      378 2023-04-13 16:39:46.100963 horsetalk-0.7.0/horsetalk/finishing_position.py
+-rw-r--r--   0        0        0      223 2023-04-13 16:39:46.100963 horsetalk-0.7.0/horsetalk/form_break.py
+-rw-r--r--   0        0        0     1426 2023-04-13 17:01:43.367227 horsetalk-0.7.0/horsetalk/form_figures.py
+-rw-r--r--   0        0        0     2566 2023-04-13 16:41:13.817125 horsetalk-0.7.0/horsetalk/gender.py
+-rw-r--r--   0        0        0      544 2023-04-13 16:39:46.101964 horsetalk-0.7.0/horsetalk/headgear.py
+-rw-r--r--   0        0        0     4549 2023-04-13 17:01:43.386995 horsetalk-0.7.0/horsetalk/horse_age.py
+-rw-r--r--   0        0        0      291 2023-04-13 16:39:46.101964 horsetalk-0.7.0/horsetalk/horse_experience_level.py
+-rw-r--r--   0        0        0     1148 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/horse_height.py
+-rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.7.0/horsetalk/horselength.py
+-rw-r--r--   0        0        0      390 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/jockey_experience_level.py
+-rw-r--r--   0        0        0      480 2023-04-13 16:39:46.102963 horsetalk-0.7.0/horsetalk/obstacle.py
+-rw-r--r--   0        0        0      529 2023-04-13 16:39:41.041691 horsetalk-0.7.0/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      420 2023-04-13 16:39:46.103964 horsetalk-0.7.0/horsetalk/race_designation.py
+-rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.7.0/horsetalk/race_distance.py
+-rw-r--r--   0        0        0     2636 2023-04-13 17:01:43.407145 horsetalk-0.7.0/horsetalk/race_title.py
+-rw-r--r--   0        0        0      372 2023-04-13 16:39:46.103964 horsetalk-0.7.0/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      258 2023-04-13 16:39:46.105966 horsetalk-0.7.0/horsetalk/sex.py
+-rw-r--r--   0        0        0      288 2023-04-13 16:39:46.105966 horsetalk-0.7.0/horsetalk/surface.py
+-rw-r--r--   0        0        0      839 2023-04-09 18:35:29.091069 horsetalk-0.7.0/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.7.0/LICENSE
+-rw-r--r--   0        0        0      723 2023-04-13 17:01:43.424654 horsetalk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.7.0/README.md
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.7.0/PKG-INFO
```

### Comparing `horsetalk-0.6.1/horsetalk/__init__.py` & `horsetalk-0.7.0/horsetalk/__init__.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/horsetalk/coat_colour.py` & `horsetalk-0.7.0/horsetalk/coat_colour.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/horsetalk/headgear.py` & `horsetalk-0.7.0/horsetalk/headgear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .parsing_enum import ParsingEnum
 
 
 class Headgear(ParsingEnum):
     """
     An enumeration representing the headgear worn by a horse in a race.
+
     """
 
     HOOD = 1
     BLINKERS = 2
     CHEEKPIECES = 3
     TONGUE_TIE = 4
     VISOR = 5
```

### Comparing `horsetalk-0.6.1/horsetalk/horse_height.py` & `horsetalk-0.7.0/horsetalk/horse_height.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from measurement.measures import Distance  # type: ignore
 
 
 class HorseHeight(Distance):
     """
     A class for measuring a horse's height, created by wrapping the measurement library Distance class to allow
     for the use of hands as a unit.
+
     """
 
     def __init__(self, distance: str) -> None:
         """
         Initialize a HorseHeight object from a string.
         """
         pattern = re.compile(r"(\d+\D+)")
```

### Comparing `horsetalk-0.6.1/horsetalk/horselength.py` & `horsetalk-0.7.0/horsetalk/horselength.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/horsetalk/parsing_enum.py` & `horsetalk-0.7.0/horsetalk/parsing_enum.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/horsetalk/race_distance.py` & `horsetalk-0.7.0/horsetalk/race_distance.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/horsetalk/race_title.py` & `horsetalk-0.7.0/horsetalk/race_title.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,38 @@
 from .horse_experience_level import HorseExperienceLevel
 from .gender import Gender
 from .obstacle import Obstacle
 from .race_designation import RaceDesignation
 
 
 class RaceTitle:
+    """
+    A class for parsing a race title into its component parts.
+
+    Attributes:
+        _words (List[str]): A list of words in the race title.
+
+    Methods:
+        parse(title: str) -> dict: Parses a race title into component parts and returns a dictionary.
+        _lookup(enum: Type[Enum], allow_multiple: bool = False) -> List[Enum] | Enum | None:
+            Private method to lookup an Enum value from a list of words.
+
+    """
+
     _words: List[str] = []
 
     @classmethod
     def parse(cls, title: str) -> dict:
-        """Parse a race title into component parts
+        """Parses a race title into component parts.
 
-        :param title: A race title
-        :type title: str
-        :return: A dictionary of component parts
-        :rtype: dict
+        Args:
+            title: A race title.
+
+        Returns:
+            dict: A dictionary of component parts.
         """
         self = cls()
         self._words = title.split()
 
         enums = [AgeCategory, HorseExperienceLevel, Gender, Obstacle, RaceDesignation]
         end_index = -1
         for i, word in enumerate(self._words):
@@ -38,20 +52,23 @@
             "race_designation": self._lookup(RaceDesignation),
             "name": name,
         }
 
     def _lookup(
         self, enum: Type[Enum], allow_multiple: bool = False
     ) -> List[Enum] | Enum | None:
-        """Private method to lookup an enum value from a list of words
+        """Private method to lookup an enum value from a list of words.
+
+        Args:
+            enum (Type[Enum]): The Enum to search through.
+            allow_multiple (bool, optional): Whether or not to allow multiple Enum values to be returned. Defaults to False.
+
+        Returns:
+            Union[List[Enum], Enum, None]: The found Enum value or None.
 
-        :param enum: Enum to search through
-        :type enum: Type[Enum]
-        :return: The found Enum value or None
-        :rtype: Enum | None
         """
         found_values = [
             found_value
             for word in self._words
             if (found_value := getattr(enum, word, None)) is not None
         ]
         return (
```

### Comparing `horsetalk-0.6.1/horsetalk/turf_going_description.py` & `horsetalk-0.7.0/horsetalk/turf_going_description.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/LICENSE` & `horsetalk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.1/pyproject.toml` & `horsetalk-0.7.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.6.1"
+version = "0.7.0"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `horsetalk-0.6.1/PKG-INFO` & `horsetalk-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.6.1
+Version: 0.7.0
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

