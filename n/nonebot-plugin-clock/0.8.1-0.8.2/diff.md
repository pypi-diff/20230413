# Comparing `tmp/nonebot-plugin-clock-0.8.1.tar.gz` & `tmp/nonebot-plugin-clock-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.1.tar", last modified: Wed Apr 12 10:48:33 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.2.tar", last modified: Thu Apr 13 03:19:51 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.1.tar` & `nonebot-plugin-clock-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1284 2023-04-12 10:23:52.000000 nonebot-plugin-clock-0.8.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     5674 2023-04-12 10:39:38.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1821 2023-04-12 10:48:21.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.1/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-12 10:48:33.000000 nonebot-plugin-clock-0.8.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-12 10:48:31.000000 nonebot-plugin-clock-0.8.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.2/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     5779 2023-04-13 03:17:41.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1936 2023-04-13 03:15:30.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 03:17:56.000000 nonebot-plugin-clock-0.8.2/setup.py
```

### Comparing `nonebot-plugin-clock-0.8.1/LICENSE` & `nonebot-plugin-clock-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.1/README.md` & `nonebot-plugin-clock-0.8.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 删除闹钟 ID
     - ID 闹钟对应id (`查看闹钟`第一项)
 ```
 
 
 
 ## 更新
-- 2023.4.12  优化⏰ [issues 1](https://github.com/Zeta-qixi/nonebot-plugin-clock/issues/1)
+- 2023.4.12  优化⏰ [issues #1](https://github.com/Zeta-qixi/nonebot-plugin-clock/issues/1)
+- 2023.4.13  优化⏰ [issues #1](https://github.com/Zeta-qixi/nonebot-plugin-clock/issues/1) 优化⏰ [issues #2](https://github.com/Zeta-qixi/nonebot-plugin-clock/issues/2)
```

### Comparing `nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     CLOCK_DATA[clock.id] = clock
 
     async def add_clock():
         if clock.verify_today():
             await get_bot().send_msg(message_type=clock.type, user_id=clock.user, group_id=clock.user, message=clock.content)          
 
             if clock.ones == 1:
-                del_clock(clock.id)
+                del_clock(clock.id, clock.user)
 
     scheduler.add_job(add_clock, "cron", hour=clock.hour, minute=clock.minute, id=f"clock_{clock.id}")
 
 
 for i in db.select_all():
     create_clock_scheduler(Clock.init_from_db(i))
 
@@ -56,20 +56,20 @@
 def add_clock(**kwargs):
     """添加闹钟"""
     kwargs['id'] = db.new_id()
     clock = Clock((kwargs))
     db.add_clock(clock)
     create_clock_scheduler(clock)
 
-def del_clock(id: int):
+def del_clock(id: int, uid: int):
     """删除闹钟"""
-    del(CLOCK_DATA[id])
-    db.del_clock(id)
-    scheduler.remove_job(f"clock_{id}")
-    return True
+    if db.del_clock(id, uid):
+        del(CLOCK_DATA[id])
+        scheduler.remove_job(f"clock_{id}")
+        return True
 
 
 
 def get_time(time_):
     t = None
     r = re.match(r'(\d+)[:|\-|：|.](\d+)',time_)
     if time_.startswith('+'):
@@ -192,18 +192,18 @@
 
 
 # 删除闹钟
 del_ = on_command('删除闹钟', block=True)
 @del_.handle()
 async def del_handle(bot: Bot, event: Event, id = CommandArg()):
     id = int(str(id))
-    if id in CLOCK_DATA:
-        del_clock(id)
+    uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
+    if del_clock(id, uid):
         await del_.finish(message='删除成功')
     else:
-        await del_.finish(message='没有这个id')
+        await del_.finish(message='不存在的id')
     await del_.finish(message='失败了')
```

### Comparing `nonebot-plugin-clock-0.8.1/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,16 +49,17 @@
 
 
     def add_clock(self, clock: Clock):
         sql = f'''INSERT INTO {self.table} (type, user, content, month, day, week, c_time, ones)
         values ("{clock.type}", {clock.user}, "{clock.content}","{clock.month}","{clock.day}","{clock.week}","{clock.time}",{clock.ones});'''
         self.execute(sql)
 
-    def del_clock(self, id):
-        self.execute(f"DELETE from {self.table} where id = {id}")
+    def del_clock(self, id: int, user: int):
+        if self.execute(f"DELETE from {self.table} where id = {id} and user = {user}"):
+            return self.execute(f"DELETE from {self.table} where id = {id}")
 
     def select_all(self):
         '''
         (id, type, user, content, c_time, ones) 
         '''
         #DataFrame(data = data, columns=['id', 'type', 'uid', 'note', 'time', 'omes'])
         return self.execute(f"SELECT * FROM {self.table};")
```

### Comparing `nonebot-plugin-clock-0.8.1/setup.py` & `nonebot-plugin-clock-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.1',
+    version='0.8.2',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

