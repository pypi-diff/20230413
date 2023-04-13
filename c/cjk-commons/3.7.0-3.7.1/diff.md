# Comparing `tmp/cjk-commons-3.7.0.tar.gz` & `tmp/cjk-commons-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjk-commons-3.7.0.tar", last modified: Tue Mar 14 18:20:43 2023, max compression
+gzip compressed data, was "cjk-commons-3.7.1.tar", last modified: Thu Apr 13 12:26:06 2023, max compression
```

## Comparing `cjk-commons-3.7.0.tar` & `cjk-commons-3.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:20:43.615934 cjk-commons-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/src/cjk_commons/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/logging_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/src/cjk_commons/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/src/cjk_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 18:20:43.000000 cjk-commons-3.7.0/src/cjk_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-14 18:20:43.000000 cjk-commons-3.7.0/src/cjk_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:20:43.000000 cjk-commons-3.7.0/src/cjk_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 18:20:43.000000 cjk-commons-3.7.0/src/cjk_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 18:20:43.000000 cjk-commons-3.7.0/src/cjk_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:20:43.619934 cjk-commons-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-14 18:20:23.000000 cjk-commons-3.7.0/tests/test_commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:06.192767 cjk-commons-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-13 12:26:06.192767 cjk-commons-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:26:06.192767 cjk-commons-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:06.188768 cjk-commons-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:06.188768 cjk-commons-3.7.1/src/cjk_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/logging_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/src/cjk_commons/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:06.192767 cjk-commons-3.7.1/src/cjk_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-13 12:26:06.000000 cjk-commons-3.7.1/src/cjk_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 12:26:06.000000 cjk-commons-3.7.1/src/cjk_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:26:06.000000 cjk-commons-3.7.1/src/cjk_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 12:26:06.000000 cjk-commons-3.7.1/src/cjk_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 12:26:06.000000 cjk-commons-3.7.1/src/cjk_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:06.192767 cjk-commons-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-13 12:25:35.000000 cjk-commons-3.7.1/tests/test_commons.py
```

### Comparing `cjk-commons-3.7.0/PKG-INFO` & `cjk-commons-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjk-commons
-Version: 3.7.0
+Version: 3.7.1
 Summary: Commons
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/commons
 Keywords: commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `cjk-commons-3.7.0/pyproject.toml` & `cjk-commons-3.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 ]
 description = "Commons"
 keywords = ["commons"]
 license = {text = "MIT"}
 name = "cjk-commons"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "3.7.0"
+version = "3.7.1"
 
 [project.urls]
 repository = "https://github.com/Cujoko-Dev/commons"
 
 [tool.pdm]
```

### Comparing `cjk-commons-3.7.0/src/cjk_commons/file.py` & `cjk-commons-3.7.1/src/cjk_commons/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 from pathlib import Path
 
 
-def rename_bak_paths(path: Path, bakfix: str = 'bak') -> None:
+def rename_bak_paths(path: Path, bakfix: str = "bak") -> None:
     n = 1
-    
+
     # Найдём самый большой n
     while True:
         if path.is_dir():
-            bak_path = path.parent / f'{path.name}-{bakfix}-{n}'
+            bak_path = path.parent / f"{path.name}-{bakfix}-{n}"
         else:
-            bak_path = path.parent / f'{path.stem}-{bakfix}-{n}{path.suffix}'
-        
+            bak_path = path.parent / f"{path.stem}-{bakfix}-{n}{path.suffix}"
+
         if bak_path.exists():
             n += 1
         else:
             n -= 1
             break
-            
+
     if n > 0:
         # Переименуем bak-пути
         for k in range(n, 0, -1):
             if path.is_dir():
