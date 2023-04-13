# Comparing `tmp/mypyllant-0.1.6.tar.gz` & `tmp/mypyllant-0.1.7.tar.gz`

## Comparing `mypyllant-0.1.6.tar` & `mypyllant-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.1.6/logo.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mypyllant-0.1.6/requirements-dev.txt
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.1.6/setup.cfg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.1.6/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/api.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2480 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/export.py
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/models.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.1.6/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/conftest.py
--rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/find_countries.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/generate_test_data.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/test_api.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/test_countries.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/test_generate_test_data.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.1.6/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.1.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.1.6/LICENSE
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.1.6/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.1.7/logo.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mypyllant-0.1.7/requirements-dev.txt
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.1.7/setup.cfg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    14949 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2480 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/export.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/models.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/conftest.py
+-rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/find_countries.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/generate_test_data.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_api.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_countries.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.1.7/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.1.7/PKG-INFO
```

### Comparing `mypyllant-0.1.6/.pre-commit-config.yaml` & `mypyllant-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/logo.png` & `mypyllant-0.1.7/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/setup.cfg` & `mypyllant-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/.github/workflows/build-test.yaml` & `mypyllant-0.1.7/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/src/myPyllant/api.py` & `mypyllant-0.1.7/src/myPyllant/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 import aiohttp
 
 from myPyllant.const import (
     API_URL_BASE,
     AUTHENTICATE_URL,
     CLIENT_ID,
     COUNTRIES,
+    DEFAULT_QUICK_VETO_DURATION,
     LOGIN_URL,
     TOKEN_URL,
 )
 from myPyllant.models import (
     Device,
     DeviceData,
     DeviceDataBucketResolution,
     DHWOperationMode,
     DomesticHotWater,
     System,
     Zone,
+    ZoneCurrentSpecialFunction,
     ZoneHeatingOperatingMode,
 )
 from myPyllant.utils import datetime_format, dict_to_snake_case, generate_code
 
 logger = logging.getLogger(__name__)
 
 
@@ -36,32 +38,30 @@
     pass
 
 
 async def on_request_start(session, context, params: aiohttp.TraceRequestStartParams):
     """
     See https://docs.aiohttp.org/en/stable/tracing_reference.html#aiohttp.TraceConfig.on_request_start
     """
-    logging.getLogger("aiohttp.client").debug(f"Starting request {params}")
+    logger.debug(f"Starting request {params}")
 
 
 async def on_request_end(session, context, params: aiohttp.TraceRequestEndParams):
     """
     See https://docs.aiohttp.org/en/stable/tracing_reference.html#aiohttp.TraceConfig.on_request_end
     """
-    logging.getLogger("aiohttp.client").debug(
-        f"Got response {await params.response.text()}"
-    )
+    logger.debug(f"Got response {await params.response.text()}")
 
 
 class MyPyllantAPI:
     username: str = None
     password: str = None
     aiohttp_session: aiohttp.ClientSession = None
     oauth_session: dict = {}
-    oauth_session_expires: datetime.datetime = None
+    oauth_session_expires: datetime.datetime | None = None
 
     def __init__(self, username: str, password: str, country: str) -> None:
         if country not in COUNTRIES.keys():
             raise ValueError(f"Country must be one of {', '.join(COUNTRIES.keys())}")
         self.username = username
         self.password = password
         self.country = country
@@ -83,24 +83,32 @@
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:
         if not self.aiohttp_session.closed:
             await self.aiohttp_session.close()
 
     async def login(self):
+        """
+        This should really be done in the browser with OIDC, but that's not easy without support from Vaillant
+
+        So instead, we grab the login endpoint from the HTML form of the login website and send username + password
+        to obtain a session
+        """
+
         code_verifier, code_challenge = generate_code()
         auth_querystring = {
             "response_type": "code",
             "client_id": CLIENT_ID,
             "code": "code_challenge",
             "redirect_uri": "enduservaillant.page.link://login",
             "code_challenge_method": "S256",
             "code_challenge": code_challenge,
         }
 
+        # Grabbing the login URL from the HTML form of the login page
         async with self.aiohttp_session.get(
             AUTHENTICATE_URL.format(country=self.country)
             + "?"
             + urlencode(auth_querystring)
         ) as resp:
             login_html = await resp.text()
 
@@ -110,25 +118,28 @@
         login_url = unescape(result.group())
 
         login_payload = {
             "username": self.username,
             "password": self.password,
             "credentialId": "",
         }
