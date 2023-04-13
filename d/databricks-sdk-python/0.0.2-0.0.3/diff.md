# Comparing `tmp/databricks_sdk_python-0.0.2.tar.gz` & `tmp/databricks_sdk_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sdk_python-0.0.2.tar", max compression
+gzip compressed data, was "databricks_sdk_python-0.0.3.tar", max compression
```

## Comparing `databricks_sdk_python-0.0.2.tar` & `databricks_sdk_python-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,40 @@
--rw-r--r--   0        0        0       25 2023-04-01 20:27:24.948624 databricks_sdk_python-0.0.2/README.md
--rw-r--r--   0        0        0     1433 2023-04-01 20:27:40.048661 databricks_sdk_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.948624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/__init__.py
--rw-r--r--   0        0        0     1449 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/client.py
--rw-r--r--   0        0        0     2196 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/credentials.py
--rw-r--r--   0        0        0     2460 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/networks.py
--rw-r--r--   0        0        0     2477 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/storage_configuration.py
--rw-r--r--   0        0        0     3010 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/client.py
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/__init__.py
--rw-r--r--   0        0        0      921 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/credentials.py
--rw-r--r--   0        0        0     1279 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/networks.py
--rw-r--r--   0        0        0      943 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/storage_config.py
--rw-r--r--   0        0        0      326 2023-04-01 20:27:24.952624 databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/base.py
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 databricks_sdk_python-0.0.2/setup.py
--rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 databricks_sdk_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1099 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/README.md
+-rw-r--r--   0        0        0     1536 2023-04-13 08:40:20.795345 databricks_sdk_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/__init__.py
+-rw-r--r--   0        0        0     1593 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/client.py
+-rw-r--r--   0        0        0     2495 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/credentials.py
+-rw-r--r--   0        0        0     2759 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/networks.py
+-rw-r--r--   0        0        0     2776 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/storage_configuration.py
+-rw-r--r--   0        0        0     5262 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/workspaces.py
+-rw-r--r--   0        0        0     3247 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/client.py
+-rw-r--r--   0        0        0      334 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/__init__.py
+-rw-r--r--   0        0        0     1209 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/client.py
+-rw-r--r--   0        0        0     3484 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/instance_profiles.py
+-rw-r--r--   0        0        0     4029 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     3250 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/unity_catalog/catalogs.py
+-rw-r--r--   0        0        0      783 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/unity_catalog/client.py
+-rw-r--r--   0        0        0     6377 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/unity_catalog/metastores.py
+-rw-r--r--   0        0        0     3328 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/workspace/unity_catalog/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.319142 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/__init__.py
+-rw-r--r--   0        0        0      921 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/credentials.py
+-rw-r--r--   0        0        0     1279 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/networks.py
+-rw-r--r--   0        0        0      943 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/storage_config.py
+-rw-r--r--   0        0        0     2928 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/workspaces.py
+-rw-r--r--   0        0        0      575 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/base.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/__init__.py
+-rw-r--r--   0        0        0     1274 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/instance_profiles.py
+-rw-r--r--   0        0        0     2322 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     2170 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/unity_catalog/catalogs.py
+-rw-r--r--   0        0        0     3530 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/unity_catalog/metastores.py
+-rw-r--r--   0        0        0     1759 2023-04-13 08:40:04.323143 databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/workspace/unity_catalog/schemas.py
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 databricks_sdk_python-0.0.3/setup.py
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 databricks_sdk_python-0.0.3/PKG-INFO
```

### Comparing `databricks_sdk_python-0.0.2/pyproject.toml` & `databricks_sdk_python-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sdk-python"
-version = "0.0.2"
+version = "0.0.3"
 description = "Objet based databricks sdk"
 authors = ["Peter van 't Hof' <peter.vanthof@godatadriven.com>"]
 
 keywords = ["databricks"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/ffinfo/databricks-sdk-python"
@@ -13,15 +13,15 @@
     "LICENSE",
 ]
 
 
 packages = [{ include = "databricks_sdk_python", from = "src"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8,<3.12"
 pydantic = "^1.4.0"
 requests = ">=2.22"
 
 [tool.poetry.group.dev.dependencies]
 pydantic-factories = "^1.17.2"
 coverage= {version=  "^7.2.2", extras=["toml"]}
 pytest= "^7.2.2"
@@ -29,14 +29,19 @@
 pyproject-flake8 ="^5.0.4"
 isort ="^5.10.0"
 black="23.3.0"
 pytest-cov="^4.0.0"
 mypy = "^1.1.1"
 requests-mock = "^1.10.0"
 
+
+[tool.poetry.group.mkdocs.dependencies]
+mkdocs = "^1.4.2"
+mkdocs-include-markdown-plugin = "^4.0.4"
+
 [tool.black]
 line-length = 120
 target-version = ["py38"]
 
 [tool.pytest.ini_options]
 addopts = "--junitxml=junit/report.xml"
 testpaths = ["tests"]
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/client.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 
 class AwsAccountClient(BaseClient):
     def __init__(self, account_id: UUID, auth: Optional[HTTPBasicAuth] = None):
         super().__init__(host=ACCOUNT_HOST, auth=auth)
         self.account_id = account_id
 
         from databricks_sdk_python.api_client.account.aws.credentials import AwsCredentialsClient
-
-        self.credentials = AwsCredentialsClient(self)
-
+        from databricks_sdk_python.api_client.account.aws.networks import AwsNetworksClient
         from databricks_sdk_python.api_client.account.aws.storage_configuration import AwsStorageConfigurationClient
+        from databricks_sdk_python.api_client.account.aws.workspaces import AwsWorkspacesClient
 
+        self.credentials = AwsCredentialsClient(self)
         self.storage_configuration = AwsStorageConfigurationClient(self)
-
-        from databricks_sdk_python.api_client.account.aws.networks import AwsNetworksClient
-
         self.networks = AwsNetworksClient(self)
+        self.workspaces = AwsWorkspacesClient(self)
 
     def _get_account_path(self):
         return f"{ACCOUNT_API_PREFIX}/{self.account_id}"
 
 
 _client_cache: Dict[UUID, AwsAccountClient] = {}
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/credentials.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/credentials.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional
 from uuid import UUID
 
 from databricks_sdk_python.api_client.account.aws.client import AwsAccountClient
-from databricks_sdk_python.resources.aws_account.credentials import Credentials
+from databricks_sdk_python.api_client.utils import UnknownApiResponse
+from databricks_sdk_python.resources.account.aws.credentials import Credentials
 
 
 class AwsCredentialsClient(object):
     def __init__(self, aws_account_client: AwsAccountClient):
         self.aws_account_client = aws_account_client
 
     def _get_path(self):
@@ -16,38 +17,45 @@
         return f"{self._get_path()}/{credentials_id}"
 
     def list(self) -> List[Credentials]:
         """List all credentials found on databricks account"""
         response = self.aws_account_client._get(self._get_path())
         if response.status_code == 404:
             return []
-        return [Credentials(**x) for x in response.json()]
+        elif response.status_code == 200:
+            return [Credentials(**x) for x in response.json()]
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_id(self, credentials_id: UUID) -> Optional[Credentials]:
         """Fetch a single credentials by id"""
         response = self.aws_account_client._get(self._get_id_path(credentials_id))
         if response.status_code == 404:
             return None
-        return Credentials(**response.json())
+        elif response.status_code == 200:
+            return Credentials(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_name(self, credentials_name: str) -> Optional[Credentials]:
         """Fetch a single credentials by name"""
         for c in self.list():
             if c.credentials_name == credentials_name:
                 return c
 
     def create(self, credentials_name: str, role_arn: str) -> Credentials:
         """Creates credentials on the databricks account"""
         body = {
             "credentials_name": credentials_name,
             "aws_credentials": {"sts_role": {"role_arn": role_arn}},
         }
         response = self.aws_account_client._post(self._get_path(), body=body)
-        return Credentials(**response.json())
+        if response.status_code == 201:
+            return Credentials(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def delete(self, credentials_id: UUID):
         """Deletes a credentials from the databricks account"""
         response = self.aws_account_client._delete(self._get_id_path(credentials_id))
-        if response.status_code == 404:
-            raise RuntimeError("Not found")
-        if response.status_code == 409:
-            raise RuntimeError(str(response.json()))
+        if response.status_code != 200:
+            raise UnknownApiResponse(response)
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/networks.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/networks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import List, Optional
 from uuid import UUID
 
 from databricks_sdk_python.api_client.account.aws.client import AwsAccountClient
-from databricks_sdk_python.resources.aws_account.networks import Network, NetworkVpcEndpoints
+from databricks_sdk_python.api_client.utils import UnknownApiResponse
+from databricks_sdk_python.resources.account.aws.networks import Network, NetworkVpcEndpoints
 
 
 class AwsNetworksClient(object):
     def __init__(self, aws_account_client: AwsAccountClient):
         self.aws_account_client = aws_account_client
 
     def _get_path(self):
@@ -15,24 +16,30 @@
 
     def _get_id_path(self, network_id: UUID):
         return f"{self._get_path()}/{network_id}"
 
     def list(self) -> List[Network]:
         """List all network found on databricks account"""
         response = self.aws_account_client._get(self._get_path())
-        if response.status_code == 404:
+        if response.status_code == 200:
+            return [Network(**x) for x in response.json()]
+        elif response.status_code == 404:
             return []
-        return [Network(**x) for x in response.json()]
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_id(self, network_id: UUID) -> Optional[Network]:
         """Fetch a single network by id"""
         response = self.aws_account_client._get(self._get_id_path(network_id))
-        if response.status_code == 404:
+        if response.status_code == 200:
+            return Network(**response.json())
+        elif response.status_code == 404:
             return None
-        return Network(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_name(self, network_name: str) -> Optional[Network]:
         """Fetch a single network by name"""
         for s in self.list():
             if s.network_name == network_name:
                 return s
         return None
@@ -51,16 +58,17 @@
             "vpc_id": vpc_id,
             "subnet_ids": subnet_ids,
             "security_group_ids": security_group_ids,
         }
         if vpc_endpoints is not None:
             body["vpc_endpoints"] = json.loads(vpc_endpoints.json())
         response = self.aws_account_client._post(self._get_path(), body=body)
-        return Network(**response.json())
+        if response.status_code == 201:
+            return Network(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def delete(self, network_id: UUID):
         """Deletes a network from the databricks account"""
         response = self.aws_account_client._delete(self._get_id_path(network_id))
-        if response.status_code == 404:
-            raise RuntimeError("Not found")
-        if response.status_code == 409:
-            raise RuntimeError(str(response.json()))
+        if response.status_code != 200:
+            raise UnknownApiResponse(response)
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/account/aws/storage_configuration.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/account/aws/storage_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional
 from uuid import UUID
 
 from databricks_sdk_python.api_client.account.aws.client import AwsAccountClient
-from databricks_sdk_python.resources.aws_account.storage_config import StorageConfiguration
+from databricks_sdk_python.api_client.utils import UnknownApiResponse
+from databricks_sdk_python.resources.account.aws.storage_config import StorageConfiguration
 
 
 class AwsStorageConfigurationClient(object):
     def __init__(self, aws_account_client: AwsAccountClient):
         self.aws_account_client = aws_account_client
 
     def _get_path(self):
@@ -14,24 +15,30 @@
 
     def _get_id_path(self, storage_configuration_id: UUID):
         return f"{self._get_path()}/{storage_configuration_id}"
 
     def list(self) -> List[StorageConfiguration]:
         """List all storage_configuration found on databricks account"""
         response = self.aws_account_client._get(self._get_path())
-        if response.status_code == 404:
+        if response.status_code == 200:
+            return [StorageConfiguration(**x) for x in response.json()]
+        elif response.status_code == 404:
             return []
-        return [StorageConfiguration(**x) for x in response.json()]
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_id(self, storage_configuration_id: UUID) -> Optional[StorageConfiguration]:
         """Fetch a single storage_configuration by id"""
         response = self.aws_account_client._get(self._get_id_path(storage_configuration_id))
-        if response.status_code == 404:
+        if response.status_code == 200:
+            return StorageConfiguration(**response.json())
+        elif response.status_code == 404:
             return None
-        return StorageConfiguration(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def get_by_name(self, storage_configuration_name: str) -> Optional[StorageConfiguration]:
         """Fetch a single storage_configuration by name"""
         for s in self.list():
             if s.storage_configuration_name == storage_configuration_name:
                 return s
         return None
@@ -39,16 +46,17 @@
     def create(self, storage_configuration_name: str, bucket_name: str) -> StorageConfiguration:
         """Creates storage_configuration on the databricks account"""
         body = {
             "storage_configuration_name": storage_configuration_name,
             "root_bucket_info": {"bucket_name": bucket_name},
         }
         response = self.aws_account_client._post(self._get_path(), body=body)
-        return StorageConfiguration(**response.json())
+        if response.status_code == 201:
+            return StorageConfiguration(**response.json())
+        else:
+            raise UnknownApiResponse(response)
 
     def delete(self, storage_configuration_id: UUID):
         """Deletes a storage_configuration from the databricks account"""
         response = self.aws_account_client._delete(self._get_id_path(storage_configuration_id))
-        if response.status_code == 404:
-            raise RuntimeError("Not found")
-        if response.status_code == 409:
-            raise RuntimeError(str(response.json()))
+        if response.status_code != 200:
+            raise UnknownApiResponse(response)
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/api_client/client.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/api_client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,24 +52,29 @@
             method_whitelist={"POST"} | set(Retry.DEFAULT_METHOD_WHITELIST),
             respect_retry_after_header=True,
             raise_on_status=False,  # return original response when retries have been exhausted
         )
         self.session.mount("https://", TlsV1HttpAdapter(max_retries=retries))
 
     def _get_url(self, path: str):
-        return f"https://{self.host}/{path}"
+        if path.startswith("/"):
+            return f"https://{self.host}{path}"
+        else:
+            return f"https://{self.host}/{path}"
 
     def _request(self, method, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
-        response = self.session.request(method, url=self._get_url(path), params=params, json=body, auth=self.auth)
-        if response.status_code == 400 or response.status_code == 401 or response.status_code >= 500:
-            logger.error(response.text)
-            response.raise_for_status()
-        return response
+        return self.session.request(method, url=self._get_url(path), params=params, json=body, auth=self.auth)
 
     def _get(self, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
         return self._request("GET", path, params=params, body=body)
 
     def _post(self, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
         return self._request("POST", path, params=params, body=body)
 
+    def _put(self, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
+        return self._request("PUT", path, params=params, body=body)
+
+    def _patch(self, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
+        return self._request("PATCH", path, params=params, body=body)
+
     def _delete(self, path: str, params: Optional[dict] = None, body: Optional[dict] = None) -> Response:
         return self._request("DELETE", path, params=params, body=body)
```

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/credentials.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/credentials.py`

 * *Files identical despite different names*

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/networks.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/networks.py`

 * *Files identical despite different names*

### Comparing `databricks_sdk_python-0.0.2/src/databricks_sdk_python/resources/aws_account/storage_config.py` & `databricks_sdk_python-0.0.3/src/databricks_sdk_python/resources/account/aws/storage_config.py`

 * *Files identical despite different names*

