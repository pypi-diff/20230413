# Comparing `tmp/prelude-sdk-0.9.96.tar.gz` & `tmp/prelude-sdk-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-0.9.96.tar", last modified: Fri Apr  7 19:49:45 2023, max compression
+gzip compressed data, was "prelude-sdk-0.9.97.tar", last modified: Thu Apr 13 13:53:41 2023, max compression
```

## Comparing `prelude-sdk-0.9.96.tar` & `prelude-sdk-0.9.97.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152553 prelude-sdk-0.9.96/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1120 2023-04-07 19:49:45.152605 prelude-sdk-0.9.96/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      677 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.149111 prelude-sdk-0.9.96/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.150785 prelude-sdk-0.9.96/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6411 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4178 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.151216 prelude-sdk-0.9.96/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2628 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/models/codes.py
--rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-0.9.96/prelude_sdk/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.149912 prelude-sdk-0.9.96/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      750 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      533 2023-04-07 19:49:45.152815 prelude-sdk-0.9.96/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152342 prelude-sdk-0.9.96/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1058 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152476 prelude-sdk-0.9.96/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-07 19:45:23.000000 prelude-sdk-0.9.96/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4369 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3462 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074432 prelude-sdk-0.9.97/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1140 2023-04-13 13:53:41.074494 prelude-sdk-0.9.97/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.069660 prelude-sdk-0.9.97/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.071733 prelude-sdk-0.9.97/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6538 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4663 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     1353 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.072236 prelude-sdk-0.9.97/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2609 2023-04-08 00:28:18.000000 prelude-sdk-0.9.97/prelude_sdk/models/codes.py
+-rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-0.9.97/prelude_sdk/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.070470 prelude-sdk-0.9.97/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1140 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      796 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-13 13:53:41.000000 prelude-sdk-0.9.97/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-0.9.97/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      533 2023-04-13 13:53:41.074722 prelude-sdk-0.9.97/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074123 prelude-sdk-0.9.97/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:53:41.074344 prelude-sdk-0.9.97/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4386 2023-04-11 22:16:02.000000 prelude-sdk-0.9.97/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3885 2023-04-13 13:44:46.000000 prelude-sdk-0.9.97/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-0.9.97/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-0.9.96/LICENSE` & `prelude-sdk-0.9.97/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.96/PKG-INFO` & `prelude-sdk-0.9.97/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.96
+Version: 0.9.97
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,13 +32,13 @@
 
 ## Documentation 
 
 TBD
 
 ## Testing
 
-To test the Python SDK and Probes, run the following commands:
+To test the Python SDK and Probes, run the following commands from the python/sdk/ directory:
 
 ```bash
-pip install -r python/sdk/tests/requirements.txt
+pip install -r tests/requirements.txt
 pytest tests --api https://api.preludesecurity.com --email <EMAIL>
 ```
```

### Comparing `prelude-sdk-0.9.96/README.md` & `prelude-sdk-0.9.97/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 ## Documentation 
 
 TBD
 
 ## Testing
 
-To test the Python SDK and Probes, run the following commands:
+To test the Python SDK and Probes, run the following commands from the python/sdk/ directory:
 
 ```bash
-pip install -r python/sdk/tests/requirements.txt
+pip install -r tests/requirements.txt
 pytest tests --api https://api.preludesecurity.com --email <EMAIL>
 ```
```

### Comparing `prelude-sdk-0.9.96/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-0.9.97/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.96/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-0.9.97/prelude_sdk/controllers/detect_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 class DetectController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def register_endpoint(self, host, serial_num, edr_id, tags):
+    def register_endpoint(self, host, serial_num, edr_id, tags, endpoint_id=None):
         """ Register (or re-register) an endpoint to your account """
         with Spinner():
-            params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags)
+            params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags) if not endpoint_id else \
+                dict(endpoint_id=endpoint_id, tags=tags, edr_id=edr_id, host=host)
             res = requests.post(
                 f'{self.account.hq}/detect/endpoint',
                 headers=self.account.headers,
                 json=params,
                 timeout=10
             )
             if res.status_code == 200:
```

### Comparing `prelude-sdk-0.9.96/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-0.9.97/prelude_sdk/controllers/iam_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -93,34 +93,48 @@
                 timeout=10
             )
             if res.status_code == 200:
                 return True
             raise Exception(res.text)
 
     @verify_credentials
-    def attach_control(self, name: str, api: str, user: str, secret: str = ''):
-        """ Attach a control to your account """
+    def attach_partner(self, name: str, api: str, user: str, secret: str = ''):
+        """ Attach a partner to your account """
         with Spinner():
