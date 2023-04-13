# Comparing `tmp/ayon-python-api-0.1.8.tar.gz` & `tmp/ayon-python-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.1.8.tar", last modified: Fri Jan 20 15:56:53 2023, max compression
+gzip compressed data, was "ayon-python-api-0.1.9.tar", last modified: Fri Jan 27 20:30:24 2023, max compression
```

## Comparing `ayon-python-api-0.1.8.tar` & `ayon-python-api-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 15:56:53.854510 ayon-python-api-0.1.8/
--rw-rw-rw-   0        0        0    11558 2022-04-28 15:40:50.000000 ayon-python-api-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1877 2023-01-20 15:56:53.854149 ayon-python-api-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1233 2023-01-10 17:48:41.000000 ayon-python-api-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 15:56:53.817677 ayon-python-api-0.1.8/ayon_api/
--rw-rw-rw-   0        0        0     4059 2023-01-20 15:39:24.000000 ayon-python-api-0.1.8/ayon_api/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/constants.py
--rw-rw-rw-   0        0        0    52144 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/entity_hub.py
--rw-rw-rw-   0        0        0     2992 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/events.py
--rw-rw-rw-   0        0        0     2576 2023-01-20 15:39:24.000000 ayon-python-api-0.1.8/ayon_api/exceptions.py
--rw-rw-rw-   0        0        0    24216 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/graphql.py
--rw-rw-rw-   0        0        0    11497 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/graphql_queries.py
--rw-rw-rw-   0        0        0    23308 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/operations.py
--rw-rw-rw-   0        0        0    92054 2023-01-20 15:39:24.000000 ayon-python-api-0.1.8/ayon_api/server.py
--rw-rw-rw-   0        0        0    15272 2023-01-20 15:39:24.000000 ayon-python-api-0.1.8/ayon_api/server_api.py
--rw-rw-rw-   0        0        0     7075 2023-01-18 15:06:41.000000 ayon-python-api-0.1.8/ayon_api/thumbnails.py
--rw-rw-rw-   0        0        0    11553 2023-01-20 15:39:24.000000 ayon-python-api-0.1.8/ayon_api/utils.py
--rw-rw-rw-   0        0        0       74 2023-01-20 15:42:19.000000 ayon-python-api-0.1.8/ayon_api/version.py
-drwxrwxrwx   0        0        0        0 2023-01-20 15:56:53.852781 ayon-python-api-0.1.8/ayon_python_api.egg-info/
--rw-rw-rw-   0        0        0     1877 2023-01-20 15:56:53.000000 ayon-python-api-0.1.8/ayon_python_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-01-20 15:56:53.000000 ayon-python-api-0.1.8/ayon_python_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       64 2023-01-20 15:56:53.000000 ayon-python-api-0.1.8/ayon_python_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-01-20 15:56:53.000000 ayon-python-api-0.1.8/ayon_python_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-20 15:56:53.000000 ayon-python-api-0.1.8/ayon_python_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      454 2023-01-20 15:42:24.000000 ayon-python-api-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-20 15:56:53.855126 ayon-python-api-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-01-17 16:38:50.000000 ayon-python-api-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.903319 ayon-python-api-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2022-04-28 15:40:50.000000 ayon-python-api-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1877 2023-01-27 20:30:24.902459 ayon-python-api-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1233 2023-01-10 17:48:41.000000 ayon-python-api-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.889407 ayon-python-api-0.1.9/ayon_api/
+-rw-rw-rw-   0        0        0     4253 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/constants.py
+-rw-rw-rw-   0        0        0    52144 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/entity_hub.py
+-rw-rw-rw-   0        0        0     2992 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/events.py
+-rw-rw-rw-   0        0        0     2576 2023-01-20 15:39:24.000000 ayon-python-api-0.1.9/ayon_api/exceptions.py
+-rw-rw-rw-   0        0        0    24216 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/graphql.py
+-rw-rw-rw-   0        0        0    11497 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/graphql_queries.py
+-rw-rw-rw-   0        0        0    23308 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/operations.py
+-rw-rw-rw-   0        0        0    92141 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/server.py
+-rw-rw-rw-   0        0        0    16725 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/server_api.py
+-rw-rw-rw-   0        0        0     7075 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/thumbnails.py
+-rw-rw-rw-   0        0        0    11553 2023-01-20 15:39:24.000000 ayon-python-api-0.1.9/ayon_api/utils.py
+-rw-rw-rw-   0        0        0       74 2023-01-27 20:26:14.000000 ayon-python-api-0.1.9/ayon_api/version.py
+drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.901553 ayon-python-api-0.1.9/ayon_python_api.egg-info/
+-rw-rw-rw-   0        0        0     1877 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      387 2023-01-27 20:28:07.000000 ayon-python-api-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-27 20:30:24.903319 ayon-python-api-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-01-27 20:26:06.000000 ayon-python-api-0.1.9/setup.py
```

### Comparing `ayon-python-api-0.1.8/LICENSE` & `ayon-python-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/PKG-INFO` & `ayon-python-api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Description: # AYON server API
         Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
