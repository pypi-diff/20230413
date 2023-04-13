# Comparing `tmp/WaveLinkCord-2.2.2.tar.gz` & `tmp/WaveLinkCord-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveLinkCord-2.2.2.tar", last modified: Wed Apr 12 16:20:35 2023, max compression
+gzip compressed data, was "WaveLinkCord-2.2.3.tar", last modified: Thu Apr 13 21:27:26 2023, max compression
```

## Comparing `WaveLinkCord-2.2.2.tar` & `WaveLinkCord-2.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.210651 WaveLinkCord-2.2.2/
--rw-rw-rw-   0        0        0     1108 2023-03-11 18:03:30.000000 WaveLinkCord-2.2.2/LICENSE
--rw-rw-rw-   0        0        0     6010 2023-04-12 16:20:35.211651 WaveLinkCord-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5123 2023-04-12 16:20:02.000000 WaveLinkCord-2.2.2/README.rst
--rw-rw-rw-   0        0        0     1015 2023-04-12 16:20:03.000000 WaveLinkCord-2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       30 2023-03-11 18:15:49.000000 WaveLinkCord-2.2.2/requirements.txt
--rw-rw-rw-   0        0        0      672 2023-04-12 16:20:35.218654 WaveLinkCord-2.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.054618 WaveLinkCord-2.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.092626 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/
--rw-rw-rw-   0        0        0     6010 2023-04-12 16:20:35.000000 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-04-12 16:20:35.000000 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 16:20:35.000000 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-12 16:20:35.000000 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 16:20:35.000000 WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.177644 WaveLinkCord-2.2.2/src/wavelinkcord/
--rw-rw-rw-   0        0        0     1495 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.2/src/wavelinkcord/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/backoff.py
--rw-rw-rw-   0        0        0     1731 2023-04-12 15:43:17.000000 WaveLinkCord-2.2.2/src/wavelinkcord/enums.py
--rw-rw-rw-   0        0        0     1995 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.056617 WaveLinkCord-2.2.2/src/wavelinkcord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.180647 WaveLinkCord-2.2.2/src/wavelinkcord/ext/spotify/
--rw-rw-rw-   0        0        0    16468 2023-04-12 16:18:34.000000 WaveLinkCord-2.2.2/src/wavelinkcord/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/filters.py
--rw-rw-rw-   0        0        0    17775 2023-04-12 16:19:22.000000 WaveLinkCord-2.2.2/src/wavelinkcord/node.py
--rw-rw-rw-   0        0        0     2474 2023-04-12 15:46:28.000000 WaveLinkCord-2.2.2/src/wavelinkcord/payloads.py
--rw-rw-rw-   0        0        0    20778 2023-04-12 15:44:18.000000 WaveLinkCord-2.2.2/src/wavelinkcord/player.py
--rw-rw-rw-   0        0        0    12384 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.2/src/wavelinkcord/queue.py
--rw-rw-rw-   0        0        0    10104 2023-04-12 15:44:29.000000 WaveLinkCord-2.2.2/src/wavelinkcord/tracks.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:20:35.208651 WaveLinkCord-2.2.2/src/wavelinkcord/types/
--rw-rw-rw-   0        0        0      860 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/types/events.py
--rw-rw-rw-   0        0        0      635 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/types/request.py
--rw-rw-rw-   0        0        0      424 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.2/src/wavelinkcord/types/state.py
--rw-rw-rw-   0        0        0      343 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.2/src/wavelinkcord/types/track.py
--rw-rw-rw-   0        0        0     9098 2023-04-12 16:19:03.000000 WaveLinkCord-2.2.2/src/wavelinkcord/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.270708 WaveLinkCord-2.2.3/
+-rw-rw-rw-   0        0        0     1108 2023-03-11 18:03:30.000000 WaveLinkCord-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6010 2023-04-13 21:27:26.271554 WaveLinkCord-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5123 2023-04-12 16:20:02.000000 WaveLinkCord-2.2.3/README.rst
+-rw-rw-rw-   0        0        0     1015 2023-04-13 21:26:50.000000 WaveLinkCord-2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       30 2023-03-11 18:15:49.000000 WaveLinkCord-2.2.3/requirements.txt
+-rw-rw-rw-   0        0        0      672 2023-04-13 21:27:26.287807 WaveLinkCord-2.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.102752 WaveLinkCord-2.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.176991 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/
+-rw-rw-rw-   0        0        0     6010 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.224517 WaveLinkCord-2.2.3/src/wavelinkcord/
+-rw-rw-rw-   0        0        0     1495 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/backoff.py
+-rw-rw-rw-   0        0        0     1731 2023-04-12 15:43:17.000000 WaveLinkCord-2.2.3/src/wavelinkcord/enums.py
+-rw-rw-rw-   0        0        0     1995 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.106935 WaveLinkCord-2.2.3/src/wavelinkcord/ext/
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.227518 WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/
+-rw-rw-rw-   0        0        0    16472 2023-04-13 21:21:23.000000 WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/filters.py
+-rw-rw-rw-   0        0        0    17775 2023-04-12 16:19:22.000000 WaveLinkCord-2.2.3/src/wavelinkcord/node.py
+-rw-rw-rw-   0        0        0     2474 2023-04-12 15:46:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/payloads.py
+-rw-rw-rw-   0        0        0    20778 2023-04-12 15:44:18.000000 WaveLinkCord-2.2.3/src/wavelinkcord/player.py
+-rw-rw-rw-   0        0        0    12384 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/queue.py
+-rw-rw-rw-   0        0        0    10104 2023-04-12 15:44:29.000000 WaveLinkCord-2.2.3/src/wavelinkcord/tracks.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.267720 WaveLinkCord-2.2.3/src/wavelinkcord/types/
+-rw-rw-rw-   0        0        0      860 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/track.py
+-rw-rw-rw-   0        0        0     9098 2023-04-12 16:19:03.000000 WaveLinkCord-2.2.3/src/wavelinkcord/websocket.py
```

### Comparing `WaveLinkCord-2.2.2/LICENSE` & `WaveLinkCord-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/PKG-INFO` & `WaveLinkCord-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveLinkCord
-Version: 2.2.2
+Version: 2.2.3
 Summary: A robust and powerful Lavalink wrapper for Nextcord
 Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
 Author: Zyb3rWolfi
 Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `WaveLinkCord-2.2.2/README.rst` & `WaveLinkCord-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/pyproject.toml` & `WaveLinkCord-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WaveLinkCord"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
   { name="Zyb3rWolfi ", email="Zyb3rWolfi@proton.me" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for Nextcord"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `WaveLinkCord-2.2.2/setup.cfg` & `WaveLinkCord-2.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6176 656c 696e 6b63 6f72 640d   = wavelinkcord.
