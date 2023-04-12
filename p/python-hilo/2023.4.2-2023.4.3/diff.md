# Comparing `tmp/python_hilo-2023.4.2.tar.gz` & `tmp/python_hilo-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_hilo-2023.4.2.tar", max compression
+gzip compressed data, was "python_hilo-2023.4.3.tar", max compression
```

## Comparing `python_hilo-2023.4.2.tar` & `python_hilo-2023.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.4.2/LICENSE
--rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.4.2/README.md
--rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.4.2/pyhilo/__init__.py
--rw-r--r--   0        0        0    28803 2023-04-07 15:37:20.467264 python_hilo-2023.4.2/pyhilo/api.py
--rw-r--r--   0        0        0     6950 2023-04-07 15:35:01.807968 python_hilo-2023.4.2/pyhilo/const.py
--rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.4.2/pyhilo/device/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.4.2/pyhilo/device/climate.py
--rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.4.2/pyhilo/device/light.py
--rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.4.2/pyhilo/device/sensor.py
--rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.4.2/pyhilo/device/switch.py
--rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.4.2/pyhilo/devices.py
--rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.4.2/pyhilo/event.py
--rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.4.2/pyhilo/exceptions.py
--rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.4.2/pyhilo/util/__init__.py
--rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.4.2/pyhilo/util/state.py
--rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.4.2/pyhilo/websocket.py
--rw-r--r--   0        0        0     3151 2023-04-07 15:46:51.125425 python_hilo-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 python_hilo-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.4.3/LICENSE
+-rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.4.3/README.md
+-rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.4.3/pyhilo/__init__.py
+-rw-r--r--   0        0        0    28803 2023-04-07 15:37:20.467264 python_hilo-2023.4.3/pyhilo/api.py
+-rw-r--r--   0        0        0     6950 2023-04-07 15:35:01.807968 python_hilo-2023.4.3/pyhilo/const.py
+-rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.4.3/pyhilo/device/__init__.py
+-rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.4.3/pyhilo/device/climate.py
+-rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.4.3/pyhilo/device/light.py
+-rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.4.3/pyhilo/device/sensor.py
+-rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.4.3/pyhilo/device/switch.py
+-rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.4.3/pyhilo/devices.py
+-rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.4.3/pyhilo/event.py
+-rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.4.3/pyhilo/exceptions.py
+-rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.4.3/pyhilo/util/__init__.py
+-rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.4.3/pyhilo/util/state.py
+-rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.4.3/pyhilo/websocket.py
+-rw-r--r--   0        0        0     3151 2023-04-12 22:18:20.675701 python_hilo-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 python_hilo-2023.4.3/PKG-INFO
```

### Comparing `python_hilo-2023.4.2/LICENSE` & `python_hilo-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/README.md` & `python_hilo-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/api.py` & `python_hilo-2023.4.3/pyhilo/api.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/const.py` & `python_hilo-2023.4.3/pyhilo/const.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/device/__init__.py` & `python_hilo-2023.4.3/pyhilo/device/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/device/climate.py` & `python_hilo-2023.4.3/pyhilo/device/climate.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/device/light.py` & `python_hilo-2023.4.3/pyhilo/device/light.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/devices.py` & `python_hilo-2023.4.3/pyhilo/devices.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/event.py` & `python_hilo-2023.4.3/pyhilo/event.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/exceptions.py` & `python_hilo-2023.4.3/pyhilo/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/util/__init__.py` & `python_hilo-2023.4.3/pyhilo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/util/state.py` & `python_hilo-2023.4.3/pyhilo/util/state.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyhilo/websocket.py` & `python_hilo-2023.4.3/pyhilo/websocket.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.2/pyproject.toml` & `python_hilo-2023.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 exclude = ".venv/.*"
 
 [tool.poetry]
 name = "python-hilo"
-version = "2023.04.02"
+version = "2023.04.03"
 description = "A Python3, async interface to the Hilo API"
 readme = "README.md"
 authors = ["David Vallee Delisle <me@dvd.dev>"]
 maintainers = ["David Vallee Delisle <me@dvd.dev>"]
 license = "MIT"
 repository = "https://github.com/dvd-dev/python-hilo"
 packages = [
```

### Comparing `python_hilo-2023.4.2/PKG-INFO` & `python_hilo-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hilo
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: A Python3, async interface to the Hilo API
 Home-page: https://github.com/dvd-dev/python-hilo
 License: MIT
 Author: David Vallee Delisle
 Author-email: me@dvd.dev
 Maintainer: David Vallee Delisle
 Maintainer-email: me@dvd.dev
```

