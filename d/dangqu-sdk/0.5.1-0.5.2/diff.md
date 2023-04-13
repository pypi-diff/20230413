# Comparing `tmp/dangqu-sdk-0.5.1.tar.gz` & `tmp/dangqu-sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dangqu-sdk-0.5.1.tar", last modified: Mon Apr  3 03:02:42 2023, max compression
+gzip compressed data, was "dangqu-sdk-0.5.2.tar", last modified: Thu Apr 13 03:19:19 2023, max compression
```

## Comparing `dangqu-sdk-0.5.1.tar` & `dangqu-sdk-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 03:02:42.329662 dangqu-sdk-0.5.1/
--rw-rw-rw-   0        0        0      474 2023-04-03 03:02:42.328664 dangqu-sdk-0.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 03:02:42.320686 dangqu-sdk-0.5.1/dangqu_sdk/
--rw-rw-rw-   0        0        0       57 2023-04-03 02:36:01.000000 dangqu-sdk-0.5.1/dangqu_sdk/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-04-03 02:36:01.000000 dangqu-sdk-0.5.1/dangqu_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:02:42.327691 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/
--rw-rw-rw-   0        0        0      474 2023-04-03 03:02:42.000000 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-03 03:02:42.000000 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 03:02:42.000000 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-03 03:02:42.000000 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-03 03:02:42.000000 dangqu-sdk-0.5.1/dangqu_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 03:02:42.329662 dangqu-sdk-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-03 03:02:38.000000 dangqu-sdk-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.891060 dangqu-sdk-0.5.2/
+-rw-rw-rw-   0        0        0      474 2023-04-13 03:19:19.890061 dangqu-sdk-0.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.878067 dangqu-sdk-0.5.2/dangqu_sdk/
+-rw-rw-rw-   0        0        0       57 2023-04-03 02:36:01.000000 dangqu-sdk-0.5.2/dangqu_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-04-13 03:18:51.000000 dangqu-sdk-0.5.2/dangqu_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.888042 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:19:19.891060 dangqu-sdk-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-13 03:18:51.000000 dangqu-sdk-0.5.2/setup.py
```

### Comparing `dangqu-sdk-0.5.1/dangqu_sdk/client.py` & `dangqu-sdk-0.5.2/dangqu_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return wrapped
 
 
 class DangquSdk:
 
     def __init__(self, domain, token_url, client_id, client_secret):
         self.doamin = domain
-        self.logical_url = f'{domain}/apis/tenancy/api/app/workflowinstance'
+        self.logical_url = f'{domain}/openapis/api/Workflow/Workflow/WorkflowInstance'
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.token_url = token_url
 
         self.client = BackendApplicationClient(client_id=client_id)
         self.oauth = OAuth2Session(client=self.client)
@@ -45,18 +45,19 @@
         token = self.oauth.fetch_token(
             token_url=self.token_url,
             client_id=self.client_id,
             client_secret=self.client_secret
         )
         return token
 
-    def execute_dangqu_request(self, unified_id: str, request_body: dict):
+    def execute_dangqu_request(self, host_tenant: str, unified_id: str, request_body: dict):
         body = {
             "isSync"            : True,
             "isReturnResult"    : True,
+            "hostTenant"        : host_tenant,
             "unifiedId"         : unified_id,
             "inputParameterJson": json.dumps(request_body)
         }
 
         _headers = {'Authorization': 'Bearer %s' % self.token}
         response = requests.post(self.logical_url, headers=_headers, json=body)
```

### Comparing `dangqu-sdk-0.5.1/setup.py` & `dangqu-sdk-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dangqu-sdk',
-    version='0.5.1',
+    version='0.5.2',
     description='dangqu sdk',
     author='ZhaoHui',
     author_email='myemail@example.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'oauthlib',
```

