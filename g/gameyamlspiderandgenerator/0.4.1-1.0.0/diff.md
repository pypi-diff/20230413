# Comparing `tmp/gameyamlspiderandgenerator-0.4.1.tar.gz` & `tmp/gameyamlspiderandgenerator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-0.4.1.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.0.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-0.4.1.tar` & `gameyamlspiderandgenerator-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2022-12-30 03:55:28.534848 gameyamlspiderandgenerator-0.4.1/LICENSE
--rwxr-xr-x   0        0        0      809 2023-02-11 13:40:27.035037 gameyamlspiderandgenerator-0.4.1/README.md
--rwxr-xr-x   0        0        0      614 2023-02-11 13:40:07.035668 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1057 2023-02-11 13:40:07.036276 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-02-09 08:13:15.170526 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-01-22 05:16:08.901166 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-01-22 05:16:08.901422 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2515 2023-02-11 13:35:56.097844 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-01-22 05:16:08.902312 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2406 2023-01-22 05:16:08.902831 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     5588 2023-02-11 13:46:30.233434 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7702 2023-02-11 13:40:07.037414 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-01-22 05:16:08.913666 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0      945 2023-02-11 13:40:07.037891 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0      812 2023-01-22 05:16:08.914586 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0      533 2023-02-11 13:40:07.038230 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2031 2023-01-22 08:08:03.762211 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     3295 2023-02-09 09:07:50.550888 gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      617 2023-02-11 13:48:22.244980 gameyamlspiderandgenerator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-0.4.1/setup.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2022-12-30 03:55:28.534848 gameyamlspiderandgenerator-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-13 11:43:35.714655 gameyamlspiderandgenerator-1.0.0/README.md
+-rwxr-xr-x   0        0        0      610 2023-04-13 11:36:40.137059 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0      980 2023-04-13 11:25:54.309363 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-02-09 08:13:15.170526 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-01-22 05:16:08.901166 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-01-22 05:16:08.901422 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     2441 2023-04-13 11:25:54.310342 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0       56 2023-01-22 05:16:08.902312 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2406 2023-01-22 05:16:08.902831 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     5469 2023-04-13 11:43:31.880195 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7593 2023-04-13 11:36:38.489756 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 05:16:08.913666 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0      889 2023-04-13 11:25:54.313431 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0      812 2023-01-22 05:16:08.914586 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1611 2023-04-13 11:36:39.905737 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1956 2023-04-13 11:25:54.315122 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2635 2023-04-13 11:36:40.039218 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      617 2023-04-13 11:43:47.612358 gameyamlspiderandgenerator-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.0.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-0.4.1/LICENSE` & `gameyamlspiderandgenerator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-0.4.1/README.md` & `gameyamlspiderandgenerator-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from typing import Optional, AnyStr
+from typing import Optional, Callable
 
 from loguru import logger
 
-from gameyamlspiderandgenerator.plugin import BasePlugin
-from gameyamlspiderandgenerator.util.plugin_manager import pkg
+from .plugin import BasePlugin
+from .util.fgi_yaml import YamlData
+from .util.plugin_manager import pkg
 
 
-def verify(url: str) -> Optional[BasePlugin]:
+def verify(url: str) -> Optional[Callable]:
     verify_list = [
         [
             pkg.plugin[n].verify,
             pkg.plugin[n],
         ]
         for n in pkg.plugin
     ]
     return next((cls for func, cls in verify_list if func(url)), None)
 
 
-def produce_yaml(url: str) -> Optional[AnyStr]:
-    ret = verify(url)
+def produce_yaml(url: str) -> Optional[YamlData]:
+    ret: Callable = verify(url)
     if ret is None:
         logger.error("URL is invalid")
         return
     return ret(url).to_yaml()
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 
 from yaml import safe_load
 
-from gameyamlspiderandgenerator import verify
-from gameyamlspiderandgenerator.util.config import config
-from gameyamlspiderandgenerator.util.plugin_manager import pkg
+from . import verify
+from .util.config import config
+from .util.plugin_manager import pkg
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "-f",
     "--config",
     type=str,
     default={"plugin": ["steam", "itchio"], "hook": ["search"]},
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from re import sub
 from typing import AnyStr
 from urllib.parse import quote_plus
 
 from bs4 import BeautifulSoup
 from loguru import logger
 