+
+        # Obtaining the code
         async with self.aiohttp_session.post(
             login_url, data=login_payload, allow_redirects=False
         ) as resp:
             if "Location" not in resp.headers:
                 raise AuthenticationFailed("Login failed")
             logger.debug(
                 f'Got location from authorize endpoint: {resp.headers["Location"]}'
             )
             parsed_url = urlparse(resp.headers["Location"])
             code = parse_qs(parsed_url.query)["code"]
 
+        # Obtaining a access token and refresh token
         token_payload = {
             "grant_type": "authorization_code",
             "client_id": "myvaillant",
             "code": code,
             "code_verifier": code_verifier,
             "redirect_uri": "enduservaillant.page.link://login",
         }
@@ -195,15 +206,15 @@
 
                 async with self.aiohttp_session.get(
                     system_url, headers=self.get_authorized_headers()
                 ) as current_system_resp:
                     current_system_json = await current_system_resp.json()
                 system = System(
                     id=system_id,
-                    current_system=current_system_json,
+                    current_system=dict_to_snake_case(current_system_json),
                     **dict_to_snake_case(system_json),
                 )
                 yield system
 
     @staticmethod
     async def get_devices_by_system(
         system: System,
@@ -212,21 +223,21 @@
             if not (isinstance(device_raw, dict) and "device_uuid" in device_raw):
                 continue
             device = Device(
                 system=system,
                 **device_raw,
             )
 
-            serial_nos = {d["serial_number"]: d for d in system.devices}
+            serial_nos = {d.serial_number: d for d in system.devices}
             if device.device_serial_number in serial_nos.keys():
                 device_info = serial_nos[device.device_serial_number]
                 device.operational_data = dict_to_snake_case(
-                    device_info.get("operational_data", {})
+                    device_info.operational_data
                 )
-                device.name = device_info.get("name", "")
+                device.name = device_info.name
 
             yield device
 
     async def get_data_by_device(
         self,
         device: Device,
         data_resolution: DeviceDataBucketResolution = DeviceDataBucketResolution.DAY,
@@ -265,25 +276,49 @@
             json={
                 "heatingOperationMode": str(mode),
             },
             headers=self.get_authorized_headers(),
         )
 
     async def quick_veto_zone_temperature(
-        self, zone: Zone, temperature: float, duration_hours: int
+        self,
+        zone: Zone,
+        temperature: float,
+        duration_hours: int | None = None,
+        default_duration: int | None = None,
     ):
+        logger.debug(
+            f"Setting quick veto for {zone.name} in {zone.current_special_function} mode"
+        )
+        if not default_duration:
+            default_duration = DEFAULT_QUICK_VETO_DURATION
         url = f"{API_URL_BASE}/systems/{zone.system_id}/zones/{zone.index}/quickVeto"
-        return await self.aiohttp_session.post(
-            url,
-            json={
+        if zone.current_special_function == ZoneCurrentSpecialFunction.QUICK_VETO:
+            logger.debug(
+                f"Patching quick veto for {zone.name} because it is already in quick veto mode"
+            )
+            payload = {
                 "desiredRoomTemperatureSetpoint": temperature,
-                "duration": duration_hours,
-            },
-            headers=self.get_authorized_headers(),
-        )
+            }
+            if duration_hours:
+                payload["duration"] = duration_hours
+            return await self.aiohttp_session.patch(
+                url,
+                json=payload,
+                headers=self.get_authorized_headers(),
+            )
+        else:
+            return await self.aiohttp_session.post(
+                url,
+                json={
+                    "desiredRoomTemperatureSetpoint": temperature,
+                    "duration": duration_hours if duration_hours else default_duration,
+                },
+                headers=self.get_authorized_headers(),
+            )
 
     async def cancel_quick_veto_zone_temperature(self, zone: Zone):
         url = f"{API_URL_BASE}/systems/{zone.system_id}/zones/{zone.index}/quickVeto"
         return await self.aiohttp_session.delete(
             url, headers=self.get_authorized_headers()
         )
 
@@ -294,16 +329,16 @@
             json={"setBackTemperature": temperature},
             headers=self.get_authorized_headers(),
         )
 
     async def set_holiday(
         self,
         system: System,
-        start: datetime.datetime = None,
-        end: datetime.datetime = None,
+        start: datetime.datetime | None = None,
+        end: datetime.datetime | None = None,
     ):
         if not start:
             start = datetime.datetime.now()
         if not end:
             # Set away for a long time if no end date is set
             end = start + datetime.timedelta(days=365)
         if not start < end:
