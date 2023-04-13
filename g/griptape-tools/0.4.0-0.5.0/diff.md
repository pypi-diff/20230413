# Comparing `tmp/griptape_tools-0.4.0.tar.gz` & `tmp/griptape_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.4.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.5.0.tar", max compression
```

## Comparing `griptape_tools-0.4.0.tar` & `griptape_tools-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,47 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.4.0/LICENSE
--rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.4.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.4.0/griptape/__init__.py
--rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.4.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.4.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.4.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-11 20:40:54.042137 griptape_tools-0.4.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0     1466 2023-04-11 17:42:54.149645 griptape_tools-0.4.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.4.0/griptape/tools/google_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.4.0/griptape/tools/google_search/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-11 20:40:54.044431 griptape_tools-0.4.0/griptape/tools/google_search/requirements.txt
--rw-r--r--   0        0        0     2389 2023-04-11 17:42:54.155798 griptape_tools-0.4.0/griptape/tools/google_search/tool.py
--rw-r--r--   0        0        0      525 2023-04-11 20:40:54.038520 griptape_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.0/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0      499 2023-04-13 16:44:18.759766 griptape_tools-0.5.0/griptape/tools/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-13 16:44:18.862164 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1729 2023-04-13 17:32:12.692546 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2023-04-13 17:00:19.874640 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.0/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-13 17:30:17.934482 griptape_tools-0.5.0/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.0/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-07 15:56:04.337980 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1782 2023-04-11 19:13:20.365906 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2023-04-13 16:51:04.094631 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 17:01:17.168803 griptape_tools-0.5.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-12 21:41:15.550396 griptape_tools-0.5.0/griptape/tools/email_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2195 2023-04-13 16:44:18.859633 griptape_tools-0.5.0/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.0/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 17:01:17.163490 griptape_tools-0.5.0/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     2354 2023-04-13 16:12:25.314046 griptape_tools-0.5.0/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-12 20:32:26.158552 griptape_tools-0.5.0/griptape/tools/sql_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1895 2023-04-13 16:51:04.196419 griptape_tools-0.5.0/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.0/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-13 17:01:17.166413 griptape_tools-0.5.0/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.0/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.0/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-12 16:01:57.738417 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3883 2023-04-12 22:07:30.759928 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     3994 2023-04-13 15:56:54.679897 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.0/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-13 17:01:17.164930 griptape_tools-0.5.0/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.0/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.0/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-07 15:56:04.338570 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2374 2023-04-10 14:23:53.062035 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     2423 2023-04-12 19:48:43.940734 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.0/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-13 17:01:17.161796 griptape_tools-0.5.0/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.0/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-13 17:50:25.659660 griptape_tools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.0/PKG-INFO
```

### Comparing `griptape_tools-0.4.0/LICENSE` & `griptape_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.4.0/README.md` & `griptape_tools-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
 
-Griptape Tools is a collection of Python tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core).
+This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core). You can run Griptape tools in [Skatepark](https://github.com/griptape-ai/skatepark), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
+
+- [Learn more](https://github.com/griptape-ai/griptape-core) about Griptape.
+- [Full list](https://github.com/griptape-ai/griptape-tools/tree/main/griptape/tools) of official Griptape tools.
+- [Tool details and docs](https://griptape.readthedocs.io).
 
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
 
 ## License
```

### Comparing `griptape_tools-0.4.0/griptape/tools/google_search/tool.py` & `griptape_tools-0.5.0/griptape/tools/web_search/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 from typing import Optional
-import requests
 from attr import define, field
 from schema import Schema, Literal
 from griptape.core import BaseTool, action
 
 
 @define
-class GoogleSearch(BaseTool):
-    configs = {
-        "search": {
-            "name": "search",
-            "description": "Used for searching Google.",
-            "value_schema": Schema({
-                Literal(
-                    "value",
-                    description="Google search request that returns a list of pages with titles, descriptions, and URLs"
-                ): str
-            })
-        }
-    }
-
-    results_count: int = field(default=5, kw_only=True, metadata={"env": "GOOGLE_RESULTS_COUNT"})
-    lang: str = field(default="lang_en", kw_only=True, metadata={"env": "GOOGLE_LANG"})
-    api_search_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_KEY"})
-    api_search_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_ID"})
-    api_country: str = field(default="us", kw_only=True, metadata={"env": "GOOGLE_API_COUNTRY"})
-
-    @action(config=configs["search"])
+class WebSearch(BaseTool):
+    results_count: int = field(default=5, kw_only=True, metadata={"env": "SEARCH_RESULTS_COUNT"})
+    google_api_lang: str = field(default="lang_en", kw_only=True, metadata={"env": "GOOGLE_API_LANG"})
+    google_api_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_KEY"})
+    google_api_search_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_ID"})
+    google_api_country: str = field(default="us", kw_only=True, metadata={"env": "GOOGLE_API_COUNTRY"})
+
+    @action(config={
+        "name": "search",
+        "description": "Can be used for searching the web",
+        "value_schema": Schema({
+            Literal(
+                "value",
+                description="Search engine request that returns a list of pages with titles, descriptions, and URLs"
+            ): str
+        })
+    })
     def search(self, value: bytes) -> dict:
         try:
             return {
-                "results": self._search_api(value.decode())
+                "results": self._search_google(value.decode())
             }
         except Exception as e:
             return {
                 "error": f"error searching Google: {e}"
             }
 
-    def _search_api(self, query: str) -> list[dict]:
+    def _search_google(self, query: str) -> list[dict]:
+        import requests
+
         url = f"https://www.googleapis.com/customsearch/v1?" \
-              f"key={self.env_value('GOOGLE_API_SEARCH_KEY')}&" \
+              f"key={self.env_value('GOOGLE_API_KEY')}&" \
               f"cx={self.env_value('GOOGLE_API_SEARCH_ID')}&" \
               f"q={query}&" \
               f"start=0&" \
-              f"lr={self.env_value('GOOGLE_LANG')}&" \
-              f"num={self.env_value('GOOGLE_RESULTS_COUNT')}&" \
+              f"lr={self.env_value('GOOGLE_API_LANG')}&" \
+              f"num={self.env_value('SEARCH_RESULTS_COUNT')}&" \
               f"gl={self.env_value('GOOGLE_API_COUNTRY')}"
         response = requests.get(url)
 
         if response.status_code == 200:
             data = response.json()
 
             links = [{
```

### Comparing `griptape_tools-0.4.0/pyproject.toml` & `griptape_tools-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = ">=0.4.0"
+griptape-core = ">=0.6.0"
+
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `griptape_tools-0.4.0/PKG-INFO` & `griptape_tools-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.4.0)
+Requires-Dist: griptape-core (>=0.6.0)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
 
-Griptape Tools is a collection of Python tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core).
+This repo is a collection of official Griptape tools for the [Griptape Framework](https://github.com/griptape-ai/griptape-core). You can run Griptape tools in [Skatepark](https://github.com/griptape-ai/skatepark), [LangChain](https://github.com/hwchase17/langchain), or as [ChatGPT Plugins](https://openai.com/blog/chatgpt-plugins).
+
+- [Learn more](https://github.com/griptape-ai/griptape-core) about Griptape.
+- [Full list](https://github.com/griptape-ai/griptape-tools/tree/main/griptape/tools) of official Griptape tools.
+- [Tool details and docs](https://griptape.readthedocs.io).
 
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
 
 ## License
```

