# Comparing `tmp/craft-store-2.3.0.tar.gz` & `tmp/craft-store-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-store-2.3.0.tar", last modified: Fri Oct  7 19:00:41 2022, max compression
+gzip compressed data, was "craft-store-2.4.0.tar", last modified: Thu Apr 13 17:43:53 2023, max compression
```

## Comparing `craft-store-2.3.0.tar` & `craft-store-2.4.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2022-10-07 19:00:41.661102 craft-store-2.3.0/
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     7652 2021-08-20 16:34:14.000000 craft-store-2.3.0/LICENSE
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2480 2022-10-07 19:00:41.661102 craft-store-2.3.0/PKG-INFO
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1393 2022-01-25 20:28:53.000000 craft-store-2.3.0/README.md
-drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2022-10-07 19:00:41.649103 craft-store-2.3.0/craft_store/
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1207 2022-10-07 18:59:52.000000 craft-store-2.3.0/craft_store/__init__.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2558 2022-08-25 23:12:48.000000 craft-store-2.3.0/craft_store/attenuations.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6854 2022-10-07 16:53:50.000000 craft-store-2.3.0/craft_store/auth.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)    10763 2022-07-12 21:12:11.000000 craft-store-2.3.0/craft_store/base_client.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6780 2022-10-07 16:53:58.000000 craft-store-2.3.0/craft_store/creds.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6708 2022-08-12 00:17:14.000000 craft-store-2.3.0/craft_store/endpoints.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6090 2022-10-07 16:53:58.000000 craft-store-2.3.0/craft_store/errors.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     5609 2022-04-26 11:47:12.000000 craft-store-2.3.0/craft_store/http_client.py
-drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2022-10-07 19:00:41.657102 craft-store-2.3.0/craft_store/models/
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1511 2022-08-25 23:12:48.000000 craft-store-2.3.0/craft_store/models/__init__.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1946 2022-04-05 18:04:45.000000 craft-store-2.3.0/craft_store/models/_base_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1886 2022-04-05 18:04:45.000000 craft-store-2.3.0/craft_store/models/_common_list_releases_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2029 2022-04-05 18:04:45.000000 craft-store-2.3.0/craft_store/models/charm_list_releases_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1477 2022-04-06 16:46:48.000000 craft-store-2.3.0/craft_store/models/release_request_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1161 2022-04-17 14:51:02.000000 craft-store-2.3.0/craft_store/models/revisions_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2138 2022-08-25 23:12:48.000000 craft-store-2.3.0/craft_store/models/snap_list_releases_model.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        0 2022-01-25 20:28:53.000000 craft-store-2.3.0/craft_store/py.typed
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     4704 2022-10-07 16:53:58.000000 craft-store-2.3.0/craft_store/store_client.py
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     5271 2022-10-07 16:53:58.000000 craft-store-2.3.0/craft_store/ubuntu_one_store_client.py
-drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2022-10-07 19:00:41.653102 craft-store-2.3.0/craft_store.egg-info/
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2480 2022-10-07 19:00:41.000000 craft-store-2.3.0/craft_store.egg-info/PKG-INFO
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1114 2022-10-07 19:00:41.000000 craft-store-2.3.0/craft_store.egg-info/SOURCES.txt
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        1 2022-10-07 19:00:41.000000 craft-store-2.3.0/craft_store.egg-info/dependency_links.txt
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        1 2022-02-07 14:19:07.000000 craft-store-2.3.0/craft_store.egg-info/not-zip-safe
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      573 2022-10-07 19:00:41.000000 craft-store-2.3.0/craft_store.egg-info/requires.txt
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)       12 2022-10-07 19:00:41.000000 craft-store-2.3.0/craft_store.egg-info/top_level.txt
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      575 2022-08-25 23:12:48.000000 craft-store-2.3.0/pyproject.toml
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2445 2022-10-07 19:00:41.665102 craft-store-2.3.0/setup.cfg
--rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      790 2022-04-05 19:23:31.000000 craft-store-2.3.0/setup.py
+drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2023-04-13 17:43:53.877257 craft-store-2.4.0/
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     7652 2021-08-20 16:34:14.000000 craft-store-2.4.0/LICENSE
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     3409 2023-04-13 17:43:53.877257 craft-store-2.4.0/PKG-INFO
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2322 2023-04-12 20:28:26.000000 craft-store-2.4.0/README.md
+drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2023-04-13 17:43:53.877257 craft-store-2.4.0/craft_store/
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1207 2023-04-13 17:42:43.000000 craft-store-2.4.0/craft_store/__init__.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2558 2022-08-25 23:12:48.000000 craft-store-2.4.0/craft_store/attenuations.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     7098 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/auth.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)    12908 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/base_client.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6776 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/creds.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6708 2022-08-12 00:17:14.000000 craft-store-2.4.0/craft_store/endpoints.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     6392 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/errors.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     5609 2022-04-26 11:47:12.000000 craft-store-2.4.0/craft_store/http_client.py
+drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2023-04-13 17:43:53.877257 craft-store-2.4.0/craft_store/models/
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1789 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/__init__.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2055 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/_base_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1886 2022-04-05 18:04:45.000000 craft-store-2.4.0/craft_store/models/_common_list_releases_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1075 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/account_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2029 2022-04-05 18:04:45.000000 craft-store-2.4.0/craft_store/models/charm_list_releases_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1886 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/registered_name_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1420 2023-04-13 17:42:43.000000 craft-store-2.4.0/craft_store/models/release_request_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1161 2022-04-17 14:51:02.000000 craft-store-2.4.0/craft_store/models/revisions_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2138 2022-08-25 23:12:48.000000 craft-store-2.4.0/craft_store/models/snap_list_releases_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1011 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/track_guardrail_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1058 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/models/track_model.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        0 2022-01-25 20:28:53.000000 craft-store-2.4.0/craft_store/py.typed
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     4736 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/store_client.py
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     5330 2023-04-12 20:28:26.000000 craft-store-2.4.0/craft_store/ubuntu_one_store_client.py
+drwxrwxr-x   0 sergiusens  (1000) sergiusens  (1000)        0 2023-04-13 17:43:53.877257 craft-store-2.4.0/craft_store.egg-info/
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     3409 2023-04-13 17:43:53.000000 craft-store-2.4.0/craft_store.egg-info/PKG-INFO
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     1272 2023-04-13 17:43:53.000000 craft-store-2.4.0/craft_store.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        1 2023-04-13 17:43:53.000000 craft-store-2.4.0/craft_store.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)        1 2022-02-07 14:19:07.000000 craft-store-2.4.0/craft_store.egg-info/not-zip-safe
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      651 2023-04-13 17:43:53.000000 craft-store-2.4.0/craft_store.egg-info/requires.txt
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)       12 2023-04-13 17:43:53.000000 craft-store-2.4.0/craft_store.egg-info/top_level.txt
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      803 2023-04-12 20:28:26.000000 craft-store-2.4.0/pyproject.toml
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)     2493 2023-04-13 17:43:53.877257 craft-store-2.4.0/setup.cfg
+-rw-rw-r--   0 sergiusens  (1000) sergiusens  (1000)      789 2023-04-12 20:28:26.000000 craft-store-2.4.0/setup.py
```

### Comparing `craft-store-2.3.0/LICENSE` & `craft-store-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/PKG-INFO` & `craft-store-2.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-store
-Version: 2.3.0
+Version: 2.4.0
 Summary: "Store bindings for Snaps and Charms"
 Home-page: https://github.com/canonical/craft-store
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Documentation, https://craft-store.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-store.git
@@ -51,14 +51,33 @@
 
 To run all tests in the suite run:
 
 ```
 make tests
 ```
 
