# Comparing `tmp/pyhealthbox3-0.0.16.tar.gz` & `tmp/pyhealthbox3-0.0.17.tar.gz`

## Comparing `pyhealthbox3-0.0.16.tar` & `pyhealthbox3-0.0.17.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/requirements.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/pyhealthbox3/__init__.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/pyhealthbox3/healthbox3.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/pyhealthbox3/models.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/requirements.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/__init__.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/healthbox3.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/models.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/PKG-INFO
```

### Comparing `pyhealthbox3-0.0.16/pyhealthbox3/healthbox3.py` & `pyhealthbox3-0.0.17/pyhealthbox3/healthbox3.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from aiohttp import ClientSession, ClientError, ClientResponseError
 from aiohttp.hdrs import METH_GET, METH_PUT, METH_POST
 
 import async_timeout
 
 import logging
 
-from socket import *
 from .models import Healthbox3DataObject, Healthbox3Room, Healthbox3RoomBoost
 
 _LOGGER = logging.getLogger(__name__)
 
 class Healthbox3():
     """Healthbox3 Device."""
 
@@ -69,14 +68,15 @@
     async def async_get_data(self) -> any:
         """Get data from the API."""
         general_data = await self.request(
             method=METH_GET, endpoint="/v2/api/data/current"
         )
         self._data = Healthbox3DataObject(general_data, advanced_features=self._advanced_features)
         for room in self._data.rooms:
+            _LOGGER.debug(f"Found room: {room.name}")
             room.boost = await self.async_get_room_boost_data(room_id=room.room_id)
         return general_data
 
     async def async_start_room_boost(
         self, room_id: int, boost_level: int, boost_timeout: int
     ) -> any:
         """Start Boosting HB3 Room."""
@@ -106,29 +106,35 @@
         except:
             return Healthbox3RoomBoost()
         
 
     async def async_enable_advanced_api_features(self):
         """Enable advanced API Features."""
         if self._api_key:
-            await self.request(
-                method=METH_POST,
-                endpoint="/v2/api/api_key",
-                data=f"{self._api_key}",
-                expect_json_error=True,
-            )
-            await asyncio.sleep(5)
-            if await self._async_validate_advanced_api_features() == False:
-                await self.close()
-                raise Healthbox3ApiClientAuthenticationError
+            already_valid = await self._async_validate_advanced_api_features()
+            if not already_valid:
+                _LOGGER.debug("Enabling Advanced API.")
+                await self.request(
+                    method=METH_POST,
+                    endpoint="/v2/api/api_key",
+                    data=f"{self._api_key}",
+                    expect_json_error=True,
+                )
+                await asyncio.sleep(5)
+                if await self._async_validate_advanced_api_features() == False:
+                    await self.close()
+                    raise Healthbox3ApiClientAuthenticationError
+            else:
+                _LOGGER.debug("Advanced API already enabled.")
         else:
             raise Healthbox3ApiClientAuthenticationError
 
     async def async_validate_connectivity(self):
         """Validate API Connectivity."""
+        _LOGGER.debug("Validating Connectivity")
         await self.request(
             method=METH_GET, endpoint="/v2/api/data/current"
         )
 
     async def _async_validate_advanced_api_features(self) -> bool:
         """Validate API Advanced Features."""
         authentication_status = await self.request(
@@ -144,25 +150,25 @@
         """Send request to the API."""
         if self._session is None:
             self._session = ClientSession()
             self._close_session = True
 
         url: str = f"http://{self.host}{endpoint}"
 
-        _LOGGER.debug(f"{method}, {url}, {data}")
+        # _LOGGER.debug(f"{method}, {url}, {data}")
 
         try:
             async with async_timeout.timeout(self._request_timeout):
                 response = await self._session.request(
                     method,
                     url,
                     headers=headers,
                     json=data
                 )
-                _LOGGER.debug("%s, %s", response.status, await response.text("utf-8"))
+                # _LOGGER.debug("%s, %s", response.status, await response.text("utf-8"))
                 if response.status in (401, 403):
                     raise Healthbox3ApiClientAuthenticationError(
                         "Invalid credentials",
                     )
                 response.raise_for_status()
 
                 if expect_json_error:
```

### Comparing `pyhealthbox3-0.0.16/pyhealthbox3/models.py` & `pyhealthbox3-0.0.17/pyhealthbox3/models.py`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.16/.gitignore` & `pyhealthbox3-0.0.17/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.16/LICENSE` & `pyhealthbox3-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.16/PKG-INFO` & `pyhealthbox3-0.0.17/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhealthbox3
-Version: 0.0.16
+Version: 0.0.17
 Summary: Renson Healthbox3 Package
 Project-URL: Homepage, https://github.com/rmassch/pyhealthbox3
 Project-URL: Bug Tracker, https://github.com/rmassch/pyhealthbox3/issues
 Author-email: rmassch <1083135+rmassch@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

