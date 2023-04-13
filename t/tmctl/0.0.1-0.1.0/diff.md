# Comparing `tmp/tmctl-0.0.1.tar.gz` & `tmp/tmctl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmctl-0.0.1.tar", last modified: Tue Apr 11 08:20:39 2023, max compression
+gzip compressed data, was "tmctl-0.1.0.tar", last modified: Thu Apr 13 08:35:17 2023, max compression
```

## Comparing `tmctl-0.0.1.tar` & `tmctl-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 1112275  (2036082349) 1437349805        0 2023-04-11 08:20:39.061819 tmctl-0.0.1/
--rw-r--r--   0 1112275  (2036082349) 1437349805      102 2023-04-11 08:20:39.061435 tmctl-0.0.1/PKG-INFO
--rw-r--r--   0 1112275  (2036082349) 1437349805       38 2023-04-11 08:20:39.061899 tmctl-0.0.1/setup.cfg
--rw-r--r--   0 1112275  (2036082349) 1437349805      300 2023-04-11 00:39:18.000000 tmctl-0.0.1/setup.py
-drwxr-xr-x   0 1112275  (2036082349) 1437349805        0 2023-04-11 08:20:39.056882 tmctl-0.0.1/tmctl/
--rw-r--r--   0 1112275  (2036082349) 1437349805       73 2023-04-11 00:39:18.000000 tmctl-0.0.1/tmctl/__init__.py
--rw-r--r--   0 1112275  (2036082349) 1437349805    22768 2023-04-11 00:39:18.000000 tmctl-0.0.1/tmctl/controller.py
--rw-r--r--   0 1112275  (2036082349) 1437349805     2088 2023-04-11 00:39:18.000000 tmctl-0.0.1/tmctl/tmctl.py
-drwxr-xr-x   0 1112275  (2036082349) 1437349805        0 2023-04-11 08:20:39.060765 tmctl-0.0.1/tmctl.egg-info/
--rw-r--r--   0 1112275  (2036082349) 1437349805      102 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/PKG-INFO
--rw-r--r--   0 1112275  (2036082349) 1437349805      237 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/SOURCES.txt
--rw-r--r--   0 1112275  (2036082349) 1437349805        1 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/dependency_links.txt
--rw-r--r--   0 1112275  (2036082349) 1437349805       37 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/entry_points.txt
--rw-r--r--   0 1112275  (2036082349) 1437349805       21 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/requires.txt
--rw-r--r--   0 1112275  (2036082349) 1437349805        6 2023-04-11 08:20:39.000000 tmctl-0.0.1/tmctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.691391 tmctl-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 08:35:17.691391 tmctl-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:35:17.691391 tmctl-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 08:35:03.000000 tmctl-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.687390 tmctl-0.1.0/tmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27802 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/tmctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.691391 tmctl-0.1.0/tmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/top_level.txt
```

### Comparing `tmctl-0.0.1/tmctl/controller.py` & `tmctl-0.1.0/tmctl/controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 from dataclasses import dataclass
 import datetime
 import json
 import logging
+import os
 import time
 
 import requests
 import yaml
 
 
 @dataclass
 class CommonOption:
     admin_url: str
     output: str = "json"
     indent: int = 4
 
 
+@dataclass
+class CommonResponse:
+    status: bool
+    error: dict = None
+    data: dict = None
+
+
 class AdminClient(object):
-    def __init__(self, common_option: CommonOption):
+    def __init__(self, common_option: CommonOption, base_url: str = None):
         self._common_option = common_option
         self._admin_url = self._common_option.admin_url
         self._output = self._common_option.output
         self._indent = self._common_option.indent
 
-    def _extract_namespace(self, cluster):
-        settings = json.loads(cluster.get("settings", None) or {})
+        self._base_url = base_url
+
+    def _response_to_object(self, response: dict) -> CommonResponse:
+        return CommonResponse(
+            status=response.get("status", False),
+            error=response.get("error", None) or {},
+            data=response.get("data", None) or {},
+        )
+
+    def _extract_namespace(self, cluster) -> str:
+        settings = cluster.get("settings", None) or {}
         namespace = settings.get("namespace", None) or None
 
         changed_name = cluster["name"].replace("_", "-")
 
         namespace = namespace or changed_name
 
         return namespace
 
