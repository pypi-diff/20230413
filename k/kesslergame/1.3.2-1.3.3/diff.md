# Comparing `tmp/kesslergame-1.3.2.tar.gz` & `tmp/kesslergame-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kesslergame-1.3.2.tar", last modified: Tue Mar  7 15:07:05 2023, max compression
+gzip compressed data, was "kesslergame-1.3.3.tar", last modified: Thu Apr 13 17:22:17 2023, max compression
```

## Comparing `kesslergame-1.3.2.tar` & `kesslergame-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.315747 kesslergame-1.3.2/
--rw-rw-rw-   0        0        0    11565 2023-03-07 15:06:39.000000 kesslergame-1.3.2/LICENSE
--rw-rw-rw-   0        0        0       73 2023-03-07 15:06:39.000000 kesslergame-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3330 2023-03-07 15:07:05.315747 kesslergame-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2023-03-07 15:06:39.000000 kesslergame-1.3.2/README.md
--rw-rw-rw-   0        0        0      423 2023-03-07 15:06:39.000000 kesslergame-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       15 2023-03-07 15:06:39.000000 kesslergame-1.3.2/requirements.txt
--rw-rw-rw-   0        0        0      882 2023-03-07 15:07:05.315747 kesslergame-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-03-07 15:06:39.000000 kesslergame-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.284498 kesslergame-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.300145 kesslergame-1.3.2/src/kesslergame/
--rw-rw-rw-   0        0        0      609 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/asteroid.py
--rw-rw-rw-   0        0        0     1524 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/bullet.py
--rw-rw-rw-   0        0        0     1489 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/collisions.py
--rw-rw-rw-   0        0        0     1420 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/controller.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.315747 kesslergame-1.3.2/src/kesslergame/graphics/
--rw-rw-rw-   0        0        0      380 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/__init__.py
--rw-rw-rw-   0        0        0      720 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/graphics_base.py
--rw-rw-rw-   0        0        0     2433 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/graphics_handler.py
--rw-rw-rw-   0        0        0     5122 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/graphics_plt.py
--rw-rw-rw-   0        0        0     8808 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/graphics_tk.py
--rw-rw-rw-   0        0        0     3992 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/graphics_ue.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.315747 kesslergame-1.3.2/src/kesslergame/graphics/images/
--rw-rw-rw-   0        0        0        0 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/images/__init__.py
--rw-rw-rw-   0        0        0     2708 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip1_green.png
--rw-rw-rw-   0        0        0     2578 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip1_orange.png
--rw-rw-rw-   0        0        0     3597 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip2_orange.png
--rw-rw-rw-   0        0        0     2725 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip3_orange.png
--rw-rw-rw-   0        0        0    14567 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/kessler_game.py
--rw-rw-rw-   0        0        0     6486 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/scenario.py
--rw-rw-rw-   0        0        0     2285 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/score.py
--rw-rw-rw-   0        0        0     8363 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/ship.py
--rw-rw-rw-   0        0        0     1506 2023-03-07 15:06:39.000000 kesslergame-1.3.2/src/kesslergame/team.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:07:05.315747 kesslergame-1.3.2/src/kesslergame.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 15:07:05.000000 kesslergame-1.3.2/src/kesslergame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.799060 kesslergame-1.3.3/
+-rw-rw-rw-   0        0        0    11565 2023-04-13 17:21:54.000000 kesslergame-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-04-13 17:21:54.000000 kesslergame-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3330 2023-04-13 17:22:17.799060 kesslergame-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2023-04-13 17:21:54.000000 kesslergame-1.3.3/README.md
+-rw-rw-rw-   0        0        0      423 2023-04-13 17:21:54.000000 kesslergame-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       23 2023-04-13 17:21:54.000000 kesslergame-1.3.3/requirements.txt
+-rw-rw-rw-   0        0        0      882 2023-04-13 17:22:17.799060 kesslergame-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-04-13 17:21:54.000000 kesslergame-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.767814 kesslergame-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.783431 kesslergame-1.3.3/src/kesslergame/
+-rw-rw-rw-   0        0        0      609 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/asteroid.py
+-rw-rw-rw-   0        0        0     1524 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/bullet.py
+-rw-rw-rw-   0        0        0     1489 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/collisions.py
+-rw-rw-rw-   0        0        0     1420 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/controller.py
+-rw-rw-rw-   0        0        0     4654 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/controller_gamepad.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.783431 kesslergame-1.3.3/src/kesslergame/graphics/
+-rw-rw-rw-   0        0        0      380 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/graphics_base.py
+-rw-rw-rw-   0        0        0     2433 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/graphics_handler.py
+-rw-rw-rw-   0        0        0     5122 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/graphics_plt.py
+-rw-rw-rw-   0        0        0     8874 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/graphics_tk.py
+-rw-rw-rw-   0        0        0     3992 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/graphics_ue.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.799060 kesslergame-1.3.3/src/kesslergame/graphics/images/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/images/__init__.py
+-rw-rw-rw-   0        0        0     2708 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip1_green.png
+-rw-rw-rw-   0        0        0     2578 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip1_orange.png
+-rw-rw-rw-   0        0        0     3597 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip2_orange.png
+-rw-rw-rw-   0        0        0     2725 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip3_orange.png
+-rw-rw-rw-   0        0        0    14596 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/kessler_game.py
+-rw-rw-rw-   0        0        0     6486 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/scenario.py
+-rw-rw-rw-   0        0        0     2285 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/score.py
+-rw-rw-rw-   0        0        0     8363 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/ship.py
+-rw-rw-rw-   0        0        0     1506 2023-04-13 17:21:54.000000 kesslergame-1.3.3/src/kesslergame/team.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:22:17.783431 kesslergame-1.3.3/src/kesslergame.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1129 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 17:22:17.000000 kesslergame-1.3.3/src/kesslergame.egg-info/zip-safe
```

### Comparing `kesslergame-1.3.2/LICENSE` & `kesslergame-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/PKG-INFO` & `kesslergame-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kesslergame
-Version: 1.3.2
+Version: 1.3.3
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zachariah.phillips@us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@psibernetix.com
 License: Apache 2.0 License