```

### Comparing `ayon-python-api-0.1.8/README.md` & `ayon-python-api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/__init__.py` & `ayon-python-api-0.1.9/ayon_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from .server_api import (
     ServerAPI,
     ServiceContext,
 
     init_service,
 
+    is_connection_created,
+    close_connection,
+    change_token,
+    set_environments,
     get_server_api_connection,
 
     get_base_url,
     get_rest_url,
 
     raw_get,
     raw_post,
@@ -112,14 +116,18 @@
 
     "ServerAPIBase",
 
     "ServerAPI",
     "ServiceContext",
     "init_service",
 
+    "is_connection_created",
+    "close_connection",
+    "change_token",
+    "set_environments",
     "get_server_api_connection",
 
     "get_base_url",
     "get_rest_url",
 
     "raw_get",
     "raw_post",
```

### Comparing `ayon-python-api-0.1.8/ayon_api/constants.py` & `ayon-python-api-0.1.9/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/entity_hub.py` & `ayon-python-api-0.1.9/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/events.py` & `ayon-python-api-0.1.9/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/exceptions.py` & `ayon-python-api-0.1.9/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/graphql.py` & `ayon-python-api-0.1.9/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/graphql_queries.py` & `ayon-python-api-0.1.9/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/operations.py` & `ayon-python-api-0.1.9/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/server.py` & `ayon-python-api-0.1.9/ayon_api/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,15 +603,15 @@
             ("status", status),
             ("description", description),
             ("summary", summary),
             ("payload", payload),
         ):
             if value is not None:
                 kwargs[key] = value
