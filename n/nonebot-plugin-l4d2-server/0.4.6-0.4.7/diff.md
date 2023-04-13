# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.6.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.7.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.6.tar` & `nonebot_plugin_l4d2_server-0.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.6/LICENSE
--rw-r--r--   0        0        0    16832 2023-04-09 16:02:28.698025 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8027 2023-04-08 18:50:15.782345 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     4966 2023-04-09 16:00:29.769094 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10845 2023-04-09 15:59:41.750644 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1505 2023-04-09 16:02:33.334787 nonebot_plugin_l4d2_server-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    11317 2023-04-09 16:03:41.480929 nonebot_plugin_l4d2_server-0.4.6/README.md
--rw-r--r--   0        0        0    13126 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.6/setup.py
--rw-r--r--   0        0        0    12982 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.7/LICENSE
+-rw-r--r--   0        0        0    16832 2023-04-13 15:54:53.327359 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8320 2023-04-13 15:13:32.781982 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     5046 2023-04-13 15:39:47.743742 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1748 2023-04-13 15:08:36.760710 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      788 2023-04-13 15:01:07.140804 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10949 2023-04-13 15:16:25.729675 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/config.py
+-rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1505 2023-04-13 15:54:44.311520 nonebot_plugin_l4d2_server-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    11486 2023-04-13 15:53:58.072926 nonebot_plugin_l4d2_server-0.4.7/README.md
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.7/setup.py
+-rw-r--r--   0        0        0    13142 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.7/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/LICENSE` & `nonebot_plugin_l4d2_server-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     from .l4d2_web import web,webUI
 else:
     pass
 
 driver = get_driver()
 
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,20 +153,27 @@
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
         if not msg:
             # 以图片输出全部当前
-            this_ips:dict = ALL_HOST[command]
+            if command in gamemode_list:
+                this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
+                igr = True
+            else:
+                this_ips:list = ALL_HOST[command]
+                igr = False
+            if not this_ips:
+                matcher.finish('')
             ip_list = []
             for one_ip in this_ips:
                 host,port = split_maohao(one_ip['ip'])
                 ip_list.append((one_ip['id'],host,port))
-            img = await qq_ip_queries_pic(ip_list)
+            img = await qq_ip_queries_pic(ip_list,igr)
             if img:
                 await matcher.finish(MessageSegment.image(img)) 
             else:
                 await matcher.finish("服务器无响应")
         else:
             if not msg[0].isdigit():
                 if any(mode in msg for mode in gamemode_list):
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -276,36 +276,41 @@
 00001130: 6162 6c65 5f64 6174 615b 315d 3a4c 3464  able_data[1]:L4d
 00001140: 325f 7365 7276 6572 5f74 6167 0d0a 7d0d  2_server_tag..}.
 00001150: 0a0d 0a23 20e6 b182 e794 9f61 6e6e 65e6  ...# ......anne.
 00001160: 9c8d e58a a1e5 99a8 0d0a 616e 6e65 5f75  ..........anne_u
 00001170: 726c 203d 2022 6874 7470 733a 2f2f 7365  rl = "https://se
 00001180: 7276 6572 2e74 7279 6765 6b2e 636f 6d2f  rver.trygek.com/
 00001190: 220d 0a0d 0a67 616d 656d 6f64 655f 6c69  "....gamemode_li
