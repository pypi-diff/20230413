# Comparing `tmp/maddaq-0.7.0.tar.gz` & `tmp/maddaq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.0.tar", last modified: Thu Apr 13 16:52:09 2023, max compression
+gzip compressed data, was "maddaq-0.7.1.tar", last modified: Thu Apr 13 17:58:38 2023, max compression
```

## Comparing `maddaq-0.7.0.tar` & `maddaq-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 16:52:09.930206 maddaq-0.7.0/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 16:52:09.929924 maddaq-0.7.0/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.0/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 16:52:09.924043 maddaq-0.7.0/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.0/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.0/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13786 2023-04-04 16:03:13.000000 maddaq-0.7.0/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.0/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.0/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-13 16:51:25.000000 maddaq-0.7.0/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 16:52:09.929230 maddaq-0.7.0/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.0/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5843 2023-04-13 16:50:28.000000 maddaq-0.7.0/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.0/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.0/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-13 16:47:46.000000 maddaq-0.7.0/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.0/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.0/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 16:52:09.926586 maddaq-0.7.0/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-13 16:52:09.000000 maddaq-0.7.0/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-13 16:24:47.000000 maddaq-0.7.0/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-13 16:52:09.930298 maddaq-0.7.0/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 17:58:38.215498 maddaq-0.7.1/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 17:58:38.215188 maddaq-0.7.1/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.1/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 17:58:38.209463 maddaq-0.7.1/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.1/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.1/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13786 2023-04-04 16:03:13.000000 maddaq-0.7.1/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.1/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.1/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      440 2023-04-13 17:57:59.000000 maddaq-0.7.1/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 17:58:38.214621 maddaq-0.7.1/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.1/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5843 2023-04-13 16:50:28.000000 maddaq-0.7.1/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.1/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.1/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-13 16:47:46.000000 maddaq-0.7.1/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.1/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.1/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 17:58:38.212005 maddaq-0.7.1/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-13 17:58:38.000000 maddaq-0.7.1/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-13 17:57:59.000000 maddaq-0.7.1/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-13 17:58:38.215596 maddaq-0.7.1/setup.cfg
```

### Comparing `maddaq-0.7.0/PKG-INFO` & `maddaq-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.0
+Version: 0.7.1
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.0/README.md` & `maddaq-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/GTimer.py` & `maddaq-0.7.1/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/MadDAQData.py` & `maddaq-0.7.1/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/MadDAQModule.py` & `maddaq-0.7.1/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/Progress.py` & `maddaq-0.7.1/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/ScanManager.py` & `maddaq-0.7.1/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.1/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/file_info.py` & `maddaq-0.7.1/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.1/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.1/maddaq/cmmds/getSpectrum.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/read_data.py` & `maddaq-0.7.1/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq/cmmds/show_data.py` & `maddaq-0.7.1/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.1/maddaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.0
+Version: 0.7.1
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.0/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.1/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.0/pyproject.toml` & `maddaq-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