+### Integration tests
+
+Some integration tests require collaborator permission on the `craft-store-test-charm`
+charm package on the staging craft-store. These can be run by creating a pull request.
+
+Other integration tests simply require a valid login to the staging charmhub store.
+These can be run by exporting charmhub staging credentials to the environment
+variable `CRAFT_STORE_CHARMCRAFT_CREDENTIALS`. An easy way to do this is to 
+create a `charmcraft.yaml` file containing the lines:
+
+    charmhub:
+      api-url: "https://api.staging.charmhub.io"
+      storage-url: "https://storage.staging.snapcraftcontent.com"
+
+and then run `charmcraft login --export cc.cred` to login and
+`export CRAFT_STORE_CHARMCRAFT_CREDENTIALS=$(cat cc.cred)` to put the credentials
+into the environment variable. Note that if you do not have collaborator permissions
+on `craft-store-test-charm`, some tests will fail rather than being skipped.
+
 ## Adding new requirements
 
 If a new dependency is added to the project run:
 
 ```
 make freeze-requirements
 ```
```

### Comparing `craft-store-2.3.0/craft_store/__init__.py` & `craft-store-2.4.0/craft_store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Interact with Canonical services such as Charmhub and the Snap Store."""
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 
 from . import creds, endpoints, errors, models
 from .auth import Auth
 from .base_client import BaseClient
 from .http_client import HTTPClient
 from .store_client import StoreClient
```

### Comparing `craft-store-2.3.0/craft_store/attenuations.py` & `craft-store-2.4.0/craft_store/attenuations.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/auth.py` & `craft-store-2.4.0/craft_store/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -123,17 +123,23 @@
         """Encode credentials to base64."""
         return base64.b64encode(credentials.encode()).decode()
 
     def ensure_no_credentials(self) -> None:
         """Check that no credentials exist.
 
         :raises errors.CredentialsAvailable: if credentials have already been set.
