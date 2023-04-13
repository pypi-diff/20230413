# Comparing `tmp/systembridgewindowssensors-3.6.3.dev6.tar.gz` & `tmp/systembridgewindowssensors-3.6.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgewindowssensors-3.6.3.dev6.tar", last modified: Mon Apr 10 15:39:18 2023, max compression
+gzip compressed data, was "systembridgewindowssensors-3.6.3.dev7.tar", last modified: Thu Apr 13 20:22:51 2023, max compression
```

## Comparing `systembridgewindowssensors-3.6.3.dev6.tar` & `systembridgewindowssensors-3.6.3.dev7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:39:18.582927 systembridgewindowssensors-3.6.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 15:39:18.582927 systembridgewindowssensors-3.6.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-10 15:38:55.000000 systembridgewindowssensors-3.6.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:39:18.582927 systembridgewindowssensors-3.6.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 15:38:55.000000 systembridgewindowssensors-3.6.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:39:18.574926 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-10 15:38:55.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-10 15:39:16.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:39:18.582927 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   242608 2023-04-10 15:38:56.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.dll
--rw-r--r--   0 runner    (1001) docker     (123)   589312 2023-04-10 15:38:56.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-04-10 15:38:56.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.xml
--rw-r--r--   0 runner    (1001) docker     (123)   716800 2023-04-10 15:38:56.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll
--rw-r--r--   0 runner    (1001) docker     (123)   122070 2023-04-10 15:38:56.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml
--rw-r--r--   0 runner    (1001) docker     (123)   701992 2023-04-10 15:38:57.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/Newtonsoft.Json.dll
--rw-r--r--   0 runner    (1001) docker     (123)   468480 2023-04-10 15:38:57.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/NvAPIWrapper.dll
--rw-r--r--   0 runner    (1001) docker     (123)  1033515 2023-04-10 15:38:57.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/NvAPIWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-04-10 15:38:57.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-10 15:38:57.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:39:18.574926 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 15:39:18.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-10 15:39:18.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:39:18.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 15:39:18.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 15:39:18.000000 systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.892686 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 20:22:49.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   242608 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   589312 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   716800 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   122070 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   701992 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/Newtonsoft.Json.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   468480 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  1033515 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.896687 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/top_level.txt
```

### Comparing `systembridgewindowssensors-3.6.3.dev6/pyproject.toml` & `systembridgewindowssensors-3.6.3.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/setup.py` & `systembridgewindowssensors-3.6.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.dll` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.pdb` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.pdb`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/HidSharp.xml` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/Newtonsoft.Json.dll` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/NvAPIWrapper.dll` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/NvAPIWrapper.xml` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev6/systembridgewindowssensors.egg-info/SOURCES.txt` & `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

