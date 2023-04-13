# Comparing `tmp/rest_api_auth_manager-1.0.3.tar.gz` & `tmp/rest_api_auth_manager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_api_auth_manager-1.0.3.tar", last modified: Thu Apr 13 20:31:12 2023, max compression
+gzip compressed data, was "rest_api_auth_manager-1.0.4.tar", last modified: Thu Apr 13 20:48:59 2023, max compression
```

## Comparing `rest_api_auth_manager-1.0.3.tar` & `rest_api_auth_manager-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.947886 rest_api_auth_manager-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:31:12.947886 rest_api_auth_manager-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:31:12.000000 rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:31:12.943886 rest_api_auth_manager-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-13 20:31:03.000000 rest_api_auth_manager-1.0.3/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 20:48:59.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 20:48:59.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:48:59.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:48:59.000000 rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:48:59.631231 rest_api_auth_manager-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-13 20:48:49.000000 rest_api_auth_manager-1.0.4/tests/test_unit.py
```

### Comparing `rest_api_auth_manager-1.0.3/LICENSE` & `rest_api_auth_manager-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_api_auth_manager-1.0.3/PKG-INFO` & `rest_api_auth_manager-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest_api_auth_manager
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple manager for REST API authentication and authorization (token based)
 Author-email: gxara <gabrielxara@gmail.com>
 Project-URL: Homepage, https://github.com/gxara/rest_api_auth_manager
 Project-URL: Bug Tracker, https://github.com/gxara/rest_api_auth_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rest_api_auth_manager-1.0.3/README.md` & `rest_api_auth_manager-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rest_api_auth_manager-1.0.3/pyproject.toml` & `rest_api_auth_manager-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rest_api_auth_manager"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="gxara", email="gabrielxara@gmail.com" },
 ]
 description = "Simple manager for REST API authentication and authorization (token based)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/__init__.py` & `rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def add_user(self, details: dict) -> str:
         """
         Create a new user and add it to the credentials repository
         """
 
         if details.get("token") is not None:
             token = details["token"]
+            del details["token"]
         else:
             characters = string.ascii_letters + string.digits
             secret = ''.join(random.choice(characters) for _ in range(self._config.token_length))
             token = self._config.environment + "_" + secret
 
         self._credentials_repository.insert_hash("USERS", details["alias"],  json.dumps(details))
         self._credentials_repository.insert_hash("CREDENTIALS", token,  details["alias"])
```

### Comparing `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager/repository.py` & `rest_api_auth_manager-1.0.4/src/rest_api_auth_manager/repository.py`

 * *Files identical despite different names*

### Comparing `rest_api_auth_manager-1.0.3/src/rest_api_auth_manager.egg-info/PKG-INFO` & `rest_api_auth_manager-1.0.4/src/rest_api_auth_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-api-auth-manager
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple manager for REST API authentication and authorization (token based)
 Author-email: gxara <gabrielxara@gmail.com>
 Project-URL: Homepage, https://github.com/gxara/rest_api_auth_manager
 Project-URL: Bug Tracker, https://github.com/gxara/rest_api_auth_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rest_api_auth_manager-1.0.3/tests/test_unit.py` & `rest_api_auth_manager-1.0.4/tests/test_unit.py`

 * *Files identical despite different names*

