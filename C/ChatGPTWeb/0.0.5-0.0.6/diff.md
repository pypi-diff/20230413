# Comparing `tmp/ChatGPTWeb-0.0.5.tar.gz` & `tmp/ChatGPTWeb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.0.5.tar", last modified: Sun Apr  9 14:17:40 2023, max compression
+gzip compressed data, was "ChatGPTWeb-0.0.6.tar", last modified: Thu Apr 13 13:43:33 2023, max compression
```

## Comparing `ChatGPTWeb-0.0.5.tar` & `ChatGPTWeb-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.253449 ChatGPTWeb-0.0.5/ChatGPTWeb/
--rw-rw-rw-   0        0        0    15098 2023-04-09 14:04:38.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/ChatGPTWeb.py
--rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/__init__.py
--rw-rw-rw-   0        0        0     1551 2023-04-08 10:18:52.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/__main__.py
--rw-rw-rw-   0        0        0     6195 2023-04-09 14:04:00.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.258397 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/
--rw-rw-rw-   0        0        0     3466 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3466 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-04-09 14:17:16.000000 ChatGPTWeb-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-04-09 14:16:59.000000 ChatGPTWeb-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.585455 ChatGPTWeb-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.575950 ChatGPTWeb-0.0.6/ChatGPTWeb/
+-rw-rw-rw-   0        0        0    19621 2023-04-13 13:41:19.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/ChatGPTWeb.py
+-rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/__init__.py
+-rw-rw-rw-   0        0        0     1958 2023-04-13 13:41:31.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/__main__.py
+-rw-rw-rw-   0        0        0     6288 2023-04-13 13:35:36.000000 ChatGPTWeb-0.0.6/ChatGPTWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:43:33.583454 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/
+-rw-rw-rw-   0        0        0     3516 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 13:43:33.000000 ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3516 2023-04-13 13:43:33.584456 ChatGPTWeb-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:43:33.585455 ChatGPTWeb-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-04-13 08:01:33.000000 ChatGPTWeb-0.0.6/setup.py
```

### Comparing `ChatGPTWeb-0.0.5/ChatGPTWeb/ChatGPTWeb.py` & `ChatGPTWeb-0.0.6/ChatGPTWeb/ChatGPTWeb.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,32 +4,42 @@
 import typing
 import threading
 from .config import *
 import logging
 import re
 from pathlib import Path
 
+# import json
+# import random
+# from playwright.async_api import async_playwright, Route, Request,BrowserContext,Page
+# import asyncio
+# import typing
+# import threading
+# from config import *
+# import logging
+# import re
+# from pathlib import Path
+
 class chatgpt():
     def __init__(self,
                  proxy: typing.Optional[ProxySettings] = None,
-                 session_token: str = "",
+                 session_token: list = [],
                  chat_file: Path = Path()/"data"/"chat_history"/"conversation",
                  personality: Optional[Personality] = Personality([{"name":"cat","value":"you are a cat now."}]),
                  log_status: bool = True,
                  plugin: bool = False) -> None:
         '''
         proxy : your proxy for openai | 你用于访问openai的代理
         session_token : your session_token | 你的session_token
         chat_file : save the chat history file path | 保存聊天文件的路径，默认 data/chat_history/..  
         personality : init personality | 初始化人格 [{"name":"人格名","value":"预设内容"},{"name":"personality name","value":"personality value"},....]
         log_status : start log? | 开启日志输出吗
         plugin : is a Nonebot bot? | 作为Nonebot 插件实现
         '''
         self.data = MsgData()
-        self.status = False
         self.join = False
         self.proxy = proxy
         self.chat_file = chat_file
         self.personality = personality
         self.log_status = log_status
         self.plugin = plugin
         self.set_chat_file()
@@ -41,253 +51,335 @@
         if not self.log_status:
             self.logger.removeHandler(sh)
             
         if session_token:
             self.cookie: typing.List[SetCookieParam] = [{
                 "url": "https://chat.openai.com",
                 "name": "__Secure-next-auth.session-token",
-                "value": session_token
-            }]
+                "value": x
+            } for x in session_token]
         else:
             raise ValueError("session_token is empty!")