-    def _parse_proxy_service(self, yamls_str):
+    def _parse_proxy_service(self, yamls_str) -> str:
         find = False
         proxy_name = None
 
         for each in yaml.load_all(yamls_str, Loader=yaml.Loader):
             if find:
                 break
 
@@ -49,100 +66,233 @@
                 for port_spec in port_list:
                     if port_spec["port"] == 8088:
                         find = True
                         proxy_name = each["metadata"]["name"]
 
         return proxy_name
 
-    def _send_delete(self, url):
+    def _send_delete(self, url) -> bool:
         response = requests.delete(self._admin_url + url)
 
         if response.ok:
-            return True
+            logging.debug(
+                f"url: {self._admin_url + url}, response ok, {response.status_code}, {response.text}"
+            )
+            return self._response_to_object(response.json()).status
         else:
+            logging.debug(
+                f"url: {self._admin_url + url}, response not ok, {response.status_code}, {response.text}"
+            )
             return False
 
-    def _send_get(self, url, params=None):
+    def _send_get(self, url, params=None) -> CommonResponse:
         params = params or {}
         response = requests.get(self._admin_url + url, params=params)
 
         if response.ok:
-            return response.json() if response.text else None
+            return self._response_to_object(response.json())
+        else:
+            return CommonResponse(
+                status=False,
+                error={"status_code": response.status_code, "text": response.text},
+                data=None,
+            )
+
+    def _send_binary_post(self, url, file_path, form_data):
+        files = {"file": open(file_path, "rb")}
+        # data = { "name": "test_name-changed", "target_path": "/etc/trino/test/222" }
+
+        response = requests.post(self._admin_url + url, data=form_data, files=files)
+        if response.ok:
+            return self._response_to_object(response.json())
+        else:
+            raise requests.exceptions.HTTPError(response.status_code)
+
+    def _send_download(self, url, params=None):
+        # res = requests.get(url + f"/v1/files/1/download")
+        # return res.content ? or write to file?
+        response = requests.get(self._admin_url + url, params=params)
+        if response.ok:
+            return response.content
         else:
             raise requests.exceptions.HTTPError(response.status_code)
 
-    def _send_post(self, url, json_data: dict = None):
+    def _send_post(self, url, json_data: dict = None, form_data: dict = None):
         json_data = json_data or {}
-        response = requests.post(self._admin_url + url, json=json_data)
+        response = requests.post(self._admin_url + url, data=form_data, json=json_data)
 
         if response.ok:
-            return response.json() if response.text else None
+            return self._response_to_object(response.json())
         else:
+            logging.debug(response.text)
             raise requests.exceptions.HTTPError(response.status_code)
 
     def _yaml_load_all(self, filepath):
         yamls = []
 
         for each in yaml.load_all(open(filepath, "r"), Loader=yaml.Loader):
             yamls.append(each)
 
         return yamls
 
+    def delete(self, name: str, model_id: int = None):
+        delete_response = None
+        identifier = model_id or name
+        return_value = None
+
+        if model_id:
+            delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+        elif name:
+            response = self._send_get(f"{self._base_url}", params={"name": name})
+
+            if response.status:
+                models = response.data
+                if models:
+                    model = models[0]
+
+                    model_id = model["id"]
+
+                    delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+
+        if delete_response:
+            return_value = f"identifier: {identifier} is successfully deleted!"
+        else:
+            return_value = f"identifier: {identifier} does not be successfully deleted!"
+
+        return return_value
+
+    def get(self, name):
+        response = self._send_get(f"{self._base_url}", {"name": name})
+
+        if response.status:
+            for each in response.data:
+                self.print(each)
+
+    def list(self):
+        response = self._send_get(self._base_url)
+        if response.status:
+            self.print(response.data)
+
+    def ls(self):
+        return self.list()
+
     def print(self, dictionary):
         dictionary = dictionary or {}
         if self._output == "json":
             print(json.dumps(dictionary, indent=self._indent))
         elif self._output == "yaml":
             print(yaml.dump(dictionary, indent=self._indent))
 
