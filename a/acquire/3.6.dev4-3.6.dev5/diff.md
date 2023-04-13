# Comparing `tmp/acquire-3.6.dev4.tar.gz` & `tmp/acquire-3.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev4.tar", last modified: Tue Apr 11 15:03:24 2023, max compression
+gzip compressed data, was "acquire-3.6.dev5.tar", last modified: Thu Apr 13 07:09:21 2023, max compression
```

## Comparing `acquire-3.6.dev4.tar` & `acquire-3.6.dev5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.828563 acquire-3.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 15:03:10.000000 acquire-3.6.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 15:03:10.000000 acquire-3.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 15:03:10.000000 acquire-3.6.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 15:03:24.828563 acquire-3.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-11 15:03:10.000000 acquire-3.6.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.812563 acquire-3.6.dev4/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75148 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.816563 acquire-3.6.dev4/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.824563 acquire-3.6.dev4/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.816563 acquire-3.6.dev4/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-11 15:03:15.000000 acquire-3.6.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:03:24.828563 acquire-3.6.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.828563 acquire-3.6.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.131761 acquire-3.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 07:09:02.000000 acquire-3.6.dev5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 07:09:02.000000 acquire-3.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 07:09:02.000000 acquire-3.6.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 07:09:21.131761 acquire-3.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 07:09:02.000000 acquire-3.6.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.115761 acquire-3.6.dev5/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75219 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.119761 acquire-3.6.dev5/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.127761 acquire-3.6.dev5/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 07:09:20.000000 acquire-3.6.dev5/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.119761 acquire-3.6.dev5/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-13 07:09:09.000000 acquire-3.6.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:09:21.131761 acquire-3.6.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.131761 acquire-3.6.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tox.ini
```

### Comparing `acquire-3.6.dev4/LICENSE` & `acquire-3.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/PKG-INFO` & `acquire-3.6.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev4
+Version: 3.6.dev5
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev4/README.md` & `acquire-3.6.dev5/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/acquire.py` & `acquire-3.6.dev5/acquire/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,14 +821,15 @@
         ("glob", "sysvol/windows/inf/setupapi*.log"),
         ("glob", "sysvol/system32/logfiles/*/*.txt"),
         ("dir", "sysvol/windows/system32/sru"),
         ("dir", "sysvol/windows/system32/drivers/etc"),
         ("dir", "sysvol/Windows/System32/WDI/LogFiles/StartupInfo"),
         ("dir", "sysvol/windows/sysvol/domain/policies/"),
         ("dir", "sysvol/windows/system32/GroupPolicy/DataStore/"),
+        ("dir", "sysvol/ProgramData/Microsoft/Group Policy/History/"),
         ("glob", "sysvol/Windows/System32/LogFiles/SUM/*.mdb"),
     ]
 
 
 @register_module("--av")
 class AV(Module):
     DESC = "various antivirus logs"
```

### Comparing `acquire-3.6.dev4/acquire/collector.py` & `acquire-3.6.dev5/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/crypt.py` & `acquire-3.6.dev5/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev5/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev5/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev5/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev5/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/dynamic/windows/types.py` & `acquire-3.6.dev5/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/esxi.py` & `acquire-3.6.dev5/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/hashes.py` & `acquire-3.6.dev5/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/log.py` & `acquire-3.6.dev5/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/outputs/base.py` & `acquire-3.6.dev5/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/outputs/dir.py` & `acquire-3.6.dev5/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/outputs/tar.py` & `acquire-3.6.dev5/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/tools/decrypter.py` & `acquire-3.6.dev5/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/uploaders/minio.py` & `acquire-3.6.dev5/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/uploaders/plugin.py` & `acquire-3.6.dev5/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev5/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire/utils.py` & `acquire-3.6.dev5/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev5/acquire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev4
+Version: 3.6.dev5
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev4/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev5/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/pyproject.toml` & `acquire-3.6.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_acquire_command.py` & `acquire-3.6.dev5/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_collector.py` & `acquire-3.6.dev5/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_esxi_memory.py` & `acquire-3.6.dev5/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_file_sorting.py` & `acquire-3.6.dev5/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_minio_uploader.py` & `acquire-3.6.dev5/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_plugin.py` & `acquire-3.6.dev5/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tests/test_utils.py` & `acquire-3.6.dev5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev4/tox.ini` & `acquire-3.6.dev5/tox.ini`

 * *Files identical despite different names*