```

### Comparing `mypyllant-0.1.6/src/myPyllant/const.py` & `mypyllant-0.1.7/src/myPyllant/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,7 +30,8 @@
     "slovakia": "Slovakia",
     "slovenia": "Slovenia",
     "spain": "Spain",
     "sweden": "Sweden",
     "switzerland": "Switzerland",
     "unitedkingdom": "United Kingdom",
 }
+DEFAULT_QUICK_VETO_DURATION = 3
```

### Comparing `mypyllant-0.1.6/src/myPyllant/export.py` & `mypyllant-0.1.7/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/src/myPyllant/models.py` & `mypyllant-0.1.7/src/myPyllant/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,25 +94,27 @@
     set_point: float
     time_windows: dict
 
 
 class System(BaseModel):
     id: str
     status: dict[str, bool]
-    devices: list[dict]
+    devices: list["SystemDevice"]
     current_system: dict = {}
     system_configuration: dict = {}
     system_control_state: dict = {}
     gateway: dict = {}
     has_ownership: bool
     zones: list[Zone] = []
     circuits: list[Circuit] = []
     domestic_hot_water: list[DomesticHotWater] = []
 
     def __init__(self, **data: Any) -> None:
+        if len(data["devices"]) > 0 and isinstance(data["devices"][0], dict):
+            data["devices"] = [SystemDevice(**d) for d in data.pop("devices")]
         super().__init__(**data)
         logger.debug(
             f'Creating related models from control_state: {self.system_control_state["control_state"]}'
         )
         self.zones = [Zone(system_id=self.id, **z) for z in self._raw_zones]
         self.circuits = [Circuit(system_id=self.id, **c) for c in self._raw_circuits]
         self.domestic_hot_water = [
@@ -181,15 +183,44 @@
         try:
             return self.system_control_state["control_state"]["general"]["system_mode"]
         except KeyError:
             logger.info("Could not get mode from system control state")
             return None
 
 
-class Device(BaseModel):
+class SystemDevice(BaseModel):
+    """
+    The System contains some information about devices already, this is saved in SystemDevice
+    The currentSystem API call returns more device info, which is saved in Device
+    """
+
+    system_id: str
+    device_id: str | None
+    name: str = ""
+    type: str = ""
+    diagnostic_trouble_codes: list = []
+    properties: list = []
+    serial_number: str | None
+    article_number: str | None
+    operational_data: dict = {}
+    data: list["DeviceData"] = []
+
+    @property
+    def name_display(self) -> str:
+        if self.name:
+            return self.name
+        elif self.device_id:
+            return f"Device {self.device_id}"
+        elif self.serial_number:
+            return f"Device {self.serial_number}"
+        else:
+            return "System Device"
+
+
+class Device(SystemDevice):
     system: System
     device_uuid: str
     name: str = ""
     product_name: str
     diagnostic_trouble_codes: list = []
     properties: list = []
     ebus_id: str
@@ -197,14 +228,18 @@
     device_serial_number: str
     device_type: str
     first_data: datetime.datetime
     last_data: datetime.datetime
     operational_data: dict = {}
     data: list["DeviceData"] = []
 
+    def __init__(self, **data):
+        data["system_id"] = data["system"].id
+        super().__init__(**data)
+
     @property
     def name_display(self) -> str:
         return self.name if self.name else self.product_name.title()
 
 
 class DeviceDataBucket(BaseModel):
     start_date: datetime.datetime
@@ -226,8 +261,10 @@
     resolution: DeviceDataBucketResolution | None
     operation_mode: str
     energy_type: str | None
     value_type: str | None
     data: list[DeviceDataBucket] = []
 
 
+# Updating string type hints for pydantic
+System.update_forward_refs()
 Device.update_forward_refs()
```

### Comparing `mypyllant-0.1.6/src/myPyllant/sample.py` & `mypyllant-0.1.7/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/src/myPyllant/utils.py` & `mypyllant-0.1.7/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/conftest.py` & `mypyllant-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/find_countries.py` & `mypyllant-0.1.7/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/generate_test_data.py` & `mypyllant-0.1.7/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/test_api.py` & `mypyllant-0.1.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/test_generate_test_data.py` & `mypyllant-0.1.7/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json` & `mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json` & `mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json` & `mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json` & `mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/.gitignore` & `mypyllant-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/LICENSE` & `mypyllant-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/README.md` & `mypyllant-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/pyproject.toml` & `mypyllant-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.6/PKG-INFO` & `mypyllant-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

