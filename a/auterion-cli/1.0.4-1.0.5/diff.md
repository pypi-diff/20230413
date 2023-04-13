# Comparing `tmp/auterion-cli-1.0.4.tar.gz` & `tmp/auterion-cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.4.tar", last modified: Tue Apr  4 13:01:34 2023, max compression
+gzip compressed data, was "auterion-cli-1.0.5.tar", last modified: Thu Apr 13 14:30:59 2023, max compression
```

## Comparing `auterion-cli-1.0.4.tar` & `auterion-cli-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 13:01:33.000000 auterion-cli-1.0.4/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:01:34.004211 auterion-cli-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-04 13:01:26.000000 auterion-cli-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.743423 auterion-cli-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:30:59.743423 auterion-cli-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/setup.py
```

### Comparing `auterion-cli-1.0.4/README.md` & `auterion-cli-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.0.5/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_command.py` & `auterion-cli-1.0.5/auterioncli/commands/app_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,25 +181,26 @@
         else:
             error(f"Failed to get apps")
 
     def _print_apps(self, apps):
         headers = ["Name", "Version", "Status", "Enable", "Services", "Status", "Enable"]
         matrix = []
         for app in apps:
-            row = [app['name'], app['version'], app['status'], app['enable']]
+            row = [app.get('name', 'unknown'), app.get('version', 'unknown'), app.get('status', 'unknown'), app.get('enable', 'unknown')]
             if len(app['services']) > 0:
-                row.append(app['services'][0]["name"])
-                row.append(app['services'][0]["status"])
-                row.append(app['services'][0]["enable"])
+                row.append(app['services'][0].get("name", 'unknown'))
+                row.append(app['services'][0].get("status", 'unknown'))
+                row.append(app['services'][0].get("enable", 'unknown'))
             else:
                 row.append("")
                 row.append("")
+                row.append("")
             matrix.append(row)
             for s in app['services'][1:]:
-                matrix.append(["", "", "", "", s["name"], s["status"], s["enable"]])
+                matrix.append(["", "", "", "", s.get("name", 'unknown'), s.get("status", 'unknown'), s.get("enable", 'unknown')])
         print(tabulate(matrix, headers=headers))
 
     def _print_app_result(self, data, app, success_message):
         try:
             body = data.json()
         except:
             body = {}
```

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.0.5/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/container_command.py` & `auterion-cli-1.0.5/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/device_command.py` & `auterion-cli-1.0.5/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/info_command.py` & `auterion-cli-1.0.5/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/report_command.py` & `auterion-cli-1.0.5/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/commands/utils.py` & `auterion-cli-1.0.5/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/main.py` & `auterion-cli-1.0.5/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/auterioncli/meta_util.py` & `auterion-cli-1.0.5/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.4/setup.py` & `auterion-cli-1.0.5/setup.py`

 * *Files identical despite different names*