-000011a0: 7374 203d 205b 0d0a 2020 2020 27e6 8898  st = [..    '...
-000011b0: e5bd b927 2c0d 0a20 2020 2027 e5a4 9ae7  ...',..    '....
-000011c0: 89b9 272c 0d0a 2020 2020 27e5 8699 e4b8  ..',..    '.....
-000011d0: 9327 2c0d 0a20 2020 2027 616e 6e65 272c  .',..    'anne',
-000011e0: 0d0a 2020 2020 27e8 8daf e68a 9727 2c0d  ..    '......',.
-000011f0: 0a20 2020 2027 e58c 85e6 8a97 272c 0d0a  .    '......',..
-00001200: 2020 2020 27e7 bb9d e5a2 8327 2c0d 0a20      '......',.. 
-00001210: 2020 2027 e6ad bbe4 b893 272c 0d0a 2020     '......',..  
-00001220: 2020 2761 7374 272c 0d0a 2020 2020 27e6    'ast',..    '.
-00001230: b885 e981 93e5 a4ab 272c 0d0a 5d0d 0a0d  ........',..]...
-00001240: 0a23 20e7 b3bb e7bb 9f0d 0a69 6620 706c  .# ........if pl
-00001250: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
-00001260: 3d3d 2027 5769 6e64 6f77 7327 3a0d 0a20  == 'Windows':.. 
-00001270: 2020 2073 7973 7465 6d73 3a73 7472 203d     systems:str =
-00001280: 2027 7769 6e27 0d0a 656c 6966 2070 6c61   'win'..elif pla
-00001290: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
-000012a0: 3d20 274c 696e 7578 273a 0d0a 2020 2020  = 'Linux':..    
-000012b0: 7379 7374 656d 733a 7374 7220 3d20 276c  systems:str = 'l
-000012c0: 696e 7578 270d 0a65 6c73 653a 0d0a 2020  inux'..else:..  
-000012d0: 2020 7379 7374 656d 733a 7374 7220 3d20    systems:str = 
-000012e0: 276f 7468 6572 7327 0d0a 414e 4e45 5f49  'others'..ANNE_I
-000012f0: 5020 3d20 7b7d 0d0a 0d0a 7472 793a 0d0a  P = {}....try:..
-00001300: 2020 2020 6f73 2e72 656d 6f76 6528 5061      os.remove(Pa
-00001310: 7468 2829 2e70 6172 656e 742e 6a6f 696e  th().parent.join
-00001320: 7061 7468 2827 6461 7461 2f4c 3444 322f  path('data/L4D2/
-00001330: 6c34 6432 2e79 6d6c 2729 290d 0a65 7863  l4d2.yml'))..exc
-00001340: 6570 743a 0d0a 2020 2020 7061 7373 0d0a  ept:..    pass..
-00001350: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00001360: 2020 2020 2020                                 
+000011a0: 7374 203d 205b 0d0a 2020 2020 27e7 baaf  st = [..    '...
+000011b0: e587 8027 2c0d 0a20 2020 2027 e9ad 94e6  ...',..    '....
+000011c0: 94b9 e688 98e5 bdb9 272c 0d0a 2020 2020  ........',..    
+000011d0: 27e5 a49a e789 b927 2c0d 0a20 2020 2027  '......',..    '
+000011e0: e9ad 94e6 94b9 e5a4 9ae7 89b9 272c 0d0a  ............',..
+000011f0: 2020 2020 27e5 8699 e4b8 9327 2c0d 0a20      '......',.. 
+00001200: 2020 2027 e5af b9e6 8a97 272c 0d0a 2020     '......',..  
+00001210: 2020 27e9 ad94 e694 b9e5 afb9 e68a 9727    '............'
+00001220: 2c0d 0a20 2020 2027 e88d afe5 bdb9 272c  ,..    '......',
+00001230: 0d0a 2020 2020 27e8 8daf e68a 9727 2c0d  ..    '......',.
+00001240: 0a20 2020 2027 e58c 85e6 8a97 272c 0d0a  .    '......',..
+00001250: 2020 2020 27e7 bb9d e5a2 8327 2c0d 0a20      '......',.. 
+00001260: 2020 2027 e6ad bbe4 b893 272c 0d0a 2020     '......',..  
+00001270: 2020 2761 7374 272c 0d0a 2020 2020 27e6    'ast',..    '.
+00001280: b885 e981 93e5 a4ab 272c 0d0a 5d0d 0a0d  ........',..]...
+00001290: 0a23 20e7 b3bb e7bb 9f0d 0a69 6620 706c  .# ........if pl
+000012a0: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
+000012b0: 3d3d 2027 5769 6e64 6f77 7327 3a0d 0a20  == 'Windows':.. 
+000012c0: 2020 2073 7973 7465 6d73 3a73 7472 203d     systems:str =
+000012d0: 2027 7769 6e27 0d0a 656c 6966 2070 6c61   'win'..elif pla
+000012e0: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
+000012f0: 3d20 274c 696e 7578 273a 0d0a 2020 2020  = 'Linux':..    
+00001300: 7379 7374 656d 733a 7374 7220 3d20 276c  systems:str = 'l
+00001310: 696e 7578 270d 0a65 6c73 653a 0d0a 2020  inux'..else:..  
+00001320: 2020 7379 7374 656d 733a 7374 7220 3d20    systems:str = 
+00001330: 276f 7468 6572 7327 0d0a 414e 4e45 5f49  'others'..ANNE_I
+00001340: 5020 3d20 7b7d 0d0a 0d0a 7472 793a 0d0a  P = {}....try:..
+00001350: 2020 2020 6f73 2e72 656d 6f76 6528 5061      os.remove(Pa
+00001360: 7468 2829 2e70 6172 656e 742e 6a6f 696e  th().parent.join
+00001370: 7061 7468 2827 6461 7461 2f4c 3444 322f  path('data/L4D2/
+00001380: 6c34 6432 2e79 6d6c 2729 290d 0a65 7863  l4d2.yml'))..exc
+00001390: 6570 743a 0d0a 2020 2020 7061 7373 0d0a  ept:..    pass..
+000013a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000013b0: 2020 2020 2020
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import httpx
 from bs4 import BeautifulSoup
 import json
 from pathlib import Path
-from ..config import TEXT_PATH,anne_url,ANNE_IP
+from ..config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
 from ..l4d2_queries.ohter import ALL_HOST
 
 # 储存anne服务器ip
 
 
 
 
@@ -53,12 +53,13 @@
         
 def server_key():
     """响应的服务器开头"""
     a = set()
     try:
         for tag1,value in ALL_HOST.items():
             a.add(tag1)
+        a.update(gamemode_list)
     except AttributeError:
         a.add('希腊那我从来没有想过这个事情')
-    return  a
+    return a
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 try:
         import ujson as json
 except:
         import json
 from pathlib import Path
+from typing import Dict,List
 import os
 
 BOT_DIR = os.path.dirname(os.path.abspath(__file__))
 filename = 'data/L4D2/l4d2.json'
 global_file = Path(Path(__file__).parent.parent,filename)
 def load_josn():
         # 本地模块
@@ -17,8 +18,8 @@
                 os.makedirs(os.path.dirname(filename), exist_ok=True)
                 data = {}
                 with open(filename, "w") as f:
                         json.dump(data, f)
                 LOCAL_HOST:dict = {}
         return LOCAL_HOST
 
-ALL_HOST:dict = load_josn()
+ALL_HOST:Dict[str, List[dict]] = load_josn()
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,62 +48,65 @@
         number,qqgroup,host,port = i
         msg2 = await player_queries(host,port)
         msg1 = await queries(host,port)
         messsage += '序号、'+ str(number) + '\n' + msg1 + msg2 + '--------------------\n'
     return messsage
             
             
-async def qq_ip_querie(msg: list):
+async def qq_ip_querie(msg: list,igr:bool):
     msg_list = []
     tasks = []  # 用来保存异步任务
     if msg != []:
         for i in msg:
             try:
                 number, host, port = i
                 qqgroup = ''
             except ValueError:
                 number, qqgroup, host, port = i
             finally:
                 # 将异步任务添加到任务列表中
-                tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup)))
+                tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup,igr)))
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
         msg_list.sort(key=lambda x: x['number'])
         result = {'msg_list': msg_list}
 
     else:
         result = {}
     return result
 
 
