# Comparing `tmp/rest_api_auth_manager-1.0.2.tar.gz` & `tmp/rest_api_auth_manager-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_api_auth_manager-1.0.2.tar", last modified: Mon Apr  3 02:36:11 2023, max compression
+gzip compressed data, was "rest_api_auth_manager-1.0.3.tar", last modified: Thu Apr 13 20:31:12 2023, max compression
```

## Comparing `rest_api_auth_manager-1.0.2.tar` & `rest_api_auth_manager-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:36:11.184333 rest_api_auth_manager-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-03 02:36:11.180333 rest_api_auth_manager-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 02:36:11.184333 rest_api_auth_manager-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:36:11.180333 rest_api_auth_manager-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:36:11.180333 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:36:11.180333 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-03 02:36:11.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-03 02:36:11.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:36:11.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 02:36:11.000000 rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:36:11.180333 rest_api_auth_manager-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-03 02:35:54.000000 rest_api_auth_manager-1.0.2/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.947886 rest_api_auth_manager-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:31:12.947886 rest_api_auth_manager-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/tests/test_unit.py
```

### Comparing `rest_api_auth_manager-1.0.2/LICENSE` & `rest_api_auth_manager-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_api_auth_manager-1.0.2/PKG-INFO` & `rest_api_auth_manager-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest_api_auth_manager
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple manager for REST API authentication and authorization (token based)
 Author-email: gxara <gabrielxara@gmail.com>
 Project-URL: Homepage, https://github.com/gxara/rest_api_auth_manager
 Project-URL: Bug Tracker, https://github.com/gxara/rest_api_auth_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,36 +28,36 @@
 
 ```python
 from rest_api_auth_manager import AuthManager, Config
 
 class CustomConfig(Config):
     credentials_database_host = "127.0.0.1"
     environment = "dev"
-    password_length = 16
+    token_length = 16
 
 auth_manager = AuthManager(CustomConfig)
 ```
 
 ### Add new user
 
 ```python
 user = {
     "alias": "ASH_KETCHUM",
     "name": "Ash Ketchum",
     "email": "ash@test.com",
-    "roles": [],
+    "roles": ["pokemons:get"],
 }
 
 token = auth_manager.add_user(user)
 ```
 
 ### Granting usage on a specific resource
 
 ```python
-auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:get")
+auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:post")
 ```
 
 ### Verifying requests authentication and authorization
 
 ```python
 token = "SUPER_SECRET"
 auth_manager.verify_auth(token, "api/pokemon", "GET")
```

### Comparing `rest_api_auth_manager-1.0.2/README.md` & `rest_api_auth_manager-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 
 ```python
 from rest_api_auth_manager import AuthManager, Config
 
 class CustomConfig(Config):
     credentials_database_host = "127.0.0.1"
     environment = "dev"
-    password_length = 16
+    token_length = 16
 
 auth_manager = AuthManager(CustomConfig)
 ```
 
 ### Add new user
 
 ```python
 user = {
     "alias": "ASH_KETCHUM",
     "name": "Ash Ketchum",
     "email": "ash@test.com",
-    "roles": [],
+    "roles": ["pokemons:get"],
 }
 
 token = auth_manager.add_user(user)
 ```
 
 ### Granting usage on a specific resource
 
 ```python
-auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:get")
+auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:post")
 ```
 
 ### Verifying requests authentication and authorization
 
 ```python
 token = "SUPER_SECRET"
 auth_manager.verify_auth(token, "api/pokemon", "GET")
```

### Comparing `rest_api_auth_manager-1.0.2/pyproject.toml` & `rest_api_auth_manager-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rest_api_auth_manager"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="gxara", email="gabrielxara@gmail.com" },
 ]
 description = "Simple manager for REST API authentication and authorization (token based)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/__init__.py` & `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,19 +52,21 @@
             return True
         return False
 
     def add_user(self, details: dict) -> str:
         """
         Create a new user and add it to the credentials repository
         """
-        characters = string.ascii_letters + string.digits
-        password = ''.join(random.choice(characters)
-                           for _ in range(self._config.password_length))
 
-        token = self._config.environment + "_" + password
+        if details.get("token") is not None:
+            token = details["token"]
+        else:
+            characters = string.ascii_letters + string.digits
+            secret = ''.join(random.choice(characters) for _ in range(self._config.token_length))
+            token = self._config.environment + "_" + secret
 
         self._credentials_repository.insert_hash("USERS", details["alias"],  json.dumps(details))
         self._credentials_repository.insert_hash("CREDENTIALS", token,  details["alias"])
 
         return token
 
     def add_role_to_user(self, user: str, role: str) -> None:
```

### Comparing `rest_api_auth_manager-1.0.2/src/rest_api_auth_manager/repository.py` & `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/repository.py`

 * *Files identical despite different names*

### Comparing `rest_api_auth_manager-1.0.2/src/rest_api_auth_manager.egg-info/PKG-INFO` & `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-api-auth-manager
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple manager for REST API authentication and authorization (token based)
 Author-email: gxara <gabrielxara@gmail.com>
 Project-URL: Homepage, https://github.com/gxara/rest_api_auth_manager
 Project-URL: Bug Tracker, https://github.com/gxara/rest_api_auth_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,36 +28,36 @@
 
 ```python
 from rest_api_auth_manager import AuthManager, Config
 
 class CustomConfig(Config):
     credentials_database_host = "127.0.0.1"
     environment = "dev"
-    password_length = 16
+    token_length = 16
 
 auth_manager = AuthManager(CustomConfig)
 ```
 
 ### Add new user
 
 ```python
 user = {
     "alias": "ASH_KETCHUM",
     "name": "Ash Ketchum",
     "email": "ash@test.com",
-    "roles": [],
+    "roles": ["pokemons:get"],
 }
 
 token = auth_manager.add_user(user)
 ```
 
 ### Granting usage on a specific resource
 
 ```python
-auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:get")
+auth_manager.add_role_to_user("ASH_KETCHUM", "pokemons:post")
 ```
 
 ### Verifying requests authentication and authorization
 
 ```python
 token = "SUPER_SECRET"
 auth_manager.verify_auth(token, "api/pokemon", "GET")
```

### Comparing `rest_api_auth_manager-1.0.2/tests/test_unit.py` & `rest_api_auth_manager-1.0.3/tests/test_unit.py`

 * *Files identical despite different names*

