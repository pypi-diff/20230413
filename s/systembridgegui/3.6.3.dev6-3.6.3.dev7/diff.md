# Comparing `tmp/systembridgegui-3.6.3.dev6.tar.gz` & `tmp/systembridgegui-3.6.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgegui-3.6.3.dev6.tar", last modified: Mon Apr 10 15:38:35 2023, max compression
+gzip compressed data, was "systembridgegui-3.6.3.dev7.tar", last modified: Thu Apr 13 20:22:12 2023, max compression
```

## Comparing `systembridgegui-3.6.3.dev6.tar` & `systembridgegui-3.6.3.dev7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/systembridgegui/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 15:38:33.000000 systembridgegui-3.6.3.dev6/systembridgegui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/systembridgegui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/widgets/timed_message_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/systembridgegui/window/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/window/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/window/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-10 15:38:14.000000 systembridgegui-3.6.3.dev6/systembridgegui/window/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:38:35.285888 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 15:38:35.000000 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 15:38:35.000000 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:38:35.000000 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 15:38:35.000000 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 15:38:35.000000 systembridgegui-3.6.3.dev6/systembridgegui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/systembridgegui/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 20:22:09.000000 systembridgegui-3.6.3.dev7/systembridgegui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/systembridgegui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/widgets/timed_message_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/systembridgegui/window/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/window/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/window/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-13 20:21:48.000000 systembridgegui-3.6.3.dev7/systembridgegui/window/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:12.393230 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 20:22:12.000000 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-13 20:22:12.000000 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:22:12.000000 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 20:22:12.000000 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 20:22:12.000000 systembridgegui-3.6.3.dev7/systembridgegui.egg-info/top_level.txt
```

### Comparing `systembridgegui-3.6.3.dev6/pyproject.toml` & `systembridgegui-3.6.3.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/setup.py` & `systembridgegui-3.6.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/__main__.py` & `systembridgegui-3.6.3.dev7/systembridgegui/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/icon.png` & `systembridgegui-3.6.3.dev7/systembridgegui/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/system_tray.py` & `systembridgegui-3.6.3.dev7/systembridgegui/system_tray.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/widgets/timed_message_box.py` & `systembridgegui-3.6.3.dev7/systembridgegui/widgets/timed_message_box.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/window/main.py` & `systembridgegui-3.6.3.dev7/systembridgegui/window/main.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/window/notification.py` & `systembridgegui-3.6.3.dev7/systembridgegui/window/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui/window/player.py` & `systembridgegui-3.6.3.dev7/systembridgegui/window/player.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.6.3.dev6/systembridgegui.egg-info/SOURCES.txt` & `systembridgegui-3.6.3.dev7/systembridgegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

