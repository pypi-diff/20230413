# Comparing `tmp/optumi-api-3.15.4.tar.gz` & `tmp/optumi-api-3.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.15.4.tar", last modified: Thu Mar 30 15:07:06 2023, max compression
+gzip compressed data, was "optumi-api-3.15.5.tar", last modified: Wed Apr 12 20:24:32 2023, max compression
```

## Comparing `optumi-api-3.15.4.tar` & `optumi-api-3.15.5.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-03-30 15:07:06.315447 optumi-api-3.15.4/
--rw-rw-r--   0 jj        (1001) jj        (1001)      281 2022-11-02 19:54:42.000000 optumi-api-3.15.4/LICENSE
--rw-rw-r--   0 jj        (1001) jj        (1001)       40 2023-03-30 15:07:01.000000 optumi-api-3.15.4/MANIFEST.in
--rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-03-30 15:07:06.315447 optumi-api-3.15.4/PKG-INFO
--rw-rw-r--   0 jj        (1001) jj        (1001)      422 2022-11-15 18:08:23.000000 optumi-api-3.15.4/README.md
--rw-rw-r--   0 jj        (1001) jj        (1001)      322 2023-03-30 15:07:06.000000 optumi-api-3.15.4/core_version.py
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-03-30 15:07:06.315447 optumi-api-3.15.4/optumi_api/
--rw-rw-r--   0 jj        (1001) jj        (1001)     2883 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/CloudFile.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3677 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5946 2023-03-17 15:00:55.000000 optumi-api-3.15.4/optumi_api/CloudStorage.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3977 2023-03-16 21:07:26.000000 optumi-api-3.15.4/optumi_api/Colab.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5352 2023-03-16 21:08:40.000000 optumi-api-3.15.4/optumi_api/Container.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4402 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4179 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6563 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Executable.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1006 2023-03-07 21:22:10.000000 optumi-api-3.15.4/optumi_api/HoldoverTime.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3070 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/LocalFile.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3200 2023-03-17 15:00:55.000000 optumi-api-3.15.4/optumi_api/LocalStorage.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1515 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Log.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6290 2023-03-07 21:22:10.000000 optumi-api-3.15.4/optumi_api/LoginServer.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6763 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Machine.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     2719 2023-03-17 15:02:19.000000 optumi-api-3.15.4/optumi_api/Machines.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      723 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Notebook.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6573 2023-03-17 14:29:27.000000 optumi-api-3.15.4/optumi_api/NotebookConfig.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     2472 2023-03-07 21:22:10.000000 optumi-api-3.15.4/optumi_api/Notifications.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1765 2023-03-17 15:00:55.000000 optumi-api-3.15.4/optumi_api/Packages.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1620 2023-03-07 21:22:10.000000 optumi-api-3.15.4/optumi_api/Program.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5284 2023-03-17 14:03:51.000000 optumi-api-3.15.4/optumi_api/Provider.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     2131 2023-03-17 15:02:24.000000 optumi-api-3.15.4/optumi_api/Providers.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3281 2023-03-17 14:29:44.000000 optumi-api-3.15.4/optumi_api/Resource.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      696 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Script.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4135 2023-03-17 14:29:50.000000 optumi-api-3.15.4/optumi_api/Server.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1968 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/Summary.py
--rw-rw-r--   0 jj        (1001) jj        (1001)    19449 2023-03-29 20:02:39.000000 optumi-api-3.15.4/optumi_api/Workload.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3879 2023-03-17 15:02:28.000000 optumi-api-3.15.4/optumi_api/Workloads.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      838 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/__init__.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      323 2023-03-29 20:03:03.000000 optumi-api-3.15.4/optumi_api/_version.py
--rw-rw-r--   0 jj        (1001) jj        (1001)    10112 2023-03-17 15:00:55.000000 optumi-api-3.15.4/optumi_api/api.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1786 2023-03-16 14:35:18.000000 optumi-api-3.15.4/optumi_api/utils.py
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-03-30 15:07:06.315447 optumi-api-3.15.4/optumi_api.egg-info/
--rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 jj        (1001) jj        (1001)     1031 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 jj        (1001) jj        (1001)       33 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)       11 2023-03-30 15:07:06.000000 optumi-api-3.15.4/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)       38 2023-03-30 15:07:06.315447 optumi-api-3.15.4/setup.cfg
--rwxrwxr-x   0 jj        (1001) jj        (1001)     2529 2023-03-30 15:04:50.000000 optumi-api-3.15.4/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-04-03 21:07:54.000000 optumi-api-3.15.5/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-04-03 21:07:54.000000 optumi-api-3.15.5/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-12 20:24:32.108225 optumi-api-3.15.5/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-03 21:07:54.000000 optumi-api-3.15.5/README.md
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-12 20:24:31.000000 optumi-api-3.15.5/core_version.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/optumi_api/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2883 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/CloudFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3677 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5148 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/CloudStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3977 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Colab.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5352 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Container.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4402 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6563 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Executable.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1006 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/LocalFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2401 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/LocalStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1515 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Log.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6290 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/LoginServer.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6763 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Machine.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1956 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Machines.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Notebook.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6568 2023-04-12 20:23:17.000000 optumi-api-3.15.5/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2472 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Notifications.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      818 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Packages.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1620 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Program.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Provider.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1359 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Providers.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3281 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Resource.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Script.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4135 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Server.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1968 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Summary.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    19449 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Workload.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3107 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Workloads.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-04-07 16:00:16.000000 optumi-api-3.15.5/optumi_api/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    11309 2023-04-04 21:44:37.000000 optumi-api-3.15.5/optumi_api/api.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-04-04 21:44:37.000000 optumi-api-3.15.5/optumi_api/cli.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1786 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/optumi_api.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       41 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-12 20:24:32.108225 optumi-api-3.15.5/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     2612 2023-04-04 21:44:37.000000 optumi-api-3.15.5/setup.py
```

### Comparing `optumi-api-3.15.4/PKG-INFO` & `optumi-api-3.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.4
+Version: 3.15.5
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.4/optumi_api/CloudFile.py` & `optumi-api-3.15.5/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/CloudFileVersion.py` & `optumi-api-3.15.5/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/CloudStorage.py` & `optumi-api-3.15.5/optumi_api/CloudStorage.py`

 * *Files 25% similar despite different names*

```diff
@@ -139,34 +139,7 @@
         elif contains:
             return CloudStorage(x for x in CloudStorage.list() if str(contains) in optumi.utils.normalize_path(x.path, strict=False))
         else:
             return CloudStorage()
 
     def __str__(self):
         return str([str(x) for x in self])