+    def rm(self, name: str, model_id: int = None):
+        return self.delete(name, model_id)
 
-class Catalog(AdminClient):
+
+class File(AdminClient):
     def __init__(self, common_option: CommonOption):
-        super(Catalog, self).__init__(common_option)
+        super(File, self).__init__(common_option, "/v1/files")
 
-    def delete(self, name: str = None, catalog_id: int = None):
-        response = None
-        catalog_identifier = catalog_id or name
+    def download(self, name, path=None):
+        path = path or "./"
+        response = self._send_get(f"{self._base_url}", {"name": name})
 
-        if catalog_id:
-            response = self._send_delete(f"/v1/catalogs/{catalog_id}")
-        elif name:
-            catalogs = self._send_get("/v1/catalogs", params={"name": name})
+        if response.status:
+            file = response.data[0]
 
-            if catalogs:
-                catalog = catalogs[0]
+            binary = self._send_download(f"{self._base_url}/{file['id']}/download")
 
-                catalog_id = catalog["id"]
+            if binary:
+                file_path = os.path.join(path, file["file_name"])
+                with open(file_path, "wb") as _f:
+                    _f.write(binary)
 
-                response = self._send_delete(f"/v1/catalogs/{catalog_id}")
-
-        if response:
-            logging.info(f"catalog id: {catalog_identifier} is successfully deleted!")
+                self.print("download success.")
+            else:
+                self.print("empty binary")
         else:
-            logging.info(
-                f"catalog id: {catalog_identifier} does not be successfully deleted!"
-            )
+            self.print("cannot download file")
 
-        return response
+    def submit(self, path):
+        yamls = self._yaml_load_all(path)
 
-    def list(self):
-        catalogs = self._send_get("/v1/catalogs")
+        for each in yamls:
+            version = each.get("version", None)
+            action_type = each.get("type", None)
 
-        self.print(catalogs)
+            if version in ["v1/file"]:
+                file_config = each.get("file", None) or {}
+                name = file_config.get("name", None)
+                file_path = file_config.get("file_path", None)
+                target_path = file_config.get("target_path", None)
 
-    def ls(self):
-        self.list()
+                if not name:
+                    print("invalid name", name)
+                    break
 
-    def get(self, name):
-        catalogs = self._send_get("/v1/catalogs", {"name": name})
+                if action_type == "create":
+                    file_exists = os.path.exists(file_path)
+
+                    if (not file_path) or (not file_exists):
+                        print("invalid file_path", file_path)
+                        break
+
+                    response = self._send_binary_post(
+                        "/v1/files",
+                        file_path,
+                        form_data={"name": name, "target_path": target_path},
+                    )
+
+                    if response.status:
+                        self.print(response.data)
+                    else:
+                        logging.warning("file failed")
+                elif action_type == "update":
+                    file_id = file_config.get("id", None)
+
+                    if file_id:
+                        if file_path:
+                            file_exists = os.path.exists(file_path)
+
+                            if (not file_path) or (not file_exists):
+                                print("invalid file_path", file_path)
+                                break
+
+                            response = self._send_binary_post(
+                                f"/v1/files/{file_id}",
+                                file_path,
+                                form_data={
+                                    "name": name,
+                                    "target_path": target_path,
+                                },
+                            )
+                        else:
+                            response = self._send_post(
+                                f"/v1/files/{file_id}",
+                                form_data={
+                                    "name": name,
+                                    "target_path": target_path,
+                                },
+                            )
+
+                        if response.status:
+                            self.print(response.data)
+                        else:
+                            logging.warning("catalog submit failed")
 
-        if catalogs:
-            catalog = catalogs[0]
 
-            self.print(catalog)
+class Catalog(AdminClient):
+    def __init__(self, common_option: CommonOption):
+        super(Catalog, self).__init__(common_option, "/v1/catalogs")
+
+    def list(self):
+        response = self._send_get("/v1/catalogs")
+        if response.status:
+            self.print(response.data)
+
+    def ls(self):
+        self.list()
 
     def rm(self, name: str = None, catalog_id: int = None):
         return self.delete(name, catalog_id)
 
     def submit(self, path):
         yamls = self._yaml_load_all(path)
 
