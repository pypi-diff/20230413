# Comparing `tmp/n8n-0.8.0.tar.gz` & `tmp/n8n-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n8n-0.8.0.tar", last modified: Tue May  3 17:58:12 2022, max compression
+gzip compressed data, was "n8n-0.9.1.tar", last modified: Tue Jun 14 18:44:38 2022, max compression
```

## Comparing `n8n-0.8.0.tar` & `n8n-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-05-03 17:58:12.160963 n8n-0.8.0/
--rw-rw-r--   0 victor    (1000) victor    (1000)     1071 2021-09-29 07:28:11.000000 n8n-0.8.0/LICENSE
--rw-rw-r--   0 victor    (1000) victor    (1000)      453 2022-05-03 17:58:12.156963 n8n-0.8.0/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)       68 2021-09-10 12:58:45.000000 n8n-0.8.0/README.md
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-05-03 17:58:12.156963 n8n-0.8.0/n8n/
--rw-rw-r--   0 victor    (1000) victor    (1000)       76 2021-10-14 06:47:30.000000 n8n-0.8.0/n8n/__init__.py
--rw-rw-r--   0 victor    (1000) victor    (1000)    10379 2022-05-03 05:43:04.000000 n8n-0.8.0/n8n/client.py
--rw-rw-r--   0 victor    (1000) victor    (1000)      106 2021-10-20 16:42:33.000000 n8n-0.8.0/n8n/exceptions.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-05-03 17:58:12.156963 n8n-0.8.0/n8n.egg-info/
--rw-rw-r--   0 victor    (1000) victor    (1000)      453 2022-05-03 17:58:12.000000 n8n-0.8.0/n8n.egg-info/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)      234 2022-05-03 17:58:12.000000 n8n-0.8.0/n8n.egg-info/SOURCES.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)        1 2022-05-03 17:58:12.000000 n8n-0.8.0/n8n.egg-info/dependency_links.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)        1 2021-09-10 13:09:48.000000 n8n-0.8.0/n8n.egg-info/not-zip-safe
--rw-rw-r--   0 victor    (1000) victor    (1000)        9 2022-05-03 17:58:12.000000 n8n-0.8.0/n8n.egg-info/requires.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)        4 2022-05-03 17:58:12.000000 n8n-0.8.0/n8n.egg-info/top_level.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)       38 2022-05-03 17:58:12.160963 n8n-0.8.0/setup.cfg
--rw-rw-r--   0 victor    (1000) victor    (1000)      681 2022-05-03 17:57:33.000000 n8n-0.8.0/setup.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-06-14 18:44:38.502912 n8n-0.9.1/
+-rw-rw-r--   0 victor    (1000) victor    (1000)     1071 2021-09-29 07:28:11.000000 n8n-0.9.1/LICENSE
+-rw-rw-r--   0 victor    (1000) victor    (1000)      415 2022-06-14 18:44:38.502912 n8n-0.9.1/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)       68 2021-09-10 12:58:45.000000 n8n-0.9.1/README.md
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-06-14 18:44:38.502912 n8n-0.9.1/n8n/
+-rw-rw-r--   0 victor    (1000) victor    (1000)       76 2021-10-14 06:47:30.000000 n8n-0.9.1/n8n/__init__.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)    11093 2022-06-14 15:49:18.000000 n8n-0.9.1/n8n/client.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)      106 2021-10-20 16:42:33.000000 n8n-0.9.1/n8n/exceptions.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2022-06-14 18:44:38.502912 n8n-0.9.1/n8n.egg-info/
+-rw-rw-r--   0 victor    (1000) victor    (1000)      415 2022-06-14 18:44:37.000000 n8n-0.9.1/n8n.egg-info/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)      234 2022-06-14 18:44:38.000000 n8n-0.9.1/n8n.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        1 2022-06-14 18:44:38.000000 n8n-0.9.1/n8n.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        1 2021-09-10 13:09:48.000000 n8n-0.9.1/n8n.egg-info/not-zip-safe
+-rw-rw-r--   0 victor    (1000) victor    (1000)        9 2022-06-14 18:44:38.000000 n8n-0.9.1/n8n.egg-info/requires.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        4 2022-06-14 18:44:38.000000 n8n-0.9.1/n8n.egg-info/top_level.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)       38 2022-06-14 18:44:38.502912 n8n-0.9.1/setup.cfg
+-rw-rw-r--   0 victor    (1000) victor    (1000)      680 2022-06-14 18:44:16.000000 n8n-0.9.1/setup.py
```

### Comparing `n8n-0.8.0/LICENSE` & `n8n-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `n8n-0.8.0/n8n/client.py` & `n8n-0.9.1/n8n/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,52 +25,65 @@
         self._login_attempts = 0
 
     def api_url(self, is_rest=True):
         url = f"{self.protocol}://{self.host}:{self.port}"
 
         return url if not is_rest else f"{url}/rest"
 
-    def _execute(self, method, uri, data=None, is_rest=True, check_login=True):
+    def _execute(self, method, uri, data=None, is_rest=True, check_login=True,
+                 stream: bool = False, session_id: str = None):
         if check_login and not self._cookies:
             self.login()
 
         url = f"{self.api_url(is_rest)}{uri}" if uri.startswith("?") \
             else f"{self.api_url(is_rest)}/{uri}"
 
         auth = HTTPBasicAuth(self.username, self.password) \
             if self.authentication_enabled else None
 
+        if stream:
+            timeout = None
+        elif data and not stream:
+            timeout = 20
+        else:
+            timeout = 10
+
+        headers = {"sessionid": session_id} if session_id else None
+
         if data:
             resp = getattr(requests, method)(
-                url, json=data, timeout=20, auth=auth, cookies=self._cookies)
+                url, json=data, timeout=timeout, auth=auth,
+                cookies=self._cookies, stream=stream, headers=headers)
         else:
             resp = getattr(requests, method)(
-                url, timeout=10, auth=auth, cookies=self._cookies)
+                url, timeout=timeout, auth=auth, cookies=self._cookies,
+                stream=stream, headers=headers)
 
         if resp.status_code == 401 and self._login_attempts == 0:
             self._cookies = None
-            # if it fails again, it's not due the cookie
+            # if it fails again, it's not due to the cookie
             self._login_attempts = 1
             self._execute(method=method, uri=uri, data=data, is_rest=is_rest,
-                          check_login=check_login)
+                          check_login=check_login, session_id=session_id)
 
         if resp.status_code == 404:
             raise ResourceNotFoundException("Resource not Found")
 
         if resp.status_code not in [200, 201]:
             raise InvalidRequestException(
                 f"[{resp.status_code}] - {resp.json().get('message')}")
 
         return resp
 
-    def post(self, uri, data, is_rest=True):
-        return self._execute("post", uri, data, is_rest=is_rest)
+    def post(self, uri, data, is_rest=True, session_id: str = None):
+        return self._execute("post", uri, data, is_rest=is_rest,
+                             session_id=session_id)
 
-    def get(self, uri, is_rest=True, check_login=True):
-        return self._execute("get", uri, is_rest=is_rest, check_login=check_login)
+    def get(self, uri, is_rest=True, check_login=True, stream=False):
+        return self._execute("get", uri, is_rest=is_rest, check_login=check_login, stream=stream)
 
     def delete(self, uri, is_rest=True):
         return self._execute("delete", uri, is_rest=is_rest)
 
     def patch(self, uri, data: dict = None, is_rest=True):
         return self._execute("patch", uri, data=data, is_rest=is_rest)
 
@@ -236,20 +249,24 @@
     def deactivate_workflow(self, workflow_id: int):
         workflow = self.get_workflow(workflow_id)["data"]
 
         workflow["active"] = False
 
         return self.patch(f"workflows/{workflow_id}", data=workflow).json()
 
-    def update(self, workflow_id: int, nodes: list, connections: dict):
+    def update(self, workflow_id: int, nodes: list, connections: dict,
+               active: bool = None):
         workflow = self.get_workflow(workflow_id)["data"]
 
         workflow["nodes"] = nodes
         workflow["connections"] = connections
 
+        if active is not None:
+            workflow["active"] = active
+
         return self.patch(f"workflows/{workflow_id}", data=workflow).json()
 
     def add_node(self, workflow_id: int, node: dict, connections: dict = None):
         workflow = self.get_workflow(workflow_id)["data"]
 
         workflow["nodes"].append(node)
         workflow["connections"] = connections or {}
@@ -284,25 +301,26 @@
 
         workflow["nodes"] = changed_nodes
         workflow["connections"] = connections if connections is not None \
             else workflow["connections"]
 
         return self.patch(f"workflows/{workflow_id}", data=workflow).json()
 
-    def execute_node(self, workflow_id: int, node_name: str, run_data: dict):
-        workflow = self.get(f"workflows/{workflow_id}").json()["data"]
+    def execute_node(self, workflow_id: int, node_name: str, session_id: str,
+                     workflow_data: dict = None):
+        workflow_data = workflow_data \
+                       or self.get(f"workflows/{workflow_id}").json()["data"]
 
         content = {
-            "workflowData": workflow,
-            "runData": run_data,
+            "workflowData": workflow_data,
             "startNodes": [node_name],
             "destinationNode": node_name,
         }
 
-        return self.post("workflows/run", content).json()
+        return self.post("workflows/run", content, session_id=session_id).json()
 
     def delete_node(self, workflow_id: int, node_name: str, connections: dict,
                     deactivate=False):
         workflow = self.get_workflow(workflow_id)["data"]
 
         new_nodes = [
             node for node in workflow["nodes"] if node["name"] != node_name]
```

### Comparing `n8n-0.8.0/setup.py` & `n8n-0.9.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='n8n',
-    version='0.8.0',
+    version='0.9.1',
     packages=find_packages(),
     include_package_data=True,
     license='GPLv3',
     url='https://github.com/victorpantoja/n8n-client-python',
     author='Victor Pantoja',
     author_email='victor.pantoja@gmail.com',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
     ],
     install_requires=[
         "requests"
     ],
     long_description=read('README.md'),
     zip_safe=False,
 )
```

