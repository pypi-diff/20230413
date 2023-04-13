# Comparing `tmp/wom_py-0.3.0.tar.gz` & `tmp/wom_py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.3.0.tar", max compression
+gzip compressed data, was "wom_py-0.3.1.tar", max compression
```

## Comparing `wom_py-0.3.0.tar` & `wom_py-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-04-08 19:46:24.132712 wom_py-0.3.0/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-08 19:46:24.132712 wom_py-0.3.0/README.md
--rw-r--r--   0        0        0     2138 2023-04-08 19:46:24.132712 wom_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4295 2023-04-08 19:46:24.212712 wom_py-0.3.0/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/_cli.py
--rw-r--r--   0        0        0     7795 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/client.py
--rw-r--r--   0        0        0     1447 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/constants.py
--rw-r--r--   0        0        0     7140 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/errors.py
--rw-r--r--   0        0        0     3138 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7364 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9075 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/http.py
--rw-r--r--   0        0        0     1381 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/enums.py
--rw-r--r--   0        0        0     3778 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/enums.py
--rw-r--r--   0        0        0    11832 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/py.typed
--rw-r--r--   0        0        0     5509 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/result.py
--rw-r--r--   0        0        0     6420 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/routes.py
--rw-r--r--   0        0        0    33973 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/__init__.py
--rw-r--r--   0        0        0     2042 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/base.py
--rw-r--r--   0        0        0    20760 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/competitions.py
--rw-r--r--   0        0        0     3477 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/deltas.py
--rw-r--r--   0        0        0     3637 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/efficiency.py
--rw-r--r--   0        0        0    23384 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/groups.py
--rw-r--r--   0        0        0     5355 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/http.py
--rw-r--r--   0        0        0     4722 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/names.py
--rw-r--r--   0        0        0    17519 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/players.py
--rw-r--r--   0        0        0     3455 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/records.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-13 00:11:49.609447 wom_py-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-13 00:11:49.609447 wom_py-0.3.1/README.md
+-rw-r--r--   0        0        0     2138 2023-04-13 00:11:49.609447 wom_py-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4295 2023-04-13 00:11:49.693447 wom_py-0.3.1/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/_cli.py
+-rw-r--r--   0        0        0     7795 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/constants.py
+-rw-r--r--   0        0        0     7212 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/errors.py
+-rw-r--r--   0        0        0     3138 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7364 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9075 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/http.py
+-rw-r--r--   0        0        0     1381 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/enums.py
+-rw-r--r--   0        0        0     3778 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11832 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/py.typed
+-rw-r--r--   0        0        0     5509 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/result.py
+-rw-r--r--   0        0        0     6420 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/routes.py
+-rw-r--r--   0        0        0    33973 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/__init__.py
+-rw-r--r--   0        0        0     2042 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/base.py
+-rw-r--r--   0        0        0    20760 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/competitions.py
+-rw-r--r--   0        0        0     3477 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/deltas.py
+-rw-r--r--   0        0        0     3637 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/efficiency.py
+-rw-r--r--   0        0        0    23384 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/groups.py
+-rw-r--r--   0        0        0     5355 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/http.py
+-rw-r--r--   0        0        0     4722 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/names.py
+-rw-r--r--   0        0        0    17519 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/players.py
+-rw-r--r--   0        0        0     3455 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/records.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.1/PKG-INFO
```

### Comparing `wom_py-0.3.0/LICENSE` & `wom_py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/README.md` & `wom_py-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/pyproject.toml` & `wom_py-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.3.0"
+version = "0.3.1"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.3.0/wom/__init__.py` & `wom_py-0.3.1/wom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,23 +130,23 @@
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.3.0"
+__version__: Final[str] = "0.3.1"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[7403fdf]"
+__git_sha__: Final[str] = "[8864456]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.3.0/wom/__main__.py` & `wom_py-0.3.1/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/_cli.py` & `wom_py-0.3.1/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/client.py` & `wom_py-0.3.1/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/constants.py` & `wom_py-0.3.1/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/enums.py` & `wom_py-0.3.1/wom/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,17 +179,19 @@
 
 
 class Bosses(Metric):
     """Bosses from OSRS."""
 
     AbyssalSire = "abyssal_sire"
     AlchemicalHydra = "alchemical_hydra"
+    Artio = "artio"
     BarrowsChests = "barrows_chests"
     Brophyta = "bryophyta"
     Callisto = "callisto"
+    Calvarion = "calvarion"
     Cerberus = "cerberus"
     ChambersOfXeric = "chambers_of_xeric"
     ChambersOfXericChallenge = "chambers_of_xeric_challenge_mode"
     ChaosElemental = "chaos_elemental"
     ChaosFanatic = "chaos_fanatic"
     CommanderZilyana = "commander_zilyana"
     CorporealBeast = "corporeal_beast"
@@ -212,14 +214,15 @@
     Nightmare = "nightmare"
     PhosanisNightmare = "phosanis_nightmare"
     Obor = "obor"
     PhantomMuspah = "phantom_muspah"
     Sarachnis = "sarachnis"
     Scorpia = "scorpia"
     Skotizo = "skotizo"
+    Spindel = "spindel"
     Tempoross = "tempoross"
     TheGuantlet = "the_gauntlet"
     TheCorruptedGauntlet = "the_corrupted_gauntlet"
     TheatreOfBlood = "theatre_of_blood"
     TheatreOfBloodHard = "theatre_of_blood_hard_mode"
     ThermonuclearSmokeDevil = "thermonuclear_smoke_devil"
     TombsOfAmascut = "tombs_of_amascut"
```

### Comparing `wom_py-0.3.0/wom/errors.py` & `wom_py-0.3.1/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/__init__.py` & `wom_py-0.3.1/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/base.py` & `wom_py-0.3.1/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/competitions/__init__.py` & `wom_py-0.3.1/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/competitions/enums.py` & `wom_py-0.3.1/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/competitions/models.py` & `wom_py-0.3.1/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/deltas/__init__.py` & `wom_py-0.3.1/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/deltas/models.py` & `wom_py-0.3.1/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/groups/__init__.py` & `wom_py-0.3.1/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/groups/enums.py` & `wom_py-0.3.1/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/groups/models.py` & `wom_py-0.3.1/wom/models/groups/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/http.py` & `wom_py-0.3.1/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/names/__init__.py` & `wom_py-0.3.1/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/names/enums.py` & `wom_py-0.3.1/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/names/models.py` & `wom_py-0.3.1/wom/models/names/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/players/__init__.py` & `wom_py-0.3.1/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/players/enums.py` & `wom_py-0.3.1/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/players/models.py` & `wom_py-0.3.1/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/records/__init__.py` & `wom_py-0.3.1/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/models/records/models.py` & `wom_py-0.3.1/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/result.py` & `wom_py-0.3.1/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/routes.py` & `wom_py-0.3.1/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/serializer.py` & `wom_py-0.3.1/wom/serializer.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/__init__.py` & `wom_py-0.3.1/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/base.py` & `wom_py-0.3.1/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/competitions.py` & `wom_py-0.3.1/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/deltas.py` & `wom_py-0.3.1/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/efficiency.py` & `wom_py-0.3.1/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/groups.py` & `wom_py-0.3.1/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/http.py` & `wom_py-0.3.1/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/names.py` & `wom_py-0.3.1/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/players.py` & `wom_py-0.3.1/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/wom/services/records.py` & `wom_py-0.3.1/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.0/PKG-INFO` & `wom_py-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