-            params = dict(name=name, api=api, user=user, secret=secret)
+            params = dict(api=api, user=user, secret=secret)
             res = requests.post(
-                f'{self.account.hq}/iam/control',
+                f'{self.account.hq}/iam/partner/{name}',
                 headers=self.account.headers,
                 json=params,
                 timeout=10
             )
             if res.status_code == 200:
                 return res.text
             raise Exception(res.text)
 
     @verify_credentials
-    def detach_control(self, name: str):
-        """ Detach a control from your Detect account """
+    def detach_partner(self, name: str):
+        """ Detach a partner from your Detect account """
         with Spinner():
             res = requests.delete(
-                f'{self.account.hq}/iam/control',
+                f'{self.account.hq}/iam/partner/{name}',
                 headers=self.account.headers,
-                json=dict(name=name),
                 timeout=10
             )
             if res.status_code == 200:
                 return res.text
             raise Exception(res.text)
+
+    @verify_credentials
+    def audit_logs(self, days: int = 7, limit: int = 1000):
+        """ Get audit logs from the last X days """
+        with Spinner():
+            params = dict(days=days, limit=limit)
+            res = requests.get(
+                f'{self.account.hq}/iam/audit',
+                headers=self.account.headers,
+                params=params,
+                timeout=30
+            )
+            if res.status_code == 200:
+                return res.json()
+            raise Exception(res.text)
```

### Comparing `prelude-sdk-0.9.96/prelude_sdk/controllers/probe_controller.py` & `prelude-sdk-0.9.97/prelude_sdk/controllers/probe_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.96/prelude_sdk/models/account.py` & `prelude-sdk-0.9.97/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.96/prelude_sdk/models/codes.py` & `prelude-sdk-0.9.97/prelude_sdk/models/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     def _missing_(cls, value):
         return RunCode.INVALID
     
 
 class Mode(Enum):
      MANUAL = 0
      FROZEN = 1
-     AUTOPILOT = 2
 
      @classmethod
      def _missing_(cls, value):
          return Mode.MANUAL
      
 
 class Permission(Enum):
```

### Comparing `prelude-sdk-0.9.96/prelude_sdk/spinner.py` & `prelude-sdk-0.9.97/prelude_sdk/spinner.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.96/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-0.9.97/prelude_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.96
+Version: 0.9.97
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,13 +32,13 @@
 
 ## Documentation 
 
 TBD
 
 ## Testing
 
-To test the Python SDK and Probes, run the following commands:
+To test the Python SDK and Probes, run the following commands from the python/sdk/ directory:
 
 ```bash
-pip install -r python/sdk/tests/requirements.txt
+pip install -r tests/requirements.txt
 pytest tests --api https://api.preludesecurity.com --email <EMAIL>
 ```
```

### Comparing `prelude-sdk-0.9.96/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-0.9.97/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 prelude_sdk.egg-info/dependency_links.txt
 prelude_sdk.egg-info/requires.txt
 prelude_sdk.egg-info/top_level.txt
 prelude_sdk/controllers/__init__.py
 prelude_sdk/controllers/build_controller.py
 prelude_sdk/controllers/detect_controller.py
 prelude_sdk/controllers/iam_controller.py
+prelude_sdk/controllers/partner_controller.py
 prelude_sdk/controllers/probe_controller.py
 prelude_sdk/models/__init__.py
 prelude_sdk/models/account.py
 prelude_sdk/models/codes.py
 tests/__init__.py
 tests/conftest.py
 tests/test_build_controller.py
```

### Comparing `prelude-sdk-0.9.96/setup.cfg` & `prelude-sdk-0.9.97/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 0.9.96
+version = 0.9.97
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-0.9.96/tests/conftest.py` & `prelude-sdk-0.9.97/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             self.capture.resume_global_capture()
 
     yield suspend()
 
 
 def pytest_addoption(parser):
     parser.addoption("--api", default='https://api.staging.preludesecurity.com', action='store', help='API target for tests')
-    parser.addoption('--email', action='store', help='Email address to use for testing', required=True)
+    parser.addoption('--email', default='test@auto-accept.developer.preludesecurity.com', action='store', help='Email address to use for testing')
 
 
 @pytest.fixture(scope='session')
 def api(pytestconfig):
     return pytestconfig.getoption('api')
```

### Comparing `prelude-sdk-0.9.96/tests/test_build_controller.py` & `prelude-sdk-0.9.97/tests/test_build_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 from importlib.resources import files
 
 from tests import templates as templates
 from prelude_sdk.controllers.build_controller import BuildController
 
 
