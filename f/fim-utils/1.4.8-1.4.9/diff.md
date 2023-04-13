# Comparing `tmp/fim_utils-1.4.8.tar.gz` & `tmp/fim_utils-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.4.8.tar", last modified: Fri Jan 20 02:30:50 2023, max compression
+gzip compressed data, was "fim_utils-1.4.9.tar", last modified: Wed Feb  1 22:52:01 2023, max compression
```

## Comparing `fim_utils-1.4.8.tar` & `fim_utils-1.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.506449 fim_utils-1.4.8/
--rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2021-03-24 00:22:11.000000 fim_utils-1.4.8/LICENSE
--rw-r--r--   0 ibaldin    (502) staff       (20)      201 2022-08-11 21:42:55.000000 fim_utils-1.4.8/MANIFEST.in
--rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-01-20 02:30:50.506215 fim_utils-1.4.8/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)     7536 2022-11-18 22:04:52.000000 fim_utils-1.4.8/README.md
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.491484 fim_utils-1.4.8/fim_utils.egg-info/
--rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-01-20 02:30:50.000000 fim_utils-1.4.8/fim_utils.egg-info/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)      809 2023-01-20 02:30:50.000000 fim_utils-1.4.8/fim_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-01-20 02:30:50.000000 fim_utils-1.4.8/fim_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)      461 2023-01-20 02:30:50.000000 fim_utils-1.4.8/fim_utils.egg-info/requires.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        8 2023-01-20 02:30:50.000000 fim_utils-1.4.8/fim_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.491723 fim_utils-1.4.8/fimutil/
--rw-r--r--   0 ibaldin    (502) staff       (20)       25 2023-01-20 02:29:35.000000 fim_utils-1.4.8/fimutil/__init__.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.493431 fim_utils-1.4.8/fimutil/al2s/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-10-26 01:51:00.000000 fim_utils-1.4.8/fimutil/al2s/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9065 2023-01-17 20:07:11.000000 fim_utils-1.4.8/fimutil/al2s/arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11087 2022-10-26 01:51:00.000000 fim_utils-1.4.8/fimutil/al2s/oess.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.496037 fim_utils-1.4.8/fimutil/netam/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2021-10-19 20:02:19.000000 fim_utils-1.4.8/fimutil/netam/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    19470 2023-01-20 02:29:04.000000 fim_utils-1.4.8/fimutil/netam/arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4247 2023-01-08 20:10:10.000000 fim_utils-1.4.8/fimutil/netam/nso.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3439 2021-09-17 00:59:00.000000 fim_utils-1.4.8/fimutil/netam/sr_pce.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.504093 fim_utils-1.4.8/fimutil/ralph/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-02-22 22:46:07.000000 fim_utils-1.4.8/fimutil/ralph/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3438 2022-10-26 01:51:00.000000 fim_utils-1.4.8/fimutil/ralph/asset.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2454 2022-11-09 23:04:15.000000 fim_utils-1.4.8/fimutil/ralph/dp_switch.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3835 2022-10-26 01:51:00.000000 fim_utils-1.4.8/fimutil/ralph/ethernetport.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    20282 2022-11-12 16:12:02.000000 fim_utils-1.4.8/fimutil/ralph/fim_helper.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1075 2021-07-02 19:22:05.000000 fim_utils-1.4.8/fimutil/ralph/gpu.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3307 2022-10-26 01:51:00.000000 fim_utils-1.4.8/fimutil/ralph/model.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1338 2023-01-17 18:41:25.000000 fim_utils-1.4.8/fimutil/ralph/nvme.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1384 2021-09-27 19:32:26.000000 fim_utils-1.4.8/fimutil/ralph/ralph_uri.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4912 2022-11-09 23:04:15.000000 fim_utils-1.4.8/fimutil/ralph/site.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      885 2021-07-02 19:22:05.000000 fim_utils-1.4.8/fimutil/ralph/storage.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9208 2022-11-18 22:04:52.000000 fim_utils-1.4.8/fimutil/ralph/worker_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      462 2022-12-21 02:37:06.000000 fim_utils-1.4.8/requirements.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-01-20 02:30:50.506514 fim_utils-1.4.8/setup.cfg
--rw-r--r--   0 ibaldin    (502) staff       (20)      984 2022-08-11 21:42:55.000000 fim_utils-1.4.8/setup.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-01-20 02:30:50.505537 fim_utils-1.4.8/utilities/
--rw-r--r--   0 ibaldin    (502) staff       (20)     6183 2022-10-26 01:51:00.000000 fim_utils-1.4.8/utilities/generate_instance_flavors.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1694 2022-10-26 01:51:00.000000 fim_utils-1.4.8/utilities/scan_net.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5482 2022-10-26 01:51:00.000000 fim_utils-1.4.8/utilities/scan_site.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1975 2021-09-27 19:32:26.000000 fim_utils-1.4.8/utilities/scan_worker.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.652475 fim_utils-1.4.9/
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2021-03-24 00:22:11.000000 fim_utils-1.4.9/LICENSE
+-rw-r--r--   0 ibaldin    (502) staff       (20)      201 2022-08-11 21:42:55.000000 fim_utils-1.4.9/MANIFEST.in
+-rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-02-01 22:52:01.652203 fim_utils-1.4.9/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)     7536 2022-11-18 22:04:52.000000 fim_utils-1.4.9/README.md
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.639320 fim_utils-1.4.9/fim_utils.egg-info/
+-rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)      809 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)      461 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/requires.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        8 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.639577 fim_utils-1.4.9/fimutil/
+-rw-r--r--   0 ibaldin    (502) staff       (20)       25 2023-02-01 22:51:36.000000 fim_utils-1.4.9/fimutil/__init__.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.641379 fim_utils-1.4.9/fimutil/al2s/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/al2s/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9065 2023-01-17 20:07:11.000000 fim_utils-1.4.9/fimutil/al2s/arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11087 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/al2s/oess.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.644067 fim_utils-1.4.9/fimutil/netam/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        2 2021-10-19 20:02:19.000000 fim_utils-1.4.9/fimutil/netam/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    19470 2023-01-20 02:29:04.000000 fim_utils-1.4.9/fimutil/netam/arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4247 2023-01-08 20:10:10.000000 fim_utils-1.4.9/fimutil/netam/nso.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3439 2021-09-17 00:59:00.000000 fim_utils-1.4.9/fimutil/netam/sr_pce.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.649751 fim_utils-1.4.9/fimutil/ralph/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-02-22 22:46:07.000000 fim_utils-1.4.9/fimutil/ralph/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3438 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/asset.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2454 2022-11-09 23:04:15.000000 fim_utils-1.4.9/fimutil/ralph/dp_switch.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3835 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/ethernetport.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    20282 2022-11-12 16:12:02.000000 fim_utils-1.4.9/fimutil/ralph/fim_helper.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1075 2021-07-02 19:22:05.000000 fim_utils-1.4.9/fimutil/ralph/gpu.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3307 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/model.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1464 2023-02-01 22:45:42.000000 fim_utils-1.4.9/fimutil/ralph/nvme.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1384 2021-09-27 19:32:26.000000 fim_utils-1.4.9/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4912 2022-11-09 23:04:15.000000 fim_utils-1.4.9/fimutil/ralph/site.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      885 2021-07-02 19:22:05.000000 fim_utils-1.4.9/fimutil/ralph/storage.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9208 2022-11-18 22:04:52.000000 fim_utils-1.4.9/fimutil/ralph/worker_node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      462 2022-12-21 02:37:06.000000 fim_utils-1.4.9/requirements.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-02-01 22:52:01.652554 fim_utils-1.4.9/setup.cfg
+-rw-r--r--   0 ibaldin    (502) staff       (20)      984 2022-08-11 21:42:55.000000 fim_utils-1.4.9/setup.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.651642 fim_utils-1.4.9/utilities/
+-rw-r--r--   0 ibaldin    (502) staff       (20)     6183 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/generate_instance_flavors.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1694 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/scan_net.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5482 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/scan_site.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1975 2021-09-27 19:32:26.000000 fim_utils-1.4.9/utilities/scan_worker.py
```

### Comparing `fim_utils-1.4.8/LICENSE` & `fim_utils-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/README.md` & `fim_utils-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fim_utils.egg-info/SOURCES.txt` & `fim_utils-1.4.9/fim_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/al2s/arm.py` & `fim_utils-1.4.9/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/al2s/oess.py` & `fim_utils-1.4.9/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/netam/arm.py` & `fim_utils-1.4.9/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/netam/nso.py` & `fim_utils-1.4.9/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/netam/sr_pce.py` & `fim_utils-1.4.9/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/asset.py` & `fim_utils-1.4.9/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/dp_switch.py` & `fim_utils-1.4.9/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/ethernetport.py` & `fim_utils-1.4.9/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/fim_helper.py` & `fim_utils-1.4.9/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/gpu.py` & `fim_utils-1.4.9/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/model.py` & `fim_utils-1.4.9/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/nvme.py` & `fim_utils-1.4.9/fimutil/ralph/nvme.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,26 +7,28 @@
     """
     This class knows how to parse necessary worker fields in Ralph
     """
     FIELD_MAP = '{SN: .serial_number, Description: .model_name}'
     # "Description": "Dell Express Flash NVMe P4510 1TB SFF in PCIe
     # SSD Slot 22 in Bay 2 (0000:21:00.0)", "BDF": "0000:21:00.0"
     REGEX_FIELDS = {'BDF': ["Description", ".+\\(([0-9a-f:.]+)\\).*"],
-                    'Model': ["Description", ".+(P4510|CD5|CD6) ([\\w]+).*"],
+                    'Model': ["Description", ".+(P4510|CD5|CD6|PE8010) ([\\w]+).*"],
                     'Disk': ["Description", ".+ ([\\d]+[MGTP]B|[\\d]+[MGTP]) .*"]}
 
     def __init__(self, *, uri: str, ralph: RalphURI):
         super().__init__(uri=uri, ralph=ralph)
         self.type = RalphAssetType.NVMe
 
     def parse(self):
         super().parse()
         # this is a hack around NVMe model names
         if 'NVMe' not in self.fields['Description'] and \
                 'CD5' not in self.fields['Description'] and \
-                'CD6' not in self.fields['Description']:
+                'CD6' not in self.fields['Description'] and \
+                'PE8010' not in self.fields['Description']:
             raise RalphAssetMimatch('This is not an NVMe drive')
         if self.fields['Model'] == 'CD5' or \
-                self.fields['Model'] == 'CD6':
+                self.fields['Model'] == 'CD6' or \
+                self.fields['Model'] == 'PE8010':
             # FIXME: temporary override to old model
             self.fields['Model'] = "P4510"
```

### Comparing `fim_utils-1.4.8/fimutil/ralph/ralph_uri.py` & `fim_utils-1.4.9/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/site.py` & `fim_utils-1.4.9/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/storage.py` & `fim_utils-1.4.9/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/fimutil/ralph/worker_node.py` & `fim_utils-1.4.9/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/setup.py` & `fim_utils-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/utilities/generate_instance_flavors.py` & `fim_utils-1.4.9/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/utilities/scan_net.py` & `fim_utils-1.4.9/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/utilities/scan_site.py` & `fim_utils-1.4.9/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.8/utilities/scan_worker.py` & `fim_utils-1.4.9/utilities/scan_worker.py`

 * *Files identical despite different names*