+        :raises errors.KeyringUnlockError: if the keyring cannot be unlocked.
         """
-        if self._keyring.get_password(self.application_name, self.host) is not None:
-            raise errors.CredentialsAlreadyAvailable(self.application_name, self.host)
+        try:
+            if self._keyring.get_password(self.application_name, self.host) is not None:
+                raise errors.CredentialsAlreadyAvailable(
+                    self.application_name, self.host
+                )
+        except keyring.errors.KeyringLocked as exc:
+            raise errors.KeyringUnlockError() from exc
 
     def set_credentials(self, credentials: str, force: bool = False) -> None:
         """Store credentials in the keyring.
 
         :param credentials: token to store.
         :param force: overwrite existing credentials.
         """
```

### Comparing `craft-store-2.3.0/craft_store/base_client.py` & `craft-store-2.4.0/craft_store/base_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Craft Store BaseClient."""
 
 import logging
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Sequence, cast
+from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, cast
 from urllib.parse import urlparse
 
 import requests
-from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
+from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor  # type: ignore
 
 from . import endpoints, errors, models
 from .auth import Auth
 from .http_client import HTTPClient
 
 logger = logging.getLogger(__name__)
 
@@ -296,7 +296,66 @@
         endpoint = f"/v1/{self._endpoints.namespace}/{name}/releases"
 
         self.request(
             "POST",
             self._base_url + endpoint,
             json=[r.marshal() for r in release_request],
         )