@@ -170,16 +320,16 @@
                         json_data={
                             "name": name,
                             "catalog_type": catalog_type,
                             "properties": properties,
                         },
                     )
 
-                    if response:
-                        self.print(response)
+                    if response.status:
+                        self.print(response.data)
                     else:
                         logging.warning("chart submit failed")
                 elif action_type == "update":
                     catalog_id = catalog_config.get("id", None)
 
                     if catalog_id:
                         response = self._send_post(
@@ -187,202 +337,197 @@
                             json_data={
                                 "name": name,
                                 "catalog_type": catalog_type,
                                 "properties": properties,
                             },
                         )
 
-                        if response:
-                            self.print(response)
+                        if response.status:
+                            self.print(response.data)
                         else:
                             logging.warning("catalog submit failed")
 
 
 class Cluster(AdminClient):
     def __init__(self, url):
-        super(Cluster, self).__init__(url)
+        super(Cluster, self).__init__(url, "/v1/clusters")
 
     def delete(self, name, force=False, refresh=1, timeout=120):
-        clusters = self._send_get("/v1/clusters", {"name": name})
+        response = self._send_get("/v1/clusters", {"name": name})
 
-        if clusters:
-            cluster = clusters[0]
-            health_check = self._helath_check_status(cluster["id"])
-
-            if health_check:
-                if force:
-                    self.off(name=name, refresh=refresh, timeout=timeout)
-                else:
-                    logging.warning("Cluster is on. please off the cluster first.")
-                    return
-
-            response = self._send_delete(f"/v1/clusters/{cluster['id']}")
-            self.print(response)
-
-    def _helath_check_status(self, cluster_id):
-        health_check = None
-
-        try:
-            health_check = self._send_get(f"/v1/clusters/{cluster_id}/gateway/health")
-        except Exception:
-            pass
+        if response.status:
+            clusters = response.data
+
+            if clusters:
+                cluster = clusters[0]
+                health_check = self._health_check_status(cluster["id"])
+
+                if health_check:
+                    if force:
+                        self.off(name=name, refresh=refresh, timeout=timeout)
+                    else:
+                        logging.warning("Cluster is on. please off the cluster first.")
+                        return
 
-        if health_check:
+            super().delete(name)
+
+    def _health_check_status(self, cluster_id):
+        response = self._send_get(f"/v1/clusters/{cluster_id}/gateway/health")
+
+        if response.status:
+            logging.debug(f"{response.data}")
             return True
         else:
             return False
 
     def _waiting_release(self, release_id, refresh, timeout):
         start_time = datetime.datetime.now(datetime.timezone.utc)
 
         response = self._send_get(f"/v1/releases/{release_id}")
         finished = False
         timeout_flag = False
+        release = response.data[0] if response.status else None
 
-        while response.get("status", "QUEUED") not in ["FINISHED", "FAILED"]:
-            self.print(response)
+        while release.get("status", "QUEUED") not in ["FINISHED", "FAILED"]:
+            time.sleep(refresh)
 
             current_time = datetime.datetime.now(datetime.timezone.utc)
 
             if (current_time - start_time).seconds > timeout:
                 timeout_flag = True
                 break
 
             response = self._send_get(f"/v1/releases/{release_id}")
-            self.print(response)
-            time.sleep(refresh)
+            release = response.data[0] if response.status else None
+            self.print(release)
 
         if timeout_flag:
             finished = False
         else:
             finished = True
 
         return finished
 
-    def _waiting_release_log(self, release_id, refresh, timeout):
+    def _waiting_and_get_release_log(self, release_id, refresh, timeout):
         start_time = datetime.datetime.now(datetime.timezone.utc)
 
         response = self._send_get(f"/v1/releases/{release_id}/log")
+        celery_response = response.data[0] if response.status else None
 
         timeout_flag = False