+        
+        self.manage = {
+            "start":False,
+            "browser_contexts":[],
+            "access_token":[],
+            "status":{}
+        }
+        
+        '''start:bool 全部启动完毕
+        
+        browser_contexts：list 浏览器环境列表
+        
+        access_token：list token列表
+        
+        status：dict name:bool 对应环境是否加载成功
         '''
-        data : base data type | 内部数据类型
-        status : is init ok? | 等待初始化完成
-        join : queue lock | 队列锁
-        cookie : chatgpt cookie
-        '''
+        
+        
         
         if not self.plugin:
             self.browser_event_loop = asyncio.get_event_loop()
             asyncio.run_coroutine_threadsafe(self.__start__(self.browser_event_loop),self.browser_event_loop)
+            
+        '''
+        data : base data type | 内部数据类型
+        join : queue lock | 队列锁
+        cookie : chatgpt cookie
+        '''
 
     
     def set_chat_file(self):
         '''mkdir chat file path 
         创建聊天文件目录'''
         self.chat_file.mkdir(parents=True,exist_ok=True)  
+        self.cc_map = self.chat_file/"map.json"
+        self.cc_map.touch()
+        if not self.cc_map.stat().st_size:
+            self.cc_map.write_text("{}")
+            
 
     async def __alive__(self):
         '''keep cf cookie alive
         保持cf cookie存活
         '''
         while 1:
-            try:
-                async with self.page.expect_response(url_session,timeout=20000) as a:
-                    res = await self.page.goto(url_session, timeout=20000)
-                res = await a.value
-                if res.status == 403 and res.url == url_session:
-                    async with self.page.expect_response(url_session,timeout=20000) as b:
-                        resb = await b.value
-                        if resb.status == 200 and resb.url == url_session:
-                            self.logger.info("flush cf cookie OK!")
-                            await self.page.wait_for_timeout(1000)
-                            #break
-                        else:
-                            self.logger.error("flush cf cookie error!")
-                elif res.status == 200 and res.url == url_session:
-                    self.logger.info("flush cf cookie OK!")
-                    await self.page.wait_for_timeout(1000)
-                else:
-                    self.logger.error("flush cf cookie error!")
-            except:
-                self.logger.error("flush cf cookie error!")
-            await self.page.wait_for_timeout(60000)
+            #browser_context:BrowserContext
+            for context_index,browser_context in enumerate(self.manage["browser_contexts"]):
+                try:
+                    page:Page = browser_context.pages[0]
+                    async with page.expect_response(url_session,timeout=20000) as a:
+                        res = await page.goto(url_session, timeout=20000)
+                    res = await a.value
+                    if res.status == 403 and res.url == url_session:
+                        async with page.expect_response(url_session,timeout=20000) as b:
+                            resb = await b.value
+                            if resb.status == 200 and resb.url == url_session:
+                                self.logger.info(f"flush {context_index} cf cookie OK!")
+                                await page.wait_for_timeout(1000)
+                                #break
+                            else:
+                                self.logger.error(f"flush {context_index} cf cookie error!")
+                    elif res.status == 200 and res.url == url_session:
+                        self.logger.info(f"flush {context_index} cf cookie OK!")
+                        await page.wait_for_timeout(1000)
+                    else:
+                        self.logger.error(f"flush {context_index} cf cookie error!")
+                    
+                    await page.wait_for_timeout(20000)
+                except:
+                    self.logger.error(f"flush {context_index} cf cookie error!")
                 
     async def __start__(self,loop):
         '''init 
         初始化'''
         self.ap = await async_playwright().start()
         self.browser = await self.ap.firefox.launch(
             #headless=False,
             slow_mo=50,proxy=self.proxy)
-        self.context = await self.browser.new_context(service_workers="block")
-        await self.context.add_cookies(self.cookie)
-        self.page = await self.context.new_page()
-        while 1:
-            async with self.page.expect_response(url_session,timeout=20000) as a:
-                
-                res = await self.page.goto(url_session, timeout=20000)
-                res = await a.value
-                if res.status == 403 and res.url == url_session:
-                    async with self.page.expect_response(url_session,timeout=20000) as b:
-                        resb = await b.value
-                        if resb.status == 200 and resb.url == url_session:
-                            await self.page.wait_for_timeout(1000)
+        for x in self.cookie:
+            self.context = await self.browser.new_context(service_workers="block")
+            await self.context.add_cookies([x])
+        for context_index,browser_context in enumerate(self.browser.contexts):
+            page = await browser_context.new_page()
+            while 1:
+                try:
+                    async with page.expect_response(url_session,timeout=30000) as a:
+                        
+                        res = await page.goto(url_session, timeout=30000)
+                        res = await a.value
+                        if res.status == 403 and res.url == url_session:
+                            async with page.expect_response(url_session,timeout=30000) as b:
+                                resb = await b.value
+                                if resb.status == 200 and resb.url == url_session:
+                                    await page.wait_for_timeout(1000)
+                                    break
+                        elif res.status == 200 and res.url == url_session:
+                            await page.wait_for_timeout(1000)
                             break
-                elif res.status == 200 and res.url == url_session:
-                    await self.page.wait_for_timeout(1000)
-                    break
-            
-            await self.page.wait_for_timeout(20000)
-
-        try:
-            json_data = await self.page.evaluate(
-                '() => JSON.parse(document.querySelector("body").innerText)')
-            access_token = json_data['accessToken']
-        except:
-            access_token = None
+                except:
+                    self.logger.debug(f"{context_index}' session_token login error!")
 
-        if access_token:
-            self.access_token = access_token
-            self.status = True
-            self.join = True
-            
+            try:
+                json_data = await page.evaluate(
+                    '() => JSON.parse(document.querySelector("body").innerText)')
+                access_token = json_data['accessToken']
+            except:
+                access_token = None
+                
+            self.manage["access_token"].append(access_token)
+            if access_token:
+                self.manage["status"][str(context_index)] = True
+            else:
+                self.manage["status"][str(context_index)] = False
+        self.manage["browser_contexts"] = self.browser.contexts    
+        
         if self.plugin:
             from nonebot.log import logger
             self.logger = logger
         self.personality.read_data()
+        self.manage["start"] = True
+        self.logger.info("start!")
         threading.Thread(target=self.tmp(loop)).start()
             
     def tmp(self,loop):
         asyncio.run_coroutine_threadsafe(self.__alive__(),loop)
 
                 
     def markdown_to_text(self,markdown_string):
         # Remove backslashes from markdown string
         markdown_string = re.sub(r'\\(.)', r'\1', markdown_string)
         # Remove markdown formatting
         markdown_string = re.sub(r'([*_~`])', '', markdown_string)
         return markdown_string      
       
-    async def send_msg(self,msg_data: MsgData):
+    async def send_msg(self,msg_data: MsgData,page:Page,token:str,context_num:int):
         '''send message body function
         发送消息处理函数'''
-        while not self.status:
-            await asyncio.sleep(0.5)
         
         if not msg_data.conversation_id and not msg_data.p_msg_id:
             msg_data.post_data = Payload.new_payload(msg_data.msg_send)
+            #msg_data.post_data = Payload.system_new_payload(msg_data.msg_send)
         else:
             msg_data.post_data = Payload.old_payload(msg_data.msg_send,msg_data.conversation_id,msg_data.p_msg_id)
             
-        self.header = Payload.headers(self.access_token,msg_data.post_data)
+        header = Payload.headers(token,msg_data.post_data)
         
         async def route_handle(route: Route, request: Request):
-            if "cookie" in request.headers:
-                self.header["Cookie"] = request.headers["cookie"]
-            if "user-agent" in request.headers:
-                self.header["User-Agent"] = request.headers["user-agent"]
-            await route.continue_(method="POST",headers=self.header,post_data=msg_data.post_data)
+            header["Cookie"] = request.headers["cookie"]
+            header["User-Agent"] = request.headers["user-agent"]
+            await route.continue_(method="POST",headers=header,post_data=msg_data.post_data)
             
-        await self.page.route("**/backend-api/conversation",route_handle) # type: ignore
+        await page.route("**/backend-api/conversation",route_handle) # type: ignore
         try:
-            async with self.page.expect_response("https://chat.openai.com/backend-api/conversation",timeout=600000) as response_info:
+            async with page.expect_response("https://chat.openai.com/backend-api/conversation",timeout=30000) as response_info:
                 try:
                     self.logger.debug(f"send:{msg_data.msg_send}")
-                    await self.page.goto(url_chatgpt,timeout=600000)
+                    await page.goto(url_chatgpt,timeout=30000)
                 except:
                     pass
             resp = await response_info.value
-            stream_text = await resp.text()
-            stream_lines = stream_text.splitlines()
-            for x in stream_lines:
+            if resp.status == 200:
+                stream_text = await resp.text()
+                stream_lines = stream_text.splitlines()
                 for x in stream_lines:
-                    if "finish_details" in x:
-                        msg = json.loads(x[6:])
-                        msg_data.msg_recv = self.markdown_to_text(msg["message"]["content"]["parts"][0]) 
-                        msg_data.conversation_id = msg["conversation_id"]
-                        msg_data.next_msg_id = msg["message"]["id"]
-                        msg_data.status = True
-                        msg_data.msg_type = "old_session"
-            if stream_lines:
-                self.logger.debug(f"recive:{msg_data.msg_recv}")
-                await self.save_chat(msg_data)
+                    for x in stream_lines:
+                        if "finish_details" in x:
+                            msg = json.loads(x[6:])
+                            msg_data.msg_recv = self.markdown_to_text(msg["message"]["content"]["parts"][0]) 
+                            msg_data.conversation_id = msg["conversation_id"]
+                            msg_data.next_msg_id = msg["message"]["id"]
+                            msg_data.status = True
+                            msg_data.msg_type = "old_session"
+                if stream_lines:
+                    self.logger.debug(f"recive:{msg_data.msg_recv}")
+                    await self.save_chat(msg_data,context_num)
+                else:
+                    msg_data.msg_recv = str(resp.status)
+            elif resp.status == 429:
+                msg_data.msg_recv = "猪咪...被玩坏了..等一个小时后再聊吧..."
             else:
-                msg_data.msg_recv = str(resp.status)
+                msg_data.msg_recv = str(resp.status) + resp.status_text
             return msg_data
         except:
             msg_data.msg_recv = "error"
             self.join = True
             return msg_data
         
 
-    async def save_chat(self,msg_data: MsgData):
+    async def save_chat(self,msg_data: MsgData,context_num:int):
         '''save chat file
         保存聊天文件'''
         path = self.chat_file/msg_data.conversation_id
         path.touch()
         if not path.stat().st_size:
-            with open(path,"w") as f:
-                tmp = {
+            tmp = {
                     "conversation_id":msg_data.conversation_id,
                     "message":[{
                         "input":msg_data.msg_send,
                         "output":msg_data.msg_recv,
                         "type":msg_data.msg_type,
                         "next_msg_id":msg_data.next_msg_id
                     }]
                 }
-                f.write(json.dumps(tmp)) 
+            path.write_text(json.dumps(tmp))
         else:
-            with open(path,"r") as f:
-                tmp = json.loads(f.read())
-            with open(path,"w") as f:
-                tmp["message"].append({
+            tmp = json.loads(path.read_text("utf8"))
+            tmp["message"].append({
                     "input":msg_data.msg_send,
                     "output":msg_data.msg_recv,
                     "type":msg_data.msg_type,
                     "next_msg_id":msg_data.next_msg_id
                 })
-                f.write(json.dumps(tmp))
+            path.write_text(json.dumps(tmp))
+        
+        map_tmp = json.loads(self.cc_map.read_text("utf8"))
+        if str(context_num) in map_tmp:
+            if msg_data.conversation_id not in map_tmp[str(context_num)]:
+                map_tmp[str(context_num)].append(msg_data.conversation_id)
+                self.cc_map.write_text(json.dumps(map_tmp))
+        else:
+            map_tmp[str(context_num)] = []
+            map_tmp[str(context_num)].append(msg_data.conversation_id)
+            self.cc_map.write_text(json.dumps(map_tmp))
+        
                 
             
     async def load_chat(self,msg_data: MsgData):
         '''load chat file
         读取聊天文件'''
         path = self.chat_file/msg_data.conversation_id
         path.touch()
         if not path.stat().st_size:
             #self.logger.warning(f"不存在{msg_data.conversation_id}历史记录文件")
             return {
                 "conversation_id":msg_data.conversation_id,
                 "message":[]
                 }
         else:
-            with open(path,"r") as f:
-                tmp = json.loads(f.read())
-                return tmp
+            return json.loads(path.read_text("utf8"))
     
     async def continue_chat(self,msg_data: MsgData) -> MsgData:
         '''Message processing entry, please use this
         聊天处理入口，一般用这个'''
-        
-        while not self.join:
-            await asyncio.sleep(0.3)
-        self.join = False
-        if msg_data.msg_type == "old_session":
-            msg_data.p_msg_id = msg_data.next_msg_id
-        if not msg_data.conversation_id:
-            # 未输入会话id，尝试开启新会话
-            pass
+        while not self.manage["start"]:
+            await asyncio.sleep(0.5)
+
+        context_num:int = 0
+        if msg_data.conversation_id:
+            map_tmp = json.loads(self.cc_map.read_text("utf8"))
+            for context_name in map_tmp:
+                # 遍历环境的cid
+                if msg_data.conversation_id in map_tmp[context_name]:
+                    #如果cid在这个环境里
+                    while not self.manage["status"][context_name]:
+                        #检查这个环境有没有准备好
+                        await asyncio.sleep(0.5)
+                    self.manage["status"][context_name] = False
+                    page = self.manage["browser_contexts"][int(context_name)].pages[0]
+                    token = self.manage["access_token"][int(context_name)]
+                    context_num = int(context_name)
+                    break
+        else:
+            keys = list(self.manage["status"].keys())
+            random.shuffle(keys)
+            self.manage["status"] = {key: self.manage["status"][key] for key in keys}
+            # 每次打乱顺序，以避免持续访问第一个
+            status = False
+            # 是否找到可用环境
+            while True:
+                for context_name in self.manage["status"]:
+                    # context_name 环境名
+                    if self.manage["status"][context_name]:
+                        # 如果该环境好了
+                        self.manage["status"][context_name] = False
+                        page = self.manage["browser_contexts"][int(context_name)].pages[0]
+                        token = self.manage["access_token"][int(context_name)]
+                        context_num = int(context_name)
+                        status = True
+                        break
+                if status:
+                    break
+                await asyncio.sleep(0.5)
+                    
+        # while not self.join:
+        #     await asyncio.sleep(0.3)
+        # self.join = False
+        # if msg_data.msg_type == "old_session":
+        #     msg_data.p_msg_id = msg_data.next_msg_id
+        # if not msg_data.conversation_id:
+        #     # 未输入会话id，尝试开启新会话
+        #     pass
         
         if msg_data.p_msg_id:
             # 存在输入的p_msg_id
             pass
         else:
             # 未输入，尝试从文件里恢复
             try:
                 msg_history = await self.load_chat(msg_data)
                 msg_data.p_msg_id = msg_history["message"][-1]["next_msg_id"]
             except:
                 # 恢复失败
                 pass
             
-        msg_data = await self.send_msg(msg_data)
-        self.join = True
+        msg_data = await self.send_msg(msg_data,page,token,context_num)
+        #self.join = True
+        self.manage["status"][str(context_num)] = True
         return msg_data
     
     
-    async def show_chat_history(self,msg_data: MsgData) -> str:
+    async def show_chat_history(self,msg_data: MsgData) -> list:
         '''show chat history
         展示聊天记录'''
         msg_history = await self.load_chat(msg_data)
-        msg = ""
+        msg = []
         for x in msg_history["message"]:
-            msg += f"Q:{x['input']}\nA:{x['output']}\np_msg_id:{x['next_msg_id']}\n\n"
+            msg.append(f"Q:{x['input']}\n\nA:{x['output']}\n\np_msg_id:{x['next_msg_id']}")
         return msg
     
     async def back_chat_from_input(self,msg_data: MsgData):
         '''back chat from input
         You can enter the text that appeared last time, or the number of dialogue rounds starts from 1
         
         通过输入来回溯