-                (path.parent / f'{path.name}-{bakfix}-{k}').rename(
-                    (path.parent / f'{path.name}-{bakfix}-{k + 1}')
+                (path.parent / f"{path.name}-{bakfix}-{k}").rename(
+                    (path.parent / f"{path.name}-{bakfix}-{k + 1}")
                 )
             else:
-                (path.parent / f'{path.stem}-{bakfix}-{k}{path.suffix}').rename(
-                    (path.parent / f'{path.stem}-{bakfix}-{k + 1}{path.suffix}')
+                (path.parent / f"{path.stem}-{bakfix}-{k}{path.suffix}").rename(
+                    (path.parent / f"{path.stem}-{bakfix}-{k + 1}{path.suffix}")
                 )
 
     if path.is_dir():
-        path.rename(path.parent / f'{path.name}-{bakfix}-1')
+        path.rename(path.parent / f"{path.name}-{bakfix}-1")
     else:
-        path.rename(path.parent / f'{path.stem}-{bakfix}-1{path.suffix}')
+        path.rename(path.parent / f"{path.stem}-{bakfix}-1{path.suffix}")
```

### Comparing `cjk-commons-3.7.0/src/cjk_commons/settings.py` & `cjk-commons-3.7.1/src/cjk_commons/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,105 +5,149 @@
 import yaml
 import yodl
 from appdirs import site_data_dir, user_data_dir
 from loguru import logger
 
 
 def get_attribute(
-        kwargs: dict, kwargs_key: str, settings: dict = None, settings_key: str = None,
-        default: Any = None, type_: type = str, allow_none: bool = False) -> Any:
+    kwargs: dict,
+    kwargs_key: str,
+    settings: dict = None,
+    settings_key: str = None,
+    default: Any = None,
+    type_: type = str,
+    allow_none: bool = False,
+) -> Any:
     result = None
     type__ = type_
+
     if default is not None:
         type__ = type(default)
+
     if kwargs_key in kwargs:
         result = kwargs[kwargs_key]
+
         if not isinstance(result, type__) and default is not None:
-            raise TypeError(f'{kwargs_key}' if kwargs_key else None)
+            raise TypeError(f"{kwargs_key}" if kwargs_key else None)
+
     if settings is not None and settings_key is not None:
         if settings_key in settings:
             result = settings[settings_key]
+
             if not isinstance(result, type__) and default is not None:
-                raise TypeError(f'{settings_key}' if settings_key else None)
+                raise TypeError(f"{settings_key}" if settings_key else None)
+
     if result is None:
         result = default
+
     if result is None and not allow_none:
-        raise AttributeError(f'{settings_key}')
+        raise AttributeError(f"{settings_key}")
+
     return result
 
 
 def get_path_attribute(
-        kwargs: dict, kwargs_key: str, settings: dict = None, settings_key: str = None,
-        default_path: Path = None, is_dir: bool = True, check_if_exists: bool = True, create_dir: bool = True,
-        create_parents: bool = True) -> Path:
+    kwargs: dict,
+    kwargs_key: str,
+    settings: dict = None,
+    settings_key: str = None,
+    default_path: Path = None,
+    is_dir: bool = True,
+    check_if_exists: bool = True,
+    create_dir: bool = True,
+    create_parents: bool = True,
+) -> Path:
     result = None
+
     if kwargs_key in kwargs:
         result = kwargs[kwargs_key]
+
         if not isinstance(result, Path):
-            raise TypeError(f'{kwargs_key}' if kwargs_key else None)
+            raise TypeError(f"{kwargs_key}" if kwargs_key else None)
+
     elif settings is not None and settings_key is not None:
         if settings_key in settings:
             result_str = settings[settings_key]
+
             if not isinstance(result_str, str):
-                raise TypeError(f'{settings_key}' if settings_key else None)
+                raise TypeError(f"{settings_key}" if settings_key else None)
+
             result = Path(result_str)
+
             if not isinstance(result, Path):
-                raise TypeError(f'{settings_key}' if settings_key else None)
+                raise TypeError(f"{settings_key}" if settings_key else None)
+
     if result is None and isinstance(default_path, Path):
         result = default_path
+
     if result is None:
-        raise AttributeError(f'{settings_key}')
+        raise AttributeError(f"{settings_key}")
+
     if result.exists():
         if not is_dir and result.is_dir():
-            raise FileExistsError(f'{kwargs_key} Not A File' if kwargs_key else None, result)
+            raise FileExistsError(
+                f"{kwargs_key} Not A File" if kwargs_key else None, result
+            )
+
         elif is_dir and result.is_file():