-        while response.get("state", "PENDING") not in ["SUCCESS", "FAILURE"]:
+        while celery_response.get("state", "PENDING") not in ["SUCCESS", "FAILURE"]:
+            time.sleep(refresh)
             current_time = datetime.datetime.now(datetime.timezone.utc)
 
             if (current_time - start_time).seconds > timeout:
                 timeout_flag = True
                 break
 
             response = self._send_get(f"/v1/releases/{release_id}/log")
-            self.print(response)
-            time.sleep(refresh)
+            celery_response = response.data[0] if response.status else None
+
+            self.print(celery_response)
 
         if timeout_flag:
             response = None
 
-        return response
+        return celery_response
 
-    def _do_install(self, cluster_id, refresh, timeout):
-        install_response = self._send_post(f"/v1/clusters/{cluster_id}/install")
+    def _execute_and_get_helm_release_log(self, url, refresh, timeout):
+        response = self._send_post(url)
+        release = response.data[0] if response.status else None
 
-        release_id = install_response["id"]
+        release_id = release["id"]
 
-        self.print(install_response)
-        release_response = self._waiting_release(release_id, refresh, timeout)
+        self.print(release)
 
-        if not release_response:
+        if not self._waiting_release(release_id, refresh, timeout):
             return None
 
-        log_response = self._waiting_release_log(release_id, refresh, timeout)
+        log_response = self._waiting_and_get_release_log(release_id, refresh, timeout)
 
         return log_response
 
-    def _do_upgrade(self, cluster_id, refresh, timeout):
-        upgarde_response = self._send_post(f"/v1/clusters/{cluster_id}/upgrade")
-
-        release_id = upgarde_response["id"]
-
-        self.print(upgarde_response)
-        release_response = self._waiting_release(release_id, refresh, timeout)
-
-        if not release_response:
-            return None
-
-        log_response = self._waiting_release_log(release_id, refresh, timeout)
+    def _do_install(self, cluster_id, refresh, timeout):
+        return self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster_id}/install", refresh, timeout
+        )
 
-        return log_response
+    def _do_upgrade(self, cluster_id, refresh, timeout):
+        return self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster_id}/upgrade", refresh, timeout
+        )
 
     def list(self):
-        clusters = self._send_get("/v1/clusters")
+        response = self._send_get(self._base_url)
 
-        for cluster in clusters:
-            cluster["settings"] = json.loads(cluster["settings"])
-            cluster["status"] = (
-                "ON" if self._helath_check_status(cluster["id"]) else "OFF"
-            )
+        if response.status:
+            clusters = response.data
 
-        self.print(clusters)
+            for cluster in clusters:
+                cluster["status"] = (
+                    "ON" if self._health_check_status(cluster["id"]) else "OFF"
+                )
+
+            self.print(clusters)
 
     def ls(self):
         self.list()
 
     def get(self, name):
-        clusters = self._send_get("/v1/clusters", {"name": name})
+        response = self._send_get("/v1/clusters", {"name": name})
 
-        if clusters:
-            cluster = clusters[0]
+        if response.status:
+            clusters = response.data
 
-            cluster["settings"] = json.loads(cluster["settings"])
-            cluster["status"] = (
-                "ON" if self._helath_check_status(cluster["id"]) else "OFF"
-            )
+            if clusters:
+                cluster = clusters[0]
+
+                cluster["status"] = (
+                    "ON" if self._health_check_status(cluster["id"]) else "OFF"
+                )
 
-            self.print(cluster)
+                self.print(cluster)
 
     def status(self, name, refresh=1, timeout=120):
         cluster = None
 
-        clusters = self._send_get("/v1/clusters", params={"name": name})
-        if clusters:
-            cluster = clusters[0]
+        response = self._send_get("/v1/clusters", params={"name": name})
 
-        if not cluster:
-            return
+        if response.status:
+            clusters = response.data
+
+            if clusters:
+                cluster = clusters[0]
 
-        cluster_response = self._send_get(f"/v1/clusters/{cluster['id']}/status")
-        if not self._waiting_release(cluster_response["id"], refresh, timeout):
-            # timeout
+        if not cluster:
             return
 