-from gameyamlspiderandgenerator.hook import BaseHook
-from gameyamlspiderandgenerator.util.config import config
-from gameyamlspiderandgenerator.util.spider import get_json, get_text
+from ..hook import BaseHook
+from ..util.config import config
+from ..util.spider import get_json, get_text
 
 print(config, type(config))
 
+
 class Search(BaseHook):
     @staticmethod
     def name_filter(s: AnyStr, rep: AnyStr = ""):
         return sub("[^A-z]", rep, s.lower())
 
     def __init__(self, name: str) -> None:
         logger.info(f"init {name}")
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from re import match, sub
 from typing import AnyStr, List
 
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
 
-from gameyamlspiderandgenerator.plugin._base import BasePlugin
-from gameyamlspiderandgenerator.util.fgi import fgi_dict
-from gameyamlspiderandgenerator.util.fgi_yaml import dump_to_yaml, pss_dedent
-from gameyamlspiderandgenerator.util.spider import get_text
+from ._base import BasePlugin
+from ..util.fgi import fgi_dict
+from ..util.fgi_yaml import YamlData, pss_dedent
+from ..util.spider import get_text
 
 
 class ItchIO(BasePlugin):
     _VERIFY_PATTERN = re.compile(r"https?://.+\.itch\.io/.+")
 
     @staticmethod
     def remove_query(s: str):
@@ -139,30 +139,30 @@
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
 
         temp = data.copy()
         for _ in pkg["hook"].values():
             temp = pkg["hook"].Search(self.get_name()).setup(temp)
         return temp
 
-    def to_yaml(self) -> str:
+    def to_yaml(self) -> YamlData:
         if type(self.data) == int:
             return self.data
         ret = {
             "name": self.get_name(),
-            "brief-description": self.get_desc(),
-            "description": self.get_brief_desc(),
+            "brief-description": self.get_brief_desc(),
+            "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
             "tags": {
                 "type": self.get_type_tag(),
                 "lang": self.get_langs(),
                 "platform": self.get_platforms(),
                 "misc": self.get_misc_tags(),
             },
             "links": self.get_links(),
-            "thumbnail": "thumbnail.png",
-            "screenshots": self.get_screenshots() #+ self.get_video(),   type: ignore
+            "thumbnail": self.get_thumbnail(),
+            "screenshots": self.get_screenshots()  # + self.get_video(),
         }
-        return dump_to_yaml(ret)
+        return YamlData(ret)
 
     def get_type_tag(self):
         pass
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import AnyStr, List, SupportsInt
 from urllib.parse import parse_qs, urlparse
 
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
 
-from gameyamlspiderandgenerator.plugin._base import BasePlugin
-from gameyamlspiderandgenerator.util.fgi import fgi_dict
-from gameyamlspiderandgenerator.util.fgi_yaml import dump_to_yaml, pss_dedent
-from gameyamlspiderandgenerator.util.spider import get_json, get_text
+from ._base import BasePlugin
+from ..util.fgi import fgi_dict
+from ..util.fgi_yaml import YamlData, pss_dedent
+from ..util.spider import get_json, get_text
 
 
 class Steam(BasePlugin):
     _VERIFY_PATTERN = re.compile(r"https?://store\.steampowered\.com/app/\d+/.+/?.+")
 
     @staticmethod
     def get_steam_id(link: AnyStr) -> SupportsInt:
@@ -34,32 +34,32 @@
         )
         self.data_html = get_text(link)
         self.soup = BeautifulSoup(self.data_html, "html.parser")
         self.name = self.get_name()
         temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
         self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
 
-    def to_yaml(self) -> AnyStr:
+    def to_yaml(self) -> YamlData:
         ret = {
             "name": self.get_name(),
-            "brief-description": self.get_desc(),
-            "description": self.get_brief_desc(),
+            "brief-description": self.get_brief_desc(),
+            "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
             "tags": {
                 "type": self.get_type_tag(),
                 "lang": self.get_langs(),
                 "platform": self.get_platforms(),
                 "misc": self.get_misc_tags(),
             },
             "links": self.get_links(),
-            "thumbnail": "thumbnail.png",
+            "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots() + self.get_video(),  # type: ignore
         }
