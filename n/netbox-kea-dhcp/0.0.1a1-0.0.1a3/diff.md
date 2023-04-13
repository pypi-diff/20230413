# Comparing `tmp/netbox_kea_dhcp-0.0.1a1.tar.gz` & `tmp/netbox_kea_dhcp-0.0.1a3.tar.gz`

## Comparing `netbox_kea_dhcp-0.0.1a1.tar` & `netbox_kea_dhcp-0.0.1a3.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/etc/netbox-kea-dhcp.example.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/config.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/connector.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/entry_point.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/listener.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/netbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/kea/__init__.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/kea/api.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/kea/app.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/netboxkea/kea/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/devices.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/interfaces.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/ip_addresses.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/ip_ranges.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/prefixes.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/virtual_machines.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/vminterfaces.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/unit/__init__.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/unit/test_connector.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/tests/unit/test_kea.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/README.md
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/config.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/connector.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/entry_point.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/listener.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/netbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/__init__.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/api.py
+-rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/app.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/devices.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/interfaces.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_addresses.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_ranges.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/prefixes.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/virtual_machines.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/vminterfaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/test_connector.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/test_kea.py
+-rw-r--r--   0        0        0   792962 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4-examples.conf
+-rw-r--r--   0        0        0   627796 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4.conf
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/netbox-kea-dhcp.example.toml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/PKG-INFO
```

### Comparing `netbox_kea_dhcp-0.0.1a1/etc/netbox-kea-dhcp.example.toml` & `netbox_kea_dhcp-0.0.1a3/examples/netbox-kea-dhcp.example.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # TODO: implement something like "full_sync_schedule = '23h00'"
 
 listen = false
 bind = "0.0.0.0"
 port = 8000
 secret = "azerQSDF1234uiopJKLM7890"
 # This is the default value:
-#secret_header = "X-netbox2kea-Secret"
+#secret_header = "X-netbox2kea-secret"
 
 #log_level = "debug"    # or "info", "warning" (default), "error"
 #ext_log_level = "warning"    # Log level for external modules
 # TODO: syslog = false
 
 netbox_url = "http://10.94.135.32:8000/"
 netbox_token = "9123456789abcdef0123456789abcdef01234568"
```

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/config.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/config.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/connector.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                         self._prefix_to_subnet(p, fullsync=True)
                     except KeaError as e:
                         logger.error(f'{pl}config failed. Error: {e}')
                         continue
 
             all_failed = False
 
+        self.kea.auto_commit = True
         if all_failed is not True:
             self.push_to_dhcp()
 
     def push_to_dhcp(self):
         if self.check:
             logger.info('check mode on: config will NOT be pushed to server')
         else:
```

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/entry_point.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/entry_point.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/listener.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from json.decoder import JSONDecodeError
 
 import bottle
 
 logger = logging.getLogger('webhook listener')
 
 
 class WebhookListener:
@@ -15,35 +16,37 @@
         self.port = port
         self.secret = secret
         self.secret_header = secret_header
 
     def run(self):
         """ Start web server """
 
-        @bottle.route('/event/<name>', 'POST')
-        def new_event(name=''):
+        @bottle.route('/event/<name>/', 'POST')
+        def new_event(name):
             """ Define an all-in-one route for our web server """
 
-            logger.debug(f'Receive data on /event/{name}')
+            logger.debug(f'Receive data on /event/{name}/')
 
             # import json
             # body = bottle.request.body.getvalue()
             # try:
             #     print(json.dumps(json.loads(body), indent=4))
             # except Exception:
             #     print(body.decode())
 
             if (self.secret_header and bottle.request.get_header(
                     self.secret_header) != self.secret):
                 self._abort(403, 'wrong secret or secret header')
 
             # Parse JSON body from request
-            body = bottle.request.json
-            if body is None:
-                self._abort(400, 'malformed body (no JSON payload)')
+            try:
+                body = bottle.request.json
+            except JSONDecodeError:
+                body = bottle.request.body.getvalue().decode()
+                self._abort(400, f'malformed body (not JSON):  {body}')
 
             logger.debug(f'Parsed JSON request: {body}')
             try:
                 model, id_, event = (
                     body['model'], body['data']['id'], body['event'])
             except KeyError as e:
                 self._abort(400, f'request missing key: {e}')
```

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/netbox.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/netbox.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/kea/api.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/kea/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,26 @@
                     self.conf = json.load(f)
             except FileNotFoundError:
                 self.conf = {}
         else:
             self.conf = {}
 
     def get_conf(self):
-        return self.conf
+        return self.conf.get('Dhcp4', {})
 
     def raise_conf_error(self, config):
         json.dumps(config)
 
     def set_conf(self, config):
         self.raise_conf_error(config)
-        self.conf = config
+        self.conf['Dhcp4'] = config
 
     def write_conf(self):
         if self.config_file:
-            with open(self.config_file, 'rw') as f:
+            with open(self.config_file, 'w') as f:
                 json.dump(self.conf, f, indent=4)
 
 
 class DHCP4API:
     def __init__(self, url):
         self.url = url
         self.session = requests.Session()
```

### Comparing `netbox_kea_dhcp-0.0.1a1/netboxkea/kea/app.py` & `netbox_kea_dhcp-0.0.1a3/netboxkea/kea/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class DHCP4App:
 
     def __init__(self, url=None):
         if url.startswith('http://') or url.startswith('https://'):
             self.api = DHCP4API(url)
         elif url.startswith('file://'):
-            self.api = FileAPI(url.lstrip('file://'))
+            self.api = FileAPI(url.removeprefix('file://'))
         else:
             raise ValueError(
                 'Kea URL must starts either with "http(s)://" or "file://"')
         self.conf = None
         self.commit_conf = None
         self._has_commit = False
         self.auto_commit = True
```

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/devices.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/devices.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/interfaces.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/ip_addresses.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/ip_ranges.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_ranges.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/prefixes.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/prefixes.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/virtual_machines.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/fixtures/pynetbox/vminterfaces.py` & `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/vminterfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/unit/test_connector.py` & `netbox_kea_dhcp-0.0.1a3/tests/unit/test_connector.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/tests/unit/test_kea.py` & `netbox_kea_dhcp-0.0.1a3/tests/unit/test_kea.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/LICENSE` & `netbox_kea_dhcp-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a1/pyproject.toml` & `netbox_kea_dhcp-0.0.1a3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "netbox-kea-dhcp"
 dynamic = ["version"]
-authors = [{ name="François", email="francoismdj@gmx.fr" },]
+authors = [{ name="francoismdj", email="" },]
 description = "Use netbox as subnets source for ISC Kea DHCP server"
 readme = "README.md"
 requires-python = ">=3.8"
+license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
@@ -25,12 +26,18 @@
     "bottle~=0.12.25",
     "tomli >= 1.1.0 ; python_version < '3.11'"
 ]
 
 [project.urls]
 Homepage = "https://github.com/francoismdj/netbox-kea-dhcp"
 
-[tool.hatch.version]
-path = "netboxkea/__about__.py"
-
 [project.scripts]
 netbox-kea-dhcp = "netboxkea.entry_point:run"
+
+[tool.hatch.version]
+path = "src/netboxkea/__about__.py"
+
+[tool.hatch.build]
+sources = ["src"]
+
+[tool.hatch.build.force-include]
+"examples/" = "examples"
```