-        response = self.put(
+        response = self.patch(
             "events/{}".format(event_id),
             **kwargs
         )
         response.raise_for_status()
 
     def dispatch_event(
         self,
@@ -1012,16 +1012,15 @@
                 code.
         """
 
         endpoint = "addons"
         if details:
             endpoint += "?details=1"
         response = self.get(endpoint)
-        if response.status != 200:
-            raise ServerError(response.text)
+        response.raise_for_status()
         return response.data
 
     def download_addon_private_file(
         self,
         addon_name,
         addon_version,
         filename,
@@ -1229,28 +1228,26 @@
             return full_settings
         return full_settings["settings"]
 
     def get_addon_studio_settings(self, addon_name, addon_version):
         result = self.get(
             "addons/{}/{}/settings".format(addon_name, addon_version)
         )
-        if result.status != 200:
-            raise ServerError(result.text)
+        result.raise_for_status()
         return result.data
 
     def get_addon_project_settings(
         self, addon_name, addon_version, project_name
     ):
         result = self.get(
             "addons/{}/{}/settings/{}".format(
                 addon_name, addon_version, project_name
             )
         )
-        if result.status != 200:
-            raise ServerError(result.text)
+        result.raise_for_status()
         return result.data
 
     def get_addon_settings(self, addon_name, addon_version, project_name=None):
         if project_name is None:
             return self.get_addon_studio_settings(addon_name, addon_version)
         return self.get_addon_project_settings(
             addon_name, addon_version, project_name
@@ -1283,15 +1280,15 @@
         Args:
             active (bool): Filter active/inactive projects. Both are returned
                 if 'None' is passed.
             library (bool): Filter standard/library projects. Both are
                 returned if 'None' is passed.
 
         Returns:
-            List[Dict[str, Any]]: List of available projects.
+            Generator[Dict[str, Any]]: Available projects.
         """
 
         for project_name in self.get_project_names(active, library):
             project = self.get_rest_project(project_name)
             if project:
                 yield project
 
@@ -1346,16 +1343,15 @@
         if query_keys:
             query = "?{}".format(",".join([
                 "{}={}".format(key, value)
                 for key, value in query_keys.items()
             ]))
 
         response = self.get("projects{}".format(query), **query_keys)
-        # TODO check status
-        response.status
+        response.raise_for_status()
         data = response.data
         project_names = []
         if data:
             for project in data["projects"]:
                 project_names.append(project["name"])
         return project_names
 
@@ -1371,15 +1367,15 @@
                 disabled when 'None' is passed.
             fields (Union[Iterable[str], None]): fields to be queried
                 for project.
             own_attributes (bool): Attribute values that are not explicitly set
                 on entity will have 'None' value.
 
         Returns:
-            List[Dict[str, Any]]: List of queried projects.
+            Generator[Dict[str, Any]]: Queried projects.
         """
 
         if fields is None:
             use_rest = True
         else:
             use_rest = False
             fields = set(fields)
@@ -1480,45 +1476,45 @@
             active (Union[bool, None]): Filter active/inactive folders.
                 Both are returned if is set to None.
             fields (Union[Iterable[str], None]): Fields to be queried for
                 folder. All possible folder fields are returned
                 if 'None' is passed.
 
         Returns:
-            Iterable[dict[str, Any]]: Queried folder entities.
+            Generator[dict[str, Any]]: Queried folder entities.
         """
 
         if not project_name:
-            return []
+            return
 
         filters = {
             "projectName": project_name
         }
         if folder_ids is not None:
             folder_ids = set(folder_ids)
             if not folder_ids:
-                return []
+                return
             filters["folderIds"] = list(folder_ids)
 
         if folder_paths is not None:
             folder_paths = set(folder_paths)
             if not folder_paths:
-                return []
+                return
             filters["folderPaths"] = list(folder_paths)
 
         if folder_names is not None:
             folder_names = set(folder_names)
             if not folder_names:
-                return []
+                return
             filters["folderNames"] = list(folder_names)
 
         if parent_ids is not None:
             parent_ids = set(parent_ids)
             if not parent_ids:
-                return []
+                return
             if None in parent_ids:
                 # Replace 'None' with '"root"' which is used during GraphQl
                 #   query for parent ids filter for folders without folder
                 #   parent
                 parent_ids.remove(None)
                 parent_ids.add("root")
 
@@ -1571,42 +1567,42 @@
         task_types=None,
         folder_ids=None,
         active=True,
         fields=None,
         own_attributes=False
     ):
         if not project_name:
-            return []
+            return
 
         filters = {
             "projectName": project_name
         }
 
         if task_ids is not None:
             task_ids = set(task_ids)
             if not task_ids:
-                return []
+                return
             filters["taskIds"] = list(task_ids)
 
         if task_names is not None:
             task_names = set(task_names)
             if not task_names:
-                return []
+                return
             filters["taskNames"] = list(task_names)
 
         if task_types is not None:
             task_types = set(task_types)
             if not task_types:
-                return []
+                return
             filters["taskTypes"] = list(task_types)
 
         if folder_ids is not None:
             folder_ids = set(folder_ids)
             if not folder_ids:
-                return []
+                return
             filters["folderIds"] = list(folder_ids)
 
         if not fields:
             fields = self.get_default_fields_for_type("task")
 
         fields = set(fields)
 
@@ -1756,58 +1752,72 @@
         parsed_data = query.query(self)
         folders = parsed_data["project"]["folders"]
         return {
             folder["id"]
             for folder in folders
         }
 
+    def _filter_subset(
+        self, project_name, subset, active, own_attributes, use_rest
+    ):
+        if active is not None and subset["active"] is not active:
+            return None
+
+        if use_rest:
+            subset = self.get_rest_subset(project_name, subset["id"])
+
+        if own_attributes:
+            fill_own_attribs(subset)
+
+        return subset
+
     def get_subsets(
         self,
         project_name,
         subset_ids=None,
         subset_names=None,
         folder_ids=None,
         names_by_folder_ids=None,
         active=True,
         fields=None,
         own_attributes=False
     ):
         if not project_name:
-            return []
+            return
 
         if subset_ids is not None:
             subset_ids = set(subset_ids)
             if not subset_ids:
-                return []
+                return
 
         filter_subset_names = None
         if subset_names is not None:
             filter_subset_names = set(subset_names)
             if not filter_subset_names:
-                return []
+                return
 
         filter_folder_ids = None
         if folder_ids is not None:
             filter_folder_ids = set(folder_ids)
             if not filter_folder_ids:
-                return []
+                return
 
         # This will disable 'folder_ids' and 'subset_names' filters
         #   - maybe could be enhanced in future?
         if names_by_folder_ids is not None:
             filter_subset_names = set()
             filter_folder_ids = set()
 
             for folder_id, names in names_by_folder_ids.items():
                 if folder_id and names:
                     filter_folder_ids.add(folder_id)
                     filter_subset_names |= set(names)
 
             if not filter_subset_names or not filter_folder_ids:
-                return []
+                return
 
         # Convert fields and add minimum required fields
         if fields:
             fields = set(fields) | {"id"}
         else:
             fields = self.get_default_fields_for_type("subset")
 
@@ -1843,43 +1853,38 @@
         query = subsets_graphql_query(fields)
         for attr, filter_value in filters.items():
             query.set_variable_value(attr, filter_value)
 
         parsed_data = query.query(self)
 
         subsets = parsed_data.get("project", {}).get("subsets", [])
-        if active is not None or own_attributes:
-            _subsets = []
-            for subset in subsets:
-                if active is not None and subset["active"] is not active:
-                    continue
-
-                if use_rest:
-                    subset = self.get_rest_subset(project_name, subset["id"])
-
-                if own_attributes:
-                    fill_own_attribs(subset)
-                _subsets.append(subset)
-            subsets = _subsets
-
         # Filter subsets by 'names_by_folder_ids'
         if names_by_folder_ids:
             subsets_by_folder_id = collections.defaultdict(list)
             for subset in subsets:
-                folder_id = subset["folderId"]
-                subsets_by_folder_id[folder_id].append(subset)
+                filtered_subset = self._filter_subset(
+                    project_name, subset, active, own_attributes, use_rest
+                )
+                if filtered_subset is not None:
+                    folder_id = filtered_subset["folderId"]
+                    subsets_by_folder_id[folder_id].append(filtered_subset)
 
-            filtered_subsets = []
             for folder_id, names in names_by_folder_ids.items():
                 for folder_subset in subsets_by_folder_id[folder_id]:
                     if folder_subset["name"] in names:
-                        filtered_subsets.append(subset)
-            subsets = filtered_subsets
+                        yield folder_subset
+
+        else:
+            for subset in subsets:
+                filtered_subset = self._filter_subset(
+                    project_name, subset, active, own_attributes, use_rest
+                )
+                if filtered_subset is not None:
+                    yield filtered_subset
 
-        return list(subsets)
 
     def get_subset_by_id(
         self,
         project_name,
         subset_id,
         fields=None,
         own_attributes=False
@@ -1968,15 +1973,15 @@
                 This can be combined only with 'standard' attribute
                 set to True.
             fields (Union[Iterable[str], None]): Fields to be queried
                 for version. All possible folder fields are returned
                 if 'None' is passed.
 
         Returns:
-            List[Dict[str, Any]]: Queried version entities.
+            Generator[Dict[str, Any]]: Queried version entities.
         """
 
         if not fields:
             fields = self.get_default_fields_for_type("version")
         fields = set(fields)
 
         if active is not None:
@@ -1995,32 +2000,32 @@
 
         filters = {
             "projectName": project_name
         }
         if version_ids is not None:
             version_ids = set(version_ids)
             if not version_ids:
-                return []
+                return
             filters["versionIds"] = list(version_ids)
 
         if subset_ids is not None:
             subset_ids = set(subset_ids)
             if not subset_ids:
-                return []
+                return
             filters["subsetIds"] = list(subset_ids)
 
         # TODO versions can't be used as fitler at this moment!
         if versions is not None:
             versions = set(versions)
             if not versions:
-                return []
+                return
             filters["versions"] = list(versions)
 
         if not hero and not standard:
-            return []
+            return
 
         queries = []
         # Add filters based on 'hero' and 'standard'
         # NOTE: There is not a filter to "ignore" hero versions or to get
         #   latest and hero version
         # - if latest and hero versions should be returned it must be done in
         #       2 graphql queries
@@ -2281,15 +2286,15 @@
             active (bool): Receive active/inactive representaions. All are
                 returned when 'None' is passed.
             fields (Union[Iterable[str], None]): Fields to be queried for
                 representation. All possible fields are returned if 'None' is
                 passed.
 
         Returns:
-            List[Dict[str, Any]]: Queried representation entities.
+            Generator[Dict[str, Any]]: Queried representation entities.
         """
 
         if not fields:
             fields = self.get_default_fields_for_type("representation")
         fields = set(fields)
 
         use_rest = False
@@ -2306,39 +2311,39 @@
         filters = {
             "projectName": project_name
         }
 
         if representation_ids is not None:
             representation_ids = set(representation_ids)
             if not representation_ids:
-                return []
+                return
             filters["representationIds"] = list(representation_ids)
 
         version_ids_filter = None
         representaion_names_filter = None
         if names_by_version_ids is not None:
             version_ids_filter = set()
             representaion_names_filter = set()
             for version_id, names in names_by_version_ids.items():
                 version_ids_filter.add(version_id)
                 representaion_names_filter |= set(names)
 
             if not version_ids_filter or not representaion_names_filter:
-                return []
+                return
 
         else:
             if representation_names is not None:
                 representaion_names_filter = set(representation_names)
                 if not representaion_names_filter:
-                    return []
+                    return
 
             if version_ids is not None:
                 version_ids_filter = set(version_ids)
                 if not version_ids_filter:
-                    return []
+                    return
 
         if version_ids_filter:
             filters["versionIds"] = list(version_ids_filter)
 
         if representaion_names_filter:
             filters["representationNames"] = list(representaion_names_filter)
 
@@ -2455,27 +2460,27 @@
         fields=None,
         own_attributes=False
     ):
         filters = {"projectName": project_name}
         if task_ids is not None:
             task_ids = set(task_ids)
             if not task_ids:
-                return []
+                return
             filters["taskIds"] = list(task_ids)
 
         if paths is not None:
             paths = set(paths)
             if not paths:
-                return []
+                return
             filters["paths"] = list(paths)
 
         if workfile_ids is not None:
             workfile_ids = set(workfile_ids)
             if not workfile_ids:
-                return []
+                return
             filters["workfileIds"] = list(workfile_ids)
 
         if not fields:
             fields = DEFAULT_WORKFILE_INFO_FIELDS
         fields = set(fields)
         if own_attributes:
             fields.add("ownAttrib")
@@ -2845,8 +2850,9 @@
                 operation_id = op_result["id"]
                 raise FailedOperations((
                     "Operation \"{}\" failed with data:\n{}\nError: {}."
                 ).format(
                     operation_id,
                     json.dumps(body_by_id[operation_id], indent=4),
                     op_result["error"],
-                ))
+                ))
+
```

### Comparing `ayon-python-api-0.1.8/ayon_api/server_api.py` & `ayon-python-api-0.1.9/ayon_api/server_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,35 @@
     Goal is to avoid create connection on import which can be dangerous in
     some cases.
     """
 
     _connection = None
 
     @classmethod
+    def is_connection_created(cls):
+        return cls._connection is not None
+
+    @classmethod
+    def change_token(cls, url, token):
+        ServerAPI.set_environments(url, token)
+        if cls._connection is None:
+            return
+
+        if cls._connection.get_base_url() == url:
+            cls._connection.set_token(token)
+        else:
+            cls.close_connection()
+
+    @classmethod
+    def close_connection(cls):
+        if cls._connection is not None:
+            cls._connection.close_session()
+        cls._connection = None
+
+    @classmethod
     def get_server_api_connection(cls):
         if cls._connection is None:
             cls._connection = ServerAPI()
         return cls._connection
 
 
 class ServiceContext:
@@ -146,28 +167,67 @@
         cls.token = token
         cls.server_url = server_url
         cls.addon_name = addon_name
         cls.addon_version = addon_version
         cls.service_name = service_name or socket.gethostname()
 
         # Make sure required environments for ServerAPI are set
-        os.environ["AYON_SERVER_URL"] = cls.server_url
-        os.environ["AYON_TOKEN"] = cls.token
+        ServerAPI.set_environments(cls.server_url, cls.token)
 
         if connect:
             print("Connecting to server \"{}\"".format(server_url))
             con = GlobalContext.get_server_api_connection()
             user = con.get_user()
             print("Logged in as user \"{}\"".format(user["name"]))
 
 
 def init_service(*args, **kwargs):
     ServiceContext.init_service(*args, **kwargs)
 
 
+def is_connection_created():
+    """Is global connection created.
+
+    Returns:
+        bool: True if connection was connected.
+    """
+
+    return GlobalContext.is_connection_created()
+
+
+def close_connection():
+    """Close global connection if is connected."""
+
+    GlobalContext.close_connection()
+
+
+def change_token(url, token):
+    """Change connection token for url.
+
+    This function can be also used to change url.
+
+    Args:
+        url (str): Server url.
+        token (str): API key token.
+    """
+
+    GlobalContext.change_token(url, token)
+
+
+def set_environments(url, token):
+    """Set global environments for global connection.
+
+    Args:
+        url (Union[str, None]): Url to server or None to unset environments.
+        token (Union[str, None]): API key token to be used for connection.
+    """
+
+    ServerAPI.set_environments(url, token)
+
+
 def get_server_api_connection():
     """Access to global scope object of ServerAPI.
 
     This access expect to have set environment variables 'AYON_SERVER_URL'
     and 'AYON_TOKEN'.
 
     Returns:
@@ -240,15 +300,15 @@
 def get_event(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_event(*args, **kwargs)
 
 
 def dispatch_event(*args, **kwargs):
     con = get_server_api_connection()
-    return con.get_event(*args, **kwargs)
+    return con.dispatch_event(*args, **kwargs)
 
 
 def update_event(*args, **kwargs):
     con = get_server_api_connection()
     return con.update_event(*args, **kwargs)
```

### Comparing `ayon-python-api-0.1.8/ayon_api/thumbnails.py` & `ayon-python-api-0.1.9/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_api/utils.py` & `ayon-python-api-0.1.9/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.1.9/ayon_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Description: # AYON server API
         Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
```

### Comparing `ayon-python-api-0.1.8/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.1.9/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.1.8/setup.py` & `ayon-python-api-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,13 +26,12 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     install_requires=[
         "requests >= 2.27.1",
         "six >= 1.15",
-    ],
-    dependency_links=[
-        "appdirs @ git+https://github.com/ActiveState/appdirs.git@master"
+        "Unidecode >= 1.3.6",
+        "appdirs >=1, <2",
     ],
     keywords=["AYON", "ynput", "OpenPype", "vfx"],
 )
```

