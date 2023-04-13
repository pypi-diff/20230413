# Comparing `tmp/cognite_gql_pygen-0.1.3.tar.gz` & `tmp/cognite_gql_pygen-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.1.3.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.1.4.tar", max compression
```

## Comparing `cognite_gql_pygen-0.1.3.tar` & `cognite_gql_pygen-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    11349 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/LICENSE
--rw-r--r--   0        0        0     1782 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/README.md
--rw-r--r--   0        0        0     8252 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      237 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/_functions.sh
--rwxr-xr-x   0        0        0      572 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      379 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      369 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/schema_render.sh
--rw-r--r--   0        0        0      167 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19067 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3910 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2628 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/get_client.py
--rw-r--r--   0        0        0      225 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/config.example.yaml
--rw-r--r--   0        0        0      709 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6273 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3046 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    15859 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     3609 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     6828 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0      868 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/main.py
--rw-r--r--   0        0        0     1423 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0      300 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0       22 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1696 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1782 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/README.md
+-rw-r--r--   0        0        0     8930 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/_functions.sh
+-rwxr-xr-x   0        0        0      572 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/cdf_signin.sh
+-rwxr-xr-x   0        0        0      379 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/schema_publish.sh
+-rwxr-xr-x   0        0        0      369 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/schema_render.sh
+-rw-r--r--   0        0        0      167 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19068 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3910 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6259 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3046 2023-04-13 10:01:26.653998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    15859 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     3609 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     6828 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0      868 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/main.py
+-rw-r--r--   0        0        0     1423 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0       22 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1900 2023-04-13 10:01:26.657998 cognite_gql_pygen-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.4/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.1.3/LICENSE` & `cognite_gql_pygen-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/README.md` & `cognite_gql_pygen-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,26 +57,37 @@
  * DomainClient - a `dm_clients` term - a Python class (or class instance) which serves as a namespace for easy access
    to all DomainModelAPIs in a use case.
 
 
 ## Installation
 
 1. `pip install cognite-gql-pygen`