-        cluster_status_response = self._waiting_release_log(
-            cluster_response["id"], refresh, timeout
+        cluster_status_response = self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster['id']}/status", refresh, timeout
         )
 
         response_log = cluster_status_response.get("log", {}) or {}
         return_value = response_log.get("return", {}) or {}
 
         is_cluster_installed = len(return_value.get("stdout", "")) > 0
 
-        proxy_response = self._send_get(f"/v1/clusters/{cluster['id']}/proxy")
-        if not self._waiting_release(proxy_response["id"], refresh, timeout):
-            # timeout
-            return
-
-        proxy_status_response = self._waiting_release_log(
-            proxy_response["id"], refresh, timeout
+        proxy_status_response = self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster['id']}/proxy/status", refresh, timeout
         )
 
         response_log = proxy_status_response.get("log", {}) or {}
         return_value = response_log.get("return", {}) or {}
 
         is_proxy_installed = len(return_value.get("stdout", "")) > 0
 
         status = {
             "cluster installed:": is_cluster_installed,
             "proxy installed:": is_proxy_installed,
-            "cluster status (health check):": self._helath_check_status(cluster["id"]),
+            "cluster status (health check):": self._health_check_status(cluster["id"]),
         }
 
         self.print(status)
 
     def rm(self, name, force=False, refresh=1, timeout=120):
         return self.delete(name, force, refresh, timeout)
 
@@ -399,31 +544,50 @@
 
                 direct_on = cluster_config.get("direct_on", True)
 
                 chart_name = cluster_config.get("chart", None)
 
                 params = {"name": chart_name}
 
-                charts = self._send_get("/v1/charts", params=params)
+                response = self._send_get("/v1/charts", params=params)
 
-                if charts:
-                    chart_id = charts[0]["id"]
+                chart_id = None
+                if response.status:
+                    charts = response.data
+                    if charts:
+                        chart_id = charts[0]["id"]
 
-                if not chart_id:
-                    raise Exception("invalid chart options")
+                    if not chart_id:
+                        raise Exception("invalid chart options")
 
                 catalog_config = cluster_config.get("catalogs", None) or []
 
                 catalog_list = []
 
                 for catalog_name in catalog_config:
                     response = self._send_get(f"/v1/catalogs?name={catalog_name}")
 
-                    if response:
-                        catalog_list.append(response[0]["id"])
+                    if response.status:
+                        catalogs = response.data
+
+                        if catalogs:
+                            catalog_list.append(catalogs[0]["id"])
+
+                file_config = cluster_config.get("files", None) or []
+
+                file_list = []
+
+                for file_name in file_config:
+                    response = self._send_get(f"/v1/files?name={file_name}")
+
+                    if response.status:
+                        files = response.data
+
+                        if files:
+                            file_list.append(files[0]["id"])
 
                 settings = cluster_config.get("settings", None) or {}
 
                 if not name:
                     print("invalid name", name)
                     break
 
@@ -434,60 +598,73 @@
                 if action_type == "create":
                     response = self._send_post(
                         "/v1/clusters",
                         json_data={
                             "name": name,
                             "chart_id": chart_id,
                             "catalog_list": catalog_list,
+                            "file_list": file_list,
                             "settings": settings,
                         },
                     )
 
-                    if response:
-                        response["settings"] = json.loads(response["settings"])
-                        self.print(response)
-                        if direct_on:
-                            self.on(cluster_id=response["id"], is_update=False)
+                    if response.status:
+                        clusters = response.data
+
+                        if clusters:
+                            cluster = clusters[0]
+                            self.print(cluster)
+                            if direct_on:
+                                self.on(cluster_id=cluster["id"], is_update=False)
                     else:
                         logging.warning("cluster submit failed")
                 elif action_type == "update":
                     cluster_id = cluster_config.get("id", None)
 
                     if cluster_id:
                         response = self._send_post(
                             f"/v1/clusters/{cluster_id}",
                             json_data={
                                 "name": name,
                                 "chart_id": chart_id,
                                 "catalog_list": catalog_list,
+                                "file_list": file_list,
                                 "settings": settings,
                             },
                         )
 
