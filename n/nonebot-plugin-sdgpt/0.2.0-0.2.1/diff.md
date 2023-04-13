# Comparing `tmp/nonebot_plugin_sdgpt-0.2.0.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.0.tar` & `nonebot_plugin_sdgpt-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.0/LICENSE
--rw-r--r--   0        0        0     6752 2023-04-13 05:20:16.403047 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     5007 2023-04-13 05:26:32.824762 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     3348 2023-04-13 03:20:37.595447 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     2983 2023-04-13 03:22:58.157097 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0      362 2023-04-13 02:43:26.492368 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1112 2023-04-13 05:37:03.631042 nonebot_plugin_sdgpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.0/README.md
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6752 2023-04-13 05:20:16.403047 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     5007 2023-04-13 05:26:32.824762 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     3440 2023-04-13 06:47:06.644004 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     3616 2023-04-13 04:20:50.670050 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     2983 2023-04-13 03:22:58.157097 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0      362 2023-04-13 02:43:26.492368 nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1160 2023-04-13 06:49:05.865430 nonebot_plugin_sdgpt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.1/README.md
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.0/LICENSE` & `nonebot_plugin_sdgpt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/config.py` & `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # -*- coding: utf-8 -*-
 import json
+import os
+
 from .lib.cons import *
 from configobj import ConfigObj
 from validate import Validator
 from .lib.check import check_ai, check_dir, check_proxy, check_api_key, check_command, check_file, check_ip, \
     ip_test_switch, check_token, check_model, check_id, check_any, check_preset
 from revChatGPT.V1 import AsyncChatbot as chatGPT
 from revChatGPT.V3 import Chatbot as chatGPT_api
 from EdgeGPT import Chatbot as Bing
 
 
+
 async def load():
+
     outData = {}
-    config = ConfigObj('config.cfg', encoding='utf-8', default_encoding='utf-8', configspec='configspec.ini',
+    path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'configspec.ini')
+    config = ConfigObj('config.cfg', encoding='utf-8', default_encoding='utf-8', configspec=path,
                        indent_type=' ', write_empty_values=True)
     validator = Validator({
         'dir': check_dir,
         'ai': check_ai,
         'cmd': check_command,
         'proxy': check_proxy,
         'file': check_file,
```

### Comparing `nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.1/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.0"
+version = "0.2.1"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
 keywords = ["nonebot", "nonebot2", "chatgpt", "new bing","Stable-Diffusion"]
 packages = [
     { include = "nonebot_plugin_SDGPT/*.py"},
+    { include = "nonebot_plugin_SDGPT/*.ini"},
     { include = "nonebot_plugin_SDGPT/lib/*.py"}
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.1"
```

### Comparing `nonebot_plugin_sdgpt-0.2.0/README.md` & `nonebot_plugin_sdgpt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.0/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.0
+Version: 0.2.1
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

