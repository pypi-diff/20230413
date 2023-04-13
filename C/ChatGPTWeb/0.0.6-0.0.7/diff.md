# Comparing `tmp/ChatGPTWeb-0.0.6.tar.gz` & `tmp/ChatGPTWeb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.0.6.tar", last modified: Thu Apr 13 13:43:33 2023, max compression
+gzip compressed data, was "ChatGPTWeb-0.0.7.tar", last modified: Thu Apr 13 13:57:48 2023, max compression
```

## Comparing `ChatGPTWeb-0.0.6.tar` & `ChatGPTWeb-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.585455 ChatGPTWeb-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.575950 ChatGPTWeb-0.0.6/ChatGPTWeb/
--rw-rw-rw-   0        0        0    19621 2023-04-13 13:41:19.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/ChatGPTWeb.py
--rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/__init__.py
--rw-rw-rw-   0        0        0     1958 2023-04-13 13:41:31.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/__main__.py
--rw-rw-rw-   0        0        0     6288 2023-04-13 13:35:36.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.583454 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/
--rw-rw-rw-   0        0        0     3516 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3516 2023-04-13 13:43:33.584456 ChatGPTWeb-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 13:43:33.585455 ChatGPTWeb-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-04-13 08:01:33.000000 ChatGPTWeb-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.296762 ChatGPTWeb-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.291762 ChatGPTWeb-0.0.7/ChatGPTWeb/
+-rw-rw-rw-   0        0        0    19656 2023-04-13 13:57:22.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/ChatGPTWeb.py
+-rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/__init__.py
+-rw-rw-rw-   0        0        0     1958 2023-04-13 13:41:31.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/__main__.py
+-rw-rw-rw-   0        0        0     6288 2023-04-13 13:35:36.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.294762 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/
+-rw-rw-rw-   0        0        0     3516 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3516 2023-04-13 13:57:48.295763 ChatGPTWeb-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:57:48.296762 ChatGPTWeb-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-04-13 13:57:32.000000 ChatGPTWeb-0.0.7/setup.py
```

### Comparing `ChatGPTWeb-0.0.6/ChatGPTWeb/ChatGPTWeb.py` & `ChatGPTWeb-0.0.7/ChatGPTWeb/ChatGPTWeb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
-from playwright.async_api import async_playwright, Route, Request
+from playwright.async_api import async_playwright, Route, Request,BrowserContext,Page
 import asyncio
 import typing
 import threading
 from .config import *
 import logging
 import re
+import random
 from pathlib import Path
 
 # import json
 # import random
 # from playwright.async_api import async_playwright, Route, Request,BrowserContext,Page
 # import asyncio
 # import typing
```

### Comparing `ChatGPTWeb-0.0.6/ChatGPTWeb/__main__.py` & `ChatGPTWeb-0.0.7/ChatGPTWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.6/ChatGPTWeb/config.py` & `ChatGPTWeb-0.0.7/ChatGPTWeb/config.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/PKG-INFO` & `ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.6
+Version: 0.0.7
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.6/LICENSE` & `ChatGPTWeb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.6/PKG-INFO` & `ChatGPTWeb-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.6
+Version: 0.0.7
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.6/README.md` & `ChatGPTWeb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.6/setup.py` & `ChatGPTWeb-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["playwright","aioconsole"] # 这里填依赖包信息
 
 setup(
     name="ChatGPTWeb",
-    version="0.0.6",
+    version="0.0.7",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="a ChatGPT API,no web ui",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/ChatGPT",
     packages=find_packages(),
```

