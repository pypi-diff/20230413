# Comparing `tmp/mypyllant-0.1.7.tar.gz` & `tmp/mypyllant-0.2.0.tar.gz`

## Comparing `mypyllant-0.1.7.tar` & `mypyllant-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.1.7/logo.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mypyllant-0.1.7/requirements-dev.txt
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.1.7/setup.cfg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    14949 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/api.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2480 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/export.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/models.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.1.7/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/conftest.py
--rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/find_countries.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/generate_test_data.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_api.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_countries.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/test_generate_test_data.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.1.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.1.7/LICENSE
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.1.7/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.0/logo.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.0/setup.cfg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    15218 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/export.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/models.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.0/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/conftest.py
+-rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/find_countries.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/generate_test_data.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_api.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_countries.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.2.0/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.2.0/PKG-INFO
```

### Comparing `mypyllant-0.1.7/.pre-commit-config.yaml` & `mypyllant-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/logo.png` & `mypyllant-0.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/setup.cfg` & `mypyllant-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/.github/workflows/build-test.yaml` & `mypyllant-0.2.0/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/src/myPyllant/api.py` & `mypyllant-0.2.0/src/myPyllant/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from urllib.parse import parse_qs, urlencode, urlparse
 
 import aiohttp
 
 from myPyllant.const import (
     API_URL_BASE,
     AUTHENTICATE_URL,
+    BRANDS,
     CLIENT_ID,
     COUNTRIES,
     DEFAULT_QUICK_VETO_DURATION,
     LOGIN_URL,
     TOKEN_URL,
 )
 from myPyllant.models import (
@@ -55,20 +56,23 @@
 class MyPyllantAPI:
     username: str = None
     password: str = None
     aiohttp_session: aiohttp.ClientSession = None
     oauth_session: dict = {}
     oauth_session_expires: datetime.datetime | None = None
 
-    def __init__(self, username: str, password: str, country: str) -> None:
+    def __init__(self, username: str, password: str, country: str, brand: str) -> None:
         if country not in COUNTRIES.keys():
             raise ValueError(f"Country must be one of {', '.join(COUNTRIES.keys())}")
+        if brand not in BRANDS.keys():
+            raise ValueError(f"Brand must be one of {', '.join(BRANDS.keys())}")
         self.username = username
         self.password = password
         self.country = country
+        self.brand = brand
         trace_config = aiohttp.TraceConfig()
         trace_config.on_request_start.append(on_request_start)
         trace_config.on_request_end.append(on_request_end)
         self.aiohttp_session = aiohttp.ClientSession(
             cookie_jar=aiohttp.CookieJar(),
             raise_for_status=True,
             trace_configs=[trace_config],
@@ -102,22 +106,23 @@
             "redirect_uri": "enduservaillant.page.link://login",
             "code_challenge_method": "S256",
             "code_challenge": code_challenge,
         }
 
         # Grabbing the login URL from the HTML form of the login page
         async with self.aiohttp_session.get(
-            AUTHENTICATE_URL.format(country=self.country)
+            AUTHENTICATE_URL.format(country=self.country, brand=self.brand)
             + "?"
             + urlencode(auth_querystring)
         ) as resp:
             login_html = await resp.text()
 
         result = re.search(
-            LOGIN_URL.format(country=self.country) + r"\?([^\"]*)", login_html
+            LOGIN_URL.format(country=self.country, brand=self.brand) + r"\?([^\"]*)",
+            login_html,
         )
         login_url = unescape(result.group())
 
         login_payload = {
             "username": self.username,
             "password": self.password,
             "credentialId": "",
@@ -141,15 +146,15 @@
             "client_id": "myvaillant",
             "code": code,
             "code_verifier": code_verifier,
             "redirect_uri": "enduservaillant.page.link://login",
         }
 
         async with self.aiohttp_session.post(
-            TOKEN_URL.format(country=self.country),
+            TOKEN_URL.format(country=self.country, brand=self.brand),
             data=token_payload,
             raise_for_status=False,
         ) as resp:
             login_json = await resp.json()
             if resp.status >= 400:
                 logger.error(
                     f"Could not log in, got status {resp.status} this response: {login_json}"
@@ -168,15 +173,16 @@
     async def refresh_token(self):
         refresh_payload = {
             "refresh_token": self.oauth_session["refresh_token"],
             "client_id": CLIENT_ID,
             "grant_type": "refresh_token",
         }
         async with self.aiohttp_session.post(
-            TOKEN_URL.format(country=self.country), data=refresh_payload
+            TOKEN_URL.format(country=self.country, brand=self.brand),
+            data=refresh_payload,
         ) as resp:
             self.oauth_session = await resp.json()
             self.set_session_expires()
             return self.oauth_session
 
     @property
     def access_token(self):
```

### Comparing `mypyllant-0.1.7/src/myPyllant/const.py` & `mypyllant-0.2.0/src/myPyllant/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-LOGIN_URL = "https://identity.vaillant-group.com/auth/realms/vaillant-{country}-b2c/login-actions/authenticate"
-AUTHENTICATE_URL = "https://identity.vaillant-group.com/auth/realms/vaillant-{country}-b2c/protocol/openid-connect/auth"
-TOKEN_URL = "https://identity.vaillant-group.com/auth/realms/vaillant-{country}-b2c/protocol/openid-connect/token"
+LOGIN_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/login-actions/authenticate"
+AUTHENTICATE_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/protocol/openid-connect/auth"
+TOKEN_URL = "https://identity.vaillant-group.com/auth/realms/{brand}-{country}-b2c/protocol/openid-connect/token"
 CLIENT_ID = "myvaillant"
 API_URL_BASE = (
     "https://api.vaillant-group.com/service-connected-control/end-user-app-api/v1"
 )
+BRANDS = {
+    "vaillant": "Vaillant",
+    "sdbg": "Saunier Duval",
+}
+DEFAULT_BRAND = "vaillant"
 COUNTRIES = {
     "austria": "Austria",
     "belgium": "Belgium",
     "bulgaria": "Bulgaria",
     "croatia": "Croatia",
     "czechrepublic": "Czechia",
     "denmark": "Denmark",
```

### Comparing `mypyllant-0.1.7/src/myPyllant/export.py` & `mypyllant-0.2.0/src/myPyllant/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 import argparse
 import asyncio
 from datetime import datetime
 import json
 import sys
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.const import COUNTRIES
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 from myPyllant.models import DeviceDataBucketResolution
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API.")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
     choices=COUNTRIES.keys(),
 )
 parser.add_argument(
+    "brand",
+    help="Brand your account is registered in, i.e. 'vaillant'",
+    default=DEFAULT_BRAND,
+    choices=BRANDS.keys(),
+)
+parser.add_argument(
     "-d",
     "--data",
     action=argparse.BooleanOptionalAction,
     help="Export historical device data",
 )
 parser.add_argument(
     "-r",
@@ -43,17 +49,17 @@
     "--end",
     type=datetime.fromisoformat,
     help="Date where the data should end (ISO format)",
 )
 
 
 async def main(
-    user, password, country, data=False, resolution=None, start=None, end=None
+    user, password, country, brand, data=False, resolution=None, start=None, end=None
 ):
-    async with MyPyllantAPI(user, password, country) as api:
+    async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
             if data:
                 data_list = [
                     {
                         "device": d.dict()
                         | {
                             "data": [
```

### Comparing `mypyllant-0.1.7/src/myPyllant/models.py` & `mypyllant-0.2.0/src/myPyllant/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from enum import Enum
 import logging
-from typing import Any, List
+from typing import Any
 
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class MyPyllantEnum(Enum):
@@ -16,14 +16,19 @@
         return self.value
 
     @property
     def display_value(self) -> str:
         return self.value.replace("_", " ").title()
 
 
+class CircuitState(MyPyllantEnum):
+    HEATING = "HEATING"
+    STANDBY = "STANDBY"
+
+
 class DeviceDataBucketResolution(MyPyllantEnum):
     HOUR = "HOUR"
     DAY = "DAY"
     MONTH = "MONTH"
 
 
 class ZoneHeatingOperatingMode(MyPyllantEnum):
@@ -69,15 +74,15 @@
     set_back_temperature: float
     time_windows: dict
 
 
 class Circuit(BaseModel):
     system_id: str
     index: int
-    circuit_state: str
+    circuit_state: CircuitState
     current_circuit_flow_temperature: float | None
     heating_curve: float | None
     is_cooling_allowed: bool
     min_flow_temperature_setpoint: float | None
     mixer_circuit_type_external: str
     set_back_mode_enabled: bool
     zones: list = []
```

### Comparing `mypyllant-0.1.7/src/myPyllant/sample.py` & `mypyllant-0.2.0/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/src/myPyllant/utils.py` & `mypyllant-0.2.0/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/conftest.py` & `mypyllant-0.2.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         def __enter__(self):
             super().__enter__()
 
             # auth endpoints
             self.get(
                 re.compile(r".*openid-connect/auth\?"),
-                body=f"{LOGIN_URL.format(country='germany')}?test=test",
+                body=f"{LOGIN_URL.format(brand='vaillant', country='germany')}?test=test",
                 status=200,
             )
             self.post(
                 re.compile(r".*login-actions/authenticate\?"),
                 status=200,
                 headers={"Location": "test?code=code"},
             )
@@ -57,13 +57,13 @@
                 )
 
     return _mypyllant_aioresponses
 
 
 @pytest.fixture
 async def mocked_api():
-    api = MyPyllantAPI("test@example.com", "test", "germany")
+    api = MyPyllantAPI("test@example.com", "test", "germany", "vaillant")
     api.oauth_session = {
         "access_token": "access_token",
         "refresh_token": "refresh_token",
     }
     return api
```

### Comparing `mypyllant-0.1.7/tests/find_countries.py` & `mypyllant-0.2.0/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/generate_test_data.py` & `mypyllant-0.2.0/tests/generate_test_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,42 +12,48 @@
 import sys
 from urllib.parse import urlencode
 
 logger = logging.getLogger(__name__)
 
 sys.path.append((Path(__file__).resolve().parent / "src").name)
 
-from myPyllant.const import COUNTRIES
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(
     description="Generates test data necessary to run integration tests."
 )
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
     choices=COUNTRIES.keys(),
 )
 parser.add_argument(
+    "brand",
+    help="Brand your account is registered in, i.e. 'vaillant'",
+    default=DEFAULT_BRAND,
+    choices=BRANDS.keys(),
+)
+parser.add_argument(
     "--debug", help="Print debug information", action=argparse.BooleanOptionalAction
 )
 
 SALT = secrets.token_bytes(16)
 JSON_DIR = Path(__file__).resolve().parent / "json"
 ANONYMIZE_ATTRIBUTES = (
     "device_uuid",
     "device_serial_number",
     "deviceId",
     "serialNumber",
     "systemId",
 )
 
 
-async def main(user, password, country):
+async def main(user, password, country, brand):
     """
     Generate json data for running testcases.
 
     :param user:
     :param password:
     :param country:
     :return:
@@ -56,15 +62,15 @@
     from myPyllant.const import API_URL_BASE
     from myPyllant.models import DeviceDataBucketResolution
     from myPyllant.utils import datetime_format
 
     user_json_dir = JSON_DIR / hashlib.sha1(user.encode("UTF-8") + SALT).hexdigest()
     user_json_dir.mkdir(parents=True, exist_ok=True)
 
-    async with MyPyllantAPI(user, password, country) as api:
+    async with MyPyllantAPI(user, password, country, brand) as api:
         systems_url = f"{API_URL_BASE}/systems"
         async with api.aiohttp_session.get(
             systems_url, headers=api.get_authorized_headers()
         ) as systems_resp:
             system = await systems_resp.json()
             with open(user_json_dir / "systems.json", "w") as fh:
                 anonymized_system = _recursive_data_anonymize(
@@ -122,8 +128,8 @@
     return data
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.debug:
         logging.basicConfig(level="DEBUG")
-    asyncio.run(main(args.user, args.password, args.country))
+    asyncio.run(main(args.user, args.password, args.country, args.brand))
```

### Comparing `mypyllant-0.1.7/tests/test_api.py` & `mypyllant-0.2.0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             user_data[f.stem] = json.loads(f.read_text())
         test_data.append(user_data)
     return test_data
 
 
 async def test_login(mypyllant_aioresponses) -> None:
     with mypyllant_aioresponses() as _:
-        async with MyPyllantAPI("test@example.com", "test", "germany") as mocked_api:
+        async with MyPyllantAPI(
+            "test@example.com", "test", "germany", "vaillant"
+        ) as mocked_api:
             assert isinstance(mocked_api.oauth_session_expires, datetime)
             assert mocked_api.oauth_session_expires > datetime.now()
             assert mocked_api.access_token == "access_token"
             assert "Authorization" in mocked_api.get_authorized_headers()
 
 
 async def test_refresh_token(mypyllant_aioresponses, mocked_api) -> None:
@@ -75,10 +77,10 @@
         assert isinstance(device_data.data[0], DeviceDataBucket)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_export(mypyllant_aioresponses, capsys, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
-        await export_main("test@example.com", "test", "germany")
+        await export_main("test@example.com", "test", "germany", "vaillant")
         captured = capsys.readouterr()
         assert isinstance(json.loads(captured.out), dict)
```

### Comparing `mypyllant-0.1.7/tests/test_generate_test_data.py` & `mypyllant-0.2.0/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json` & `mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.2.0/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json` & `mypyllant-0.2.0/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json` & `mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json` & `mypyllant-0.2.0/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/.gitignore` & `mypyllant-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/LICENSE` & `mypyllant-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/README.md` & `mypyllant-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/pyproject.toml` & `mypyllant-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.1.7/PKG-INFO` & `mypyllant-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