-
-    def __add__(self, other):
-        return CloudStorage(super.__add__(self, other))
-
-    def __iadd__(self, other):
-        return CloudStorage(super.__iadd__(self, other))
-
-    def __imul__(self, other):
-        return CloudStorage(super.__imul__(self, other))
-
-    def __mul__(self, other):
-        return CloudStorage(super.__mul__(self, other))
-
-    def __reversed__(self, other):
-        return CloudStorage(super.__reversed__(self, other))
-
-    def __rmul__(self, other):
-        return CloudStorage(super.__rmul__(self, other))
-
-    def copy(self):
-        return CloudStorage(super.copy(self, other))
-
-    def reverse(self, key=None, reverse=False):
-        return CloudStorage(super.reverse(self, key, reverse))
-
-    def copy(self):
-        return CloudStorage(super.copy(self, other))
```

### Comparing `optumi-api-3.15.4/optumi_api/Colab.py` & `optumi-api-3.15.5/optumi_api/Colab.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Container.py` & `optumi-api-3.15.5/optumi_api/Container.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/ContainerRegistry.py` & `optumi-api-3.15.5/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/EnvironmentVariables.py` & `optumi-api-3.15.5/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Executable.py` & `optumi-api-3.15.5/optumi_api/Executable.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/HoldoverTime.py` & `optumi-api-3.15.5/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/LocalFile.py` & `optumi-api-3.15.5/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Log.py` & `optumi-api-3.15.5/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/LoginServer.py` & `optumi-api-3.15.5/optumi_api/LoginServer.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Machine.py` & `optumi-api-3.15.5/optumi_api/Machine.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Machines.py` & `optumi-api-3.15.5/optumi_api/Machines.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,35 +50,8 @@
         response = json.loads(optumi.core.get_machines().text)
 
         for machine in response["machines"]:
             machine = Machine(*Machine.reconstruct(machine))
             if (status is None and machine.is_visible()) or (machine.status == status):
                 machines.append(machine)
 
