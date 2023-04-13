# Comparing `tmp/python_roborock-0.6.4.tar.gz` & `tmp/python_roborock-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.4.tar", max compression
+gzip compressed data, was "python_roborock-0.6.5.tar", max compression
```

## Comparing `python_roborock-0.6.4.tar` & `python_roborock-0.6.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-11 16:29:11.922855 python_roborock-0.6.4/LICENSE
--rw-r--r--   0        0        0     2221 2023-04-11 16:29:11.922855 python_roborock-0.6.4/README.md
--rw-r--r--   0        0        0     1152 2023-04-11 16:29:12.738876 python_roborock-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/__init__.py
--rw-r--r--   0        0        0    17099 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/api.py
--rw-r--r--   0        0        0     3957 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/cli.py
--rw-r--r--   0        0        0     8276 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/cloud_api.py
--rw-r--r--   0        0        0     3703 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/code_mappings.py
--rw-r--r--   0        0        0     9190 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/containers.py
--rw-r--r--   0        0        0     1022 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/exceptions.py
--rw-r--r--   0        0        0     7066 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/local_api.py
--rw-r--r--   0        0        0     1194 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/offline/offline.py
--rw-r--r--   0        0        0     6030 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12709 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/typing.py
--rw-r--r--   0        0        0      809 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/util.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 17:45:45.491427 python_roborock-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-13 17:45:45.491427 python_roborock-0.6.5/README.md
+-rw-r--r--   0        0        0     1370 2023-04-13 17:45:46.427436 python_roborock-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/__init__.py
+-rw-r--r--   0        0        0    18886 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/cli.py
+-rw-r--r--   0        0        0     8595 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9404 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/exceptions.py
+-rw-r--r--   0        0        0     7217 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/local_api.py
+-rw-r--r--   0        0        0     6108 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/roborock_message.py
+-rw-r--r--   0        0        0      644 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/roborock_queue.py
+-rw-r--r--   0        0        0    12762 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/typing.py
+-rw-r--r--   0        0        0      868 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.5/PKG-INFO
```

### Comparing `python_roborock-0.6.4/LICENSE` & `python_roborock-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.4/README.md` & `python_roborock-0.6.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,86 @@
-# Roborock
-
-<p align="center">
-  <a href="https://pypi.org/project/python-roborock/">
-    <img src="https://img.shields.io/pypi/v/python-roborock.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
-  </a>
-  <img src="https://img.shields.io/pypi/pyversions/python-roborock.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
-  <img src="https://img.shields.io/pypi/l/python-roborock.svg?style=flat-square" alt="License">
-</p>
-
-Roborock library for online and offline control of your vacuums.
-
-## Installation
-
-Install this via pip (or your favourite package manager):
-
-`pip install python-roborock`
-
-## Functionality
-
-This package can encrypt and decrypt the following commands:
-    
-- GET_CLEAN_RECORD
-- GET_CONSUMABLE
-- GET_MULTI_MAPS_LIST
-- APP_START
-- APP_PAUSE
-- APP_STOP
-- APP_CHARGE
-- APP_SPOT
-- FIND_ME
-- RESUME_ZONED_CLEAN
-- RESUME_SEGMENT_CLEAN 
-- SET_CUSTOM_MODE
-- SET_MOP_MODE
-- SET_WATER_BOX_CUSTOM_MODE
-- RESET_CONSUMABLE
-- LOAD_MULTI_MAP
-- APP_RC_START
-- APP_RC_END
-- APP_RC_MOVE
-- APP_GOTO_TARGET
-- APP_SEGMENT_CLEAN
-- APP_ZONED_CLEAN
-- APP_GET_DRYER_SETTING
-- APP_SET_DRYER_SETTING
-- APP_START_WASH
-- APP_STOP_WASH
-- GET_DUST_COLLECTION_MODE
-- SET_DUST_COLLECTION_MODE
-- GET_SMART_WASH_PARAMS
-- SET_SMART_WASH_PARAMS
-- GET_WASH_TOWEL_MODE
-- SET_WASH_TOWEL_MODE
-- SET_CHILD_LOCK_STATUS
-- GET_CHILD_LOCK_STATUS
-- START_WASH_THEN_CHARGE
-- GET_CURRENT_SOUND
-- GET_SERIAL_NUMBER
-- GET_TIMEZONE
-- GET_SERVER_TIMER
-- GET_CUSTOMIZE_CLEAN_MODE
-- GET_CLEAN_SEQUENCE
-- SET_FDS_ENDPOINT
-- ENABLE_LOG_UPLOAD
-- APP_WAKEUP_ROBOT
-- GET_LED_STATUS
-- GET_FLOW_LED_STATUS
-- SET_FLOW_LED_STATUS
-- GET_SOUND_PROGRESS
-- GET_SOUND_VOLUME
-- TEST_SOUND_VOLUME
-- CHANGE_SOUND_VOLUME
-- GET_CARPET_MODE
-- SET_CARPET_MODE
-- GET_CARPET_CLEAN_MODE
-- SET_CARPET_CLEAN_MODE
-- UPD_SERVER_TIMER
-- SET_SERVER_TIMER
-- APP_GET_INIT_STATUS
-- SET_APP_TIMEZONE
-- GET_NETWORK_INFO
-
-
-
-## Credits
-
-Thanks @rovo89 for https://gist.github.com/rovo89/dff47ed19fca0dfdda77503e66c2b7c7 And thanks @PiotrMachowski for https://github.com/PiotrMachowski/Home-Assistant-custom-components-Xiaomi-Cloud-Map-Extractor
-
-
+# Roborock
+
+<p align="center">
+  <a href="https://pypi.org/project/python-roborock/">
+    <img src="https://img.shields.io/pypi/v/python-roborock.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/python-roborock.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/python-roborock.svg?style=flat-square" alt="License">
+</p>
+
+Roborock library for online and offline control of your vacuums.
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install python-roborock`
+
+## Functionality
+
+This package can encrypt and decrypt the following commands:
+
+- GET_CLEAN_RECORD
+- GET_CONSUMABLE
+- GET_MULTI_MAPS_LIST
+- APP_START
+- APP_PAUSE
+- APP_STOP
+- APP_CHARGE
+- APP_SPOT
+- FIND_ME
+- RESUME_ZONED_CLEAN
+- RESUME_SEGMENT_CLEAN
+- SET_CUSTOM_MODE
+- SET_MOP_MODE
+- SET_WATER_BOX_CUSTOM_MODE
+- RESET_CONSUMABLE
+- LOAD_MULTI_MAP
+- APP_RC_START
+- APP_RC_END
+- APP_RC_MOVE
+- APP_GOTO_TARGET
+- APP_SEGMENT_CLEAN
+- APP_ZONED_CLEAN
+- APP_GET_DRYER_SETTING
+- APP_SET_DRYER_SETTING
+- APP_START_WASH
+- APP_STOP_WASH
+- GET_DUST_COLLECTION_MODE
+- SET_DUST_COLLECTION_MODE
+- GET_SMART_WASH_PARAMS
+- SET_SMART_WASH_PARAMS
+- GET_WASH_TOWEL_MODE
+- SET_WASH_TOWEL_MODE
+- SET_CHILD_LOCK_STATUS
+- GET_CHILD_LOCK_STATUS
+- START_WASH_THEN_CHARGE
+- GET_CURRENT_SOUND
+- GET_SERIAL_NUMBER
+- GET_TIMEZONE
+- GET_SERVER_TIMER
+- GET_CUSTOMIZE_CLEAN_MODE
+- GET_CLEAN_SEQUENCE
+- SET_FDS_ENDPOINT
+- ENABLE_LOG_UPLOAD
+- APP_WAKEUP_ROBOT
+- GET_LED_STATUS
+- GET_FLOW_LED_STATUS
+- SET_FLOW_LED_STATUS
+- GET_SOUND_PROGRESS
+- GET_SOUND_VOLUME
+- TEST_SOUND_VOLUME
+- CHANGE_SOUND_VOLUME
+- GET_CARPET_MODE
+- SET_CARPET_MODE
+- GET_CARPET_CLEAN_MODE
+- SET_CARPET_CLEAN_MODE
+- UPD_SERVER_TIMER
+- SET_SERVER_TIMER
+- APP_GET_INIT_STATUS
+- SET_APP_TIMEZONE
+- GET_NETWORK_INFO
+
+## Credits
+
+Thanks @rovo89 for https://gist.github.com/rovo89/dff47ed19fca0dfdda77503e66c2b7c7 And thanks @PiotrMachowski for https://github.com/PiotrMachowski/Home-Assistant-custom-components-Xiaomi-Cloud-Map-Extractor
```

### Comparing `python_roborock-0.6.4/pyproject.toml` & `python_roborock-0.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.4"
+version = "0.6.5"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -32,12 +32,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 pytest-asyncio = "*"
 pytest = "*"