-async def qq_ip_queries_pic(msg: list):
-    result = await qq_ip_querie(msg)
+async def qq_ip_queries_pic(msg: list,igr = False):
+    result = await qq_ip_querie(msg,igr)
     if 'msg_list' in result:
         pic = await server_ip_pic(result['msg_list'])
     else:
         pic = None
     return pic
             
 
 
 
-async def process_message(number, host, port, msg_list:list,qqgroup = ''):
+async def process_message(number, host, port, msg_list:list,igr:bool,qqgroup = ''):
     try:
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
         msg1.update({'Players':msg2,'number':number,})
         if qqgroup:
             msg1.update({'tag':qqgroup})
         msg_list.append(msg1)
     except errors:
-        # 空白字典
-        null_dict = {key: 'null' for key in ['name', 'map_', 'players', 'max_players', 'rank_players', 'ping']}
-        null_dict.update({'number':number,'ip':f'{host}:{port}','Players':[]})
-        msg_list.append(null_dict)  
+        if igr:
+            pass
+        else:
+            # 空白字典
+            null_dict = {key: 'null' for key in ['name', 'map_', 'players', 'max_players', 'rank_players', 'ping']}
+            null_dict.update({'number':number,'ip':f'{host}:{port}','Players':[]})
+            msg_list.append(null_dict)  
 
 
     
 async def get_tan_jian(msg:List[tuple],mode:int):
     """获取anne列表抽一个"""
     msg_list = []
     random.shuffle(msg)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/config.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.4.7/nonebot_plugin_l4d2_server/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.6/pyproject.toml` & `nonebot_plugin_l4d2_server-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.6"
