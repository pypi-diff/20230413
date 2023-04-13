# Comparing `tmp/commons-1c-3.6.6.tar.gz` & `tmp/commons-1c-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commons-1c-3.6.6.tar", last modified: Thu Mar  9 12:05:04 2023, max compression
+gzip compressed data, was "commons-1c-3.6.8.tar", last modified: Thu Apr 13 12:27:49 2023, max compression
```

## Comparing `commons-1c-3.6.6.tar` & `commons-1c-3.6.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:05:04.624116 commons-1c-3.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-09 12:05:04.624116 commons-1c-3.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-09 12:04:45.000000 commons-1c-3.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-09 12:04:45.000000 commons-1c-3.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 12:05:04.624116 commons-1c-3.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:05:04.624116 commons-1c-3.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:05:04.624116 commons-1c-3.6.6/src/commons_1c/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 12:04:45.000000 commons-1c-3.6.6/src/commons_1c/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 12:04:45.000000 commons-1c-3.6.6/src/commons_1c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-09 12:04:45.000000 commons-1c-3.6.6/src/commons_1c/platform_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-09 12:04:45.000000 commons-1c-3.6.6/src/commons_1c/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:05:04.624116 commons-1c-3.6.6/src/commons_1c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-09 12:05:04.000000 commons-1c-3.6.6/src/commons_1c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-09 12:05:04.000000 commons-1c-3.6.6/src/commons_1c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:05:04.000000 commons-1c-3.6.6/src/commons_1c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-09 12:05:04.000000 commons-1c-3.6.6/src/commons_1c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-09 12:05:04.000000 commons-1c-3.6.6/src/commons_1c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:05:04.624116 commons-1c-3.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-09 12:04:45.000000 commons-1c-3.6.6/tests/test_commons_1c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:27:49.066872 commons-1c-3.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-13 12:27:49.066872 commons-1c-3.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 12:27:18.000000 commons-1c-3.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 12:27:18.000000 commons-1c-3.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:27:49.066872 commons-1c-3.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:27:49.066872 commons-1c-3.6.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:27:49.066872 commons-1c-3.6.8/src/commons_1c/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 12:27:18.000000 commons-1c-3.6.8/src/commons_1c/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 12:27:18.000000 commons-1c-3.6.8/src/commons_1c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 12:27:18.000000 commons-1c-3.6.8/src/commons_1c/platform_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 12:27:18.000000 commons-1c-3.6.8/src/commons_1c/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:27:49.066872 commons-1c-3.6.8/src/commons_1c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-13 12:27:49.000000 commons-1c-3.6.8/src/commons_1c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 12:27:49.000000 commons-1c-3.6.8/src/commons_1c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:27:49.000000 commons-1c-3.6.8/src/commons_1c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 12:27:49.000000 commons-1c-3.6.8/src/commons_1c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:27:49.000000 commons-1c-3.6.8/src/commons_1c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:27:49.066872 commons-1c-3.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 12:27:18.000000 commons-1c-3.6.8/tests/test_commons_1c.py
```

### Comparing `commons-1c-3.6.6/PKG-INFO` & `commons-1c-3.6.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commons-1c
-Version: 3.6.6
+Version: 3.6.8
 Summary: Commons for 1C:Enterprise
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/commons-1c
 Keywords: 1c,commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `commons-1c-3.6.6/pyproject.toml` & `commons-1c-3.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 ]
 description = "Commons for 1C:Enterprise"
 keywords = ["1c", "commons"]
 license = {text = "MIT"}
 name = "commons-1c"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "3.6.6"
+version = "3.6.8"
 
 [project.urls]
 repository = "https://github.com/Cujoko-Dev/commons-1c"
 
 [tool.pdm]
```

### Comparing `commons-1c-3.6.6/src/commons_1c/platform_.py` & `commons-1c-3.6.8/src/commons_1c/platform_.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,54 +7,73 @@
 
 from commons_1c.version import get_version_as_number
 
 logger.disable(__name__)
 
 
 def get_last_exe_file_fullpath(file_name: str, **kwargs) -> Path:
+    """Получить путь к exe-файлу из последней установленной платформы 1С
+
+    Args:
+        - file_name (str) -- Имя файла
+
+    Raises:
+        - FileExistsError -- Возникает, если файл не существует
+
+    Returns:
+        - Path -- Путь к exe-файлу
+    """
+
     result = None
 
-    config_file_fullpath = get_path_attribute(
-        kwargs, 'config_file_path', default_path=Path(site_data_dir('1CEStart', '1C'), '1CEStart.cfg'), is_dir=False,
-        check_if_exists=False)
+    config_file_path = get_path_attribute(
+        kwargs,
+        "config_file_path",
+        default_path=Path(site_data_dir("1CEStart", "1C"), "1CEStart.cfg"),
+        is_dir=False,
+        check_if_exists=False,
+    )
 
-    if config_file_fullpath.is_file():
-        installed_location_fullpaths = []
+    if config_file_path.is_file():
+        installed_location_paths = []
 
