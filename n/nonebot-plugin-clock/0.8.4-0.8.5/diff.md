# Comparing `tmp/nonebot-plugin-clock-0.8.4.tar.gz` & `tmp/nonebot-plugin-clock-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-clock-0.8.4.tar", last modified: Thu Apr 13 04:03:14 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.5.tar", last modified: Thu Apr 13 07:57:01 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.4.tar` & `nonebot-plugin-clock-0.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.282221 nonebot-plugin-clock-0.8.4/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.4/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-13 04:03:14.281702 nonebot-plugin-clock-0.8.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.4/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.279517 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     6241 2023-04-13 03:48:48.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.281246 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 04:03:14.282330 nonebot-plugin-clock-0.8.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 04:03:09.000000 nonebot-plugin-clock-0.8.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.5/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.5/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     6352 2023-04-13 07:56:37.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 07:56:07.000000 nonebot-plugin-clock-0.8.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nonebot-plugin-clock-0.8.4/LICENSE` & `nonebot-plugin-clock-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.4/README.md` & `nonebot-plugin-clock-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
 from datetime import datetime, timedelta
 from nonebot.permission import SUPERUSER
-from nonebot import on_command, get_bot, get_driver
+from nonebot import on_command, on_regex ,get_bot, get_driver
 from nonebot.adapters.onebot.v11.bot import Bot
 from nonebot.adapters.onebot.v11.event import Event
 from nonebot.adapters.onebot.v11.message import Message, MessageSegment
 from nonebot.params import CommandArg
 from nonebot.typing import T_State
 from nonebot import require
 
@@ -172,17 +172,17 @@
     ones_ = {1:'不重复', 0:'重复'}
     await add_clock_qq.finish(message=f"[{ones_[ones]}]添加成功～")
 
 
 
 
 # # 查看闹钟
-check = on_command('查看闹钟',  aliases={'提醒事项', '闹钟','⏰'}, block=True)
+check = on_regex("^(查看闹钟|提醒事项|闹钟|⏰)$" ,block=True)
 @check.handle()
-async def add_handle(bot: Bot, event: Event):
+async def _(bot: Bot, event: Event):
 
     uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
 
 
     def check_(msg: str) -> str:
 
         message = ""
@@ -205,20 +205,20 @@
         await bot.send(event, message='目前没有闹钟')
     
 
 
 # 删除闹钟
 del_ = on_command('删除闹钟', block=True)
 @del_.handle()
-async def del_handle(bot: Bot, event: Event, id = CommandArg()):
-    id = int(str(id))
-    uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
-    if del_clock(id, uid):
-        await del_.finish(message='删除成功')
-    else:
-        await del_.finish(message='不存在的id')
-    await del_.finish(message='失败了')
-
-
-
-
-
+async def _(bot: Bot, event: Event, ids = CommandArg()):
+    ids = str(ids).split()
+    
+    if ids:
+        uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
+        task = [[],[]]
+        for id in ids:
+            id = int(id)
+            if del_clock(id, uid):
+                task[0].append(id) # succeed
+            else:
+                task[1].append(id) # fail
+        await del_.finish(message=f'删除闹钟{task[0]}\n不存在的id{task[1]}')
```

### Comparing `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.4/setup.py` & `nonebot-plugin-clock-0.8.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.4',
+    version='0.8.5',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

