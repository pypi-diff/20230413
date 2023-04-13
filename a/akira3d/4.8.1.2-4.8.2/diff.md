# Comparing `tmp/akira3d-4.8.1.2.tar.gz` & `tmp/akira3d-4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akira3d-4.8.1.2.tar", last modified: Thu Apr 13 11:05:57 2023, max compression
+gzip compressed data, was "akira3d-4.8.2.tar", last modified: Thu Apr 13 13:35:38 2023, max compression
```

## Comparing `akira3d-4.8.1.2.tar` & `akira3d-4.8.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:57.830442 akira3d-4.8.1.2/
--rw-rw-rw-   0        0        0      146 2023-04-13 11:05:57.830442 akira3d-4.8.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:57.826439 akira3d-4.8.1.2/akira3d/
--rw-rw-rw-   0        0        0      518 2023-04-12 17:31:21.000000 akira3d-4.8.1.2/akira3d/__init__.py
--rw-rw-rw-   0        0        0     2045 2023-04-12 17:20:27.000000 akira3d-4.8.1.2/akira3d/camera.py
--rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/colliders.py
--rw-rw-rw-   0        0        0      170 2023-04-12 17:46:39.000000 akira3d-4.8.1.2/akira3d/createNewGame.py
--rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/gameEngine.py
--rw-rw-rw-   0        0        0      522 2023-04-12 17:17:16.000000 akira3d-4.8.1.2/akira3d/light.py
--rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/mesh.py
--rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/mobs.py
--rw-rw-rw-   0        0        0     7810 2023-04-11 08:26:43.000000 akira3d-4.8.1.2/akira3d/model.py
--rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/phisics.py
--rw-rw-rw-   0        0        0     6942 2023-04-11 08:32:00.000000 akira3d-4.8.1.2/akira3d/render.py
--rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.8.1.2/akira3d/shader_program.py
--rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.8.1.2/akira3d/texture.py
--rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.8.1.2/akira3d/vao.py
--rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.8.1.2/akira3d/vbo.py
--rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.8.1.2/akira3d/vidSys.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:05:57.829441 akira3d-4.8.1.2/akira3d.egg-info/
--rw-rw-rw-   0        0        0      146 2023-04-13 11:05:57.000000 akira3d-4.8.1.2/akira3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:05:57.000000 akira3d-4.8.1.2/akira3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:05:57.000000 akira3d-4.8.1.2/akira3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 11:05:57.000000 akira3d-4.8.1.2/akira3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-13 11:05:57.000000 akira3d-4.8.1.2/akira3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:05:57.831442 akira3d-4.8.1.2/setup.cfg
--rw-rw-rw-   0        0        0      243 2023-04-13 11:05:53.000000 akira3d-4.8.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.493916 akira3d-4.8.2/
+-rw-rw-rw-   0        0        0      144 2023-04-13 13:35:38.493916 akira3d-4.8.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.488915 akira3d-4.8.2/akira3d/
+-rw-rw-rw-   0        0        0      518 2023-04-12 17:31:21.000000 akira3d-4.8.2/akira3d/__init__.py
+-rw-rw-rw-   0        0        0     2045 2023-04-12 17:20:27.000000 akira3d-4.8.2/akira3d/camera.py
+-rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/colliders.py
+-rw-rw-rw-   0        0        0      170 2023-04-12 17:46:39.000000 akira3d-4.8.2/akira3d/createNewGame.py
+-rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/gameEngine.py
+-rw-rw-rw-   0        0        0      522 2023-04-12 17:17:16.000000 akira3d-4.8.2/akira3d/light.py
+-rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/mesh.py
+-rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/mobs.py
+-rw-rw-rw-   0        0        0     7810 2023-04-11 08:26:43.000000 akira3d-4.8.2/akira3d/model.py
+-rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/phisics.py
+-rw-rw-rw-   0        0        0     6942 2023-04-11 08:32:00.000000 akira3d-4.8.2/akira3d/render.py
+-rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/shader_program.py
+-rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/texture.py
+-rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/vao.py
+-rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.8.2/akira3d/vbo.py
+-rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/vidSys.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.493916 akira3d-4.8.2/akira3d.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       84 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:35:38.494917 akira3d-4.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-04-13 13:35:17.000000 akira3d-4.8.2/setup.py
```

### Comparing `akira3d-4.8.1.2/akira3d/__init__.py` & `akira3d-4.8.2/akira3d/__init__.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/camera.py` & `akira3d-4.8.2/akira3d/camera.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/colliders.py` & `akira3d-4.8.2/akira3d/colliders.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/light.py` & `akira3d-4.8.2/akira3d/light.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/mobs.py` & `akira3d-4.8.2/akira3d/mobs.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/model.py` & `akira3d-4.8.2/akira3d/model.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/phisics.py` & `akira3d-4.8.2/akira3d/phisics.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/render.py` & `akira3d-4.8.2/akira3d/render.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/shader_program.py` & `akira3d-4.8.2/akira3d/shader_program.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/texture.py` & `akira3d-4.8.2/akira3d/texture.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/vao.py` & `akira3d-4.8.2/akira3d/vao.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/vbo.py` & `akira3d-4.8.2/akira3d/vbo.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.1.2/akira3d/vidSys.py` & `akira3d-4.8.2/akira3d/vidSys.py`

 * *Files identical despite different names*

