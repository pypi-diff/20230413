# Comparing `tmp/nonebot-plugin-clock-0.8.2.tar.gz` & `tmp/nonebot-plugin-clock-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.2.tar", last modified: Thu Apr 13 03:19:51 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.3.tar", last modified: Thu Apr 13 03:44:20 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.2.tar` & `nonebot-plugin-clock-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.2/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.2/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     5779 2023-04-13 03:17:41.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1936 2023-04-13 03:15:30.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.2/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 03:19:51.000000 nonebot-plugin-clock-0.8.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 03:17:56.000000 nonebot-plugin-clock-0.8.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.3/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     5779 2023-04-13 03:32:44.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1936 2023-04-13 03:15:30.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.3/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 03:44:20.000000 nonebot-plugin-clock-0.8.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 03:43:56.000000 nonebot-plugin-clock-0.8.3/setup.py
```

### Comparing `nonebot-plugin-clock-0.8.2/LICENSE` & `nonebot-plugin-clock-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.2/README.md` & `nonebot-plugin-clock-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from nonebot import require
 
 from .database import db
 from .Clock import Clock
 
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 
-WHITELIST = getattr(get_driver().config, 'CLOCK_WHITE_LIST', [])
-BLACKLIST = getattr(get_driver().config, 'CLOCK_BLACK_LIST', [])
+WHITELIST = getattr(get_driver().config, 'clock_white_list', [])
+BLACKLIST = getattr(get_driver().config, 'clock_black_list', [])
 CLOCK_DATA = {}
 
 async def CLOCK_RULE(event: Event) -> bool:
     
     # 黑名单优先判定
     if BLACKLIST:
         return event.user_id not in BLACKLIST
```

### Comparing `nonebot-plugin-clock-0.8.2/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.3/nonebot_plugin_clock/database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.2/setup.py` & `nonebot-plugin-clock-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.2',
+    version='0.8.3',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