-        return dump_to_yaml(ret)
+        return YamlData(ret)
 
     def get_langs(self) -> List[str]:
         temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
         return list({find(i).language for i in temp})
 
     def get_desc(self):
         return pss_dedent(
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from gameyamlspiderandgenerator.exception import ReadOrWriteConfigFailed
-from gameyamlspiderandgenerator.util.fgi_yaml import fgi
+from .fgi_yaml import fgi
+from ..exception import ReadOrWriteConfigFailed
 
 
 class Config:
     proxy = {}
     api = {}
     plugin = {}
     hook = {}
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 from typing import Dict, Literal, Type, Union, List
 
 from loguru import logger
 
-from gameyamlspiderandgenerator.hook import BaseHook
-from gameyamlspiderandgenerator.plugin import BasePlugin
-from gameyamlspiderandgenerator.util.config import config
+from ..hook import BaseHook
+from ..plugin import BasePlugin
+from ..util.config import config
 
 
 class Package:
     plugin: Dict[str, BasePlugin] = {}
     hook: Dict[str, BaseHook] = {}
     log: List[str] = []
```

### Comparing `gameyamlspiderandgenerator-0.4.1/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from pathlib import Path
-from typing import Dict, Union
+from typing import Dict
 
 import requests
 from requests import JSONDecodeError
 
-from gameyamlspiderandgenerator.exception import (
+from ..exception import (
     CommunicateWithServerFailed,
     InvalidResponse,
 )
-from gameyamlspiderandgenerator.util.config import config
+from ..util.config import config
 
 
 class GetResponse:
     """
     对 requests.get 的简单封装，使用上下文以保证资源被正确释放
 
     使用方法：
@@ -85,32 +84,17 @@
         Proxied for `self.response.status_code`
 
         Returns:
             状态码
         """
         return self.response.status_code
 
-    def to_disk(self, path: Union[str, Path], allow_exist: bool = False, /):
-        """
-        将响应内容写入磁盘
-
-        Args:
-            path: 路径
-            allow_exist: 是否允许覆盖已存在的文件
-        """
-        path = Path(path)
-        if path.is_file():
-            if allow_exist:
-                path.unlink()
-            else:
-                raise FileExistsError(f"File {path} already exists")
-        elif path.is_dir():
-            raise IsADirectoryError(f"{path} is a directory")
-        path.parent.mkdir(parents=True, exist_ok=True)
-        path.write_bytes(self.response.content)
+    @property
+    def bytes(self):
+        return self.response.content
 
 
 def get_json(url: str) -> Dict:
     with GetResponse(url) as resp:
         return resp.json
 
 
@@ -120,10 +104,10 @@
 
 
 def get_status(url: str) -> int:
     with GetResponse(url) as resp:
         return resp.status
 
 
-def download_file(url: str, save: Union[str, Path]):
+def get_bytes(url: str) -> bytes:
     with GetResponse(url) as resp:
-        resp.to_disk(save)
+        return resp.bytes
```

### Comparing `gameyamlspiderandgenerator-0.4.1/pyproject.toml` & `gameyamlspiderandgenerator-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "0.4.1"
+version = "1.0.0"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langcodes = "^3.3.0"
 language-data = "^1.1"
 html2text = "^2020.1.16"
 "ruamel.yaml" = "^0.17.21"
 "ruamel.yaml.string" = "^0.1.0"
 urllib3 = "^1.26.14"
-beautifulsoup4 = "^4.11.2"
+beautifulsoup4 = "^4.11.1"
 pillow = "^9.4.0"
 pygithub = "^1.57"
 requests = "^2.28.2"
 ruamel-base = "^1.0.0"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
```

### Comparing `gameyamlspiderandgenerator-0.4.1/PKG-INFO` & `gameyamlspiderandgenerator-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 0.4.1
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pygithub (>=1.57,<2.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
```