+pre-commit = "*"
+mypy = "*"
+ruff = "*"
+isort = "*"
+black = "*"
+codespell = "*"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 build_command = "pip install poetry && poetry build"
+
+[tool.ruff]
+ignore = ["F403", "E741"]
+line-length = 120
+
+[tool.black]
+line-length = 120
+
+[tool.isort]
+profile = "black"
+line_length = 120
```

### Comparing `python_roborock-0.6.4/roborock/api.py` & `python_roborock-0.6.5/roborock/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,47 +10,41 @@
 import json
 import logging
 import math
 import secrets
 import struct
 import time
 from random import randint
-from typing import Any, Callable
+from typing import Any, Callable, Coroutine, Mapping, Optional
 
 import aiohttp
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import unpad
 
-from roborock.exceptions import (
-    RoborockException, RoborockTimeout, VacuumError,
-)
-from .code_mappings import RoborockDockTypeCode
+from roborock.exceptions import RoborockException, RoborockTimeout, VacuumError
+
+from .code_mappings import RoborockDockTypeCode, RoborockEnum
 from .containers import (
-    UserData,
-    Status,
+    CleanRecord,
     CleanSummary,
     Consumable,
     DNDTimer,
-    CleanRecord,
+    DustCollectionMode,
     HomeData,
     MultiMapsList,
-    SmartWashParams,
+    NetworkInfo,
     RoborockDeviceInfo,
+    SmartWashParams,
+    Status,
+    UserData,
     WashTowelMode,
-    DustCollectionMode,
-    NetworkInfo,
-
 )
 from .roborock_message import RoborockMessage
 from .roborock_queue import RoborockQueue
-from .typing import (
-    RoborockDeviceProp,
-    RoborockCommand,
-    RoborockDockSummary
-)
+from .typing import RoborockCommand, RoborockDeviceProp, RoborockDockSummary
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
 MQTT_KEEPALIVE = 60
 SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
@@ -59,37 +53,34 @@
 def md5hex(message: str) -> str:
     md5 = hashlib.md5()
     md5.update(message.encode())
     return md5.hexdigest()
 
 
 class PreparedRequest:
-    def __init__(self, base_url: str, base_headers: dict = None) -> None:
+    def __init__(self, base_url: str, base_headers: Optional[dict] = None) -> None:
         self.base_url = base_url
         self.base_headers = base_headers or {}
 
-    async def request(
-            self, method: str, url: str, params=None, data=None, headers=None
-    ) -> dict | list:
+    async def request(self, method: str, url: str, params=None, data=None, headers=None) -> dict:
         _url = "/".join(s.strip("/") for s in [self.base_url, url])
         _headers = {**self.base_headers, **(headers or {})}
         async with aiohttp.ClientSession() as session:
             async with session.request(
-                    method,
-                    _url,
-                    params=params,
-                    data=data,
-                    headers=_headers,
+                method,
+                _url,
+                params=params,
+                data=data,
+                headers=_headers,
             ) as resp:
                 return await resp.json()
 
 
 class RoborockClient:
-
-    def __init__(self, endpoint: str, devices_info: dict[str, RoborockDeviceInfo]) -> None:
+    def __init__(self, endpoint: str, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
         self.devices_info = devices_info
         self._endpoint = endpoint
         self._nonce = secrets.token_bytes(16)
         self._waiting_queue: dict[int, RoborockQueue] = {}
         self._status_listeners: list[Callable[[int, str], None]] = []
 
     def add_status_listener(self, callback: Callable[[int, str], None]):
@@ -113,35 +104,32 @@
                                 if queue.protocol == protocol:
                                     error = data_point_response.get("error")
                                     if error:
                                         await queue.async_put(
                                             (
                                                 None,
                                                 VacuumError(
-                                                    error.get("code"), error.get("message")
+                                                    error.get("code"),
+                                                    error.get("message"),
                                                 ),
                                             ),
                                             timeout=QUEUE_TIMEOUT,
                                         )
                                     else:
                                         result = data_point_response.get("result")
                                         if isinstance(result, list) and len(result) == 1:
                                             result = result[0]
-                                        await queue.async_put(
-                                            (result, None), timeout=QUEUE_TIMEOUT
-                                        )
+                                        await queue.async_put((result, None), timeout=QUEUE_TIMEOUT)
                 elif protocol == 301:
                     payload = data.payload[0:24]
                     [endpoint, _, request_id, _] = struct.unpack("<15sBH6s", payload)
                     if endpoint.decode().startswith(self._endpoint):
                         iv = bytes(AES.block_size)
                         decipher = AES.new(self._nonce, AES.MODE_CBC, iv)
-                        decrypted = unpad(
-                            decipher.decrypt(data.payload[24:]), AES.block_size
-                        )
+                        decrypted = unpad(decipher.decrypt(data.payload[24:]), AES.block_size)
                         decrypted = gzip.decompress(decrypted)
                         queue = self._waiting_queue.get(request_id)
                         if queue:
                             if isinstance(decrypted, list):
                                 decrypted = decrypted[0]
                             await queue.async_put((decrypted, None), timeout=QUEUE_TIMEOUT)
         except Exception as ex:
@@ -150,23 +138,19 @@
     async def _async_response(self, request_id: int, protocol_id: int = 0) -> tuple[Any, VacuumError | None]:
         try:
             queue = RoborockQueue(protocol_id)
             self._waiting_queue[request_id] = queue
             (response, err) = await queue.async_get(QUEUE_TIMEOUT)
             return response, err
         except (asyncio.TimeoutError, asyncio.CancelledError):
-            raise RoborockTimeout(
-                f"Timeout after {QUEUE_TIMEOUT} seconds waiting for response"
-            ) from None
+            raise RoborockTimeout(f"Timeout after {QUEUE_TIMEOUT} seconds waiting for response") from None
         finally:
             del self._waiting_queue[request_id]
 
-    def _get_payload(
-            self, method: RoborockCommand, params: list = None, secured=False
-    ):
+    def _get_payload(self, method: RoborockCommand, params: Optional[list] = None, secured=False):
         timestamp = math.floor(time.time())
         request_id = randint(10000, 99999)
         inner = {
             "id": request_id,
             "method": method,
             "params": params or [],
         }
@@ -182,144 +166,159 @@
                     "t": timestamp,
                 },
                 separators=(",", ":"),
             ).encode()
         )
         return request_id, timestamp, payload
 
-    async def send_command(
-            self, device_id: str, method: RoborockCommand, params: list = None
-    ):
+    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
         raise NotImplementedError
 
-    async def get_status(self, device_id: str) -> Status:
+    async def get_status(self, device_id: str) -> Status | None:
         status = await self.send_command(device_id, RoborockCommand.GET_STATUS)
         if isinstance(status, dict):
             return Status.from_dict(status)
+        return None
 
-    async def get_dnd_timer(self, device_id: str) -> DNDTimer:
+    async def get_dnd_timer(self, device_id: str) -> DNDTimer | None:
         try:
             dnd_timer = await self.send_command(device_id, RoborockCommand.GET_DND_TIMER)
             if isinstance(dnd_timer, dict):
                 return DNDTimer.from_dict(dnd_timer)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_clean_summary(self, device_id: str) -> CleanSummary:
+    async def get_clean_summary(self, device_id: str) -> CleanSummary | None:
         try:
-            clean_summary = await self.send_command(
-                device_id, RoborockCommand.GET_CLEAN_SUMMARY
-            )
+            clean_summary = await self.send_command(device_id, RoborockCommand.GET_CLEAN_SUMMARY)
             if isinstance(clean_summary, dict):
                 return CleanSummary.from_dict(clean_summary)
             elif isinstance(clean_summary, bytes):
-                return CleanSummary(clean_time=int.from_bytes(clean_summary, 'big'))
+                return CleanSummary(clean_time=int.from_bytes(clean_summary, "big"))
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_clean_record(self, device_id: str, record_id: int) -> CleanRecord:
+    async def get_clean_record(self, device_id: str, record_id: int) -> CleanRecord | None:
         try:
-            clean_record = await self.send_command(
-                device_id, RoborockCommand.GET_CLEAN_RECORD, [record_id]
-            )
+            clean_record = await self.send_command(device_id, RoborockCommand.GET_CLEAN_RECORD, [record_id])
             if isinstance(clean_record, dict):
                 return CleanRecord.from_dict(clean_record)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_consumable(self, device_id: str) -> Consumable:
+    async def get_consumable(self, device_id: str) -> Consumable | None:
         try:
             consumable = await self.send_command(device_id, RoborockCommand.GET_CONSUMABLE)
             if isinstance(consumable, dict):
                 return Consumable.from_dict(consumable)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_wash_towel_mode(self, device_id: str) -> WashTowelMode:
+    async def get_wash_towel_mode(self, device_id: str) -> WashTowelMode | None:
         try:
             washing_mode = await self.send_command(device_id, RoborockCommand.GET_WASH_TOWEL_MODE)
             if isinstance(washing_mode, dict):
                 return WashTowelMode.from_dict(washing_mode)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_dust_collection_mode(self, device_id: str) -> DustCollectionMode:
+    async def get_dust_collection_mode(self, device_id: str) -> DustCollectionMode | None:
         try:
             dust_collection = await self.send_command(device_id, RoborockCommand.GET_DUST_COLLECTION_MODE)
             if isinstance(dust_collection, dict):
                 return DustCollectionMode.from_dict(dust_collection)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_smart_wash_params(self, device_id: str) -> SmartWashParams:
+    async def get_smart_wash_params(self, device_id: str) -> SmartWashParams | None:
         try:
             mop_wash_mode = await self.send_command(device_id, RoborockCommand.GET_SMART_WASH_PARAMS)
             if isinstance(mop_wash_mode, dict):
                 return SmartWashParams.from_dict(mop_wash_mode)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_dock_summary(self, device_id: str, dock_type: RoborockDockTypeCode) -> RoborockDockSummary:
-        try:
-            commands = [self.get_dust_collection_mode(device_id)]
-            if dock_type == RoborockDockTypeCode['3']:
-                commands += [self.get_wash_towel_mode(device_id), self.get_smart_wash_params(device_id)]
-            [
-                dust_collection_mode,
-                wash_towel_mode,
-                smart_wash_params
-            ] = (
-                        list(await asyncio.gather(*commands))
-                        + [None, None]
-                )[:3]
+    async def get_dock_summary(self, device_id: str, dock_type: RoborockEnum) -> RoborockDockSummary | None:
+        """Gets the status summary from the dock with the methods available for a given dock.
+
+        :param dock_type: RoborockDockTypeCode"""
+        if RoborockDockTypeCode.name != "RoborockDockTypeCode":
+            raise RoborockException("Invalid enum given for dock type")
+        try:
+            commands: list[
+                Coroutine[
+                    Any,
+                    Any,
+                    DustCollectionMode | WashTowelMode | SmartWashParams | None,
+                ]
+            ] = [self.get_dust_collection_mode(device_id)]
+            if dock_type == RoborockDockTypeCode["3"]:
+                commands += [
+                    self.get_wash_towel_mode(device_id),
+                    self.get_smart_wash_params(device_id),
+                ]
+            [dust_collection_mode, wash_towel_mode, smart_wash_params] = (
+                list(await asyncio.gather(*commands)) + [None, None]
+            )[:3]
 
             return RoborockDockSummary(dust_collection_mode, wash_towel_mode, smart_wash_params)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
     async def get_prop(self, device_id: str) -> RoborockDeviceProp | None:
         [status, dnd_timer, clean_summary, consumable] = await asyncio.gather(
             *[
                 self.get_status(device_id),
                 self.get_dnd_timer(device_id),
                 self.get_clean_summary(device_id),
                 self.get_consumable(device_id),
             ]
         )
         last_clean_record = None
         if clean_summary and clean_summary.records and len(clean_summary.records) > 0:
-            last_clean_record = await self.get_clean_record(
-                device_id, clean_summary.records[0]
-            )
+            last_clean_record = await self.get_clean_record(device_id, clean_summary.records[0])
         dock_summary = None
-        if status and status.dock_type != RoborockDockTypeCode['0']:
+        if status and status.dock_type != RoborockDockTypeCode["0"]:
             dock_summary = await self.get_dock_summary(device_id, status.dock_type)
         if any([status, dnd_timer, clean_summary, consumable]):
             return RoborockDeviceProp(
-                status, dnd_timer, clean_summary, consumable, last_clean_record, dock_summary
+                status,
+                dnd_timer,
+                clean_summary,
+                consumable,
+                last_clean_record,
+                dock_summary,
             )
         return None
 
-    async def get_multi_maps_list(self, device_id) -> MultiMapsList:
+    async def get_multi_maps_list(self, device_id) -> MultiMapsList | None:
         try:
-            multi_maps_list = await self.send_command(
-                device_id, RoborockCommand.GET_MULTI_MAPS_LIST
-            )
+            multi_maps_list = await self.send_command(device_id, RoborockCommand.GET_MULTI_MAPS_LIST)
             if isinstance(multi_maps_list, dict):
                 return MultiMapsList.from_dict(multi_maps_list)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
-    async def get_networking(self, device_id) -> NetworkInfo:
+    async def get_networking(self, device_id) -> NetworkInfo | None:
         try:
             networking_info = await self.send_command(device_id, RoborockCommand.GET_NETWORK_INFO)
             if isinstance(networking_info, dict):
                 return NetworkInfo.from_dict(networking_info)
         except RoborockTimeout as e:
             _LOGGER.error(e)
+        return None
 
 
 class RoborockApiClient:
     def __init__(self, username: str, base_url=None) -> None:
         """Sample API Client."""
         self._username = username
         self._default_url = "https://euiot.roborock.com"
@@ -330,17 +329,22 @@
         if not self.base_url:
             url_request = PreparedRequest(self._default_url)
             response = await url_request.request(
                 "post",
                 "/api/v1/getUrlByEmail",
                 params={"email": self._username, "needtwostepauth": "false"},
             )
+            if response is None:
+                raise RoborockException("get url by email returned None")
             if response.get("code") != 200:
                 raise RoborockException(response.get("error"))
-            self.base_url = response.get("data").get("url")
+            response_data = response.get("data")
+            if response_data is None:
+                raise RoborockException("response does not have 'data'")
+            self.base_url = response_data.get("url")
         return self.base_url
 
     def _get_header_client_id(self):
         md5 = hashlib.md5()
         md5.update(self._username.encode())
         md5.update(self._device_identifier.encode())
         return base64.b64encode(md5.digest()).decode()
@@ -354,15 +358,16 @@
             "post",
             "/api/v1/sendEmailCode",
             params={
                 "username": self._username,
                 "type": "auth",
             },
         )
-
+        if code_response is None:
+            raise RoborockException("Failed to get a response from send email code")
         if code_response.get("code") != 200:
             raise RoborockException(code_response.get("msg"))
 
     async def pass_login(self, password: str) -> UserData:
         base_url = await self._get_base_url()
         header_clientid = self._get_header_client_id()
 
@@ -372,18 +377,22 @@
             "/api/v1/login",
             params={
                 "username": self._username,
                 "password": password,
                 "needtwostepauth": "false",
             },
         )
-
+        if login_response is None:
+            raise RoborockException("Login response is none")
         if login_response.get("code") != 200:
             raise RoborockException(login_response.get("msg"))
-        return UserData.from_dict(login_response.get("data"))
+        user_data = login_response.get("data")
+        if not isinstance(user_data, dict):
+            raise RoborockException("Got unexpected data type for user_data")
+        return UserData.from_dict(user_data)
 
     async def code_login(self, code) -> UserData:
         base_url = await self._get_base_url()
         header_clientid = self._get_header_client_id()
 
         login_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
         login_response = await login_request.request(
@@ -391,55 +400,65 @@
             "/api/v1/loginWithCode",
             params={
                 "username": self._username,
                 "verifycode": code,
                 "verifycodetype": "AUTH_EMAIL_CODE",
             },
         )
-
+        if login_response is None:
+            raise RoborockException("Login request response is None")
         if login_response.get("code") != 200:
             raise RoborockException(login_response.get("msg"))
-        return UserData.from_dict(login_response.get("data"))
+        user_data = login_response.get("data")
+        if not isinstance(user_data, dict):
+            raise RoborockException("Got unexpected data type for user_data")
+        return UserData.from_dict(user_data)
 
     async def get_home_data(self, user_data: UserData) -> HomeData:
         base_url = await self._get_base_url()
         header_clientid = self._get_header_client_id()
         rriot = user_data.rriot
-        home_id_request = PreparedRequest(
-            base_url, {"header_clientid": header_clientid}
-        )
+        if rriot is None:
+            raise RoborockException("rriot is none")
+        home_id_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
         home_id_response = await home_id_request.request(
             "get",
             "/api/v1/getHomeDetail",
             headers={"Authorization": user_data.token},
         )
+        if home_id_response is None:
+            raise RoborockException("home_id_response is None")
         if home_id_response.get("code") != 200:
             raise RoborockException(home_id_response.get("msg"))
-        home_id = home_id_response.get("data").get("rrHomeId")
+
+        home_id = home_id_response["data"].get("rrHomeId")
         timestamp = math.floor(time.time())
         nonce = secrets.token_urlsafe(6)
         prestr = ":".join(
             [
                 rriot.u,
                 rriot.s,
                 nonce,
                 str(timestamp),
                 hashlib.md5(("/user/homes/" + str(home_id)).encode()).hexdigest(),
                 "",
                 "",
             ]
         )
-        mac = base64.b64encode(
-            hmac.new(rriot.h.encode(), prestr.encode(), hashlib.sha256).digest()
-        ).decode()
+        mac = base64.b64encode(hmac.new(rriot.h.encode(), prestr.encode(), hashlib.sha256).digest()).decode()
+        if rriot.r.a is None:
+            raise RoborockException("Missing field 'a' in rriot reference")
         home_request = PreparedRequest(
             rriot.r.a,
             {
                 "Authorization": f'Hawk id="{rriot.u}", s="{rriot.s}", ts="{timestamp}", nonce="{nonce}", '
-                                 f'mac="{mac}"',
+                f'mac="{mac}"',
             },
         )
         home_response = await home_request.request("get", "/user/homes/" + str(home_id))
         if not home_response.get("success"):
             raise RoborockException(home_response)
         home_data = home_response.get("result")