```

### Comparing `kesslergame-1.3.2/README.md` & `kesslergame-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/setup.cfg` & `kesslergame-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/__init__.py` & `kesslergame-1.3.3/src/kesslergame/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .scenario import Scenario
 from .score import Score
 from .graphics import GraphicsType, KesslerGraphics
 
 
 __all__ = ['KesslerGame', 'TrainerEnvironment', 'KesslerController', 'Scenario', 'Score', 'GraphicsType',
            'KesslerGraphics']
-__version__ = '1.3.2'
+__version__ = '1.3.3'
```

### Comparing `kesslergame-1.3.2/src/kesslergame/asteroid.py` & `kesslergame-1.3.3/src/kesslergame/asteroid.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/bullet.py` & `kesslergame-1.3.3/src/kesslergame/bullet.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/collisions.py` & `kesslergame-1.3.3/src/kesslergame/collisions.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/controller.py` & `kesslergame-1.3.3/src/kesslergame/controller.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/graphics_base.py` & `kesslergame-1.3.3/src/kesslergame/graphics/graphics_base.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/graphics_handler.py` & `kesslergame-1.3.3/src/kesslergame/graphics/graphics_handler.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/graphics_plt.py` & `kesslergame-1.3.3/src/kesslergame/graphics/graphics_plt.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/graphics_tk.py` & `kesslergame-1.3.3/src/kesslergame/graphics/graphics_tk.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 class GraphicsTK(KesslerGraphics):
     def __init__(self, UI_settings):
         # UI settings
         # lives, accuracy, asteroids hit, shots taken, bullets left
         # default_ui = {'ships': True, 'lives_remaining': True, 'accuracy': True, 'asteroids_hit': True}
+        UI_settings = {} if UI_settings is None else UI_settings
         self.show_ships = UI_settings.get('ships', True)
         self.show_lives = UI_settings.get('lives_remaining', True)
         self.show_accuracy = UI_settings.get('accuracy', True)
         self.show_asteroids_hit = UI_settings.get('asteroids_hit', True)
         self.show_shots_fired = UI_settings.get('shots_fired', False)
         self.show_bullets_remaining = UI_settings.get('bullets_remaining', False)
         self.show_controller_name = UI_settings.get('controller_name', True)
```

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/graphics_ue.py` & `kesslergame-1.3.3/src/kesslergame/graphics/graphics_ue.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip1_green.png` & `kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip1_green.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip1_orange.png` & `kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip1_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip2_orange.png` & `kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip2_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/graphics/images/playerShip3_orange.png` & `kesslergame-1.3.3/src/kesslergame/graphics/images/playerShip3_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/kessler_game.py` & `kesslergame-1.3.3/src/kesslergame/kessler_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             # No asteroids remain
             if not asteroids:
                 stop_reason = StopReason.no_asteroids
             # No ships are alive
             elif not liveships:
                 stop_reason = StopReason.no_ships
             # All live ships are out of bullets and no bullets are on map
-            elif not sum([ship.bullets_remaining for ship in liveships]) and not len(bullets)>0:
+            elif not sum([ship.bullets_remaining for ship in liveships]) and not len(bullets)>0 and scenario.stop_if_no_ammo:
                 stop_reason = StopReason.out_of_bullets
             # Out of time
             elif sim_time > time_limit:
                 stop_reason = StopReason.time_expired
 
             # --- FINISHING TIME STEP ----------------------------------------------------------------------------------
             # Get overall time step compute time
```

### Comparing `kesslergame-1.3.2/src/kesslergame/scenario.py` & `kesslergame-1.3.3/src/kesslergame/scenario.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/score.py` & `kesslergame-1.3.3/src/kesslergame/score.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/ship.py` & `kesslergame-1.3.3/src/kesslergame/ship.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame/team.py` & `kesslergame-1.3.3/src/kesslergame/team.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.2/src/kesslergame.egg-info/PKG-INFO` & `kesslergame-1.3.3/src/kesslergame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kesslergame
-Version: 1.3.2
+Version: 1.3.3
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zachariah.phillips@us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@psibernetix.com
 License: Apache 2.0 License
```

### Comparing `kesslergame-1.3.2/src/kesslergame.egg-info/SOURCES.txt` & `kesslergame-1.3.3/src/kesslergame.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.cfg
 setup.py
 src/kesslergame/__init__.py
 src/kesslergame/asteroid.py
 src/kesslergame/bullet.py
 src/kesslergame/collisions.py
 src/kesslergame/controller.py
+src/kesslergame/controller_gamepad.py
 src/kesslergame/kessler_game.py
 src/kesslergame/scenario.py
 src/kesslergame/score.py
 src/kesslergame/ship.py
 src/kesslergame/team.py
 src/kesslergame.egg-info/PKG-INFO
 src/kesslergame.egg-info/SOURCES.txt
```