@@ -325,18 +417,22 @@
             msg_data.msg_recv = "back error"
             return msg_data
             
     async def init_personality(self,msg_data: MsgData):
         '''init_personality
         初始化人格'''
         msg_data.msg_send = self.personality.get_value_by_name(msg_data.msg_send)
-        msg_data.conversation_id = ""
-        msg_data.p_msg_id = ""
-        msg_data.msg_type = "new_session"
-        return await self.continue_chat(msg_data)
+        if msg_data.msg_send:
+            msg_data.conversation_id = ""
+            msg_data.p_msg_id = ""
+            msg_data.msg_type = "new_session"
+            return await self.continue_chat(msg_data)
+        else:
+            msg_data.msg_recv = "not found"
+            return msg_data
     
     async def back_init_personality(self,msg_data: MsgData):
         '''
         back the init_personality time
         回到初始化人格之后'''
         msg_data.msg_send = "1"
         msg_data.msg_type = "back_loop"
```

### Comparing `ChatGPTWeb-0.0.5/ChatGPTWeb/config.py` & `ChatGPTWeb-0.0.6/ChatGPTWeb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         self.read_data()
         
     def del_data_by_name(self,name:str):
         for item in self.init_list:
             if item.get('name') == name:
                 self.init_list.remove(item)
         self.save_data()
