# Comparing `tmp/appcenter-3.1.0.dev1.tar.gz` & `tmp/appcenter-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appcenter-3.1.0.dev1.tar", max compression
+gzip compressed data, was "appcenter-3.2.0.tar", max compression
```

## Comparing `appcenter-3.1.0.dev1.tar` & `appcenter-3.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1162 2022-07-02 11:21:23.151279 appcenter-3.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     2186 2022-07-02 11:21:23.151548 appcenter-3.1.0.dev1/README.md
--rwxr-xr-x   0        0        0     1702 2022-07-02 11:21:23.152385 appcenter-3.1.0.dev1/appcenter/__init__.py
--rw-r--r--   0        0        0     3730 2022-07-02 11:21:23.152685 appcenter-3.1.0.dev1/appcenter/account.py
--rw-r--r--   0        0        0     1697 2022-07-02 11:21:23.153064 appcenter-3.1.0.dev1/appcenter/analytics.py
--rwxr-xr-x   0        0        0      179 2022-07-02 11:21:23.153393 appcenter-3.1.0.dev1/appcenter/constants.py
--rw-r--r--   0        0        0    16012 2022-07-02 11:21:23.153762 appcenter-3.1.0.dev1/appcenter/crashes.py
--rw-r--r--   0        0        0    10121 2022-07-02 11:21:23.154045 appcenter-3.1.0.dev1/appcenter/derived_client.py
--rw-r--r--   0        0        0    14532 2022-07-02 11:21:23.154580 appcenter-3.1.0.dev1/appcenter/models.py
--rw-r--r--   0        0        0        0 2022-07-03 11:55:41.367692 appcenter-3.1.0.dev1/appcenter/py.typed
--rw-r--r--   0        0        0     2244 2022-07-02 11:21:23.154909 appcenter-3.1.0.dev1/appcenter/tokens.py
--rw-r--r--   0        0        0    25235 2022-07-02 11:21:23.155315 appcenter-3.1.0.dev1/appcenter/versions.py
--rw-r--r--   0        0        0      995 2022-07-03 12:00:39.755680 appcenter-3.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2960 2022-07-03 12:00:49.018560 appcenter-3.1.0.dev1/setup.py
--rw-r--r--   0        0        0     3183 2022-07-03 12:00:49.018851 appcenter-3.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1162 2022-07-02 11:21:23.151279 appcenter-3.2.0/LICENSE
+-rw-r--r--   0        0        0     2186 2022-07-02 11:21:23.151548 appcenter-3.2.0/README.md
+-rwxr-xr-x   0        0        0     1702 2022-07-02 11:21:23.152385 appcenter-3.2.0/appcenter/__init__.py
+-rw-r--r--   0        0        0     3730 2022-07-02 11:21:23.152685 appcenter-3.2.0/appcenter/account.py
+-rw-r--r--   0        0        0     1697 2022-07-02 11:21:23.153064 appcenter-3.2.0/appcenter/analytics.py
+-rwxr-xr-x   0        0        0      179 2022-07-02 11:21:23.153393 appcenter-3.2.0/appcenter/constants.py
+-rw-r--r--   0        0        0    16012 2022-07-02 11:21:23.153762 appcenter-3.2.0/appcenter/crashes.py
+-rw-r--r--   0        0        0    10057 2022-07-06 10:18:20.535483 appcenter-3.2.0/appcenter/derived_client.py
+-rw-r--r--   0        0        0    14558 2022-07-06 10:34:29.663698 appcenter-3.2.0/appcenter/models.py
+-rw-r--r--   0        0        0        1 2022-07-03 12:20:31.753001 appcenter-3.2.0/appcenter/py.typed
+-rw-r--r--   0        0        0     2244 2022-07-02 11:21:23.154909 appcenter-3.2.0/appcenter/tokens.py
+-rw-r--r--   0        0        0    25235 2022-07-02 11:21:23.155315 appcenter-3.2.0/appcenter/versions.py
+-rw-r--r--   0        0        0      995 2022-07-06 10:39:41.430815 appcenter-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2994 2022-07-06 10:40:01.287141 appcenter-3.2.0/setup.py
+-rw-r--r--   0        0        0     3231 2022-07-06 10:40:01.287514 appcenter-3.2.0/PKG-INFO
```

### Comparing `appcenter-3.1.0.dev1/LICENSE` & `appcenter-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/README.md` & `appcenter-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/__init__.py` & `appcenter-3.2.0/appcenter/__init__.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/account.py` & `appcenter-3.2.0/appcenter/account.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/analytics.py` & `appcenter-3.2.0/appcenter/analytics.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/crashes.py` & `appcenter-3.2.0/appcenter/crashes.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/derived_client.py` & `appcenter-3.2.0/appcenter/derived_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return AppCenterDecodedHTTPException(
             response, deserialize.deserialize(AppCenterHTTPError, response_json)
         )
     except Exception:
         return AppCenterHTTPException(response)
 
 
-def _is_connection_failure(exception: Exception) -> bool:
+def _is_connection_failure(exception: BaseException) -> bool:
     exception_checks = [
         "Operation timed out",
         "Connection aborted.",
         "bad handshake: ",
         "Failed to establish a new connection",
     ]
 
@@ -129,26 +129,23 @@
 
     def __init__(self, name: str, token: str, parent_logger: logging.Logger) -> None:
         self.log = parent_logger.getChild(name)
         self.token = token
         self.session = requests.Session()
         self.session.headers.update({"X-API-Token": self.token})
 