+version = "0.4.7"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/README.md` & `nonebot_plugin_l4d2_server-0.4.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
+        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
 </a>
@@ -24,76 +24,79 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
-    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 </div>
 
 
 ## 快速使用（env示例）
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
     l4_master = ['1145149191']            # 允许上传地图的qq号
     l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
     l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
     l4_port = ['20715']                   # 服务器端口
     l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
     l4_font = 'simsun.ttc'                # 服务器字体
+    l4_web = True                         # 网页控制台，默认是关闭
 
 
-## 新文档（暂未完成）
 
-[点击这里](https://Agnes4m.github.io/l4d2)
-
-<h2 id="gn">主要功能</h2>
+## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
 
-<h2 id="gn">如何获取key</h2>
+## 如何获取key
 
 为了使得ip不被滥用，我采取这种方式管理。
 
 这并不影响正常使用，如果不需要可以忽略
 
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
         l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
         l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
 
 
-## 🚑  提交自己的服务器？
+## 提交自己的服务器？
 
 **本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
 
 **那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**
 
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
 
         {
         "呆呆": [
                 {
                 "id": 1,
                 "version": "战役",
                 "ip": "43.248.188.17:27031"
+                },
+                {
+                "id": 2,
+                "version": "战役",
+                "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
-<h2 id="ty">🌐 默认服务器</h2>
+## 🌐 默认服务器
 目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
 | 云 | anne电信服云服 | 东 | 27
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
@@ -108,14 +111,19 @@
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.7--2022.4.13
+
+ - 新增模式查询
+ - 列表推导替换套娃循环
+
 ### 0.4.6--2022.4.9
 
  - 显示无效服
  - 优化服务器排序算法（list.sort()天下第一）
  - 默认关闭web端
 
 ### 0.4.5--2022.4.9
@@ -318,16 +326,17 @@
 
 + 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
 + [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
-<h2 id="ty">🌐 感谢</h2>
+## 🌐 感谢
 
+- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架
 - [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
 - [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
 - [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
 - 呆呆 - 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -9,46 +9,45 @@
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
 # ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
 åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
 æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
 æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
 æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
 æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
-'simsun.ttc' # æå¡å¨å­ä½ ## æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é]
-(https://Agnes4m.github.io/l4d2)
-***** ä¸»è¦åè½ *****
-- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+'simsun.ttc' # æå¡å¨å­ä½ l4_web = True #
+ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­ ## ä¸»è¦åè½ - æ±çæå¡å¨-
+æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)
-***** å¦ä½è·åkey *****
+ranking/index.php) ## å¦ä½è·åkey
 ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
 è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
 (https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
 l4_key = 'qwertyuiopasdfg' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
 æäº¤èªå·±çæå¡å¨ï¼
 **æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
 **é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
-{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
-***** ð é»è®¤æå¡å¨ *****
-ç®å **å·²ææ**
+{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
+{ "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
+é»è®¤æå¡å¨ ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
+0.4.7--2022.4.13 - æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ###
 0.4.6--2022.4.9 - æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort
 ()å¤©ä¸ç¬¬ä¸ï¼ - é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼
 ### 0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯
 - webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
@@ -124,17 +123,17 @@
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
 æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)
-***** ð æè°¢ *****
-- [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
+[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
+github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:
+//github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
 github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
 MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
 github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
 webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/setup.py` & `nonebot_plugin_l4d2_server-0.4.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,17 @@
  'rarfile>=4.0,<5.0',
  'rcon>=2.1.0,<3.0.0',
  'ruamel.yaml>=0.17.21,<0.18.0',
  'srctools>=2.3.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.6',
+    'version': '0.4.7',
     'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://Agnes4m.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14\n| 橘 | 橘希实香的小窝 | 橘希实香 | 14\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.6--2022.4.9\n\n - 显示无效服\n - 优化服务器排序算法（list.sort()天下第一）\n - 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n    l4_web = True                         # 网页控制台，默认是关闭\n\n\n\n## 主要功能\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n## 如何获取key\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                },\n                {\n                "id": 2,\n                "version": "战役",\n                "ip": "43.248.188.17:27032"\n                }\n        ]\n        }\n\n## 🌐 默认服务器\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14\n| 橘 | 橘希实香的小窝 | 橘希实香 | 14\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.7--2022.4.13\n\n - 新增模式查询\n - 列表推导替换套娃循环\n\n### 0.4.6--2022.4.9\n\n - 显示无效服\n - 优化服务器排序算法（list.sort()天下第一）\n - 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
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
@@ -12,15 +12,15 @@
 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
 'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
 a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
 'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
 'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
-server', 'version': '0.4.6', 'description': 'L4D2 server related operations
+server', 'version': '0.4.7', 'description': 'L4D2 server related operations
 plugin for NoneBot2', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
          \n\n# nonebot_plugin_l4d2_server\n_â¨Nonebot & Left 4 Dead 2
@@ -33,44 +33,42 @@
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®\n
 # ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\'] #
 åè®¸ä¸ä¼ å°å¾çqqå·\n l4_file = [\'/home/ubuntu/l4d2/coop\'] #
 æ¬å°æå¡å¨è·¯å¾\n l4_host = [\'127.0.0.1\'] #
 æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼\n l4_port = [\'20715\'] #
 æå¡å¨ç«¯å£\n l4_rcon = [\'1145149191810\'] #
 æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´ \n l4_font =
-\'simsun.ttc\' # æå¡å¨å­ä½\n\n\n## æ°ææ¡£ï¼ææªå®æï¼\n\n
-[ç¹å»è¿é](https://Agnes4m.github.io/l4d2)\n\n
-***** ä¸»è¦åè½ *****
-\n\n- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
+\'simsun.ttc\' # æå¡å¨å­ä½\n l4_web = True #
+ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­\n\n\n\n## ä¸»è¦åè½\n\n- æ±çæå¡å¨-
+æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
 åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)\n\n\n
-***** å¦ä½è·åkey *****
-\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n\nè¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥\n\n
+ranking/index.php)\n\n\n##
+å¦ä½è·åkey\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n\nè¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥\n\n
 [ç¹å»è¿éå ç¾¤](https://jq.qq.com/
 ?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ\nå¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼\n\n
 l4_tag = [\'åå\',\'æ©\'] #
 è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡\n l4_key = \'qwertyuiopasdfg\' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n\n\n## ð
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n\n\n##
 æäº¤èªå·±çæå¡å¨ï¼\n\n**æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**\n\n**é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**\n\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n\n
 {\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27031"\n }\n ]\n }\n\n
-***** ð é»è®¤æå¡å¨ *****
-\nç®å **å·²ææ**
+27031"\n },\n {\n "id": 2,\n "version": "æå½¹",\n "ip": "43.248.188.17:
+27032"\n }\n ]\n }\n\n## ð é»è®¤æå¡å¨\nç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸»\n\n|
 æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3\n| äº | anneçµä¿¡æäºæ | ä¸
 | 27\n| åå | ååçå°çª | æè«å¤§é­ç | 14\n| æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
 | 6\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
 æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
 15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.4.6--2022.4.9\n\n - æ¾ç¤ºæ ææ\n -
+æ¶èµ·\n\n### 0.4.7--2022.4.13\n\n - æ°å¢æ¨¡å¼æ¥è¯¢\n -
+åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯\n\n### 0.4.6--2022.4.9\n\n - æ¾ç¤ºæ ææ\n -
 ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼\n -
 é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n- ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--
 2022.4.9\n\n - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n -
 ä¿®å¤raråç¼©åå½åéè¯¯\n - æ´æ°äºtagçåæ°è¯»åæ¹å¼\n -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n -
 ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n -
@@ -152,17 +150,17 @@
 2022.1.3\n\n- ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç \n\n### 0.0.1--
 2022.1.3\n\n- æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾\n\n\n\n## ð
 å¶ä»\n\n+
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr\n+ å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)\n \n\n
-***** ð æè°¢ *****
-\n\n- [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
+[@Agnes4m](https://github.com/Agnes4m)\n \n\n## ð æè°¢\n\n- [nonebot2]
+(https://github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶\n-
+[ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä»\n- [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
 github.com/Agnes4m/VSQ)(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq) -
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q](https://github.com/
 MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å©\n- [ç¾¤èå­¦ä¹ ](https:/
 /github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
 webæ§å¶å°çåæ³æ¥èªäºä»\n- [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè\n- åå -
```

### Comparing `nonebot_plugin_l4d2_server-0.4.6/PKG-INFO` & `nonebot_plugin_l4d2_server-0.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.4.6
+Version: 0.4.7
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -52,17 +52,17 @@
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
+        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
 </a>
@@ -71,76 +71,79 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
-    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 </div>
 
 
 ## 快速使用（env示例）
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
     l4_master = ['1145149191']            # 允许上传地图的qq号
     l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
     l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
     l4_port = ['20715']                   # 服务器端口
     l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
     l4_font = 'simsun.ttc'                # 服务器字体
+    l4_web = True                         # 网页控制台，默认是关闭
 
 
-## 新文档（暂未完成）
 
-[点击这里](https://Agnes4m.github.io/l4d2)
-
-<h2 id="gn">主要功能</h2>
+## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
 
-<h2 id="gn">如何获取key</h2>
+## 如何获取key
 
 为了使得ip不被滥用，我采取这种方式管理。
 
 这并不影响正常使用，如果不需要可以忽略
 
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
         l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
         l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
 
 
-## 🚑  提交自己的服务器？
+## 提交自己的服务器？
 
 **本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
 
 **那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**
 
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
 
         {
         "呆呆": [
                 {
                 "id": 1,
                 "version": "战役",
                 "ip": "43.248.188.17:27031"
+                },
+                {
+                "id": 2,
+                "version": "战役",
+                "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
-<h2 id="ty">🌐 默认服务器</h2>
+## 🌐 默认服务器
 目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
 | 云 | anne电信服云服 | 东 | 27
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
@@ -155,14 +158,19 @@
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.7--2022.4.13
+
+ - 新增模式查询
+ - 列表推导替换套娃循环
+
 ### 0.4.6--2022.4.9
 
  - 显示无效服
  - 优化服务器排序算法（list.sort()天下第一）
  - 默认关闭web端
 
 ### 0.4.5--2022.4.9
@@ -365,16 +373,17 @@
 
 + 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
 + [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
-<h2 id="ty">🌐 感谢</h2>
+## 🌐 感谢
 
+- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架
 - [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
 - [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
 - [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
 - 呆呆 - 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.7 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -36,46 +36,45 @@
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
 # ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
 åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
 æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
 æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
 æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
 æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
-'simsun.ttc' # æå¡å¨å­ä½ ## æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é]
-(https://Agnes4m.github.io/l4d2)
-***** ä¸»è¦åè½ *****
-- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+'simsun.ttc' # æå¡å¨å­ä½ l4_web = True #
+ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­ ## ä¸»è¦åè½ - æ±çæå¡å¨-
+æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)
-***** å¦ä½è·åkey *****
+ranking/index.php) ## å¦ä½è·åkey
 ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
 è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
 (https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
 l4_key = 'qwertyuiopasdfg' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
 æäº¤èªå·±çæå¡å¨ï¼
 **æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
 **é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
-{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
-***** ð é»è®¤æå¡å¨ *****
-ç®å **å·²ææ**
+{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
+{ "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
+é»è®¤æå¡å¨ ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
+0.4.7--2022.4.13 - æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ###
 0.4.6--2022.4.9 - æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort
 ()å¤©ä¸ç¬¬ä¸ï¼ - é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼
 ### 0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯
 - webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
@@ -151,17 +150,17 @@
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
 æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)
-***** ð æè°¢ *****
-- [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
+[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
+github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:
+//github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
 github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
 MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
 github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
 webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
```