-        return 
 
 
 class SetCookieParam(TypedDict, total=False):
     name: str
     value: str
     url: Optional[str]
     domain: Optional[str]
@@ -168,29 +167,29 @@
             "Connection": "keep-alive",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "TE": "trailers"
         }
         
-        
-def new_payload(prompt: str) -> str:
-    return json.dumps({
-        "action":
-        "next",
-        "messages": [{
-            "id": str(uuid.uuid4()),
-            "author": {
-                "role": "user"
-            },
-            "content": {
-                "content_type": "text",
-                "parts": [prompt]
-            }
-        }],
-        "parent_message_id":
-        str(uuid.uuid4()),
-        "model":
-        "text-davinci-002-render-sha",
-        "timezone_offset_min":
-        -480
-    })
+    @staticmethod        
+    def system_new_payload(prompt: str) -> str:
+        return json.dumps({
+            "action":
+            "next",
+            "messages": [{
+                "id": str(uuid.uuid4()),
+                "author": {
+                    "role": "system"
+                },
+                "content": {
+                    "content_type": "text",
+                    "parts": [prompt]
+                }
+            }],
+            "parent_message_id":
+            str(uuid.uuid4()),
+            "model":
+            "text-davinci-002-render-sha",
+            "timezone_offset_min":
+            -480
+        })
```

### Comparing `ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/PKG-INFO` & `ChatGPTWeb-0.0.6/ChatGPTWeb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.5
+Version: 0.0.6
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 # 待填坑
 -   [x] 网页api对话构成
 -   [x] 多人格预设与切换
 -   [x] 聊天记录存储与导出
 -   [x] 自定义人设
 -   [x] 重置聊天或回到某一时刻