+
+    def list_registered_names(
+        self, *, include_collaborations: bool = False
+    ) -> List[models.RegisteredNameModel]:
+        """List the registered names available to the logged in account.
+
+        :param include_collaborations: if True, includes names the user is a
+            collaborator on but does not own.
+        """
+        endpoint = f"/v1/{self._endpoints.namespace}"
+        params = {
+            "include-collaborations": "true" if include_collaborations else "false",
+        }
+        response = self.request("GET", self._base_url + endpoint, params=params)
+        results = response.json().get("results", [])
+        return [models.RegisteredNameModel.unmarshal(item) for item in results]
+
+    def register_name(
+        self,
+        name: str,
+        *,
+        entity_type: Optional[Literal["charm", "bundle", "snap"]] = None,
+        private: bool = False,
+        team: Optional[str] = None,
+    ) -> str:
+        """Register a name on the store.
+
+        :param name: the name to register.
+        :param entity_type: The type of package to register (e.g. charm or snap)
+        :param private: Whether this entity is private or not.
+        :param team: An optional team ID to register the name with.
+
+        :returns: the ID of the registered name.
+        """
+        endpoint = f"/v1/{self._endpoints.namespace}"
+
+        request_json = {
+            "name": name,
+            "private": private,
+        }
+        if team is not None:
+            request_json["team"] = team
+        if entity_type is not None:
+            request_json["type"] = entity_type
+
+        response = self.request("POST", self._base_url + endpoint, json=request_json)
+        return response.json()["id"]
+
+    def unregister_name(self, name: str) -> str:
+        """Unregister a name with no published packages.
+
+        :param name: The name to unregister.
+
+        :returns: the ID of the deleted name.
+        """
+        endpoint = f"/v1/{self._endpoints.namespace}/{name}"
+        response = self.request("DELETE", self._base_url + endpoint)
+
+        return response.json()["package-id"]
```

### Comparing `craft-store-2.3.0/craft_store/creds.py` & `craft-store-2.4.0/craft_store/creds.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
     This function creates a string that contains the desired `candid_creds` but also
     stores their "type", for unmarshalling later with `unmarshal_candid_credentials()`.
 
     :param candid_creds: The actual Candid credentials.
     :return: A payload string ready to be passed to Auth.set_credentials()
     """
-    return json.dumps(CandidModel(v=candid_creds).marshal())  # pyright: ignore
+    model = CandidModel(v=candid_creds)  # type: ignore
+    return json.dumps(model.marshal())
 
 
 def unmarshal_candid_credentials(marshalled_creds: str) -> str:
     """Deserialize previously stored Candid credentials.
 
     This function is meant to be called with the returned value from
     Auth.get_credentials(). As such, it supports parsing credentials from before we
@@ -129,15 +130,16 @@
 
     This function creates a string that contains the desired `u1_creds` but also
     stores their "type", for unmarshalling later with `unmarshal_u1_credentials()`.
 
     :param u1_creds: The actual Ubuntu One macaroons credentials.
     :return: A payload string ready to be passed to Auth.set_credentials()
     """
-    return json.dumps(UbuntuOneModel(v=u1_creds).marshal())  # pyright: ignore
+    model = UbuntuOneModel(v=u1_creds)  # type: ignore
+    return json.dumps(model.marshal())
 
 
 def unmarshal_u1_credentials(marshalled_creds: str) -> UbuntuOneMacaroons:
     """Deserialize previously stored Ubuntu One credentials.
 
     This function is meant to be called with the returned value from
     Auth.get_credentials(). As such, it supports parsing credentials from before we
@@ -162,21 +164,20 @@
     try:
         creds = json.loads(marshalled_creds)
     except json.JSONDecodeError as err:
         # Case (3).
         raise errors.CredentialsNotParseable(
             "Expected valid Ubuntu One credentials"
         ) from err
+    if "t" in creds:
+        # Cases (1) and (4).
+        data = creds
     else:
-        if "t" in creds:
-            # Cases (1) and (4).
-            data = creds
-        else:
-            # Case (2).
-            data["v"] = creds
+        # Case (2).
+        data["v"] = creds
 
     try:
         return UbuntuOneModel.unmarshal(data).value
     except pydantic.ValidationError as err:
         # Case (4): dict for some other credential type.
         raise errors.CredentialsNotParseable(
             "Expected valid Ubuntu One credentials"
```

### Comparing `craft-store-2.3.0/craft_store/endpoints.py` & `craft-store-2.4.0/craft_store/endpoints.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/errors.py` & `craft-store-2.4.0/craft_store/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,24 @@
 class NoKeyringError(CraftStoreError):
     """Error raised when no keyring can be used."""
 
     def __init__(self) -> None:
         super().__init__("No keyring found to store or retrieve credentials from.")
 
 
+class KeyringUnlockError(CraftStoreError):
+    """Error raised when keyring unlocking fails."""
+
+    def __init__(self) -> None:
+        super().__init__(
+            "Failed to unlock the keyring.",
+            resolution="Make sure the password is correct and the keyring is available.",
+        )
+
+
 class CandidTokenTimeoutError(CraftStoreError):
     """Error raised when timeout is reached trying to discharge a macaroon."""
 
     def __init__(self, url: str) -> None:
         super().__init__(f"Timed out waiting for token response from {url!r}.")
```

### Comparing `craft-store-2.3.0/craft_store/http_client.py` & `craft-store-2.4.0/craft_store/http_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/models/__init__.py` & `craft-store-2.4.0/craft_store/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,24 +20,32 @@
 from . import (
     charm_list_releases_model,
     release_request_model,
     revisions_model,
     snap_list_releases_model,
 )
 from ._base_model import MarshableModel
+from .account_model import AccountModel
 from .charm_list_releases_model import ListReleasesModel as CharmListReleasesModel
+from .registered_name_model import RegisteredNameModel
 from .release_request_model import ReleaseRequestModel
 from .revisions_model import RevisionsRequestModel, RevisionsResponseModel
 from .snap_list_releases_model import ListReleasesModel as SnapListReleasesModel
+from .track_guardrail_model import TrackGuardrailModel
+from .track_model import TrackModel
 
 __all__ = [
+    "AccountModel",
     "CharmListReleasesModel",
     "MarshableModel",
+    "RegisteredNameModel",
     "ReleaseRequestModel",
     "RevisionsRequestModel",
     "RevisionsResponseModel",
     "SnapListReleasesModel",
+    "TrackGuardrailModel",
+    "TrackModel",
     "charm_list_releases_model",
     "release_request_model",
     "revisions_model",
     "snap_list_releases_model",
 ]
```

### Comparing `craft-store-2.3.0/craft_store/models/_base_model.py` & `craft-store-2.4.0/craft_store/models/_base_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """BaseModel with marshaling capabilities."""
 
-from typing import Any, Dict
+from typing import Any, Dict, Type, TypeVar
 
 from pydantic import BaseModel
 
+Model = TypeVar("Model")
+
 
 class MarshableModel(BaseModel):
     """A BaseModel that can be marshaled and unmarshaled."""
 
     class Config:  # type: ignore # pylint: disable=too-few-public-methods
         """Pydantic model configuration."""
 
         validate_assignment = True
         allow_mutation = False
         alias_generator = lambda s: s.replace("_", "-")  # noqa: E731
+        allow_population_by_field_name = True
 
     @classmethod
-    def unmarshal(cls, data: Dict[str, Any]) -> "MarshableModel":
+    def unmarshal(cls: Type[Model], data: Dict[str, Any]) -> Model:
         """Create and populate a new ``MarshableModel`` from a dict.
 
         The unmarshal method validates entries in the input dictionary, populating
         the corresponding fields in the data object.
 
         :param data: The dictionary data to unmarshal.
 
@@ -51,8 +54,8 @@
 
     def marshal(self) -> Dict[str, Any]:
         """Create a dictionary containing the part specification data.
 
         :return: The newly created dictionary.
 
         """
-        return self.dict(by_alias=True)
+        return self.dict(by_alias=True, exclude_unset=True)
```

### Comparing `craft-store-2.3.0/craft_store/models/_common_list_releases_model.py` & `craft-store-2.4.0/craft_store/models/_common_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/models/charm_list_releases_model.py` & `craft-store-2.4.0/craft_store/models/charm_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/models/revisions_model.py` & `craft-store-2.4.0/craft_store/models/revisions_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/models/snap_list_releases_model.py` & `craft-store-2.4.0/craft_store/models/snap_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.3.0/craft_store/store_client.py` & `craft-store-2.4.0/craft_store/store_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 """Craft Store StoreClient."""
 
 import base64
 import json
 from typing import Optional
 
-from macaroonbakery import bakery, httpbakery
+from macaroonbakery import bakery, httpbakery  # type: ignore
 from overrides import overrides
-from pymacaroons.serializers import json_serializer
+from pymacaroons.serializers import json_serializer  # type: ignore
 
 from . import creds, endpoints, errors
 from .base_client import BaseClient
 from .http_client import HTTPClient
 
 
 def _macaroon_to_json_string(macaroon) -> str:
```

### Comparing `craft-store-2.3.0/craft_store/ubuntu_one_store_client.py` & `craft-store-2.4.0/craft_store/ubuntu_one_store_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """Craft Store StoreClient."""
 
 from typing import Dict, Optional
 from urllib.parse import urlparse
 
 import requests
 from overrides import overrides
-from pymacaroons import Macaroon
+from pymacaroons import Macaroon  # type: ignore
 
 from . import creds, endpoints, errors
 from .base_client import BaseClient
 
 
 class UbuntuOneStoreClient(BaseClient):
     """Encapsulates API calls for the Snap Store or Charmhub with Ubuntu One."""
@@ -96,15 +96,15 @@
             if caveat.location == sso_host:
                 return caveat.caveat_id
         raise errors.CraftStoreError("Invalid root macaroon")
 
     def _discharge(
         self, email: str, password: str, otp: Optional[str], caveat_id
     ) -> str:
-        data = dict(email=email, password=password, caveat_id=caveat_id)
+        data = {"email": email, "password": password, "caveat_id": caveat_id}
         if otp:
             data["otp"] = otp
 
         response = self.http_client.request(
             "POST",
             self._auth_url + self._endpoints.tokens_exchange,
             json=data,
@@ -122,15 +122,17 @@
         otp = kwargs.get("otp")
 
         cavead_id = self._extract_caveat_id(root_macaroon)
         discharged_macaroon = self._discharge(
             email=email, password=password, otp=otp, caveat_id=cavead_id
         )
 
-        u1_macaroon = creds.UbuntuOneMacaroons(r=root_macaroon, d=discharged_macaroon)
+        u1_macaroon = creds.UbuntuOneMacaroons(
+            r=root_macaroon, d=discharged_macaroon
+        )  # type: ignore
         return creds.marshal_u1_credentials(u1_macaroon)
 
     @overrides
     def request(
         self,
         method: str,
         url: str,
```

### Comparing `craft-store-2.3.0/craft_store.egg-info/PKG-INFO` & `craft-store-2.4.0/craft_store.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-store
-Version: 2.3.0
+Version: 2.4.0
 Summary: "Store bindings for Snaps and Charms"
 Home-page: https://github.com/canonical/craft-store
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Documentation, https://craft-store.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-store.git
@@ -51,14 +51,33 @@
 
 To run all tests in the suite run:
 
 ```
 make tests
 ```
 
+### Integration tests
+
+Some integration tests require collaborator permission on the `craft-store-test-charm`
+charm package on the staging craft-store. These can be run by creating a pull request.
+
+Other integration tests simply require a valid login to the staging charmhub store.
+These can be run by exporting charmhub staging credentials to the environment
+variable `CRAFT_STORE_CHARMCRAFT_CREDENTIALS`. An easy way to do this is to 
+create a `charmcraft.yaml` file containing the lines:
+
+    charmhub:
+      api-url: "https://api.staging.charmhub.io"
+      storage-url: "https://storage.staging.snapcraftcontent.com"
+
+and then run `charmcraft login --export cc.cred` to login and
+`export CRAFT_STORE_CHARMCRAFT_CREDENTIALS=$(cat cc.cred)` to put the credentials
+into the environment variable. Note that if you do not have collaborator permissions
+on `craft-store-test-charm`, some tests will fail rather than being skipped.
+
 ## Adding new requirements
 
 If a new dependency is added to the project run:
 
 ```
 make freeze-requirements
 ```
```

### Comparing `craft-store-2.3.0/craft_store.egg-info/SOURCES.txt` & `craft-store-2.4.0/craft_store.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,11 +29,15 @@
 craft_store.egg-info/dependency_links.txt
 craft_store.egg-info/not-zip-safe
 craft_store.egg-info/requires.txt
 craft_store.egg-info/top_level.txt
 craft_store/models/__init__.py
 craft_store/models/_base_model.py
 craft_store/models/_common_list_releases_model.py
+craft_store/models/account_model.py
 craft_store/models/charm_list_releases_model.py
+craft_store/models/registered_name_model.py
 craft_store/models/release_request_model.py
 craft_store/models/revisions_model.py
-craft_store/models/snap_list_releases_model.py
+craft_store/models/snap_list_releases_model.py
+craft_store/models/track_guardrail_model.py
+craft_store/models/track_model.py
```

### Comparing `craft-store-2.3.0/craft_store.egg-info/requires.txt` & `craft-store-2.4.0/craft_store.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pydantic
-keyring
+pydantic>=1.10
+keyring>=23.0
 macaroonbakery
 overrides
 requests
 requests_toolbelt
 
 [dev]
 autoflake
@@ -16,16 +16,18 @@
 isort
 mypy
 pydocstyle
 pylint
 pylint-fixme-info
 pylint-pytest
 pytest
+pytest-check
 pytest-mock
 pytest-subprocess
+pytest-timeout>=2.0
 tox
 types-requests
 types-setuptools
 types-pyyaml
 PyYAML
 
 [doc]
@@ -46,14 +48,16 @@
 isort
 mypy
 pydocstyle
 pylint
 pylint-fixme-info
 pylint-pytest
 pytest
+pytest-check
 pytest-mock
 pytest-subprocess
+pytest-timeout>=2.0
 tox
 types-requests
 types-setuptools
 types-pyyaml
 PyYAML
```

### Comparing `craft-store-2.3.0/setup.cfg` & `craft-store-2.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 project_urls = 
 	Documentation = https://craft-store.readthedocs.io/en/latest/
 	Source = https://github.com/canonical/craft-store.git
 	Issues = https://github.com/canonical/craft-store/issues
 author = Canonical Ltd.
 author_email = snapcraft@lists.snapcraft.io
 license = GNU Lesser General Public License v3 (LGPLv3)
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Operating System :: MacOS :: MacOS X
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
@@ -25,16 +25,16 @@
 
 [options]
 python_requires = >= 3.8
 include_package_data = True
 packages = find:
 zip_safe = False
 install_requires = 
-	pydantic
-	keyring
+	pydantic>=1.10
+	keyring>=23.0
 	macaroonbakery
 	overrides
 	requests
 	requests_toolbelt
 
 [options.package_data]
 craft_store = py.typed
@@ -56,16 +56,18 @@
 	isort
 	mypy
 	pydocstyle
 	pylint
 	pylint-fixme-info
 	pylint-pytest
 	pytest
+	pytest-check
 	pytest-mock
 	pytest-subprocess
+	pytest-timeout>=2.0
 	tox
 	types-requests
 	types-setuptools
 	types-pyyaml
 	PyYAML
 dev = 
 	autoflake
```

### Comparing `craft-store-2.3.0/setup.py` & `craft-store-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 #
 
 
 """The setup script."""
 
 from setuptools import setup
 
-
 setup()
```

