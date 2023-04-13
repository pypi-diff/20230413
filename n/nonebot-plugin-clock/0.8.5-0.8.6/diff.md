# Comparing `tmp/nonebot-plugin-clock-0.8.5.tar.gz` & `tmp/nonebot-plugin-clock-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.5.tar", last modified: Thu Apr 13 07:57:01 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.6.tar", last modified: Thu Apr 13 09:32:33 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.5.tar` & `nonebot-plugin-clock-0.8.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.5/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.5/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     6352 2023-04-13 07:56:37.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.5/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 07:57:01.000000 nonebot-plugin-clock-0.8.5/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 07:56:07.000000 nonebot-plugin-clock-0.8.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.6/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.6/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     6182 2023-04-13 09:30:23.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 09:30:52.000000 nonebot-plugin-clock-0.8.6/setup.py
```

### Comparing `nonebot-plugin-clock-0.8.5/LICENSE` & `nonebot-plugin-clock-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.5/README.md` & `nonebot-plugin-clock-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,36 +104,28 @@
     return t
         
 
 # 创建闹钟
 add_clock_qq = on_command('添加闹钟', aliases={'设置闹钟',})
 @add_clock_qq.handle()
 async def _(bot: Bot, event: Event, state: T_State, messages: Message = CommandArg()):
-
+    
     messages = str(messages).split(' ', 1)
-    content = ''
 
     if len(messages) < 2:
         await add_clock_qq.finish(message="添加格式为: “添加闹钟 时间 内容”")
 
     time_ = get_time(messages[0])
     if not time_:
         await add_clock_qq.finish(message="时间格式错误")
 
-    for msg in Message(messages[1]):
-        if url:=msg.data.get("url"):
-            content += str(MessageSegment(msg.type, {"file":url}))
-        else:
-            content += str(msg)
-
-
     state['time'] = time_
     state['type'] = 'private'
     state['user'] = event.user_id
-    state['content'] = content if content else '⏰'
+    state['content'] = messages[1] if messages[1] else '⏰'
 
     if 'group' in event.get_event_name():
         res1 = await SUPERUSER(bot, event)
         res2 = await CLOCK_RULE(event)
         if not (res1 or res2):
             await add_clock_qq.finish(message="你没有该权限哦～")
         state['type'] = 'group'
@@ -217,8 +209,8 @@
         task = [[],[]]
         for id in ids:
             id = int(id)
             if del_clock(id, uid):
                 task[0].append(id) # succeed
             else:
                 task[1].append(id) # fail
-        await del_.finish(message=f'删除闹钟{task[0]}\n不存在的id{task[1]}')
+        await del_.finish(message=f'删除闹钟{task[0]}'+ f'\n不存在的id{task[1]}' if task[1] else '')
```

### Comparing `nonebot-plugin-clock-0.8.5/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.5/setup.py` & `nonebot-plugin-clock-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.5',
+    version='0.8.6',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

