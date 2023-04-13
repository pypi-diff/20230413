# Comparing `tmp/nonebot_plugin_bilifan-0.0.1.tar.gz` & `tmp/nonebot_plugin_bilifan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.0.1.tar` & `nonebot_plugin_bilifan-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-04-10 21:10:25.759690 nonebot_plugin_bilifan-0.0.1/LICENSE
--rw-r--r--   0        0        0     2307 2023-04-11 16:15:09.417980 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     5494 2023-04-11 16:23:06.641492 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     5686 2023-04-11 16:14:59.683601 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       52 2023-04-10 20:50:48.000000 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17524 2023-04-11 15:27:39.724923 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    17084 2023-04-11 15:27:24.891916 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2219 2023-04-11 15:48:05.006283 nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     1101 2023-04-11 16:29:48.452224 nonebot_plugin_bilifan-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2459 2023-04-11 16:19:43.702899 nonebot_plugin_bilifan-0.0.1/README.md
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.1/setup.py
--rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2457 2023-04-13 14:32:34.095783 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     5453 2023-04-13 14:32:34.586527 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2219 2023-04-13 11:46:28.245642 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     1098 2023-04-13 14:35:43.118435 nonebot_plugin_bilifan-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2029 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.0.2/README.md
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.2/setup.py
+-rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.0.1/LICENSE` & `nonebot_plugin_bilifan-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from nonebot.log import logger
 from pathlib import Path
+import shutil
 from .main import *
 from .src import BiliUser
 
 from .login import get_tv_qrcode_url_and_auth_code,draw_QR,verify_login
 