-        return Machines(machines)
-
-    def __add__(self, other):
-        return Machines(super.__add__(self, other))
-
-    def __iadd__(self, other):
-        return Machines(super.__iadd__(self, other))
-
-    def __imul__(self, other):
-        return Machines(super.__imul__(self, other))
-
-    def __mul__(self, other):
-        return Machines(super.__mul__(self, other))
-
-    def __reversed__(self, other):
-        return Machines(super.__reversed__(self, other))
-
-    def __rmul__(self, other):
-        return Machines(super.__rmul__(self, other))
-
-    def copy(self):
-        return Machines(super.copy(self, other))
-
-    def reverse(self, key=None, reverse=False):
-        return Machines(super.reverse(self, key, reverse))
-
-    def copy(self):
-        return Machines(super.copy(self, other))
+        return Machines(machines)
```

### Comparing `optumi-api-3.15.4/optumi_api/Notebook.py` & `optumi-api-3.15.5/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/NotebookConfig.py` & `optumi-api-3.15.5/optumi_api/NotebookConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     resource: Resource = None,
     notifications: Notifications = None,
     registry: ContainerRegistry = None,
     launch_mode: str = "job",
 ):
     # Start with blank config
     nb_config = {
-        "intent": 0.5,
+        "intent": 0.25,
         "compute": {
             "expertise": "component",
             "required": False,
             "rating": [-1, -1, -1],
             "score": [-1, -1, -1],
             "cores": [-1, -1, -1],
             "frequency": [-1, -1, -1],
@@ -152,15 +152,15 @@
             for e in env
         ]
 
     # Plug in container registry
     if registry:
         nb_config["integrations"] += [
             {
-                "name": self._registry.name,
+                "name": registry.name,
                 "enabled": True,
                 "integrationType": "generic container registry",
             }
         ]
 
     # Plug in resource requirements
     if type(resource) is Server:
```

### Comparing `optumi-api-3.15.4/optumi_api/Notifications.py` & `optumi-api-3.15.5/optumi_api/Notifications.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Program.py` & `optumi-api-3.15.5/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Provider.py` & `optumi-api-3.15.5/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Resource.py` & `optumi-api-3.15.5/optumi_api/Resource.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Script.py` & `optumi-api-3.15.5/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Server.py` & `optumi-api-3.15.5/optumi_api/Server.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Summary.py` & `optumi-api-3.15.5/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/Workload.py` & `optumi-api-3.15.5/optumi_api/Workload.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/__init__.py` & `optumi-api-3.15.5/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api/api.py` & `optumi-api-3.15.5/optumi_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from .LoginServer import login as oauth_login
 from .HoldoverTime import HoldoverTime
 from .Workloads import Workloads
 
 import datetime, json, os, webbrowser
 import phonenumbers
+from pwinput import pwinput
 from requests.exceptions import ConnectionError
 
 
 # Optumi imports
 import optumi_core as optumi
 from optumi_core.exceptions import (
     NotLoggedInException,
@@ -34,15 +35,18 @@
     """Print or open the url for full Optumi API documentation.
 
     Args:
         open (bool, optional): Wether to print the url or open the docs in a new browser tab. Defaults to True.
     """
     url = "https://portal.optumi.net/docs"
     if open:
-        webbrowser.open_new_tab(url)
+        try:
+            webbrowser.open_new_tab(url)
+        except webbrowser.Error:
+            pass
     else:
         print("Optumi API documentation is available at: " + url)
 
 
 docs(False)
 
 
@@ -52,15 +56,15 @@
 ):
     """Log in to the Optumi service platform.
 
     If a connection token is provided - as an argument or stored on the local disk - it will be leveraged to complete the login operation otherwise a new browser tab is opened to prompt the user for credentials.
 
     Args:
         connection_token (str, optional): A connection token (can be generated in the webapp). Defaults to None.
-        save_token (bool, optional): Whether to store the connection token on disk. Defaults to True.
+        save_token (bool, optional): Whether to store the connection token on the disk. Defaults to True.
 
     Raises:
         NotLoggedInException: Raised if the login was not successful.
         OptumiException: Raised if the browser login could not be initiated.
     """
 
     def handle_login_response(login_status, message):
@@ -109,27 +113,52 @@
             # Try to log in with the login token from the disk
             login_status, message = optumi.login.login_rest_server(dnsName, port, login_type="token", save_token=save_token)
 
             # Fall back on the browser login
             if login_status != 1:
                 if DEBUG_LOGIN:
                     print("Trying browser login")
+
+                headless = True
                 try:
+                    webbrowser.get()
+                    headless = False
+                except webbrowser.Error:
+                    pass
+
+                if headless:
+                    # Prompt the user in the cli for their connection token
+                    print("You can find your connection token in the settings tab here: https://portal.optumi.net")
+                    connection_token = pwinput(prompt="Enter connection token: ")
+
+                    if DEBUG_LOGIN:
+                        print("Connection token")
                     login_status, message = optumi.login.login_rest_server(
                         dnsName,
                         port,
-                        oauth_login(),
-                        login_type="oauth",
+                        connection_token,
+                        login_type="token",
                         save_token=save_token,
                     )
                     handle_login_response(login_status, message)
-                except RuntimeError:
-                    raise OptumiException(
-                        "Unable to perform browser login from Notebook. Try logging in with a connection token as shown here: https://optumi.notion.site/Login-using-a-connection-token-710bccdeaf734cbf825aae94b79a8109"
-                    )
+                else:
+                    # Open a new browser tab and complete the browser login
+                    try:
+                        login_status, message = optumi.login.login_rest_server(
+                            dnsName,
+                            port,
+                            oauth_login(),
+                            login_type="oauth",
+                            save_token=save_token,
+                        )
+                        handle_login_response(login_status, message)
+                    except RuntimeError:
+                        raise OptumiException(
+                            "Unable to perform browser login from Notebook. Try logging in with a connection token as shown here: https://optumi.notion.site/Login-using-a-connection-token-710bccdeaf734cbf825aae94b79a8109"
+                        )
         else:
             if DEBUG_LOGIN:
                 print("Connection token")
             login_status, message = optumi.login.login_rest_server(
                 dnsName,
                 port,
                 connection_token,
@@ -143,15 +172,15 @@
     print("Logged in", user_information["name"])
 
 
 def logout(remove_token: bool = True):
     """Log out of the Optumi service platform, optionally removing any stored connection token.
 
     Args:
-        remove_token (bool, optional): Whether to remove the connection token on logout. Defaults to True.
+        remove_token (bool, optional): Whether to remove the connection token from the disk. Defaults to True.
     """
     try:
         optumi.login.logout(remove_token=remove_token)
     except NotLoggedInException:
         pass
```

### Comparing `optumi-api-3.15.4/optumi_api/utils.py` & `optumi-api-3.15.5/optumi_api/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.4/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.15.5/optumi_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.4
+Version: 3.15.5
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.4/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.15.5/optumi_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 optumi_api/Server.py
 optumi_api/Summary.py
 optumi_api/Workload.py
 optumi_api/Workloads.py
 optumi_api/__init__.py
 optumi_api/_version.py
 optumi_api/api.py
+optumi_api/cli.py
 optumi_api/utils.py
 optumi_api.egg-info/PKG-INFO
 optumi_api.egg-info/SOURCES.txt
 optumi_api.egg-info/dependency_links.txt
+optumi_api.egg-info/entry_points.txt
 optumi_api.egg-info/not-zip-safe
 optumi_api.egg-info/requires.txt
 optumi_api.egg-info/top_level.txt
```

### Comparing `optumi-api-3.15.4/setup.py` & `optumi-api-3.15.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     url="https://optumi.com",
     author="Optumi Inc Authors",
     author_email="cs@optumi.com",
     description="Optumi api library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    install_requires=["optumi_core" + core_dependency_string, "phonenumbers"],
+    entry_points={"console_scripts": ["optumi = optumi_api.cli:main"]},
+    install_requires=["optumi_core" + core_dependency_string, "phonenumbers", "pwinput"],
     zip_safe=False,
     python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Optumi"],
     classifiers=[
         "License :: Other/Proprietary License",
         "Development Status :: 4 - Beta",
```