--   [ ] 多账号并发
+-   [x] 多账号并发
 -   [ ] GPT4
 -   [ ] 代码过于混乱等优化
 -   [ ] 抽空完善readme
 
 
 # 安装/Install
 Ubuntu & Windows
@@ -61,15 +61,15 @@
 just simple to use
 
 简单使用
 
 ### copy __main__.py or this code to start / 复制 __main__.py 或者以下code来开始
 ```bash
 from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import Personality
+from ChatGPTWeb.config import Personality,MsgData
 import asyncio
 import aioconsole
 
 session_token=""
 
 personality_definition = Personality(
     [
@@ -85,29 +85,30 @@
 
 chat = chatgpt(session_token=session_token,log_status=False,personality=personality_definition)
 
 async def main():
     
     c_id = await aioconsole.ainput("your conversation_id if you have:")
     p_id = await aioconsole.ainput("your parent_message_id if you have:")
-    chat.data.conversation_id,chat.data.p_msg_id = c_id,p_id
+    data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
     while 1:
         print("\n------------------------------")
         data.msg_send = await aioconsole.ainput("input：")
         print("------------------------------\n")
         if data.msg_send == "quit":
             break
         elif data.msg_send == "re":
             data.msg_type = "back_loop"
             data.p_msg_id = await aioconsole.ainput("your parent_message_id if you go back:")
         elif data.msg_send == "reset":
             data = await chat.back_init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "init_personality":
+            data.msg_send = "your ..."
             data = await chat.init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "history":
             print(await chat.show_chat_history(data))
             continue
         data = await chat.continue_chat(data)
```