-@pytest.mark.order(after='test_iam_controller.py::TestIAMController::test_detach_control')
+@pytest.mark.order(after='test_iam_controller.py::TestIAMController::test_detach_partner')
 class TestBuildController:
 
     def setup_class(self):
         """Setup the test class"""
         self.test_id = str(uuid.uuid4())
         self.test_name = 'test'
         self.build = BuildController(pytest.account)
```

### Comparing `prelude-sdk-0.9.96/tests/test_detect_controller.py` & `prelude-sdk-0.9.97/tests/test_detect_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,22 @@
     def test_enable_test(self, unwrap):
         """Test enable_test method"""
         unwrap(self.detect.enable_test)(self.detect, ident=pytest.test_id, run_code=RunCode.DEBUG.value, tags=self.tags)
         res = unwrap(self.detect.list_queue)(self.detect)
         assert len([test for test in res if test['test'] == pytest.test_id]) == 1
 
     def test_describe_activity(self, unwrap):
-        """Test spawn_probe_run_tests method"""
+        """Test describe_activity method"""
         try:
             subprocess.run([pytest.probe], capture_output=True, env={'PRELUDE_TOKEN': pytest.endpoint_token}, timeout=20)
         except subprocess.TimeoutExpired:
             describe_activity = unwrap(self.detect.describe_activity)(self.detect, filters={'endpoint_id': pytest.endpoint_id})
             assert len(describe_activity) == 2
-        os.remove(pytest.probe)
+        finally:
+            os.remove(pytest.probe)
 
     def test_disable_test(self, unwrap):
         """Test disable_test method"""
         unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id)
         res = unwrap(self.detect.list_queue)(self.detect)
         assert len([test for test in res if test['test'] == pytest.test_id]) == 0
```

### Comparing `prelude-sdk-0.9.96/tests/test_iam_controller.py` & `prelude-sdk-0.9.97/tests/test_iam_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,38 +61,46 @@
         iam = IAMController(pytest.account)
         res = unwrap(iam.create_user)(iam, handle='registration', permission=Permission.SERVICE.value, expires=(datetime.utcnow() + timedelta(days=1)))
         assert check_if_string_is_uuid(res['token'])
         res = unwrap(iam.get_account)(iam)
         assert len([user for user in res['users'] if user['handle'] == 'registration']) == 1
 
     @pytest.mark.order(4)
-    def test_update_account(self, unwrap):
-        """Test update_account method"""
+    def test_delete_user(self, unwrap):
+        """Test delete_user method"""
         iam = IAMController(pytest.account)
-        unwrap(iam.update_account)(iam, mode=Mode.AUTOPILOT.value)
+        res = unwrap(iam.delete_user)(iam, handle='registration')
         res = unwrap(iam.get_account)(iam)
-        assert res['mode'] == Mode.AUTOPILOT.value
+        assert len([user for user in res['users'] if user['handle'] == 'registration']) == 0
 
     @pytest.mark.order(5)
-    def test_attach_control(self, unwrap):
-        """Test attach_control method"""
+    def test_attach_partner(self, unwrap):
+        """Test attach_partner method"""
         try:
             iam = IAMController(pytest.account)
-            unwrap(iam.attach_control)(iam, 'crowdstrike', 'https://api.us-2.crowdstrike.com', 'test')
+            unwrap(iam.attach_partner)(iam, 'crowdstrike', 'https://api.us-2.crowdstrike.com', 'test')
         except Exception as e:
             assert 'Authentication failed with crowdstrike' in str(e)
 
     @pytest.mark.order(6)
-    def test_detach_control(self, unwrap):
-        """Test detach_control method"""
+    def test_detach_partner(self, unwrap):
+        """Test detach_partner method"""
         try:
             iam = IAMController(pytest.account)
-            unwrap(iam.detach_control)(iam, 'crowdstrike')
+            unwrap(iam.detach_partner)(iam, 'crowdstrike')
         except Exception as e:
-            assert 'No control by that name' in str(e)
+            assert 'No partner by that name' in str(e)
+
+    @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_describe_activity')
+    def test_update_account(self, unwrap):
+        """Test update_account method"""
+        iam = IAMController(pytest.account)
+        unwrap(iam.update_account)(iam, mode=Mode.FROZEN.value)
+        res = unwrap(iam.get_account)(iam)
+        assert res['mode'] == Mode.FROZEN.value
 
     @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_make_decision')
     def test_purge_account(self, unwrap):
         """Test purge_account method"""
         iam = IAMController(pytest.account)
         res = unwrap(iam.purge_account)(iam)
         assert res is not None
```

### Comparing `prelude-sdk-0.9.96/tests/test_probe_controller.py` & `prelude-sdk-0.9.97/tests/test_probe_controller.py`

 * *Files identical despite different names*