-        return HomeData.from_dict(home_data)
+        if isinstance(home_data, dict):
+            return HomeData.from_dict(home_data)
+        else:
+            raise RoborockException("home_response result was an unexpected type")
```

### Comparing `python_roborock-0.6.4/roborock/cli.py` & `python_roborock-0.6.5/roborock/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import logging
 from pathlib import Path
 from typing import Any, Dict
 
 import click
 
@@ -12,29 +14,29 @@
 from roborock.util import run_sync
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RoborockContext:
     roborock_file = Path("~/.roborock").expanduser()
-    _login_data: LoginData = None
+    _login_data: LoginData | None = None
 
     def __init__(self):
         self.reload()
 
     def reload(self):
         if self.roborock_file.is_file():
-            with open(self.roborock_file, 'r') as f:
+            with open(self.roborock_file, "r") as f:
                 data = json.load(f)
                 if data:
                     self._login_data = LoginData.from_dict(data)
 
     def update(self, login_data: LoginData):
         data = json.dumps(login_data.as_dict(), default=vars)
-        with open(self.roborock_file, 'w') as f:
+        with open(self.roborock_file, "w") as f:
             f.write(data)
         self.reload()
 
     def validate(self):
         if self._login_data is None:
             raise RoborockException("You must login first")
 
@@ -44,17 +46,15 @@
 
 
 @click.option("-d", "--debug", default=False, count=True)
 @click.version_option(package_name="python-roborock")
 @click.group()
 @click.pass_context
 def cli(ctx, debug: int):
-    logging_config: Dict[str, Any] = {
-        "level": logging.DEBUG if debug > 0 else logging.INFO
-    }
+    logging_config: Dict[str, Any] = {"level": logging.DEBUG if debug > 0 else logging.INFO}
     logging.basicConfig(**logging_config)  # type: ignore
     ctx.obj = RoborockContext()
 
 
 @click.command()
 @click.option("--email", required=True)
 @click.option("--password", required=True)
@@ -77,15 +77,16 @@
 async def _discover(ctx):
     context: RoborockContext = ctx.obj
     login_data = context.login_data()
     client = RoborockApiClient(login_data.email)
     home_data = await client.get_home_data(login_data.user_data)
     context.update(LoginData({**login_data, "home_data": home_data}))
     click.echo(
-        f"Discovered devices {', '.join([device.name for device in home_data.devices + home_data.received_devices])}")
+        f"Discovered devices {', '.join([device.name for device in home_data.devices + home_data.received_devices])}"
+    )
 
 
 @click.command()
 @click.pass_context
 @run_sync()
 async def discover(ctx):
     await _discover(ctx)
```

### Comparing `python_roborock-0.6.4/roborock/cloud_api.py` & `python_roborock-0.6.5/roborock/cloud_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from __future__ import annotations
 
 import base64
 import logging
 import threading
 import uuid
 from asyncio import Lock
-from typing import Any
+from typing import Any, Mapping, Optional
 from urllib.parse import urlparse
 
 import paho.mqtt.client as mqtt
 
-from roborock.api import md5hex, RoborockClient, SPECIAL_COMMANDS
-from roborock.exceptions import (
-    RoborockException,
-    CommandVacuumError,
-    VacuumError,
-)
-from .containers import (
-    UserData,
-    RoborockDeviceInfo,
-)
-from .roborock_message import RoborockParser, md5bin, RoborockMessage
+from roborock.api import SPECIAL_COMMANDS, RoborockClient, md5hex
+from roborock.exceptions import CommandVacuumError, RoborockException, VacuumError
+
+from .containers import RoborockDeviceInfo, UserData
+from .roborock_message import RoborockMessage, RoborockParser, md5bin
 from .roborock_queue import RoborockQueue
 from .typing import RoborockCommand
 from .util import run_in_executor
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
 MQTT_KEEPALIVE = 60
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
 