-            raise NotADirectoryError(f'{kwargs_key}' if kwargs_key else None, result)
+            raise NotADirectoryError(f"{kwargs_key}" if kwargs_key else None, result)
     else:
         if check_if_exists:
-            raise FileExistsError(f'{kwargs_key}' if kwargs_key else None, result)
+            raise FileExistsError(f"{kwargs_key}" if kwargs_key else None, result)
+
         if is_dir and create_dir:
             result.mkdir(parents=create_parents)
+
     return result
 
 
 class SettingsError(Exception):
     """Settings Error"""
 
 
-def get_settings(file_path=Path('settings.yaml'), **kwargs) -> dict:
+def get_settings(file_path=Path("settings.yaml"), **kwargs) -> dict:
     if not file_path.is_file():
-        app_name = get_attribute(kwargs, 'app_name', allow_none=True)
-        app_author = get_attribute(kwargs, 'app_author', allow_none=True)
-        file_path = Path(user_data_dir(app_name, app_author, roaming=True), file_path.name)
+        app_name = get_attribute(kwargs, "app_name", allow_none=True)
+        app_author = get_attribute(kwargs, "app_author", allow_none=True)
+        file_path = Path(
+            user_data_dir(app_name, app_author, roaming=True), file_path.name
+        )
+
         if not file_path.is_file():
             file_path = Path(site_data_dir(app_name, app_author), file_path.name)
     if file_path.is_file():
-        with file_path.open(encoding='utf-8') as settings_file:
+        with file_path.open(encoding="utf-8") as settings_file:
             settings = yaml.load(settings_file, yodl.OrderedDictYAMLLoader)
+
         if settings is None:
             settings = {}
     else:
         settings = {}
+
     return settings
 
 
 class OrderedDictMergeException(Exception):
     """Ordered Dict Merge Exception"""
 
 
 def merge(a: dict, b: dict, path=None) -> dict:
     if path is None:
         path = []
+
     for key in b:
         if key in a:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
                 merge(a[key], b[key], path + [str(key)])
             elif a[key] == b[key]:
                 pass
             else:
-                raise OrderedDictMergeException(f'Conflict at \'{".".join(path + [str(key)])}\'')
+                raise OrderedDictMergeException(
+                    f'Conflict at \'{".".join(path + [str(key)])}\''
+                )
         else:
             a[key] = b[key]
+
     return a
 
 
 logger.disable(__name__)
```

### Comparing `cjk-commons-3.7.0/src/cjk_commons/zip.py` & `cjk-commons-3.7.1/src/cjk_commons/zip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # -*- coding: utf-8 -*-
 import os
-from pathlib import Path
 import time
-from typing import List
 import zipfile
+from pathlib import Path
+from typing import List
 
 from loguru import logger
 
 
 def extract_from_zip(zip_path: Path, dir_path: Path) -> None:
     with zipfile.ZipFile(zip_path) as zip_file:
         for zip_member in zip_file.infolist():
             zip_file.extract(zip_member, dir_path)
             zip_member_time = time.mktime(zip_member.date_time + (0, 0, -1))
-            os.utime(Path(dir_path, zip_member.filename), (zip_member_time, zip_member_time))
+            os.utime(
+                Path(dir_path, zip_member.filename), (zip_member_time, zip_member_time)
+            )
 
 
 def write_to_zip(zip_path: Path, in_path: Path, file_paths: List[Path] = None) -> float:
-    with zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED) as zip_file:
-        mtime = -1.
+    with zipfile.ZipFile(zip_path, "w", zipfile.ZIP_DEFLATED) as zip_file:
+        mtime = -1.0
+
         if in_path.is_file():
             zip_file.write(in_path, in_path.name)
             mtime = in_path.stat().st_mtime
         elif in_path.is_dir():
             if not file_paths:
                 file_paths = []
+
                 for root, dirnames, filenames in os.walk(str(in_path)):
                     for filename in filenames:
                         file_paths.append(Path(root, filename))
