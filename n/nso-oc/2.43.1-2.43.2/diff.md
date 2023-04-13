# Comparing `tmp/nso-oc-2.43.1.tar.gz` & `tmp/nso-oc-2.43.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.43.1.tar", last modified: Thu Apr 13 00:04:07 2023, max compression
+gzip compressed data, was "nso-oc-2.43.2.tar", last modified: Thu Apr 13 18:04:36 2023, max compression
```

## Comparing `nso-oc-2.43.1.tar` & `nso-oc-2.43.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:04:07.503641 nso-oc-2.43.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-13 00:03:40.000000 nso-oc-2.43.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 00:03:40.000000 nso-oc-2.43.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 00:04:07.503641 nso-oc-2.43.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 00:03:40.000000 nso-oc-2.43.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:04:07.499641 nso-oc-2.43.1/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 00:04:07.000000 nso-oc-2.43.1/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:04:07.499641 nso-oc-2.43.1/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:04:07.499641 nso-oc-2.43.1/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29448 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:04:07.503641 nso-oc-2.43.1/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-13 00:03:40.000000 nso-oc-2.43.1/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 00:03:40.000000 nso-oc-2.43.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 00:04:07.503641 nso-oc-2.43.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-13 00:03:40.000000 nso-oc-2.43.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-13 18:03:59.000000 nso-oc-2.43.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 18:03:59.000000 nso-oc-2.43.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 18:04:36.440905 nso-oc-2.43.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 18:03:59.000000 nso-oc-2.43.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.436905 nso-oc-2.43.2/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 18:04:36.000000 nso-oc-2.43.2/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.436905 nso-oc-2.43.2/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29451 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:36.440905 nso-oc-2.43.2/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-13 18:03:59.000000 nso-oc-2.43.2/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 18:03:59.000000 nso-oc-2.43.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 18:04:36.440905 nso-oc-2.43.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-13 18:03:59.000000 nso-oc-2.43.2/setup.py
```

### Comparing `nso-oc-2.43.1/LICENSE` & `nso-oc-2.43.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/PKG-INFO` & `nso-oc-2.43.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.43.1
+Version: 2.43.2
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.43.1/README.md` & `nso-oc-2.43.2/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.43.2/nso_oc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.43.1
+Version: 2.43.2
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.43.1/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.43.2/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/README.md` & `nso-oc-2.43.2/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/common.py` & `nso-oc-2.43.2/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/main.py` & `nso-oc-2.43.2/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         conditions["openconfig-bgp-policy:bgp-conditions"]["openconfig-bgp-policy:config"].update({
             "openconfig-bgp-policy:ext-community-set": route_map_match["extcommunity"][0]
         })
     if len(route_map_match.get("ip", {}).get("address", {}).get("access-list", [])) > 0:
         conditions.update({
             "openconfig-routing-policy-ext:match-acl-ipv4-set": {
                 "openconfig-routing-policy-ext:config": {
-                    "openconfig-routing-policy-ext:acl-set": route_map_match["ip"]["address"]["access-list"]
+                    "openconfig-routing-policy-ext:acl-set": route_map_match["ip"]["address"]["access-list"][0]
                 }
             }
         })
 
 
 def format_well_known_communities(community_number):
     for i in well_known_members:
```

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.43.2/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.43.2/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.43.2/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.43.2/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.43.2/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.43.2/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.43.1/setup.py` & `nso-oc-2.43.2/setup.py`

 * *Files identical despite different names*