-                        if response:
-                            response["settings"] = json.loads(response["settings"])
-                            self.print(response)
-                            if direct_on:
-                                self.on(cluster_id=cluster_id, is_update=True)
+                        if response.status:
+                            clusters = response.data
+
+                            if clusters:
+                                cluster = clusters[0]
+                                self.print(cluster)
+                                if direct_on:
+                                    self.on(cluster_id=cluster_id, is_update=True)
                         else:
                             logging.warning("cluster submit failed")
                     else:
                         logging.warning("cluster id is unknown.")
 
     def on(self, name=None, cluster_id=None, is_update=False, refresh=1, timeout=120):
         cluster = None
         cluster_identifer = name or cluster_id
 
         if cluster_id:
-            cluster = self._send_get(f"/v1/clusters/{cluster_id}")
-        if name:
-            clusters = self._send_get("/v1/clusters", params={"name": name})
+            response = self._send_get(f"/v1/clusters/{cluster_id}")
 
-            if clusters:
-                cluster = clusters[0]
+            if response.status:
+                cluster = response.data[0]
+        elif name:
+            response = self._send_get("/v1/clusters", params={"name": name})
+
+            if response.status:
+                clusters = response.data
+                if clusters:
+                    cluster = clusters[0]
 
         if not cluster:
             logging.warning(f"cluster: {cluster_identifer} is invalid")
             return
 
         cluster_id = cluster["id"]
         namespace_name = self._extract_namespace(cluster)
@@ -507,24 +684,17 @@
             logging.info("cluster install is succeeded!")
             logging.info("try to register proxy to api gateway...")
         else:
             logging.warning(response_log)
             logging.warning("cluster install failed")
             return
 
-        proxy_release = self._send_get(f"/v1/clusters/{cluster_id}/proxy/manifest")
-        proxy_release_id = proxy_release["id"]
-
-        proxy_manifest_ended = self._waiting_release(proxy_release_id, refresh, timeout)
-
-        if not proxy_manifest_ended:
-            logging.warning("getting cluster proxy information is failed")
-            return None
-
-        proxy_manifest = self._waiting_release_log(proxy_release_id, refresh, timeout)
+        proxy_manifest = self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster_id}/proxy/manifest", refresh, timeout
+        )
 
         if not proxy_manifest:
             logging.warning("getting cluster proxy information is failed")
             return None
 
         response_log = proxy_manifest.get("log", {}) or {}
         return_value = response_log.get("return", {}) or {}
@@ -546,85 +716,48 @@
 
         logging.info(response)
 
     def off(self, name=None, cluster_id=None, refresh=1, timeout=120):
         cluster = None
 
         if cluster_id:
-            cluster = self._send_get(f"/v1/clusters/{cluster_id}")
+            response = self._send_get(f"/v1/clusters/{cluster_id}")
+
+            if response.status:
+                cluster = response.data[0]
         if name:
-            clusters = self._send_get("/v1/clusters", params={"name": name})
+            response = self._send_get("/v1/clusters", params={"name": name})
 
-            if clusters:
-                cluster = clusters[0]
+            if response.status:
+                clusters = response.data
+                if clusters:
+                    cluster = clusters[0]
 
         if not cluster:
             logging.warning("cluster id or name is invalid")
             return
 
         cluster_id = cluster["id"]
 
         response = self._send_delete(f"/v1/clusters/{cluster_id}/gateway/deregister")
         logging.info(response)
 
-        response = self._send_post(f"/v1/clusters/{cluster_id}/uninstall")
-
-        uninstall_response = self._waiting_release(response["id"], refresh, timeout)
+        uninstall_response = self._execute_and_get_helm_release_log(
+            f"/v1/clusters/{cluster_id}/uninstall", refresh, timeout
+        )
 
         if not uninstall_response:
-            logging.warning("cluster uninstall is failed")
+            self.print("cluster uninstall is failed")
         else:
-            logging.info("cluster uninstall is succeeded!")
+            self.print("cluster uninstall is succeeded!")
 
 
 class HelmChart(AdminClient):
     def __init__(self, url):