+
             for file_path in file_paths:
                 if file_path.is_file():
                     zip_file.write(file_path, file_path.relative_to(in_path))
                     file_stat_result = file_path.stat()  # todo
+
                     if mtime < file_stat_result.st_mtime:
                         mtime = file_stat_result.st_mtime
+
         return mtime
 
 
 logger.disable(__name__)
```

### Comparing `cjk-commons-3.7.0/src/cjk_commons.egg-info/PKG-INFO` & `cjk-commons-3.7.1/src/cjk_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjk-commons
-Version: 3.7.0
+Version: 3.7.1
 Summary: Commons
 Author-email: Cujoko <cujoko@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/Cujoko-Dev/commons
 Keywords: commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `cjk-commons-3.7.0/tests/test_commons.py` & `cjk-commons-3.7.1/tests/test_commons.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,57 +5,65 @@
 
 from cjk_commons.settings import OrderedDictMergeException, get_settings, merge
 from cjk_commons.zip import extract_from_zip, write_to_zip
 
 
 def test_get_settings_1():
     with pytest.raises(Exception) as e:
-        get_settings(app_name='bla', app_author='bla')
-        assert e == 'Settings file does not exist'
+        get_settings(app_name="bla", app_author="bla")
+
+        assert e == "Settings file does not exist"
 
 
 def test_get_settings_2():
     with pytest.raises(Exception) as e:
-        get_settings(Path('bla.yaml'))
-        assert e == 'Argument \'app_name\' does not exist'
+        get_settings(Path("bla.yaml"))
+
+        assert e == "Argument 'app_name' does not exist"
 
 
 def test_get_settings_3():
-    assert isinstance(get_settings(Path('tests/data/settings.yaml')), dict)
+    assert isinstance(get_settings(Path("tests/data/settings.yaml")), dict)
 
 
 def test_merge_1():
-    a = {'a': 1}
-    b = {'a': 1}
+    a = {"a": 1}
+    b = {"a": 1}
+
     assert isinstance(merge(a, b), dict)
 
 
 def test_merge_2():
-    a = {'a': 1}
-    b = {'a': 2}
+    a = {"a": 1}
+    b = {"a": 2}
+
     with pytest.raises(OrderedDictMergeException):
         merge(a, b)
 
 
 def test_merge_3():
-    a = {'b': {'a', 1}}
-    b = {'b': {'b', 2}}
+    a = {"b": {"a", 1}}
+    b = {"b": {"b", 2}}
     c = merge(a, b)
+
     assert isinstance(c, dict)
 
 
 def test_extract_from_zip(tmpdir):
-    temp_dir_fullpath = Path(tmpdir)
-    extract_from_zip(Path('tests/data/test.zip'), temp_dir_fullpath)
-    assert Path(temp_dir_fullpath, 'test.txt').is_file()
+    temp_dir_path = Path(tmpdir)
+    extract_from_zip(Path("tests/data/test.zip"), temp_dir_path)
+
+    assert Path(temp_dir_path, "test.txt").is_file()
 
 
 def test_write_to_zip_1(tmpdir):
-    temp_dir_fullpath = Path(tmpdir)
-    write_to_zip(Path(temp_dir_fullpath, 'test.zip'), Path('tests/data/test.txt'))
-    assert Path(temp_dir_fullpath, 'test.zip').is_file()
+    temp_dir_path = Path(tmpdir)
+    write_to_zip(Path(temp_dir_path, "test.zip"), Path("tests/data/test.txt"))
+
+    assert Path(temp_dir_path, "test.zip").is_file()
 
 
 def test_write_to_zip_2(tmpdir):
-    temp_dir_fullpath = Path(tmpdir)
-    write_to_zip(Path(temp_dir_fullpath, 'test.zip'), Path('tests/data/test'))
-    assert Path(temp_dir_fullpath, 'test.zip').is_file()
+    temp_dir_path = Path(tmpdir)
+    write_to_zip(Path(temp_dir_path, "test.zip"), Path("tests/data/test"))
+
+    assert Path(temp_dir_path, "test.zip").is_file()
```