-    # pylint: disable=no-self-use
     def base_url(self, *, version: str = "0.1") -> str:
         """Generate the base URL for the API.
 
         :param str version: The API version to hit
 
         :returns: The base URL
         """
         return f"{API_BASE_URL}/v{version}"
 
-    # pylint: enable=no-self-use
-
     def generate_url(self, *, version: str = "0.1", owner_name: str, app_name: str) -> str:
         """Generate a URL to use for querying the API.
 
         :param str version: The API version to hit
         :param str owner_name: The name of the owner of the app
         :param str app_name: The name of the app
```

### Comparing `appcenter-3.1.0.dev1/appcenter/models.py` & `appcenter-3.2.0/appcenter/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 
 
 class ReleaseOrigin(enum.Enum):
     HOCKEY = "hockeyapp"
     APP_CENTER = "appcenter"
 
 
+@deserialize.auto_snake()
 class BuildInfo:
     branch_name: Optional[str]
     commit_hash: Optional[str]
     commit_message: Optional[str]
 
     def __init__(
         self,
```

### Comparing `appcenter-3.1.0.dev1/appcenter/tokens.py` & `appcenter-3.2.0/appcenter/tokens.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/appcenter/versions.py` & `appcenter-3.2.0/appcenter/versions.py`

 * *Files identical despite different names*

### Comparing `appcenter-3.1.0.dev1/pyproject.toml` & `appcenter-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appcenter"
-version = "3.1.0.dev1"
+version = "3.2.0"
 description = "A Python wrapper around the App Center REST API."
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -22,24 +22,24 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Topic :: Software Development',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 azure-storage-blob = "^2.1.0"
-deserialize = "^1"
+deserialize = "^1.8.0"
 requests = "^2.22.0"
-tenacity = "^6.2.0"
+tenacity = "^8.0.1"
+types-requests = "=2.27.7"
 
 [tool.poetry.dev-dependencies]
-black = "=21.12b0"
-mypy = "=0.931"
-pylint = "=2.12.2"
-pytest = "=6.2.5"
+black = "=22.6.0"
+mypy = "=0.961"
+pylint = "=2.14.4"
+pytest = "=7.1.2"
 pytest-cov = "=3.0.0"
-types-requests = "=2.27.7"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `appcenter-3.1.0.dev1/setup.py` & `appcenter-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 ['appcenter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['azure-storage-blob>=2.1.0,<3.0.0',
- 'deserialize>=1,<2',
+ 'deserialize>=1.8.0,<2.0.0',
  'requests>=2.22.0,<3.0.0',
- 'tenacity>=6.2.0,<7.0.0']
+ 'tenacity>=8.0.1,<9.0.0',
+ 'types-requests==2.27.7']
 
 setup_kwargs = {
     'name': 'appcenter',
-    'version': '3.1.0.dev1',
+    'version': '3.2.0',
     'description': 'A Python wrapper around the App Center REST API.',
     'long_description': 'This is a minimal Python wrapper around the App Center REST APIs to get you up and running. If you are looking for something more substantial, please refer to the REST API documentation: https://openapi.appcenter.ms/\n\nYou can install with `pip install appcenter`\n\n## Usage\n\n```python\n# 1. Import the library\nimport appcenter\n\n# 2. Create a new client\nclient = appcenter.AppCenterClient(access_token="abc123def456")\n\n# 3. Check some error groups\nstart = datetime.datetime.now() - datetime.timedelta(days=10)\nfor group in client.crashes.get_error_groups(owner_name="owner", app_name="myapp", start_time=start):\n    print(group.errorGroupId)\n    \n# 4. Get recent versions\nfor version in client.versions.all(owner_name="owner", app_name="myapp"):\n    print(version)\n    \n# 5. Create a new release\nclient.versions.upload_and_release(\n    owner_name="owner",\n    app_name="myapp",\n    version="0.1",\n    build_number="123",\n    binary_path="/path/to/some.ipa",\n    group_id="12345678-abcd-9012-efgh-345678901234",\n    release_notes="These are some release notes",\n    branch_name="test_branch",\n    commit_hash="1234567890123456789012345678901234567890",\n    commit_message="This is a commit message"\n)\n```\n\n## Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.\n\nWhen you submit a pull request, a CLA bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n',
     'author': 'Dale Myers',
     'author_email': 'dalemy@microsoft.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Microsoft/appcenter-rest-python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.7.2,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `appcenter-3.1.0.dev1/PKG-INFO` & `appcenter-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: appcenter
-Version: 3.1.0.dev1
+Version: 3.2.0
 Summary: A Python wrapper around the App Center REST API.
 Home-page: https://github.com/Microsoft/appcenter-rest-python
 License: MIT
 Keywords: app center,api
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: azure-storage-blob (>=2.1.0,<3.0.0)
-Requires-Dist: deserialize (>=1,<2)
+Requires-Dist: deserialize (>=1.8.0,<2.0.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
-Requires-Dist: tenacity (>=6.2.0,<7.0.0)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: types-requests (==2.27.7)
 Project-URL: Repository, https://github.com/Microsoft/appcenter-rest-python
 Description-Content-Type: text/markdown
 
 This is a minimal Python wrapper around the App Center REST APIs to get you up and running. If you are looking for something more substantial, please refer to the REST API documentation: https://openapi.appcenter.ms/
 
 You can install with `pip install appcenter`
```