### Comparing `ChatGPTWeb-0.0.5/LICENSE` & `ChatGPTWeb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.5/PKG-INFO` & `ChatGPTWeb-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.5
+Version: 0.0.6
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 # 待填坑
 -   [x] 网页api对话构成
 -   [x] 多人格预设与切换
 -   [x] 聊天记录存储与导出
 -   [x] 自定义人设
 -   [x] 重置聊天或回到某一时刻
--   [ ] 多账号并发
+-   [x] 多账号并发
 -   [ ] GPT4
 -   [ ] 代码过于混乱等优化
 -   [ ] 抽空完善readme
 
 
 # 安装/Install
 Ubuntu & Windows
@@ -61,15 +61,15 @@
 just simple to use
 
 简单使用
 
 ### copy __main__.py or this code to start / 复制 __main__.py 或者以下code来开始
 ```bash
 from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import Personality
+from ChatGPTWeb.config import Personality,MsgData
 import asyncio
 import aioconsole
 
 session_token=""
 
 personality_definition = Personality(
     [
@@ -85,29 +85,30 @@
 
 chat = chatgpt(session_token=session_token,log_status=False,personality=personality_definition)
 
 async def main():
     
     c_id = await aioconsole.ainput("your conversation_id if you have:")
     p_id = await aioconsole.ainput("your parent_message_id if you have:")
-    chat.data.conversation_id,chat.data.p_msg_id = c_id,p_id
+    data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
     while 1:
         print("\n------------------------------")
         data.msg_send = await aioconsole.ainput("input：")
         print("------------------------------\n")
         if data.msg_send == "quit":
             break
         elif data.msg_send == "re":
             data.msg_type = "back_loop"
             data.p_msg_id = await aioconsole.ainput("your parent_message_id if you go back:")
         elif data.msg_send == "reset":
             data = await chat.back_init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "init_personality":
+            data.msg_send = "your ..."
             data = await chat.init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "history":
             print(await chat.show_chat_history(data))
             continue
         data = await chat.continue_chat(data)
```