-        super(HelmChart, self).__init__(url)
-
-    def delete(self, name: str = None, chart_id: int = None):
-        response = None
-        chart_identifier = chart_id or name
-
-        if chart_id:
-            response = self._send_delete(f"/v1/charts/{chart_id}")
-        elif name:
-            chart = self._send_get("/v1/charts", params={"name": name})
-
-            if chart:
-                chart_id = chart[0]["id"]
-
-                response = self._send_delete(f"/v1/charts/{chart_id}")
-
-        if response:
-            logging.info(f"chart id: {chart_identifier} is successfully deleted!")
-        else:
-            logging.info(
-                f"chart id: {chart_identifier} does not be successfully deleted!"
-            )
-
-        return response
-
-    def get(self, name):
-        charts = self._send_get("/v1/charts", {"name": name})
-
-        if charts:
-            chart = charts[0]
-            chart["registry"] = json.loads(chart["registry"])
-            chart["repository"] = json.loads(chart["repository"])
-
-            self.print(charts)
-
-    def list(self):
-        helm_charts = self._send_get("/v1/charts")
-
-        for chart in helm_charts:
-            chart["registry"] = json.loads(chart["registry"])
-            chart["repository"] = json.loads(chart["repository"])
-
-        self.print(helm_charts)
+        super(HelmChart, self).__init__(url, "/v1/charts")
 
     def ls(self):
         self.list()
 
     def rm(self, name: str = None, chart_id: int = None):
         return self.delete(name, chart_id)
 
@@ -636,16 +769,17 @@
             action_type = each.get("type", None)
 
             if version in ["v1/chart"]:
                 chart_config = each.get("chart", None) or {}
                 name = chart_config.get("name", None)
                 chart_name = chart_config.get("chart_name", None)
                 chart_version = chart_config.get("version", None)
-                registry = chart_config.get("registry", None) or {}
-                repository = chart_config.get("repository", None) or {}
+                registry = chart_config.get("registry", None)
+                repository = chart_config.get("repository", None)
+                values = chart_config.get("values", None)
 
                 if not name:
                     print("invalid name", name)
                     break
 
                 if not chart_name:
                     print("invalid chart name", chart_name)
@@ -656,21 +790,20 @@
                         "/v1/charts",
                         json_data={
                             "name": name,
                             "chart_name": chart_name,
                             "version": chart_version,
                             "registry": registry,
                             "repository": repository,
+                            "values": values,
                         },
                     )
 
-                    if response:
-                        response["registry"] = json.loads(response["registry"])
-                        response["repository"] = json.loads(response["repository"])
-                        self.print(response)
+                    if response.status:
+                        self.print(response.data[0])
                     else:
                         logging.warning("chart submit failed")
                 elif action_type == "update":
                     chart_id = chart_config.get("id", None)
 
                     if chart_id:
                         response = self._send_post(
@@ -680,13 +813,11 @@
                                 "chart_name": chart_name,
                                 "version": chart_version,
                                 "registry": registry,
                                 "repository": repository,
                             },
                         )
 
-                        if response:
-                            response["registry"] = json.loads(response["registry"])
-                            response["repository"] = json.loads(response["repository"])
-                            self.print(response)
+                        if response.status:
+                            self.print(response.data[0])
                         else:
                             logging.warning("chart submit failed")
```

### Comparing `tmctl-0.0.1/tmctl/tmctl.py` & `tmctl-0.1.0/tmctl/tmctl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import fire
 import logging
 import yaml
 
-from .controller import CommonOption, Catalog, Cluster, HelmChart
+from .controller import CommonOption, Catalog, Cluster, File, HelmChart
 
 
 class TMCtl(object):
     """Class Documentation"""
 
     def __init__(
         self, url=None, output=None, indent=4, log_level="WARNING", verbose=False
@@ -21,14 +21,15 @@
         indent = indent or 4
 
         common_option = CommonOption(admin_url=admin_url, output=output, indent=indent)
 
         self.catalog = Catalog(common_option)
         self.cluster = Cluster(common_option)
         self.helm_chart = HelmChart(common_option)
+        self.file = File(common_option)
 
         log_config = self._config.get("logging", None) or {}
         self._init_logging(log_config, log_level, verbose)
 
     def _init_config(self):
         config = None
         try:
```

