# Comparing `tmp/vclog-0.1.2.tar.gz` & `tmp/vclog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vclog-0.1.2.tar", last modified: Fri Mar 17 10:20:35 2023, max compression
+gzip compressed data, was "vclog-1.0.0.tar", last modified: Thu Apr 13 08:30:12 2023, max compression
```

## Comparing `vclog-0.1.2.tar` & `vclog-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-03-17 10:20:35.503971 vclog-0.1.2/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1062 2023-03-16 11:51:10.000000 vclog-0.1.2/LICENSE
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2563 2023-03-17 10:20:35.503971 vclog-0.1.2/PKG-INFO
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2090 2023-03-17 10:20:02.000000 vclog-0.1.2/README.md
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      563 2023-03-17 09:42:37.000000 vclog-0.1.2/pyproject.toml
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       38 2023-03-17 10:20:35.503971 vclog-0.1.2/setup.cfg
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-03-17 10:20:35.503971 vclog-0.1.2/vclog/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       51 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/__init__.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-03-17 10:20:35.503971 vclog-0.1.2/vclog/core/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       51 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/core/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     1299 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/core/codes.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      509 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/core/colors.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     4225 2023-03-17 10:05:59.000000 vclog-0.1.2/vclog/logger.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-03-17 10:20:35.503971 vclog-0.1.2/vclog/use_cases/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)       32 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      582 2023-03-16 11:51:10.000000 vclog-0.1.2/vclog/use_cases/formatter.py
-drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-03-17 10:20:35.503971 vclog-0.1.2/vclog.egg-info/
--rw-rw-r--   0 vistor    (1001) vistor    (1001)     2563 2023-03-17 10:20:35.000000 vclog-0.1.2/vclog.egg-info/PKG-INFO
--rw-rw-r--   0 vistor    (1001) vistor    (1001)      303 2023-03-17 10:20:35.000000 vclog-0.1.2/vclog.egg-info/SOURCES.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)        1 2023-03-17 10:20:35.000000 vclog-0.1.2/vclog.egg-info/dependency_links.txt
--rw-rw-r--   0 vistor    (1001) vistor    (1001)        6 2023-03-17 10:20:35.000000 vclog-0.1.2/vclog.egg-info/top_level.txt
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-13 08:30:12.223101 vclog-1.0.0/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1062 2023-03-01 11:15:44.000000 vclog-1.0.0/LICENSE
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2563 2023-04-13 08:30:12.223101 vclog-1.0.0/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2090 2023-04-13 06:58:28.000000 vclog-1.0.0/README.md
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      563 2023-04-13 08:28:25.000000 vclog-1.0.0/pyproject.toml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-13 08:30:12.223101 vclog-1.0.0/setup.cfg
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-13 08:30:12.223101 vclog-1.0.0/vclog/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       51 2023-03-01 10:29:37.000000 vclog-1.0.0/vclog/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-13 08:30:12.223101 vclog-1.0.0/vclog/core/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       51 2023-03-01 10:29:15.000000 vclog-1.0.0/vclog/core/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      472 2023-04-13 08:23:53.000000 vclog-1.0.0/vclog/core/codes.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1130 2023-04-13 08:22:12.000000 vclog-1.0.0/vclog/core/colors.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6373 2023-04-13 08:11:10.000000 vclog-1.0.0/vclog/logger.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-13 08:30:12.223101 vclog-1.0.0/vclog/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-03-01 11:00:04.000000 vclog-1.0.0/vclog/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      669 2023-04-13 08:13:29.000000 vclog-1.0.0/vclog/use_cases/formatter.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-13 08:30:12.223101 vclog-1.0.0/vclog.egg-info/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2563 2023-04-13 08:30:12.000000 vclog-1.0.0/vclog.egg-info/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      303 2023-04-13 08:30:12.000000 vclog-1.0.0/vclog.egg-info/SOURCES.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        1 2023-04-13 08:30:12.000000 vclog-1.0.0/vclog.egg-info/dependency_links.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        6 2023-04-13 08:30:12.000000 vclog-1.0.0/vclog.egg-info/top_level.txt
```

### Comparing `vclog-0.1.2/LICENSE` & `vclog-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vclog-0.1.2/PKG-INFO` & `vclog-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vclog
-Version: 0.1.2
+Version: 1.0.0
 Summary: A minimal logger for a minimal experience
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/vclog
 Project-URL: Bug Tracker, https://github.com/vistormu/vclog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vclog-0.1.2/README.md` & `vclog-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vclog-0.1.2/pyproject.toml` & `vclog-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vclog"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name="Vistor"},
 ]
 description = "A minimal logger for a minimal experience"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `vclog-0.1.2/vclog/core/codes.py` & `vclog-1.0.0/vclog/core/colors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-import dataclasses
+from typing import NamedTuple
 
 
-@dataclasses.dataclass
-class Codes:
-    end = "\x1b[0m"
-    bold = "\x1b[1m"
-    dim = "\x1b[2m"
-    italic = "\x1b[2m"
-    underscore = "\x1b[4m"
-    blink = "\x1b[5m"
-    highlight = "\x1b[7m"
-    hidden = "\x1b[8m"
-    strikethrough = "\x1b[9m"
-    double_underscore = "\x1b[21m"
-
+class Colors(NamedTuple):
     black = "\x1b[30m"
     red = "\x1b[31m"
     green = "\x1b[32m"
     yellow = "\x1b[33m"
     blue = "\x1b[34m"
     magenta = "\x1b[35m"
     cyan = "\x1b[36m"
     white = "\x1b[37m"
 
-    black_bg = "\x1b[40m"
-    red_bg = "\x1b[41m"
-    green_bg = "\x1b[42m"
-    yellow_bg = "\x1b[43m"
-    blue_bg = "\x1b[44m"
-    magenta_bg = "\x1b[45m"
-    cyan_bg = "\x1b[46m"
-    white_bg = "\x1b[47m"
-
     secondary_black = "\x1b[90m"
     secondary_red = "\x1b[91m"
     secondary_green = "\x1b[92m"
     secondary_yellow = "\x1b[93m"
     secondary_blue = "\x1b[94m"
     secondary_magenta = "\x1b[95m"
     secondary_cyan = "\x1b[96m"
     secondary_white = "\x1b[97m"
 
-    secondary_black_bg = "\x1b[40m"
-    secondary_red_bg = "\x1b[41m"
-    secondary_green_bg = "\x1b[42m"
-    secondary_yellow_bg = "\x1b[43m"
-    secondary_blue_bg = "\x1b[44m"
-    secondary_magenta_bg = "\x1b[45m"
-    secondary_cyan_bg = "\x1b[46m"
-    secondary_white_bg = "\x1b[47m"
+    black_bg = "\x1b[40m"
+    red_bg = "\x1b[41m"
+    green_bg = "\x1b[42m"
+    yellow_bg = "\x1b[43m"
+    blue_bg = "\x1b[44m"
+    magenta_bg = "\x1b[45m"
+    cyan_bg = "\x1b[46m"
+    white_bg = "\x1b[47m"
 
-    line_up = "\x1b[1A"
-    line_clear = "\x1b[2K"
+    secondary_black_bg = "\x1b[100m"
+    secondary_red_bg = "\x1b[101m"
+    secondary_green_bg = "\x1b[102m"
+    secondary_yellow_bg = "\x1b[103m"
+    secondary_blue_bg = "\x1b[104m"
+    secondary_magenta_bg = "\x1b[105m"
+    secondary_cyan_bg = "\x1b[106m"
+    secondary_white_bg = "\x1b[107m"
+
+    @classmethod
+    def get(cls, color: str) -> str:
+        return getattr(cls, color) if hasattr(cls, color) else ''
```

### Comparing `vclog-0.1.2/vclog.egg-info/PKG-INFO` & `vclog-1.0.0/vclog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vclog
-Version: 0.1.2
+Version: 1.0.0
 Summary: A minimal logger for a minimal experience
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/vclog
 Project-URL: Bug Tracker, https://github.com/vistormu/vclog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