-00000020: 0a76 6572 7369 6f6e 203d 2032 2e32 2e32  .version = 2.2.2
+00000020: 0a76 6572 7369 6f6e 203d 2032 2e32 2e33  .version = 2.2.3
 00000030: 0d0a 6175 7468 6f72 203d 205a 7962 3372  ..author = Zyb3r
 00000040: 576f 6c66 690d 0a61 7574 686f 725f 656d  Wolfi..author_em
 00000050: 6169 6c20 3d20 7a79 6233 7277 6f6c 6669  ail = zyb3rwolfi
 00000060: 4070 726f 746f 6e2e 6d65 0d0a 6465 7363  @proton.me..desc
 00000070: 7269 7074 696f 6e20 3d20 4120 706f 7765  ription = A powe
 00000080: 7266 756c 204c 6176 616c 696e 6b20 6c69  rful Lavalink li
 00000090: 6272 6172 7920 666f 7220 4e65 7874 636f  brary for Nextco
```

### Comparing `WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/PKG-INFO` & `WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveLinkCord
-Version: 2.2.2
+Version: 2.2.3
 Summary: A robust and powerful Lavalink wrapper for Nextcord
 Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
 Author: Zyb3rWolfi
 Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `WaveLinkCord-2.2.2/src/WaveLinkCord.egg-info/SOURCES.txt` & `WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/__init__.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/__init__.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/backoff.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/backoff.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/enums.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/enums.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/exceptions.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/exceptions.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/ext/spotify/__init__.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
         player: :class:`wavelink.player.Player`
             If Player.autoplay is enabled, this search will fill the AutoPlay Queue.
         cls
             The class to convert this Spotify Track to.
         """
         try:
             tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-        except wavelink.NoTracksError:
+        except wavelinkcord.NoTracksError:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
 
         if not player.autoplay or not populate:
             return tracks[0]
 
         node: Node = player.current_node
         sc: SpotifyClient | None = node._spotify
```

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/filters.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/filters.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/node.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/node.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/payloads.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/payloads.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/player.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/player.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/queue.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/queue.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/tracks.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/tracks.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/types/events.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/types/events.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/types/request.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/types/request.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.2/src/wavelinkcord/websocket.py` & `WaveLinkCord-2.2.3/src/wavelinkcord/websocket.py`

 * *Files identical despite different names*

