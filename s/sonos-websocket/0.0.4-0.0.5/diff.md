# Comparing `tmp/sonos-websocket-0.0.4.tar.gz` & `tmp/sonos-websocket-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonos-websocket-0.0.4.tar", last modified: Tue Apr 11 02:45:55 2023, max compression
+gzip compressed data, was "sonos-websocket-0.0.5.tar", last modified: Thu Apr 13 04:24:20 2023, max compression
```

## Comparing `sonos-websocket-0.0.4.tar` & `sonos-websocket-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.989349 sonos-websocket-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:45:55.989349 sonos-websocket-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/sonos_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/sonos_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.927635 sonos-websocket-0.0.5/sonos_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/sonos_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/top_level.txt
```

### Comparing `sonos-websocket-0.0.4/PKG-INFO` & `sonos-websocket-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.4
+Version: 0.0.5
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sonos-websocket-0.0.4/README.md` & `sonos-websocket-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.4/pyproject.toml` & `sonos-websocket-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -48,11 +48,21 @@
     "E",  # pycodestyle
     "F",  # pyflakes/autoflake
     "I",  # isort
     "RUF006", # Store a reference to the return value of asyncio.create_task
     "W",  # pycodestyle
 ]
 
+ignore = [
+    "D203",  # 1 blank line required before class docstring
+    "D213",  # Multi-line docstring summary should start at the second line
+    "E501",  # line too long
+]
+
+[tool.ruff.isort]
+combine-as-imports = true
+force-sort-within-sections = true
+
 [tool.pylint]
 disable = [
     "invalid-name",
 ]
```

### Comparing `sonos-websocket-0.0.4/sonos_websocket/__main__.py` & `sonos-websocket-0.0.5/sonos_websocket/__main__.py`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.4/sonos_websocket/websocket.py` & `sonos-websocket-0.0.5/sonos_websocket/websocket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Handler for Sonos websockets."""
 import asyncio
 import logging
+import sys
 from typing import Any, cast
 
 import aiohttp
 
-from .const import API_KEY
+from .const import API_KEY, MAX_ATTEMPTS
 from .exception import (
     SonosWebsocketError,
     SonosWSConnectionError,
     Unauthorized,
     Unsupported,
 )
 
+if sys.version_info[:2] < (3, 11):
+    from async_timeout import timeout as asyncio_timeout
+else:
+    from asyncio import timeout as asyncio_timeout
+
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class SonosWebsocket:
     """Sonos websocket handler."""
 
     def __init__(
@@ -38,55 +45,73 @@
     async def connect(self) -> None:
         """Open a persistent websocket connection and act on events."""
         async with self._connect_lock:
             if self.ws and not self.ws.closed:
                 _LOGGER.warning("Websocket is already connected")
                 return
 
+        _LOGGER.debug("Opening websocket to %s", self.uri)
         headers = {
             "X-Sonos-Api-Key": API_KEY,
             "Sec-WebSocket-Protocol": "v1.api.smartspeaker.audio",
         }
         try:
-            self.ws = await self.session.ws_connect(
-                self.uri, headers=headers, heartbeat=15, verify_ssl=False
-            )
+            async with asyncio_timeout(3):
+                self.ws = await self.session.ws_connect(
+                    self.uri, headers=headers, verify_ssl=False
+                )
         except aiohttp.ClientResponseError as exc:
             if exc.code == 401:
                 _LOGGER.error("Credentials rejected: %s", exc)
                 raise Unauthorized("Credentials rejected") from exc
             raise SonosWSConnectionError(
                 f"Unexpected response received: {exc}"
             ) from exc
-        except (aiohttp.ClientConnectionError, asyncio.TimeoutError) as exc:
-            raise SonosWSConnectionError("Connection error: {exc}") from exc
+        except aiohttp.ClientConnectionError as exc:
+            raise SonosWSConnectionError(f"Connection error: {exc}") from exc
+        except asyncio.TimeoutError as exc:
+            raise SonosWSConnectionError("Connection timed out") from exc
         except Exception as exc:  # pylint: disable=broad-except
             raise SonosWSConnectionError(f"Unknown error: {exc}") from exc
+        _LOGGER.debug("Successfully connected to %s", self.uri)
 
     async def close(self):
         """Close the websocket connection."""
         if self.ws and not self.ws.closed:
             await self.ws.close()
         if self._own_session and self.session and not self.session.closed:
             await self.session.close()
 
     async def send_command(
         self, command: dict[str, Any], options: dict[str, Any] | None = None
     ) -> list[dict[str, Any]]:
         """Send commands over the websocket and handle their responses."""
-        if not self.ws or self.ws.closed:
-            await self.connect()
-            assert self.ws
-
-        payload = [command, options or {}]
-        _LOGGER.debug("Sending command: %s", payload)
-        await self.ws.send_json(payload)
-        response = await self.ws.receive_json()
-        _LOGGER.debug("Response: %s", response)
-        return response
+        attempt = 1
+        while attempt <= MAX_ATTEMPTS:
+            if not self.ws or self.ws.closed:
+                _LOGGER.debug("Websocket not available, reconnecting")
+                await self.connect()
+                assert self.ws
+
+            payload = [command, options or {}]
+            _LOGGER.debug("Sending command: %s", payload)
+            try:
+                async with asyncio_timeout(3):
+                    await self.ws.send_json(payload)
+                    return await self.ws.receive_json()
+            except asyncio.TimeoutError:
+                _LOGGER.error("Command timed out")
+            except TypeError as exc:
+                _LOGGER.error("Bad response received: %s", exc)
+            attempt += 1
+
+        command_name = command.get("command", "Empty")
+        raise SonosWebsocketError(
+            f"{command_name} command failed after {MAX_ATTEMPTS} attempts"
+        )
 
     async def play_clip(
         self, uri: str, volume: int | None = None
     ) -> list[dict[str, Any]]:
         """Play an audio clip."""
         command = {
             "namespace": "audioClip:1",
```

### Comparing `sonos-websocket-0.0.4/sonos_websocket.egg-info/PKG-INFO` & `sonos-websocket-0.0.5/sonos_websocket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.4
+Version: 0.0.5
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

