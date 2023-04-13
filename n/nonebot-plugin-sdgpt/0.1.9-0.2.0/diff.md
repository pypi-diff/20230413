# Comparing `tmp/nonebot_plugin_sdgpt-0.1.9.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.1.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.1.9.tar` & `nonebot_plugin_sdgpt-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.9/LICENSE
--rw-r--r--   0        0        0     3468 2023-04-11 09:43:15.736752 nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     9983 2023-04-11 05:21:10.304226 nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     1004 2023-04-11 09:44:51.579889 nonebot_plugin_sdgpt-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.9/README.md
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6752 2023-04-13 05:20:16.403047 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     5007 2023-04-13 05:26:32.824762 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     3348 2023-04-13 03:20:37.595447 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     2983 2023-04-13 03:22:58.157097 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0      362 2023-04-13 02:43:26.492368 nonebot_plugin_sdgpt-0.2.0/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1112 2023-04-13 05:37:03.631042 nonebot_plugin_sdgpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.0/README.md
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.1.9/LICENSE` & `nonebot_plugin_sdgpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.9/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.1.9"
+version = "0.2.0"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
 keywords = ["nonebot", "nonebot2", "chatgpt", "new bing","Stable-Diffusion"]
 packages = [
-    { include = "nonebot_plugin_SDGPT/*.py"}
+    { include = "nonebot_plugin_SDGPT/*.py"},
+    { include = "nonebot_plugin_SDGPT/lib/*.py"}
 ]
 
 [tool.poetry.dependencies]
+
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.1"
 python-dotenv = "*"
 revChatGPT = "*"
 EdgeGPT = "*"
 webuiapi = "*"
 nonebot-plugin-guild-patch ="*"
 nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
+websockets = "^10.0"
+aiofiles = "*"
+configobj = "*"
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_sdgpt-0.1.9/README.md` & `nonebot_plugin_sdgpt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.9/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.1.9
+Version: 0.2.0
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,19 +12,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot
 Requires-Dist: EdgeGPT
+Requires-Dist: aiofiles
+Requires-Dist: configobj
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-plugin-guild-patch
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: python-dotenv
 Requires-Dist: revChatGPT
+Requires-Dist: websockets (>=10.0,<11.0)
 Requires-Dist: webuiapi
 Project-URL: Documentation, https://github.com/thx114/SDGPTreadme
 Project-URL: Repository, https://github.com/thx114/SDGPT
 Description-Content-Type: text/markdown
 
 # SDGPT 
 基于 **[NoneBot2](https://v2.nonebot.dev/)**
```