-2. Create a `config.yaml` file (exact name not important), see [config.example.yaml](./config.example.yaml).
-   - > TODO: Then need for `config.yaml` should be removed...
-3. Define `DM_CLIENTS_CONFIG` env variable to contain the full path to `config.yaml` file.
-4. Test if it works:
+2. Create a `settings.toml` file, see [settings.toml](./settings.toml) for a template.
+   * this step is optional, all settings can be specified in code or via env variables
+   * `settings.toml` should contain only things which are safe to commit to git
+   * also create `.secrets.toml` and put sensitive settings here
+      * the structure of both files (`settings.toml` and `.secrets.toml`) is the same, and the values are merged together
+      * example `.secrets.toml`:
+        ```toml
+        [cognite]
+        client_secret = "the secret goes here"
+        ```
+    * `.secrets.toml` is in `.gitignore`, `settings.toml` is not
+      * hint: if you don't want to commit any settings, it's ok to put everything in `.secrets.toml`
+    * settings (including secrets) are handled by [Dynaconf](https://www.dynaconf.com/)
+       * it is simple to override these settings via env variables, e.g. `export DM_CLIENTS__COGNITE__TENANT_ID = ...`
+3. Test if it works:
    ```
    $ python
    >>> from cognite.dm_clients.domain_modeling.domain_client import get_empty_domain_client
    >>> c = get_empty_domain_client()
    >>> c._client.spaces.list()
    [Space(space="...
    ```
-5. Install CDF CLI client
+4. Install CDF CLI client
    - [setup instructions](https://docs.cognite.com/cdf/cli/)
    - But basically:
      ```
      npm i -g @cognite/cdf-cli
      ```
```

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/cdf_signin.sh` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/bin/cdf_signin.sh`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from cognite.client.exceptions import CogniteAPIError
 from pydantic import parse_obj_as
 from requests import Response
 from retry import retry
 
 from cognite.dm_clients.cdf.data_classes_dm_v3 import Container, DataModel, Edge, Node, Space, View
 from cognite.dm_clients.cdf.get_client import get_client_config
-from cognite.dm_clients.config import CONFIG
+from cognite.dm_clients.config import settings
 
 logger = logging.getLogger(__name__)
 
 
 HttpVerbT = Literal["GET", "PUT", "DELETE", "POST"]
 
-_MAX_TRIES = int(CONFIG["dm_clients"].get("max_tries", 15))
+_MAX_TRIES = int(settings.get("dm_clients.max_tries", 15))
 
 
 class DataModelStorageAPI(APIClient):
     """Base for other API classes"""
 
     @property
     def url(self) -> str:
```

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/cdf/get_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import OAuthClientCredentials, OAuthInteractive
 from pydantic import BaseSettings, validator
 
-from cognite.dm_clients.config import CONFIG
+from cognite.dm_clients.config import settings
 
 
 class CogniteConfig(BaseSettings):
     project: str
     cdf_cluster: str
     tenant_id: str
     client_id: Optional[str]
@@ -41,15 +41,15 @@
 
     @validator("client_name", always=True)
     def replace_none_with_user(cls, value):
         return getpass.getuser() if value is None else value
 
 
 def get_cognite_config() -> CogniteConfig:
-    cognite_config = CogniteConfig(**CONFIG["cognite"])
+    cognite_config = CogniteConfig(**settings.cognite)
     return cognite_config
 
 
 def get_client_config(config: Optional[CogniteConfig] = None) -> ClientConfig:
     if config is None:
         config = get_cognite_config()
```

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING, Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
 from cachelib import BaseCache
 from cognite.client import ClientConfig
 
 from cognite.dm_clients.cdf.client_dm_v3 import CogniteClientDmV3, EdgesAPI, NodesAPI
-from cognite.dm_clients.config import CONFIG
+from cognite.dm_clients.config import settings
 
 from ..cdf.client_dm_v3 import ViewsAPI
 from .domain_model import DomainModel
 
 if TYPE_CHECKING:
     from .domain_model_api import DomainModelAPI
     from .schema import Schema
@@ -45,18 +45,18 @@
         # TODO make all these attributes "_private" to distinguish from domain model APIs
         self.schema = schema
         self._domain_model_api_class = domain_model_api_class
         self.cache: BaseCache = cache
         self._client = CogniteClientDmV3(config)
         self._client._config.headers["cdf-version"] = "alpha"
         if space_id is None:
-            space_id = CONFIG["dm_clients"]["space"]
+            space_id = settings.dm_clients.space
         self.space_id = space_id
-        self._data_model = data_model or CONFIG["dm_clients"].get("datamodel")
-        self.schema_version = schema_version or CONFIG["dm_clients"].get("schema_version")
+        self._data_model = data_model or settings.dm_clients.get("datamodel")
+        self.schema_version = schema_version or settings.dm_clients.get("schema_version")
         if self.schema_version is None:
             raise NotImplementedError("Please specify the schema version")
             # TODO find latest version of the data model
         self._api_map: Dict[Type[DomainModelT], str] = {}
 
         nodes_api = NodesAPI(
             self._client.config,
@@ -134,20 +134,20 @@
         return self._client.graph(self.space_id, self._data_model, str(self.schema_version), query)
 
 
 def get_empty_domain_client():
     from cachelib import SimpleCache
 
     from cognite.dm_clients.cdf.get_client import get_client_config
-    from cognite.dm_clients.config import CONFIG
+    from cognite.dm_clients.config import settings
     from cognite.dm_clients.domain_modeling.domain_model_api import DomainModelAPI
     from cognite.dm_clients.domain_modeling.schema import Schema
 
     return DomainClient(
         schema=Schema(),
         domain_model_api_class=DomainModelAPI,
         cache=SimpleCache(),
         config=get_client_config(),
-        space_id=CONFIG["dm_clients"]["space"],
-        data_model=CONFIG["dm_clients"]["datamodel"],
-        schema_version=CONFIG["dm_clients"]["schema_version"],
+        space_id=settings.dm_clients.space,
+        data_model=settings.dm_clients.datamodel,
+        schema_version=settings.dm_clients.schema_version,
     )
```

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/main.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.1.4/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.3/PKG-INFO` & `cognite_gql_pygen-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
 Requires-Dist: cachelib (>=0.10.2,<0.11.0)
 Requires-Dist: cognite-sdk[pandas] (>=5.9.0,<6.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: msal (>=1.16.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: strawberry-graphql (>=0.156.4,<0.157.0)
 Requires-Dist: typer[all]
```

