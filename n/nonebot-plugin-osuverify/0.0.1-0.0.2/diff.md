# Comparing `tmp/nonebot-plugin-osuverify-0.0.1.tar.gz` & `tmp/nonebot-plugin-osuverify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-osuverify-0.0.1.tar", last modified: Thu Apr 13 13:04:16 2023, max compression
+gzip compressed data, was "nonebot-plugin-osuverify-0.0.2.tar", last modified: Thu Apr 13 13:09:04 2023, max compression
```

## Comparing `nonebot-plugin-osuverify-0.0.1.tar` & `nonebot-plugin-osuverify-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:04:16.451376 nonebot-plugin-osuverify-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-13 13:04:05.000000 nonebot-plugin-osuverify-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:04:16.451376 nonebot-plugin-osuverify-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-04-13 13:04:05.000000 nonebot-plugin-osuverify-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:04:16.447376 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify/
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-04-13 13:04:05.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:04:16.447376 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:04:16.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-13 13:04:16.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 13:04:16.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-13 13:04:16.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 13:04:16.000000 nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 13:04:16.451376 nonebot-plugin-osuverify-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-04-13 13:04:05.000000 nonebot-plugin-osuverify-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.367813 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/setup.py
```

### Comparing `nonebot-plugin-osuverify-0.0.1/LICENSE` & `nonebot-plugin-osuverify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.0.1/PKG-INFO` & `nonebot-plugin-osuverify-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.0.1
+Version: 0.0.2
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.2 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-osuverify-0.0.1/README.md` & `nonebot-plugin-osuverify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify/__init__.py` & `nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.0.1/nonebot_plugin_osuverify.egg-info/PKG-INFO` & `nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.0.1
+Version: 0.0.2
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.2 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-osuverify-0.0.1/setup.py` & `nonebot-plugin-osuverify-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-osuverify",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.1",  # 程序版本
+    version="0.0.2",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="通过osu!账号审核入群功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.8",  # 使用Python3.8
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        'httpx>=0.23.3',
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.0.0b1'
     ]
 )
```