-
+from nonebot.log import logger
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageSegment,MessageEvent
 from nonebot.plugin import PluginMetadata
 
 
 __version__ = "0.0.1"
 __plugin_meta__ = PluginMetadata(
@@ -24,15 +24,18 @@
 
 
 
 login_in = on_command('blogin',aliases={'b站登录'},block=False)
 
 @login_in.handle()
 async def _(event:MessageEvent):
-    login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
+    try:
+        login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
+    except aiohttp.client_exceptions.ClientTimeoutError:
+        await login_in.finish("已超时，请稍后重试！")
     data_path = Path().joinpath(f'data/bilifan/{event.user_id}')
     data_path.mkdir(parents=True, exist_ok=True)
     data = await draw_QR(login_url)
     try:
         await login_in.send(MessageSegment.image(data))
     except:
         logger.warning('二维码可能被风控，发送链接')
```

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/login/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,106 @@
 import hashlib
 import urllib.parse as urlparse
 import time
 import os
 import shutil
-import requests
-import json
 import yaml
-from http import cookiejar
-import requests
+import aiohttp , asyncio
 import time
 import hashlib
 import urllib.parse as urlparse
 from io import BytesIO
 from pathlib import Path
 # import qrcode_terminal
 import qrcode
 from nonebot.log import logger
 
-Cookies = cookiejar.CookieJar()
-session = requests.Session()
-session.cookies = Cookies
+# Cookies = cookiejar.CookieJar()
+# session = requests.Session()
+# session.cookies = Cookies
 
 csrf = ""
 access_key = ""
 base_path = Path().joinpath('data/bilifan')
 
-# async def is_login():
-    # global cookies
-    # api = "https://api.bilibili.com/x/web-interface/nav"
-    # req = urllib.request.Request(api)
-    # for c in cookies:
-        # req.add_header("Cookie", f"{c['name']}={c['value']}")
-    # with urllib.request.urlopen(req) as response:
-        # body = response.read().decode()
-        # data = json.loads(body)
-        # return data["code"] == 0, data["data"]["uname"]
 
 
 
-
-async def map_to_string(data):
-    string = ""
-    keys = sorted(data.keys())
-    for key in keys:
-        string += f"{key}={data[key]}&"
-    return string[:-1]
-
-
-
-async def is_login():
+async def is_login(session, cookies):
     api = 'https://api.bilibili.com/x/web-interface/nav'
     headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
-    session = requests.Session()
-    for c in Cookies:
-        session.cookies.set(c['name'], c['value'])
-    resp = session.get(api, headers=headers)
-    data = resp.json()
-    return data['code'] == 0, data['data']['uname']
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
+    }
+    async with session.get(api, headers=headers, cookies=cookies) as resp:
+        data = await resp.json()
+        return data['code'] == 0, data['data']['uname']
+
+
 
 async def get_tv_qrcode_url_and_auth_code():
     api = 'http://passport.bilibili.com/x/passport-tv-login/qrcode/auth_code'
     data = {
         "local_id": "0",
         "ts": str(int(time.time())),
     }
     await signature(data)
-    resp = requests.post(api, data= await map_to_string(data), headers={"Content-Type": "application/x-www-form-urlencoded"})
-    resp_data = resp.json()
-    code = resp_data['code']
-    if code == 0:
-        qrcode_url = resp_data['data']['url']
-        auth_code = resp_data['data']['auth_code']
-        return qrcode_url, auth_code
-    else:
-        raise Exception('get_tv_qrcode_url_and_auth_code error')
-
-
-# async def map_to_string(params):
-    # query = ""
-    # for k, v in params.items():
-        # query += k + "=" + v + "&"
-    # return query[:-1]
+    async with aiohttp.ClientSession() as session:
+        async with session.post(api, data=await map_to_string(data), headers={"Content-Type": "application/x-www-form-urlencoded"}) as resp:
+            resp_data = await resp.json()
+            code = resp_data['code']
+            if code == 0:
+                qrcode_url = resp_data['data']['url']
+                auth_code = resp_data['data']['auth_code']
+                return qrcode_url, auth_code
+            else:
+                raise Exception('get_tv_qrcode_url_and_auth_code error')
+
+
+
 
 async def verify_login(auth_code,data_path):
     api = "http://passport.bilibili.com/x/passport-tv-login/qrcode/poll"
     data = {
         "auth_code": auth_code,
         "local_id": "0",
         "ts": str(int(time.time())),
     }
     await signature(data)
     data_string = await map_to_string(data)
     headers = {
         "Content-Type": "application/x-www-form-urlencoded",
     }
     while True:
-        resp = requests.post(api, headers=headers, data=data_string)
-        if resp.status_code != 200:
-            raise Exception("Failed to connect to server")
-        response_dict = json.loads(resp.text)
-        code = response_dict["code"]
-        try:
-            access_key = response_dict["data"]["access_token"]
-        except:
-            time.sleep(3)
+        async with aiohttp.ClientSession() as session:
+            async with session.post(api, headers=headers, data=data_string) as resp:
+                if resp.status != 200:
+                    raise Exception("Failed to connect to server")
+                response_dict = await resp.json()
+                code = response_dict["code"]
+                try:
+                    access_key = response_dict["data"]["access_token"]
+                except:
+                    await asyncio.sleep(3)
             
-        if code == 0:
-            logger.success("登录成功")
-            with open(data_path/"login_info.txt", "w") as f:
-                f.write(access_key)
-            if not os.path.exists(data_path/'users.yaml'):
-                logger.info('初始化配置文件')
-                shutil.copy2(Path().joinpath('data/bilifan/users.yaml'), data_path/'users.yaml')
-            with open('data_path/users.yaml', 'r', encoding='utf-8') as f:
-                config = yaml.safe_load(f)
-            config['USERS'][0]['access_key'] = access_key
-            with open('data_path/users.yaml', 'w', encoding='utf-8') as f:
-                yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
-            return "access_key已保存"
-        else:
-            time.sleep(3)
+            if code == 0:
+                logger.success("登录成功")
+                with open(data_path/"login_info.txt", "w") as f:
+                    f.write(access_key)
+                if not os.path.exists(data_path/'users.yaml'):
+                    logger.info('初始化配置文件')
+                    shutil.copy2(Path().joinpath('data/bilifan/users.yaml'), data_path/'users.yaml')
+                with open(data_path/'users.yaml', 'r', encoding='utf-8') as f:
+                    config = yaml.safe_load(f)
+                config['USERS'][0]['access_key'] = access_key
+                with open(data_path/'users.yaml', 'w', encoding='utf-8') as f:
+                    yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
+                return "access_key已保存"
+            else:
+                time.sleep(3)
+
 
 appkey = "4409e2ce8ffd12b8"
 appsec = "59b43e04ad6965f34319062b478f83dd"
 
 async def signature(params: dict):
     keys = list(params.keys())
     params["appkey"] = appkey
```

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import json
 import os
-import shutil
-import sys
-import time
 from nonebot.log import logger as log
 import warnings
 import asyncio
 import aiohttp
 import itertools
 from pathlib import Path
 from .src import BiliUser
@@ -55,74 +52,71 @@
         exit(1)
 
 
 @log.catch
 async def main(msg_path):
     await read_yaml(msg_path)
     messageList = []
-    session = aiohttp.ClientSession()
-    try:
-        log.warning("当前版本为: " + __VERSION__)
-        resp = await (
-            await session.get(
+    async with aiohttp.ClientSession() as session:
+        try:
+            log.warning("当前版本为: " + __VERSION__)
+            resp = await session.get(
                 "http://version.fansmedalhelper.1961584514352337.cn-hangzhou.fc.devsapp.net/"
             )
-        ).json()
-        if resp['version'] != __VERSION__:
-            log.warning("新版本为: " + resp['version'] + ",请更新")
-            log.warning("更新内容: " + resp['changelog'])
-            messageList.append(f"当前版本: {__VERSION__} ,最新版本: {resp['version']}")
-            messageList.append(f"更新内容: {resp['changelog']} ")
-        if resp['notice']:
-            log.warning("公告: " + resp['notice'])
-            messageList.append(f"公告: {resp['notice']}")
-    except Exception as ex:
-        messageList.append(f"检查版本失败，{ex}")
-        log.warning(f"检查版本失败，{ex}")
-    initTasks = []
-    startTasks = []
-    catchMsg = []
+            data = await resp.json()
+            if data['version'] != __VERSION__:
+                log.warning("新版本为: " + data['version'] + ",请更新")
+                log.warning("更新内容: " + data['changelog'])
+                messageList.append(f"当前版本: {__VERSION__} ,最新版本: {data['version']}")
+                messageList.append(f"更新内容: {data['changelog']} ")
+            if data['notice']:
+                log.warning("公告: " + data['notice'])
+                messageList.append(f"公告: {data['notice']}")
+        except Exception as ex:
+            messageList.append(f"检查版本失败，{ex}")
+            log.warning(f"检查版本失败，{ex}")
+    init_tasks = []
+    start_tasks = []
+    catch_msg = []
+
     for user in users['USERS']:
         if user['access_key']:
-            biliUser = BiliUser(
-                user['access_key'],
-                user.get('white_uid', ''),
-                user.get('banned_uid', ''),
-                config,
-            )
-            initTasks.append(biliUser.init())
-            startTasks.append(biliUser.start())
-            catchMsg.append(biliUser.sendmsg())
+            bili_user = BiliUser(user['access_key'], user.get('white_uid', ''), user.get('banned_uid', ''), config)
+            init_tasks.append(bili_user.init())
+            start_tasks.append(bili_user.start())
+            catch_msg.append(bili_user.sendmsg())
+
     try:
-        await asyncio.gather(*initTasks)
-        await asyncio.gather(*startTasks)
+        await asyncio.gather(*init_tasks)
+        await asyncio.gather(*start_tasks)
     except Exception as e:
         log.exception(e)
-        # messageList = messageList + list(itertools.chain.from_iterable(await asyncio.gather(*catchMsg)))
-        messageList.append(f"任务执行失败: {e}")
-    finally:
-        messageList = messageList + list(
-            itertools.chain.from_iterable(await asyncio.gather(*catchMsg))
-        )
-    [log.info(message) for message in messageList]
-    return messageList
+        message_list = [f"任务执行失败: {e}"]
+    else:
+        message_list = []
+
+    try:
+        catch_msg_results = await asyncio.gather(*catch_msg)
+    except Exception as e:
+        log.exception(e)
+        message_list.append(f"发送消息失败: {e}")
+    else:
+        message_list += list(itertools.chain.from_iterable(catch_msg_results))
+
+    [log.info(message) for message in message_list]
+    return message_list
+
 
 
 def run(*args, **kwargs):
     loop = asyncio.new_event_loop()
     loop.run_until_complete(main())
     log.info("任务结束，等待下一次执行。")
 
 
-async def push_message(session, sendkey, message):
-    url = f"https://sctapi.ftqq.com/{sendkey}.send"
-    data = {"title": f"【B站粉丝牌助手推送】", "desp": message}
-    await session.post(url, data=data)
-    log.info("Server酱已推送")
-
         
 # if __name__ == '__main__':
     # cron = users.get('CRON', None)
 
     # if cron:
     #     from apscheduler.schedulers.blocking import BlockingScheduler
     #     from apscheduler.triggers.cron import CronTrigger
```

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import asyncio
 from hashlib import md5
 import hashlib
-import os
 import random
-import sys
 import time
 import json
 from typing import Union
 from nonebot.log import logger
-from nonebot.log import logger as log
 from urllib.parse import urlencode, urlparse
 
 
 from aiohttp import ClientSession
 
 # sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
```

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from aiohttp import ClientSession, ClientTimeout
-import sys
-import os
 import asyncio
 import uuid
 from loguru import logger
 from nonebot.log import logger as log
 from datetime import datetime, timedelta
 
 # sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
```

### Comparing `nonebot_plugin_bilifan-0.0.1/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.1/pyproject.toml` & `nonebot_plugin_bilifan-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.0.1"
+version = "0.0.2"
 description = "刷bili粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["bilibili", "nonebot2", "plugin"]
@@ -26,12 +26,12 @@
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_apscheduler = "^0.2.0"
 
 pillow = "^9.3.0"
 aiohttp = "^3.8.3"
 aiohttp-socks = "^0.8.0"
 pyyaml = "^6.0"
-requests = "^2.28.2"
+qrcode = "^7.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_bilifan-0.0.1/README.md` & `nonebot_plugin_bilifan-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,15 @@
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_bilifan
 _✨自动b站粉丝牌✨_
-<div align = "center">
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
-</div><br>
+
 <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-             # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_
-                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
-
-   [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
+  # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
+               issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
 å¼å§æ§è¡å½ä»¤  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
```

### Comparing `nonebot_plugin_bilifan-0.0.1/setup.py` & `nonebot_plugin_bilifan-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 ['aiohttp-socks>=0.8.0,<0.9.0',
  'aiohttp>=3.8.3,<4.0.0',
  'nonebot-adapter-onebot>=2.1.5',
  'nonebot2>=2.0.0rc4,<3.0.0',
  'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
  'pillow>=9.3.0,<10.0.0',
  'pyyaml>=6.0,<7.0',
- 'requests>=2.28.2,<3.0.0']
+ 'qrcode>=7.4.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-bilifan',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '刷bili粉丝牌子的机器人插件',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n<div align = "center">\n        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_bilifan', 'nonebot_plugin_bilifan.login',
 'nonebot_plugin_bilifan.src'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp-socks>=0.8.0,<0.9.0', 'aiohttp>=3.8.3,<4.0.0', 'nonebot-adapter-
 onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0', 'pillow>=9.3.0,<10.0.0',
-'pyyaml>=6.0,<7.0', 'requests>=2.28.2,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-bilifan', 'version': '0.0.1', 'description':
+'pyyaml>=6.0,<7.0', 'qrcode>=7.4.2,<8.0.0'] setup_kwargs = { 'name': 'nonebot-
+plugin-bilifan', 'version': '0.0.2', 'description':
 'å·biliç²ä¸çå­çæºå¨äººæä»¶', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
-          \n\n# nonebot_plugin_bilifan\n_â¨èªå¨bç«ç²ä¸çâ¨_\n
-            \n ææ¡£   Â·  \n æä»¤åè¡¨   Â·  \n å¸¸è§é®é¢\n
-
-    \n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_
-                       [pypi]\n\n [python]\n [NoneBot]\n
+    \n\n# nonebot_plugin_bilifan\n_â¨èªå¨bç«ç²ä¸çâ¨_\n\n\n_[GitHub
+stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_[pypi]\n\n [python]\n
+                                  [NoneBot]\n
 \n\n\n## éç½®\n\nå¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶\n\n## æä»¤\n\n -
 bç«ç»å½ - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå·\n -
 å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤\n\n\n\n## ð å¶ä»\n\n+
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr\n+ å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [GPL-3.0 License]
```

### Comparing `nonebot_plugin_bilifan-0.0.1/PKG-INFO` & `nonebot_plugin_bilifan-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.0.1
+Version: 0.0.2
 Summary: 刷bili粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -22,33 +22,29 @@
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_bilifan
 _✨自动b站粉丝牌✨_
-<div align = "center">
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
-</div><br>
+
 <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
```

#### html2text {}

```diff
@@ -1,31 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.0.2 Summary:
 å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: nonebot-adapter-
 onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
 nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow
-(>=9.3.0,<10.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
-(>=2.28.2,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
+(>=9.3.0,<10.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode
+(>=7.4.2,<8.0.0) Project-URL: Repository, https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-             # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_
-                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
-
-   [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
+  # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
+               issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
 å¼å§æ§è¡å½ä»¤  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
```