-    def __init__(self, user_data: UserData, devices_info: dict[str, RoborockDeviceInfo]) -> None:
+    def __init__(self, user_data: UserData, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
         rriot = user_data.rriot
+        if rriot is None:
+            raise RoborockException("Got no rriot data from user_data")
         endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
         RoborockClient.__init__(self, endpoint, devices_info)
         mqtt.Client.__init__(self, protocol=mqtt.MQTTv5)
         self._mqtt_user = rriot.u
         self._hashed_user = md5hex(self._mqtt_user + ":" + rriot.k)[2:10]
         url = urlparse(rriot.r.m)
+        if not isinstance(url.hostname, str):
+            raise RoborockException("Url parsing returned an invalid hostname")
         self._mqtt_host = url.hostname
         self._mqtt_port = url.port
         self._mqtt_ssl = url.scheme == "ssl"
         if self._mqtt_ssl:
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
@@ -62,28 +60,24 @@
     @run_in_executor()
     async def on_connect(self, _client, _, __, rc, ___=None) -> None:
         connection_queue = self._waiting_queue.get(0)
         if rc != mqtt.MQTT_ERR_SUCCESS:
             message = f"Failed to connect (rc: {rc})"
             _LOGGER.error(message)
             if connection_queue:
-                await connection_queue.async_put(
-                    (None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT
-                )
+                await connection_queue.async_put((None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT)
             return
         _LOGGER.info(f"Connected to mqtt {self._mqtt_host}:{self._mqtt_port}")
         topic = f"rr/m/o/{self._mqtt_user}/{self._hashed_user}/#"
         (result, mid) = self.subscribe(topic)
         if result != 0:
             message = f"Failed to subscribe (rc: {result})"
             _LOGGER.error(message)
             if connection_queue:
-                await connection_queue.async_put(
-                    (None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT
-                )
+                await connection_queue.async_put((None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT)
             return
         _LOGGER.info(f"Subscribed to topic {topic}")
         if connection_queue:
             await connection_queue.async_put((True, None), timeout=QUEUE_TIMEOUT)
 
     @run_in_executor()
     async def on_message(self, _client, _, msg, __=None) -> None:
@@ -99,33 +93,36 @@
             self._last_disconnection = mqtt.time_func()
             message = f"Roborock mqtt client disconnected (rc: {rc})"
             if rc == mqtt.MQTT_ERR_PROTOCOL:
                 self.update_client_id()
             _LOGGER.warning(message)
             connection_queue = self._waiting_queue.get(1)
             if connection_queue:
-                await connection_queue.async_put(
-                    (True, None), timeout=QUEUE_TIMEOUT
-                )
+                await connection_queue.async_put((True, None), timeout=QUEUE_TIMEOUT)
         except Exception as ex:
             _LOGGER.exception(ex)
 
     def update_client_id(self):
         self._client_id = mqtt.base62(uuid.uuid4().int, padding=22)
 
     @run_in_executor()
     async def _async_check_keepalive(self) -> None:
         async with self._mutex:
             now = mqtt.time_func()
-            if now - self._last_disconnection > self._keepalive ** 2 and now - self._last_device_msg_in > self._keepalive:
+            # noinspection PyUnresolvedReferences
+            if (
+                now - self._last_disconnection > self._keepalive**2  # type: ignore[attr-defined]
+                and now - self._last_device_msg_in > self._keepalive  # type: ignore[attr-defined]
+            ):
                 self._ping_t = self._last_device_msg_in
 
     def _check_keepalive(self) -> None:
         self._async_check_keepalive()
-        super()._check_keepalive()
+        # noinspection PyUnresolvedReferences
+        super()._check_keepalive()  # type: ignore[misc]
 
     def sync_stop_loop(self) -> None:
         if self._thread:
             _LOGGER.info("Stopping mqtt loop")
             super().loop_stop()
 
     def sync_start_loop(self) -> None:
@@ -135,28 +132,26 @@
             super().loop_start()
 
     def sync_disconnect(self) -> bool:
         rc = mqtt.MQTT_ERR_AGAIN
         if self.is_connected():
             _LOGGER.info("Disconnecting from mqtt")
             rc = super().disconnect()
-            if not rc in [mqtt.MQTT_ERR_SUCCESS, mqtt.MQTT_ERR_NO_CONN]:
+            if rc not in [mqtt.MQTT_ERR_SUCCESS, mqtt.MQTT_ERR_NO_CONN]:
                 raise RoborockException(f"Failed to disconnect (rc:{rc})")
         return rc == mqtt.MQTT_ERR_SUCCESS
 
     def sync_connect(self) -> bool:
         rc = mqtt.MQTT_ERR_AGAIN
         self.sync_start_loop()
         if not self.is_connected():
+            if self._mqtt_port is None or self._mqtt_host is None:
+                raise RoborockException("Mqtt information was not entered. Cannot connect.")
             _LOGGER.info("Connecting to mqtt")
-            rc = super().connect(
-                host=self._mqtt_host,
-                port=self._mqtt_port,
-                keepalive=MQTT_KEEPALIVE
-            )
+            rc = super().connect(host=self._mqtt_host, port=self._mqtt_port, keepalive=MQTT_KEEPALIVE)
             if rc != mqtt.MQTT_ERR_SUCCESS:
                 raise RoborockException(f"Failed to connect (rc:{rc})")
         return rc == mqtt.MQTT_ERR_SUCCESS
 
     async def async_disconnect(self) -> Any:
         async with self._mutex:
             disconnecting = self.sync_disconnect()
@@ -175,42 +170,32 @@
                     raise RoborockException(err) from err
                 return response
 
     async def validate_connection(self) -> None:
         await self.async_connect()
 
     def _send_msg_raw(self, device_id, msg) -> None:
-        info = self.publish(
-            f"rr/m/i/{self._mqtt_user}/{self._hashed_user}/{device_id}", msg
-        )
+        info = self.publish(f"rr/m/i/{self._mqtt_user}/{self._hashed_user}/{device_id}", msg)
         if info.rc != mqtt.MQTT_ERR_SUCCESS:
             raise RoborockException(f"Failed to publish (rc: {info.rc})")
 
-    async def send_command(
-            self, device_id: str, method: RoborockCommand, params: list = None
-    ):
+    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
         await self.validate_connection()
         request_id, timestamp, payload = super()._get_payload(method, params, True)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         request_protocol = 101
         response_protocol = 301 if method in SPECIAL_COMMANDS else 102
-        roborock_message = RoborockMessage(
-            timestamp=timestamp,
-            protocol=request_protocol,
-            payload=payload
-        )
+        roborock_message = RoborockMessage(timestamp=timestamp, protocol=request_protocol, payload=payload)
         local_key = self.devices_info[device_id].device.local_key
         msg = RoborockParser.encode(roborock_message, local_key)
         self._send_msg_raw(device_id, msg)
         (response, err) = await self._async_response(request_id, response_protocol)
         if err:
             raise CommandVacuumError(method, err) from err
         if response_protocol == 301:
-            _LOGGER.debug(
-                f"id={request_id} Response from {method}: {len(response)} bytes"
-            )
+            _LOGGER.debug(f"id={request_id} Response from {method}: {len(response)} bytes")
         else:
             _LOGGER.debug(f"id={request_id} Response from {method}: {response}")
         return response
 
     async def get_map_v1(self, device_id):
         return await self.send_command(device_id, RoborockCommand.GET_MAP_V1)
```

### Comparing `python_roborock-0.6.4/roborock/code_mappings.py` & `python_roborock-0.6.5/roborock/code_mappings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 from __future__ import annotations
 
 from enum import Enum
+from typing import Any, Type, TypeVar
+
+_StrEnumT = TypeVar("_StrEnumT", bound="RoborockEnum")
 
 
 class RoborockEnum(str, Enum):
+    def __new__(cls: Type[_StrEnumT], value: str, *args: Any, **kwargs: Any) -> _StrEnumT:
+        """Create a new StrEnum instance."""
+        if not isinstance(value, str):
+            raise TypeError(f"{value!r} is not a string")
+        return super().__new__(cls, value, *args, **kwargs)
+
     def __str__(self):
         return str(self.value)
 
     @classmethod
-    def _missing_(cls, code: int):
+    def _missing_(cls: Type[_StrEnumT], code: object):
         return cls._member_map_.get(str(code))
 
     @classmethod
-    def as_dict(cls):
+    def as_dict(cls: Type[_StrEnumT]):
         return {int(i.name): i.value for i in cls}
 
     @classmethod
-    def values(cls):
+    def values(cls: Type[_StrEnumT]):
         return list(cls.as_dict().values())
 
     @classmethod
-    def keys(cls):
+    def keys(cls: Type[_StrEnumT]):
         return list(cls.as_dict().keys())
 
     @classmethod
-    def items(cls):
+    def items(cls: Type[_StrEnumT]):
         return cls.as_dict().items()
 
+    @classmethod
+    def __getitem__(cls: Type[_StrEnumT], item):
+        return cls.__getitem__(item)
+
 
 def create_code_enum(name: str, data: dict) -> RoborockEnum:
     return RoborockEnum(name, {str(key): value for key, value in data.items()})
 
 
 RoborockStateCode = create_code_enum(
     "RoborockStateCode",
```

### Comparing `python_roborock-0.6.4/roborock/containers.py` & `python_roborock-0.6.5/roborock/containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 from __future__ import annotations
 
 import re
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
 from enum import Enum
 from typing import Any, Optional
 
-from dacite import from_dict, Config
+from dacite import Config, from_dict
 
-from roborock.code_mappings import RoborockDockWashTowelModeCode, RoborockDockTypeCode, RoborockMopIntensityCode, \
-    RoborockStateCode
-from .code_mappings import RoborockMopModeCode, RoborockDockErrorCode, \
-    RoborockErrorCode, RoborockDockDustCollectionModeCode, RoborockFanPowerCode
+from roborock.code_mappings import (
+    RoborockDockTypeCode,
+    RoborockDockWashTowelModeCode,
+    RoborockMopIntensityCode,
+    RoborockStateCode,
+)
+
+from .code_mappings import (
+    RoborockDockDustCollectionModeCode,
+    RoborockDockErrorCode,
+    RoborockErrorCode,
+    RoborockFanPowerCode,
+    RoborockMopModeCode,
+)
 
 
 def camelize(s: str):
-    first, *others = s.split('_')
-    return ''.join([first.lower(), *map(str.title, others)])
+    first, *others = s.split("_")
+    return "".join([first.lower(), *map(str.title, others)])
 
 
 def decamelize(s: str):
-    return re.sub('([A-Z]+)', '_\\1', s).lower()
+    return re.sub("([A-Z]+)", "_\\1", s).lower()
 
 
 def decamelize_obj(d: dict | list):
     if isinstance(d, list):
         return [decamelize_obj(i) if isinstance(i, (dict, list)) else i for i in d]
     return {decamelize(a): decamelize_obj(b) if isinstance(b, (dict, list)) else b for a, b in d.items()}
 
 
 @dataclass
 class RoborockBase:
-
     @classmethod
-    def from_dict(cls, data: dict[str, any]):
+    def from_dict(cls, data: dict[str, Any]):
         return from_dict(cls, decamelize_obj(data), config=Config(cast=[Enum]))
 
     def as_dict(self):
-        return asdict(self, dict_factory=lambda _fields: {
-            camelize(key): value for (key, value) in _fields if value is not None
-        })
+        return asdict(
+            self,
+            dict_factory=lambda _fields: {camelize(key): value for (key, value) in _fields if value is not None},
+        )
 
 
 @dataclass
 class Reference(RoborockBase):
     r: Optional[str] = None
     a: Optional[str] = None
     m: Optional[str] = None
     l: Optional[str] = None
 
 
 @dataclass
 class RRiot(RoborockBase):
-    u: Optional[str] = None
-    s: Optional[str] = None
-    h: Optional[str] = None
-    k: Optional[str] = None
-    r: Optional[Reference] = None
+    u: str
+    s: str
+    h: str
+    k: str
+    r: Reference
 
 
 @dataclass
 class UserData(RoborockBase):
     uid: Optional[int] = None
     tokentype: Optional[str] = None
     token: Optional[str] = None
@@ -165,52 +175,52 @@
     email: Optional[str] = None
 
 
 @dataclass
 class Status(RoborockBase):
     msg_ver: Optional[int] = None
     msg_seq: Optional[int] = None
-    state: Optional[RoborockStateCode] = None
+    state: Optional[RoborockStateCode] = None  # type: ignore[valid-type]
     battery: Optional[int] = None
     clean_time: Optional[int] = None
     clean_area: Optional[int] = None
-    error_code: Optional[RoborockErrorCode] = None
+    error_code: Optional[RoborockErrorCode] = None  # type: ignore[valid-type]
     map_present: Optional[int] = None
     in_cleaning: Optional[int] = None
     in_returning: Optional[int] = None
     in_fresh_state: Optional[int] = None
     lab_status: Optional[int] = None
     water_box_status: Optional[int] = None
     back_type: Optional[int] = None
     wash_phase: Optional[int] = None
     wash_ready: Optional[int] = None
-    fan_power: Optional[RoborockFanPowerCode] = None
+    fan_power: Optional[RoborockFanPowerCode] = None  # type: ignore[valid-type]
     dnd_enabled: Optional[int] = None
     map_status: Optional[int] = None
     is_locating: Optional[int] = None
     lock_status: Optional[int] = None
-    water_box_mode: Optional[RoborockMopIntensityCode] = None
+    water_box_mode: Optional[RoborockMopIntensityCode] = None  # type: ignore[valid-type]
     mop_intensity: Optional[str] = None
     water_box_carriage_status: Optional[int] = None
     mop_forbidden_enable: Optional[int] = None
     camera_status: Optional[int] = None
     is_exploring: Optional[int] = None
     home_sec_status: Optional[int] = None
     home_sec_enable_password: Optional[int] = None
     adbumper_status: Optional[list[int]] = None
     water_shortage_status: Optional[int] = None
-    dock_type: Optional[RoborockDockTypeCode] = None
+    dock_type: Optional[RoborockDockTypeCode] = None  # type: ignore[valid-type]
     dust_collection_status: Optional[int] = None
     auto_dust_collection: Optional[int] = None
     avoid_count: Optional[int] = None
-    mop_mode: Optional[RoborockMopModeCode] = None
+    mop_mode: Optional[RoborockMopModeCode] = None  # type: ignore[valid-type]
     debug_mode: Optional[int] = None
     collision_avoid_status: Optional[int] = None
     switch_map_mode: Optional[int] = None
-    dock_error_status: Optional[RoborockDockErrorCode] = None
+    dock_error_status: Optional[RoborockDockErrorCode] = None  # type: ignore[valid-type]
     charge_status: Optional[int] = None
     unsave_map_reason: Optional[int] = None
     unsave_map_flag: Optional[int] = None
 
 
 @dataclass
 class DNDTimer(RoborockBase):
@@ -286,20 +296,20 @@
 class SmartWashParams(RoborockBase):
     smart_wash: Optional[int] = None
     wash_interval: Optional[int] = None
 
 
 @dataclass
 class DustCollectionMode(RoborockBase):
-    mode: Optional[RoborockDockDustCollectionModeCode] = None
+    mode: Optional[RoborockDockDustCollectionModeCode] = None  # type: ignore[valid-type]
 
 
 @dataclass
 class WashTowelMode(RoborockBase):
-    wash_mode: Optional[RoborockDockWashTowelModeCode] = None
+    wash_mode: Optional[RoborockDockWashTowelModeCode] = None  # type: ignore[valid-type]
 
 
 @dataclass
 class NetworkInfo(RoborockBase):
     ip: str
     ssid: Optional[str] = None
     mac: Optional[str] = None
```

### Comparing `python_roborock-0.6.4/roborock/exceptions.py` & `python_roborock-0.6.5/roborock/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """Roborock exceptions."""
 
+
 class RoborockException(BaseException):
     """Class for Roborock exceptions."""
 
+
 class RoborockTimeout(RoborockException):
     """Class for Roborock timeout exceptions."""
 
+
 class RoborockConnectionException(RoborockException):
     """Class for Roborock connection exceptions."""
 
+
 class RoborockBackoffException(RoborockException):
     """Class for Roborock exceptions when many retries were made."""
 
+
 class VacuumError(RoborockException):
     """Class for vacuum errors."""
+
     def __init__(self, code, message):
         self.code = code
         self.message = message
         super().__init__()
 
-    def __str__(self, *args, **kwargs): # real signature unknown
-        """ Return str(self). """
+    def __str__(self, *args, **kwargs):  # real signature unknown
+        """Return str(self)."""
         return f"{self.code}: {self.message}"
 
 
 class CommandVacuumError(RoborockException):
     """Class for command vacuum errors."""
+
     def __init__(self, command: str, vacuum_error: VacuumError):
         self.message = f"{command}: {str(vacuum_error)}"
         super().__init__(self.message)
```

### Comparing `python_roborock-0.6.4/roborock/local_api.py` & `python_roborock-0.6.5/roborock/local_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
 from asyncio import Lock
-from typing import Callable, Coroutine
+from typing import Any, Awaitable, Callable, Mapping, Optional
 
 import async_timeout
 
-from roborock.api import RoborockClient, SPECIAL_COMMANDS
+from roborock.api import SPECIAL_COMMANDS, RoborockClient
 from roborock.containers import RoborockLocalDeviceInfo
-from roborock.exceptions import RoborockTimeout, CommandVacuumError, RoborockConnectionException, RoborockException
-from roborock.roborock_message import RoborockParser, RoborockMessage
-from roborock.typing import RoborockCommand, CommandInfoMap
+from roborock.exceptions import CommandVacuumError, RoborockConnectionException, RoborockException, RoborockTimeout
+from roborock.roborock_message import RoborockMessage, RoborockParser
+from roborock.typing import CommandInfoMap, RoborockCommand
 from roborock.util import get_running_loop_or_create_one
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RoborockLocalClient(RoborockClient):
-
-    def __init__(self, devices_info: dict[str, RoborockLocalDeviceInfo]):
+    def __init__(self, devices_info: Mapping[str, RoborockLocalDeviceInfo]):
         super().__init__("abc", devices_info)
         self.loop = get_running_loop_or_create_one()
         self.device_listener: dict[str, RoborockSocketListener] = {
             device_id: RoborockSocketListener(
                 device_info.network_info.ip,
                 device_info.device.local_key,
-                self.on_message
+                self.on_message,
             )
             for device_id, device_info in devices_info.items()
         }
         self._mutex = Lock()
         self._batch_structs: list[RoborockMessage] = []
         self._executing = False
 
     async def async_connect(self):
-        await asyncio.gather(*[
-            listener.connect()
-            for listener in self.device_listener.values()
-        ])
+        await asyncio.gather(*[listener.connect() for listener in self.device_listener.values()])
 
     async def async_disconnect(self) -> None:
         await asyncio.gather(*[listener.disconnect() for listener in self.device_listener.values()])
 
-    def build_roborock_message(
-            self, method: RoborockCommand, params: list = None
-    ) -> RoborockMessage:
+    def build_roborock_message(self, method: RoborockCommand, params: Optional[list] = None) -> RoborockMessage:
         secured = True if method in SPECIAL_COMMANDS else False
         request_id, timestamp, payload = self._get_payload(method, params, secured)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         command_info = CommandInfoMap.get(method)
         if not command_info:
             raise RoborockException(f"Request {method} have unknown prefix. Can't execute in offline mode")
-        prefix = CommandInfoMap.get(method).prefix
+        command = CommandInfoMap.get(method)
+        if command is None:
+            raise RoborockException(f"No prefix found for {method}")
+        prefix = command.prefix
         request_protocol = 4
         return RoborockMessage(
             prefix=prefix,
             timestamp=timestamp,
             protocol=request_protocol,
-            payload=payload
+            payload=payload,
         )
 
-    async def send_command(
-            self, device_id: str, method: RoborockCommand, params: list = None
-    ):
+    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
         roborock_message = self.build_roborock_message(method, params)
         response = (await self.send_message(device_id, roborock_message))[0]
         if isinstance(response, BaseException):
             raise response
         return response
 
     async def async_local_response(self, roborock_message: RoborockMessage):
@@ -78,63 +73,69 @@
             response_protocol = 4
             (response, err) = await self._async_response(request_id, response_protocol)
             if err:
                 raise CommandVacuumError("", err) from err
             _LOGGER.debug(f"id={request_id} Response from {roborock_message.get_method()}: {response}")
             return response
 
-    async def send_message(
-            self, device_id: str, roborock_messages: list[RoborockMessage] | RoborockMessage
-    ):
+    async def send_message(self, device_id: str, roborock_messages: list[RoborockMessage] | RoborockMessage):
         if isinstance(roborock_messages, RoborockMessage):
             roborock_messages = [roborock_messages]
         local_key = self.devices_info[device_id].device.local_key
         msg = RoborockParser.encode(roborock_messages, local_key)
         # Send the command to the Roborock device
         listener = self.device_listener.get(device_id)
+        if listener is None:
+            raise RoborockException(f"No device listener for {device_id}")
         _LOGGER.debug(f"Requesting device with {roborock_messages}")
         await listener.send_message(msg)
 
         return await asyncio.gather(
             *[self.async_local_response(roborock_message) for roborock_message in roborock_messages],
-            return_exceptions=True)
+            return_exceptions=True,
+        )
 
 
 class RoborockSocket(socket.socket):
     _closed = None
 
     @property
     def is_closed(self):
         return self._closed
 
 
 class RoborockSocketListener:
     roborock_port = 58867
 
-    def __init__(self, ip: str, local_key: str, on_message: Callable[[list[RoborockMessage]], Coroutine[None] | None],
-                 timeout: float | int = 4):
+    def __init__(
+        self,
+        ip: str,
+        local_key: str,
+        on_message: Callable[[list[RoborockMessage]], Awaitable[Any]],
+        timeout: float | int = 4,
+    ):
         self.ip = ip
         self.local_key = local_key
         self.socket = RoborockSocket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket.setblocking(False)
         self.loop = get_running_loop_or_create_one()
         self.on_message = on_message
         self.timeout = timeout
         self.is_connected = False
         self._mutex = Lock()
-        self.remaining = b''
+        self.remaining = b""
 
     async def _main_coro(self):
         while not self.socket.is_closed:
             try:
                 message = await self.loop.sock_recv(self.socket, 4096)
                 try:
                     if self.remaining:
                         message = self.remaining + message
-                        self.remaining = b''
+                        self.remaining = b""
                     (parser_msg, remaining) = RoborockParser.decode(message, self.local_key)
                     self.remaining = remaining
                     await self.on_message(parser_msg)
                 except Exception as e:
                     _LOGGER.exception(e)
             except BrokenPipeError as e:
                 _LOGGER.exception(e)
@@ -155,23 +156,19 @@
                     raise RoborockConnectionException(f"Failed connecting to {self.ip}") from e
                 self.loop.create_task(self._main_coro())
 
     async def disconnect(self):
         self.socket.close()
         self.is_connected = False
 
-    async def send_message(self, data: bytes):
-        response = {}
+    async def send_message(self, data: bytes) -> None:
         await self.connect()
         try:
             async with self._mutex:
                 async with async_timeout.timeout(self.timeout):
                     await self.loop.sock_sendall(self.socket, data)
         except (asyncio.TimeoutError, asyncio.CancelledError):
             await self.disconnect()
-            raise RoborockTimeout(
-                f"Timeout after {self.timeout} seconds waiting for response"
-            ) from None
+            raise RoborockTimeout(f"Timeout after {self.timeout} seconds waiting for response") from None
         except BrokenPipeError as e:
             _LOGGER.exception(e)
             await self.disconnect()
-        return response
```

### Comparing `python_roborock-0.6.4/roborock/roborock_message.py` & `python_roborock-0.6.5/roborock/roborock_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 import hashlib
 import json
 import math
 import struct
 import time
 from dataclasses import dataclass
 from random import randint
-from typing import Optional
 
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
-from roborock.typing import RoborockCommand
 
 from roborock.exceptions import RoborockException
+from roborock.typing import RoborockCommand
 
 
 def md5bin(message: str) -> bytes:
     md5 = hashlib.md5()
     md5.update(message.encode())
     return md5.digest()
 
@@ -31,19 +30,19 @@
 salt = "TXdfu$jyZ#TZHsg4"
 
 
 @dataclass
 class RoborockMessage:
     protocol: int
     payload: bytes
-    seq: Optional[int] = randint(100000, 999999)
-    prefix: Optional[bytes] = b''
-    version: Optional[bytes] = b'1.0'
-    random: Optional[int] = randint(10000, 99999)
-    timestamp: Optional[int] = math.floor(time.time())
+    seq: int = randint(100000, 999999)
+    prefix: bytes = b""
+    version: bytes = b"1.0"
+    random: int = randint(10000, 99999)
+    timestamp: int = math.floor(time.time())
 
     def get_request_id(self) -> int | None:
         protocol = self.protocol
         if protocol in [4, 101, 102]:
             payload = json.loads(self.payload.decode())
             for data_point_number, data_point in payload.get("dps").items():
                 if data_point_number in ["101", "102"]:
@@ -69,21 +68,20 @@
                 if data_point_number in ["101", "102"]:
                     data_point_response = json.loads(data_point)
                     return data_point_response.get("params")
         return None
 
 
 class RoborockParser:
-
     @staticmethod
     def encode(roborock_messages: list[RoborockMessage] | RoborockMessage, local_key: str):
         if isinstance(roborock_messages, RoborockMessage):
             roborock_messages = [roborock_messages]
 
-        msg = b''
+        msg = b""
         for roborock_message in roborock_messages:
             aes_key = md5bin(encode_timestamp(roborock_message.timestamp) + local_key + salt)
             cipher = AES.new(aes_key, AES.MODE_ECB)
             payload = roborock_message.payload
             if payload:
                 payload = pad(roborock_message.payload, AES.block_size)
             encrypted = cipher.encrypt(payload)
@@ -92,84 +90,90 @@
                 f"!3sIIIHH{encrypted_len}s",
                 "1.0".encode(),
                 roborock_message.seq,
                 roborock_message.random,
                 roborock_message.timestamp,
                 roborock_message.protocol,
                 encrypted_len,
-                encrypted
+                encrypted,
             )
             if payload:
                 crc32 = binascii.crc32(_msg)
                 _msg += struct.pack("!I", crc32)
             else:
-                _msg += b'\x00\x00'
+                _msg += b"\x00\x00"
             msg += roborock_message.prefix + _msg
         return msg
 
     @staticmethod
     def decode(msg: bytes, local_key: str, index=0) -> tuple[list[RoborockMessage], bytes]:
-        prefix = None
+        prefix = b""
         original_index = index
         if len(msg) - index < 17:
             ## broken message
             return [], msg[original_index:]
 
-        if msg[index + 4:index + 7] == "1.0".encode():
-            prefix = msg[index:index + 4]
+        if msg[index + 4 : index + 7] == "1.0".encode():
+            prefix = msg[index : index + 4]
             index += 4
-        elif msg[index:index + 3] != "1.0".encode():
-            raise RoborockException(f"Unknown protocol version {msg[0:3]}")
-
+        elif msg[index : index + 3] != "1.0".encode():
+            raise RoborockException(f"Unknown protocol version {msg[0:3]!r}")
         if len(msg) - index in [17]:
-            [version, request_id, random, timestamp, protocol] = struct.unpack_from(
-                "!3sIIIH", msg, index
-            )
-            return [RoborockMessage(
-                prefix=prefix,
-                version=version,
-                seq=request_id,
-                random=random,
-                timestamp=timestamp,
-                protocol=protocol,
-                payload=b''
-            )], b''
+            [version, request_id, random, timestamp, protocol] = struct.unpack_from("!3sIIIH", msg, index)
+            return [
+                RoborockMessage(
+                    prefix=prefix,
+                    version=version,
+                    seq=request_id,
+                    random=random,
+                    timestamp=timestamp,
+                    protocol=protocol,
+                    payload=b"",
+                )
+            ], b""
 
         if len(msg) - index < 19:
             ## broken message
             return [], msg[original_index:]
 
-        [version, request_id, random, timestamp, protocol, payload_len] = struct.unpack_from(
-            "!3sIIIHH", msg, index
-        )
+        [
+            version,
+            request_id,
+            random,
+            timestamp,
+            protocol,
+            payload_len,
+        ] = struct.unpack_from("!3sIIIHH", msg, index)
         index += 19
 
         if payload_len + index + 4 > len(msg):
             ## broken message
             return [], msg[original_index:]
 
-        payload = b''
+        payload = b""
         if payload_len == 0:
             index += 2
         else:
             [payload, expected_crc32] = struct.unpack_from(f"!{payload_len}sI", msg, index)
-            crc32 = binascii.crc32(msg[index - 19: index + payload_len])
+            crc32 = binascii.crc32(msg[index - 19 : index + payload_len])
             index += 4 + payload_len
             if crc32 != expected_crc32:
                 raise RoborockException(f"Wrong CRC32 {crc32}, expected {expected_crc32}")
 
         if payload:
             aes_key = md5bin(encode_timestamp(timestamp) + local_key + salt)
             decipher = AES.new(aes_key, AES.MODE_ECB)
             payload = unpad(decipher.decrypt(payload), AES.block_size)
 
-        [structs, remaining] = RoborockParser.decode(msg, local_key, index) if index < len(msg) else ([], b'')
+        [structs, remaining] = RoborockParser.decode(msg, local_key, index) if index < len(msg) else ([], b"")
 
-        return [RoborockMessage(
-            prefix=prefix,
-            version=version,
-            seq=request_id,
-            random=random,
-            timestamp=timestamp,
-            protocol=protocol,
-            payload=payload
-        )] + structs, remaining
+        return [
+            RoborockMessage(
+                prefix=prefix,
+                version=version,
+                seq=request_id,
+                random=random,
+                timestamp=timestamp,
+                protocol=protocol,
+                payload=payload,
+            )
+        ] + structs, remaining
```

### Comparing `python_roborock-0.6.4/roborock/roborock_queue.py` & `python_roborock-0.6.5/roborock/roborock_queue.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.4/roborock/typing.py` & `python_roborock-0.6.5/roborock/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from __future__ import annotations
 
 import typing
 from dataclasses import dataclass
 from enum import Enum
 
-from .containers import Status, CleanSummary, Consumable, \
-    DNDTimer, CleanRecord, SmartWashParams, DustCollectionMode, WashTowelMode
+from .containers import (
+    CleanRecord,
+    CleanSummary,
+    Consumable,
+    DNDTimer,
+    DustCollectionMode,
+    SmartWashParams,
+    Status,
+    WashTowelMode,
+)
 
 
 class RoborockDevicePropField(str, Enum):
     STATUS = "status"
     DND_TIMER = "dnd_timer"
     CLEAN_SUMMARY = "clean_summary"
     CONSUMABLE = "consumable"
@@ -113,121 +121,125 @@
 
 @dataclass
 class CommandInfo:
     prefix: bytes
 
 
 CommandInfoMap: dict[RoborockCommand, CommandInfo] = {
-    RoborockCommand.GET_PROP: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x77'),
-    RoborockCommand.SET_CUSTOM_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_CHILD_LOCK_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.SET_WATER_BOX_CUSTOM_MODE: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_CLEAN_SEQUENCE: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_CUSTOMIZE_CLEAN_MODE: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_CARPET_CLEAN_MODE: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.SET_CAMERA_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.SET_DND_TIMER: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_FLOW_LED_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.CLOSE_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.SET_FLOW_LED_STATUS: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_CLEAN_RECORD: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_MAP_V1: CommandInfo(prefix=b'\x00\x00\x00\xc7'),
-    RoborockCommand.SET_CLEAN_MOTOR_MODE: CommandInfo(prefix=b'\x00\x00\x00\xb7'),
-    RoborockCommand.GET_CONSUMABLE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_SERVER_TIMER: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_SERIAL_NUMBER: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_CURRENT_SOUND: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.SET_LED_STATUS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_CAMERA_STATUS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_PAUSE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_CLEAN_SUMMARY: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_NETWORK_INFO: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_LED_STATUS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.CLOSE_DND_TIMER: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_WAKEUP_ROBOT: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.SET_MOP_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_DND_TIMER: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_CARPET_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.GET_TIMEZONE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.SET_CARPET_MODE: CommandInfo(prefix=b'\x00\x00\x00\xd7'),
-    RoborockCommand.GET_MULTI_MAP: CommandInfo(prefix=b'\x00\x00\x00\xd7'),
-    RoborockCommand.SET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SET_CARPET_CLEAN_MODE: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.GET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SWITCH_WATER_MARK: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.SET_CHILD_LOCK_STATUS: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.GET_CLEAN_RECORD_MAP: CommandInfo(prefix=b'\x00\x00\xe7'),
-    RoborockCommand.APP_START: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_STOP: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_CHARGE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_SPOT: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.FIND_ME: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.RESUME_ZONED_CLEAN: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.RESUME_SEGMENT_CLEAN: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.RESET_CONSUMABLE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.LOAD_MULTI_MAP: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_RC_START: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_RC_END: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_RC_MOVE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_GOTO_TARGET: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.APP_SEGMENT_CLEAN: CommandInfo(prefix=b'\x00\x00\x00\xc7'),
-    RoborockCommand.APP_ZONED_CLEAN: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_START_WASH: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.APP_STOP_WASH: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.SET_FDS_ENDPOINT: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.ENABLE_LOG_UPLOAD: CommandInfo(prefix=b'\x00\x00\x87'),
-    RoborockCommand.GET_SOUND_VOLUME: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.TEST_SOUND_VOLUME: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.UPD_SERVER_TIMER: CommandInfo(prefix=b'\x00\x00\x00\x97'),
-    RoborockCommand.SET_APP_TIMEZONE: CommandInfo(prefix=b'\x00\x00\x97'),
-    RoborockCommand.CHANGE_SOUND_VOLUME: CommandInfo(prefix=b'\x00\x00\x00\x87'),
-    RoborockCommand.GET_SOUND_PROGRESS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.SET_SERVER_TIMER: CommandInfo(prefix=b'\x00\x00\x00\xc7'),
-    RoborockCommand.GET_ROOM_MAPPING: CommandInfo(prefix=b'\x00\x00\x00w'),
-    RoborockCommand.NAME_SEGMENT: CommandInfo(prefix=b'\x00\x00\x027'),
-    RoborockCommand.SET_TIMEZONE: CommandInfo(prefix=b'\x00\x00\x00\x97')
+    RoborockCommand.GET_PROP: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x77"),
+    RoborockCommand.SET_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_WATER_BOX_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_CLEAN_SEQUENCE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_CUSTOMIZE_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_CAMERA_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_FLOW_LED_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.CLOSE_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_FLOW_LED_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_CLEAN_RECORD: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_MAP_V1: CommandInfo(prefix=b"\x00\x00\x00\xc7"),
+    RoborockCommand.SET_CLEAN_MOTOR_MODE: CommandInfo(prefix=b"\x00\x00\x00\xb7"),
+    RoborockCommand.GET_CONSUMABLE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_SERVER_TIMER: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_SERIAL_NUMBER: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_CURRENT_SOUND: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.SET_LED_STATUS: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_CAMERA_STATUS: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_PAUSE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_CLEAN_SUMMARY: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_NETWORK_INFO: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_LED_STATUS: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.CLOSE_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_WAKEUP_ROBOT: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.SET_MOP_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_CARPET_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.GET_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.SET_CARPET_MODE: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
+    RoborockCommand.GET_MULTI_MAP: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
+    RoborockCommand.SET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.GET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SWITCH_WATER_MARK: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.GET_CLEAN_RECORD_MAP: CommandInfo(prefix=b"\x00\x00\xe7"),
+    RoborockCommand.APP_START: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_STOP: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_CHARGE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_SPOT: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.FIND_ME: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.RESUME_ZONED_CLEAN: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.RESUME_SEGMENT_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.RESET_CONSUMABLE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.LOAD_MULTI_MAP: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_RC_START: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_RC_END: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_RC_MOVE: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_GOTO_TARGET: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.APP_SEGMENT_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\xc7"),
+    RoborockCommand.APP_ZONED_CLEAN: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_START_WASH: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_STOP_WASH: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.SET_FDS_ENDPOINT: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.ENABLE_LOG_UPLOAD: CommandInfo(prefix=b"\x00\x00\x87"),
+    RoborockCommand.GET_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.TEST_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.UPD_SERVER_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_APP_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.CHANGE_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_SOUND_PROGRESS: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.SET_SERVER_TIMER: CommandInfo(prefix=b"\x00\x00\x00\xc7"),
+    RoborockCommand.GET_ROOM_MAPPING: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.NAME_SEGMENT: CommandInfo(prefix=b"\x00\x00\x027"),
+    RoborockCommand.SET_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00\x97")
     # TODO discover prefix for following commands
     # RoborockCommand.APP_GET_DRYER_SETTING: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.APP_SET_DRYER_SETTING: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.GET_DUST_COLLECTION_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.SET_DUST_COLLECTION_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.GET_SMART_WASH_PARAMS: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.SET_SMART_WASH_PARAMS: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.GET_WASH_TOWEL_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.SET_WASH_TOWEL_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
     # RoborockCommand.START_WASH_THEN_CHARGE: CommandInfo(prefix=b'\x00\x00\x00w'),
 }
 
 
 class RoborockDockSummary:
-    def __init__(self, dust_collection_mode: DustCollectionMode,
-                 wash_towel_mode: WashTowelMode, smart_wash_params: SmartWashParams) -> None:
+    def __init__(
+        self,
+        dust_collection_mode: DustCollectionMode,
+        wash_towel_mode: WashTowelMode,
+        smart_wash_params: SmartWashParams,
+    ) -> None:
         self.dust_collection_mode = dust_collection_mode
         self.wash_towel_mode = wash_towel_mode
         self.smart_wash_params = smart_wash_params
 
 
 @dataclass
 class RoborockDeviceProp:
     status: typing.Optional[Status] = None
     dnd_timer: typing.Optional[DNDTimer] = None
     clean_summary: typing.Optional[CleanSummary] = None
     consumable: typing.Optional[Consumable] = None
     last_clean_record: typing.Optional[CleanRecord] = None
     dock_summary: typing.Optional[RoborockDockSummary] = None
 
-    def update(self, device_prop: 'RoborockDeviceProp'):
+    def update(self, device_prop: "RoborockDeviceProp"):
         if device_prop.status:
             self.status = device_prop.status
         if device_prop.dnd_timer:
             self.dnd_timer = device_prop.dnd_timer
         if device_prop.clean_summary:
             self.clean_summary = device_prop.clean_summary
         if device_prop.consumable:
```

### Comparing `python_roborock-0.6.4/PKG-INFO` & `python_roborock-0.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,26 +44,26 @@
 Install this via pip (or your favourite package manager):
 
 `pip install python-roborock`
 
 ## Functionality
 
 This package can encrypt and decrypt the following commands:
-    
+
 - GET_CLEAN_RECORD
 - GET_CONSUMABLE
 - GET_MULTI_MAPS_LIST
 - APP_START
 - APP_PAUSE
 - APP_STOP
 - APP_CHARGE
 - APP_SPOT
 - FIND_ME
 - RESUME_ZONED_CLEAN
-- RESUME_SEGMENT_CLEAN 
+- RESUME_SEGMENT_CLEAN
 - SET_CUSTOM_MODE
 - SET_MOP_MODE
 - SET_WATER_BOX_CUSTOM_MODE
 - RESET_CONSUMABLE
 - LOAD_MULTI_MAP
 - APP_RC_START
 - APP_RC_END
@@ -106,15 +106,11 @@
 - SET_CARPET_CLEAN_MODE
 - UPD_SERVER_TIMER
 - SET_SERVER_TIMER
 - APP_GET_INIT_STATUS
 - SET_APP_TIMEZONE
 - GET_NETWORK_INFO
 
-
-
 ## Credits
 
 Thanks @rovo89 for https://gist.github.com/rovo89/dff47ed19fca0dfdda77503e66c2b7c7 And thanks @PiotrMachowski for https://github.com/PiotrMachowski/Home-Assistant-custom-components-Xiaomi-Cloud-Map-Extractor
 
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.4 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.5 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