-        with config_file_fullpath.open(encoding='utf-16') as config_file:
+        with config_file_path.open(encoding="utf-16") as config_file:
             for line in config_file.readlines():
-                key_and_value = line.split('=')
-                if key_and_value[0] == 'InstalledLocation':
-                    value = '='.join(key_and_value[1:])
-                    installed_location_fullpaths.append(Path(value.rstrip('\n')))
+                key_and_value = line.split("=")
+                if key_and_value[0] == "InstalledLocation":
+                    value = "=".join(key_and_value[1:])
+                    installed_location_paths.append(Path(value.rstrip("\n")))
 
         platform_versions = []
 
-        for installed_location_fullpath in installed_location_fullpaths:
-            if installed_location_fullpath.is_dir():
-                for version_dir_fullpath in installed_location_fullpath.rglob('*'):  # todo
-                    version_as_number = get_version_as_number(version_dir_fullpath.name)
+        for installed_location_path in installed_location_paths:
+            if installed_location_path.is_dir():
+                # todo
+                for version_dir_path in installed_location_path.rglob("*"):
+                    version_as_number = get_version_as_number(version_dir_path.name)
                     if version_as_number:
-                        exe_file_fullpath = Path(version_dir_fullpath, 'bin', file_name)
-                        if exe_file_fullpath.is_file():
-                            platform_versions.append((version_as_number, exe_file_fullpath))
-
-        platform_versions_reversed = sorted(platform_versions, key=lambda x: x[0], reverse=True)
+                        exe_file_path = Path(version_dir_path, "bin", file_name)
+                        if exe_file_path.is_file():
+                            platform_versions.append((version_as_number, exe_file_path))
+
+        platform_versions_reversed = sorted(
+            platform_versions, key=lambda x: x[0], reverse=True
+        )
 
         if platform_versions_reversed:
             result = platform_versions_reversed[0][1]
     else:
-        raise FileExistsError('1CEStart.cfg file does not exist')
+        raise FileExistsError("1CEStart.cfg file does not exist")
 
     return result
 
 
 def get_last_1c_exe_file_fullpath(**kwargs) -> Path:
-    return get_last_exe_file_fullpath('1cv8.exe', **kwargs)
+    return get_last_exe_file_fullpath("1cv8.exe", **kwargs)
 
 
 def get_last_ibcmd_exe_file_fullpath(**kwargs) -> Path:
-    return get_last_exe_file_fullpath('ibcmd.exe', **kwargs)
+    return get_last_exe_file_fullpath("ibcmd.exe", **kwargs)
 
 
 def get_last_rac_exe_file_fullpath(**kwargs) -> Path:
-    return get_last_exe_file_fullpath('rac.exe', **kwargs)
+    return get_last_exe_file_fullpath("rac.exe", **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commons-1c-3.6.6/src/commons_1c/version.py` & `commons-1c-3.6.8/src/commons_1c/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,60 @@
 import re
 from typing import List
 
 from loguru import logger
 
 logger.disable(__name__)
 
-pattern_version = re.compile(r'\D*(?P<version>(?:(\d+)|)(?:\.(\d+)|)(?:\.(\d+)|)(?:\.(\d+)|))\D*')
+pattern_version = re.compile(
+    r"\D*(?P<version>(?:(\d+)|)(?:\.(\d+)|)(?:\.(\d+)|)(?:\.(\d+)|))\D*"
+)
 
 
 def get_version_as_number(version: str, m: int = 10000) -> int:
     result = 0
 
     match = pattern_version.match(version)
     if match is not None:
         a = match.group(2)
-        a = '0' if a is None else a
+        a = "0" if a is None else a
+
         b = match.group(3)
-        b = '0' if b is None else b
+        b = "0" if b is None else b
+
         c = match.group(4)
-        c = '0' if c is None else c
+        c = "0" if c is None else c
+
         d = match.group(5)
-        d = '0' if d is None else d
-        result = int(a) * m ** 3 + int(b) * m ** 2 + int(c) * m + int(d)
+        d = "0" if d is None else d
+
+        result = int(a) * m**3 + int(b) * m**2 + int(c) * m + int(d)
 
     return result
 
 
 def get_version_as_parts(version: str) -> List[str]:
     result = []
     match = pattern_version.match(version)
+
     if match is not None:
         a = match.group(2)
+
         if a is not None:
             result.append(a)
+
         b = match.group(3)
+
         if b is not None:
             result.append(b)
+
         c = match.group(4)
+
         if c is not None:
             result.append(c)
+
         d = match.group(5)
+
         if d is not None:
             result.append(d)
+
     return result
```

### Comparing `commons-1c-3.6.6/src/commons_1c.egg-info/PKG-INFO` & `commons-1c-3.6.8/src/commons_1c.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commons-1c
-Version: 3.6.6
+Version: 3.6.8
 Summary: Commons for 1C:Enterprise
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/commons-1c
 Keywords: 1c,commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