### Comparing `ChatGPTWeb-0.0.5/README.md` & `ChatGPTWeb-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # 待填坑
 -   [x] 网页api对话构成
 -   [x] 多人格预设与切换
 -   [x] 聊天记录存储与导出
 -   [x] 自定义人设
 -   [x] 重置聊天或回到某一时刻
--   [ ] 多账号并发
+-   [x] 多账号并发
 -   [ ] GPT4
 -   [ ] 代码过于混乱等优化
 -   [ ] 抽空完善readme
 
 
 # 安装/Install
 Ubuntu & Windows
@@ -49,15 +49,15 @@
 just simple to use
 
 简单使用
 
 ### copy __main__.py or this code to start / 复制 __main__.py 或者以下code来开始
 ```bash
 from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import Personality
+from ChatGPTWeb.config import Personality,MsgData
 import asyncio
 import aioconsole
 
 session_token=""
 
 personality_definition = Personality(
     [
@@ -73,29 +73,30 @@
 
 chat = chatgpt(session_token=session_token,log_status=False,personality=personality_definition)
 
 async def main():
     
     c_id = await aioconsole.ainput("your conversation_id if you have:")
     p_id = await aioconsole.ainput("your parent_message_id if you have:")
-    chat.data.conversation_id,chat.data.p_msg_id = c_id,p_id
+    data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
     while 1:
         print("\n------------------------------")
         data.msg_send = await aioconsole.ainput("input：")
         print("------------------------------\n")
         if data.msg_send == "quit":
             break
         elif data.msg_send == "re":
             data.msg_type = "back_loop"
             data.p_msg_id = await aioconsole.ainput("your parent_message_id if you go back:")
         elif data.msg_send == "reset":
             data = await chat.back_init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "init_personality":
+            data.msg_send = "your ..."
             data = await chat.init_personality(data)
             print(f"ChatGPT:{data.msg_recv}")
             continue
         elif data.msg_send == "history":
             print(await chat.show_chat_history(data))
             continue
         data = await chat.continue_chat(data)
```

### Comparing `ChatGPTWeb-0.0.5/setup.py` & `ChatGPTWeb-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["playwright","aioconsole"] # 这里填依赖包信息
 
 setup(
     name="ChatGPTWeb",
-    version="0.0.5",
+    version="0.0.6",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="a ChatGPT API,no web ui",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/ChatGPT",
     packages=find_packages(),
```

