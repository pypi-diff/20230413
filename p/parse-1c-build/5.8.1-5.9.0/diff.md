# Comparing `tmp/parse-1c-build-5.8.1.tar.gz` & `tmp/parse-1c-build-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse-1c-build-5.8.1.tar", last modified: Wed Jun 26 15:03:36 2019, max compression
+gzip compressed data, was "parse-1c-build-5.9.0.tar", last modified: Sun Jun 30 08:17:14 2019, max compression
```

## Comparing `parse-1c-build-5.8.1.tar` & `parse-1c-build-5.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2026 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/README.md
--rw-r--r--   0        0        0       74 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/__about__.py
--rw-r--r--   0        0        0      404 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/__init__.py
--rw-r--r--   0        0        0      185 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/__main__.py
--rw-r--r--   0        0        0     1615 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/base.py
--rw-r--r--   0        0        0     4582 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/build.py
--rw-r--r--   0        0        0      807 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/cli.py
--rw-r--r--   0        0        0      329 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/core.py
--rw-r--r--   0        0        0     4396 2019-06-26 15:03:05.628671 parse-1c-build-5.8.1/parse_1c_build/parse.py
--rw-r--r--   0        0        0      873 2019-06-26 15:03:05.632669 parse-1c-build-5.8.1/pyproject.toml
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 parse-1c-build-5.8.1/setup.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 parse-1c-build-5.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2026 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/README.md
+-rw-r--r--   0        0        0       74 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/__about__.py
+-rw-r--r--   0        0        0      333 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/__init__.py
+-rw-r--r--   0        0        0      185 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/__main__.py
+-rw-r--r--   0        0        0     1615 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/base.py
+-rw-r--r--   0        0        0     4555 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/build.py
+-rw-r--r--   0        0        0      807 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/cli.py
+-rw-r--r--   0        0        0      309 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/core.py
+-rw-r--r--   0        0        0     4503 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/parse_1c_build/parse.py
+-rw-r--r--   0        0        0      891 2019-06-30 08:16:45.013506 parse-1c-build-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 parse-1c-build-5.9.0/setup.py
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 parse-1c-build-5.9.0/PKG-INFO
```

### Comparing `parse-1c-build-5.8.1/README.md` & `parse-1c-build-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `parse-1c-build-5.8.1/parse_1c_build/base.py` & `parse-1c-build-5.9.0/parse_1c_build/base.py`

 * *Files identical despite different names*

### Comparing `parse-1c-build-5.8.1/parse_1c_build/build.py` & `parse-1c-build-5.9.0/parse_1c_build/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
-import logging
 import os
 from pathlib import Path
 import subprocess
 import sys
 import tempfile
 
+from loguru import logger
 import shutil
 
 from parse_1c_build.base import Processor, add_generic_arguments
 
-logger = logging.getLogger(__name__)
-
 
 class Builder(Processor):
     @staticmethod
     def get_temp_source_dir_fullpath(input_dir_fullpath: Path) -> Path:
         temp_source_dir_fullpath = Path(tempfile.mkdtemp())
         renames_file_fullpath = Path(input_dir_fullpath, 'renames.txt')
         with renames_file_fullpath.open(encoding='utf-8-sig') as renames_file:
```

### Comparing `parse-1c-build-5.8.1/parse_1c_build/cli.py` & `parse-1c-build-5.9.0/parse_1c_build/cli.py`

 * *Files identical despite different names*

### Comparing `parse-1c-build-5.8.1/parse_1c_build/parse.py` & `parse-1c-build-5.9.0/parse_1c_build/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
-import logging
 import os
 from pathlib import Path
 import subprocess
 import sys
 import tempfile
 
+from loguru import logger
 import shutil
 
 from cjk_commons.settings import get_path_attribute
 from commons_1c import platform_
 from parse_1c_build.base import Processor, add_generic_arguments
 
-logger = logging.getLogger(__name__)
+logger.enable('cjk_commons')
+logger.enable('commons_1c')
 
 
 class Parser(Processor):
     def get_1c_exe_file_fullpath(self, **kwargs) -> Path:
-        return get_path_attribute(kwargs, '1c_file_path', default_path=platform_.get_last_1c_exe_file_fullpath(),
-                                  is_dir=False)
+        result = get_path_attribute(kwargs, '1c_file_path', default_path=platform_.get_last_1c_exe_file_fullpath(),
+                                    is_dir=False)
+        return result
 
     def get_ib_dir_fullpath(self, **kwargs) -> Path:
-        return get_path_attribute(kwargs, 'ib_dir_path', self.settings, 'ib_dir', Path('IB'), create_dir=False)
+        result = get_path_attribute(kwargs, 'ib_dir_path', self.settings, 'ib_dir', Path('IB'), create_dir=False)
+        return result
 
     def get_v8_reader_file_fullpath(self, **kwargs) -> Path:
-        return get_path_attribute(kwargs, 'v8reader_file_path', self.settings, 'v8reader_file',
-                                  Path('V8Reader/V8Reader.epf'), False)
+        result = get_path_attribute(kwargs, 'v8reader_file_path', self.settings, 'v8reader_file',
+                                    Path('V8Reader/V8Reader.epf'), False)
+        return result
 
     def run(self, input_file_fullpath: Path, output_dir_fullpath: Path = None) -> None:
         input_file_fullpath_suffix_lower = input_file_fullpath.suffix.lower()
         if output_dir_fullpath is None:
             output_dir_fullpath = Path(input_file_fullpath.parent,
                                        input_file_fullpath.stem + '_' + input_file_fullpath.suffix[1:] + '_src')
         if input_file_fullpath_suffix_lower in ['.epf', '.erf']:
```

### Comparing `parse-1c-build-5.8.1/pyproject.toml` & `parse-1c-build-5.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parse-1c-build"
-version = "5.8.1"
+version = "5.9.0"
 description = "Parse and build utilities for 1C:Enterprise"
 authors = ["Cujoko <cujoko@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Cujoko/parse-1c-build"
 keywords = ["1c", "parse", "build", "v8reader", "v8unpack", "gcomp"]
 classifiers=[
@@ -20,14 +20,15 @@
 [tool.poetry.scripts]
 p1cb = "parse_1c_build.__main__:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cjk-commons = "^3.3"
 commons-1c = "^3.1"
+loguru = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.4"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `parse-1c-build-5.8.1/setup.py` & `parse-1c-build-5.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['parse_1c_build']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cjk-commons>=3.3,<4.0', 'commons-1c>=3.1,<4.0']
+['cjk-commons>=3.3,<4.0', 'commons-1c>=3.1,<4.0', 'loguru>=0.3.0,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['p1cb = parse_1c_build.__main__:run']}
 
 setup_kwargs = {
     'name': 'parse-1c-build',
-    'version': '5.8.1',
+    'version': '5.9.0',
     'description': 'Parse and build utilities for 1C:Enterprise',
     'long_description': 'Утилита для разборки и сборки *epf*-, *erf*-, *ert*- и *md*-файлов\n===\n\nЧто делает\n---\n\nПри установке пакета в каталоге скриптов интерпретатора Python создаётся исполняемый файл *p1cb.exe*. Его можно \nзапустить с командой *parse* для разборки *epf*- и *erf*-файлов с помощью [V8Reader][1] или V8Unpack, *ert*- и \n*md*-файлов с помощью [GComp][2], или с командой *build* для сборки *epf*- и *erf*-файлов с помощью V8Unpack, *ert*- и \n*md*-файлов с помощью [GComp][2].\n\nПути к сервисной информационной базе, *V8Reader.epf*, *V8Unpack.exe* и GComp указываются в файле настроек \n*settings.yaml*, который сначала ищется в текущем каталоге, затем в каталоге данных приложения пользователя \n(в Windows 10 каталог *C:\\Users\\\\<Пользователь>\\AppData\\Roaming\\util-1c\\parse-1c-build\\>*), а затем в общем каталоге \nданных приложения (в Windows 10 каталог *C:\\ProgramData\\util-1c\\parse-1c-build\\>*). Если путь к платформе \n1С:Предприятие 8 в файле настроек не указан, то он ищется автоматически.\n\nТребования\n---\n\n- Windows\n- Python 3.7 и выше. Каталоги интерпретатора и скриптов Python должны быть прописаны в переменной окружения Path\n- Платформа 1С:Предприятие 8.3\n- Сервисная информационная база (в которой будет запускаться *V8Reader.epf*)\n- [V8Reader][1]\n- V8Unpack\n- [GComp][2]\n\n[1]: https://github.com/xDrivenDevelopment/v8Reader\n[2]: http://1c.alterplast.ru/gcomp/\n',
     'author': 'Cujoko',
     'author_email': 'cujoko@gmail.com',
     'url': 'https://github.com/Cujoko/parse-1c-build',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `parse-1c-build-5.8.1/PKG-INFO` & `parse-1c-build-5.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-1c-build
-Version: 5.8.1
+Version: 5.9.0
 Summary: Parse and build utilities for 1C:Enterprise
 Home-page: https://github.com/Cujoko/parse-1c-build
 License: MIT
 Keywords: 1c,parse,build,v8reader,v8unpack,gcomp
 Author: Cujoko
 Author-email: cujoko@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: cjk-commons (>=3.3,<4.0)
 Requires-Dist: commons-1c (>=3.1,<4.0)
+Requires-Dist: loguru (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/Cujoko/parse-1c-build
 Description-Content-Type: text/markdown
 
 Утилита для разборки и сборки *epf*-, *erf*-, *ert*- и *md*-файлов
 ===
 
 Что делает
```

