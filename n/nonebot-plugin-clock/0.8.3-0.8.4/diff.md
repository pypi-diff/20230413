# Comparing `tmp/nonebot-plugin-clock-0.8.3.tar.gz` & `tmp/nonebot-plugin-clock-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.3.tar", last modified: Thu Apr 13 03:44:20 2023, max compression
+gzip compressed data, was "nonebot-plugin-clock-0.8.4.tar", last modified: Thu Apr 13 04:03:14 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.3.tar` & `nonebot-plugin-clock-0.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.3/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.3/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     5779 2023-04-13 03:32:44.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1936 2023-04-13 03:15:30.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 03:43:56.000000 nonebot-plugin-clock-0.8.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.282221 nonebot-plugin-clock-0.8.4/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.4/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-13 04:03:14.281702 nonebot-plugin-clock-0.8.4/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.4/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.279517 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     6241 2023-04-13 03:48:48.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 04:03:14.281246 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 04:03:14.000000 nonebot-plugin-clock-0.8.4/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.4/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 04:03:14.282330 nonebot-plugin-clock-0.8.4/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 04:03:09.000000 nonebot-plugin-clock-0.8.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nonebot-plugin-clock-0.8.3/LICENSE` & `nonebot-plugin-clock-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.3/README.md` & `nonebot-plugin-clock-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,23 +57,38 @@
     """添加闹钟"""
     kwargs['id'] = db.new_id()
     clock = Clock((kwargs))
     db.add_clock(clock)
     create_clock_scheduler(clock)
 
 def del_clock(id: int, uid: int):
-    """删除闹钟"""
+    """
+    删除闹钟 防止用户误删
+    Args:
+        id(int): database中的clock id (唯一)
+        uid(int): user_id 或 group_id
+    Returns:
+        bool
+    """
     if db.del_clock(id, uid):
         del(CLOCK_DATA[id])
         scheduler.remove_job(f"clock_{id}")
         return True
 
 
 
 def get_time(time_):
+    """
+    获取指定时间字符串的标准化时间格式
+    Args:
+        time_ (str): 输入的时间字符串，可以为 "+2H30M"（表示2小时30分钟后的时间） 或 "13:45"（指定的具体时间）
+    
+    Returns:
+        str: 标准化的时间格式字符串，例如 "13:45"
+    """
     t = None
     r = re.match(r'(\d+)[:|\-|：|.](\d+)',time_)
     if time_.startswith('+'):
         h = re.search(r"(\d+)[Hh时]",time_)
         m = re.search(r"(\d+)[Mm分]",time_)
         h=int(h.groups()[0]) if h else 0
         m=int(m.groups()[0]) if m else 0
```

### Comparing `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.4/nonebot_plugin_clock/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 
     def add_clock(self, clock: Clock):
         sql = f'''INSERT INTO {self.table} (type, user, content, month, day, week, c_time, ones)
         values ("{clock.type}", {clock.user}, "{clock.content}","{clock.month}","{clock.day}","{clock.week}","{clock.time}",{clock.ones});'''
         self.execute(sql)
 
     def del_clock(self, id: int, user: int):
-        if self.execute(f"DELETE from {self.table} where id = {id} and user = {user}"):
-            return self.execute(f"DELETE from {self.table} where id = {id}")
+        if self.execute(f"SELECT id FROM {self.table} where id = {id} and user = {user}"):
+            self.execute(f"DELETE from {self.table} where id = {id}")
+            return True
 
     def select_all(self):
         '''
         (id, type, user, content, c_time, ones) 
         '''
         #DataFrame(data = data, columns=['id', 'type', 'uid', 'note', 'time', 'omes'])
         return self.execute(f"SELECT * FROM {self.table};")
```

### Comparing `nonebot-plugin-clock-0.8.3/setup.py` & `nonebot-plugin-clock-0.8.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.3',
+    version='0.8.4',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

