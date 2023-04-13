# Comparing `tmp/vanilla_violin-0.1.3.tar.gz` & `tmp/vanilla_violin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanilla_violin-0.1.3.tar", last modified: Thu Apr  6 11:03:01 2023, max compression
+gzip compressed data, was "vanilla_violin-0.1.4.tar", last modified: Thu Apr 13 13:44:08 2023, max compression
```

## Comparing `vanilla_violin-0.1.3.tar` & `vanilla_violin-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.533763 vanilla_violin-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-06 11:03:01.533763 vanilla_violin-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 11:03:01.533763 vanilla_violin-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.528763 vanilla_violin-0.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/tests/test_gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.528763 vanilla_violin-0.1.3/vanilla_violin/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/vanilla_violin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.532763 vanilla_violin-0.1.3/vanilla_violin/aws/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/vanilla_violin/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/vanilla_violin/aws/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.532763 vanilla_violin-0.1.3/vanilla_violin/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/vanilla_violin/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9796 2023-04-06 11:02:35.000000 vanilla_violin-0.1.3/vanilla_violin/gitlab/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 11:03:01.531763 vanilla_violin-0.1.3/vanilla_violin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-06 11:03:01.000000 vanilla_violin-0.1.3/vanilla_violin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.498652 vanilla_violin-0.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/tests/test_gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.498652 vanilla_violin-0.1.4/vanilla_violin/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.502652 vanilla_violin-0.1.4/vanilla_violin/aws/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/aws/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.502652 vanilla_violin-0.1.4/vanilla_violin/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9944 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/gitlab/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.501652 vanilla_violin-0.1.4/vanilla_violin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/top_level.txt
```

### Comparing `vanilla_violin-0.1.3/LICENSE` & `vanilla_violin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.3/tests/test_gitlab.py` & `vanilla_violin-0.1.4/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.3/vanilla_violin/aws/aws.py` & `vanilla_violin-0.1.4/vanilla_violin/aws/aws.py`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.3/vanilla_violin/gitlab/gitlab.py` & `vanilla_violin-0.1.4/vanilla_violin/gitlab/gitlab.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,25 @@
       headers=self.request_headers
     )
     return {
       'text': json.loads(response.text),
       'status_code': response.status_code,
     }
 
+  def get_projects(self):
+
+    response = requests.get(
+      f'{self.base_url}{self.api_url}projects', 
+      headers=self.request_headers
+    )
+    return {
+      'text': json.loads(response.text),
+      'status_code': response.status_code,
+    }
+
   def unprotect_branch(self, project_id, branch_name='main'):
 
     response = requests.delete(
       f'{self.base_url}{self.api_url}projects/{project_id}/protected_branches/{branch_name}', 
       headers=self.request_headers
     )
     return {'status_code': response.status_code}
@@ -225,23 +236,22 @@
     for obj in array_of_objs:
       if obj['path'] == path and obj['full_path'] == path :
         return obj
 
     return []
 
   def get_project_id(self, full_path):
-    paths = full_path.split('/')
-    parent_id = None
+    projects = self.get_projects()['text']
 
     try:
-      for path in paths[:-1]:
-        parent_id = self.find_base_group_by_path(path, self.get_groups(parent_id))['id']
-
-      proj = self.find_object_by_path(path, self.list_group_projects(parent_id))
-      return proj['id']
+      for proj in projects:
+        if proj['path_with_namespace'] == full_path:
+          return proj['id']
+      
+      return None
 
     except Exception as ex:
       raise ex
 
   def build_request_chain(self, full_path):
 
     print(f'--- BUILDING FOR {full_path} ---')
```

