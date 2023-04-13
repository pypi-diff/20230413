# Comparing `tmp/comwares-0.1.2.tar.gz` & `tmp/comwares-0.1.3.macosx-10.15-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/comwares-0.1.2.tar", last modified: Thu Apr 13 08:32:47 2023, max compression
+gzip compressed data, was "/Users/kevinzhu/PycharmProjects/comwares/dist/comwares-0.1.3.macosx-10.15-x86_64.tar", last modified: Thu Apr 13 18:35:06 2023, max compression
```

## Comparing `comwares-0.1.2.tar` & `comwares-0.1.3.macosx-10.15-x86_64.tar`

### file list

```diff
@@ -1,74 +1,141 @@
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.615708 comwares-0.1.2/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 08:32:47.614752 comwares-0.1.2/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.2/README.md
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.586746 comwares-0.1.2/comwares.egg-info/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 08:32:47.000000 comwares-0.1.2/comwares.egg-info/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1687 2023-04-13 08:32:47.000000 comwares-0.1.2/comwares.egg-info/SOURCES.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 08:32:47.000000 comwares-0.1.2/comwares.egg-info/dependency_links.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 08:32:47.000000 comwares-0.1.2/comwares.egg-info/requires.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)       12 2023-04-13 08:32:47.000000 comwares-0.1.2/comwares.egg-info/top_level.txt
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.587115 comwares-0.1.2/middlewares/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      237 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.589106 comwares-0.1.2/middlewares/captcha/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.2/middlewares/captcha/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3945 2020-06-30 03:37:40.000000 comwares-0.1.2/middlewares/captcha/captcha_dev.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1443 2020-06-30 07:43:25.000000 comwares-0.1.2/middlewares/captcha/icredit_captcha.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.2/middlewares/captcha/slider.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.592996 comwares-0.1.2/middlewares/commons/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.2/middlewares/commons/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/commons/logger.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.2/middlewares/commons/md5.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.2/middlewares/commons/path_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.2/middlewares/commons/sorting.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.2/middlewares/commons/string_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.2/middlewares/commons/time_funcs.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.594001 comwares-0.1.2/middlewares/crawler/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.2/middlewares/crawler/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/crawler/user_agents.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.596774 comwares-0.1.2/middlewares/data/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.2/middlewares/data/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/data/loaders.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/data/mongo_to_pg.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.2/middlewares/data/pandas_utils.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/data/pg_utils.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.598152 comwares-0.1.2/middlewares/decorators/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.2/middlewares/decorators/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.2/middlewares/decorators/batchify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.2/middlewares/decorators/time.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.600132 comwares-0.1.2/middlewares/e-mail/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/e-mail/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.2/middlewares/e-mail/check.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/e-mail/exmail.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.2/middlewares/e-mail/send.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.602365 comwares-0.1.2/middlewares/google/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/google/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/google/auth.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3205 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/google/gdrive.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/google/sheets.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      867 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/google/values.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.603722 comwares-0.1.2/middlewares/image/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.2/middlewares/image/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.2/middlewares/image/io.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.2/middlewares/image/visualize.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.605203 comwares-0.1.2/middlewares/pdf/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.2/middlewares/pdf/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.2/middlewares/pdf/b64_transfer.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.2/middlewares/pdf/pdf_analyzer.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.607542 comwares-0.1.2/middlewares/tencent/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.2/middlewares/tencent/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 comwares-0.1.2/middlewares/tencent/cos.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.2/middlewares/tencent/sms.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.2/middlewares/tencent/translate.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.608969 comwares-0.1.2/middlewares/traffic/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.2/middlewares/traffic/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.2/middlewares/traffic/alexacn.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.610113 comwares-0.1.2/middlewares/video/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.2/middlewares/video/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.2/middlewares/video/snap.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:32:47.613642 comwares-0.1.2/middlewares/webhooks/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.2/middlewares/webhooks/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.2/middlewares/webhooks/chanify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.2/middlewares/webhooks/feishu.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.2/middlewares/webhooks/work_weixin.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-13 08:32:47.615974 comwares-0.1.2/setup.cfg
--rw-r--r--   0 kevinzhu   (501) staff       (20)      897 2023-04-13 08:32:44.000000 comwares-0.1.2/setup.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.050607 ./
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.050893 ./Users/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051162 ./Users/kevinzhu/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051420 ./Users/kevinzhu/PycharmProjects/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051690 ./Users/kevinzhu/PycharmProjects/comwares/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051911 ./Users/kevinzhu/PycharmProjects/comwares/venv/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.052155 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.052432 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.169885 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106647 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      219 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106947 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      392 2023-04-13 18:35:06.106832 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.107274 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.111994 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.107451 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4155 2023-04-13 18:35:06.111888 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/captcha_dev.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1638 2023-04-13 18:35:06.108366 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/icredit_captcha.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     5781 2023-04-13 18:35:06.110341 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/slider.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3942 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/captcha_dev.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1440 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/icredit_captcha.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/slider.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.085270 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.090264 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.085970 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      998 2023-04-13 18:35:06.086730 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      719 2023-04-13 18:35:06.088943 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/md5.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      931 2023-04-13 18:35:06.090048 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/path_funcs.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      796 2023-04-13 18:35:06.085450 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/sorting.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      502 2023-04-13 18:35:06.088275 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/string_funcs.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1964 2023-04-13 18:35:06.087639 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/time_funcs.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/logger.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/md5.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/path_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/sorting.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/string_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/time_funcs.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.097467 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.098488 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.097661 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      384 2023-04-13 18:35:06.098371 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/user_agents.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/user_agents.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.122950 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.126494 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      190 2023-04-13 18:35:06.125169 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      428 2023-04-13 18:35:06.124674 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/loaders.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2811 2023-04-13 18:35:06.126384 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/mongo_to_pg.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      972 2023-04-13 18:35:06.123124 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/pandas_utils.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2030 2023-04-13 18:35:06.124093 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/pg_utils.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/loaders.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/mongo_to_pg.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pandas_utils.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pg_utils.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.083194 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.084806 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      196 2023-04-13 18:35:06.084701 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1433 2023-04-13 18:35:06.084209 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/batchify.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      977 2023-04-13 18:35:06.083363 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/time.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/batchify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/time.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.099711 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.103181 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      192 2023-04-13 18:35:06.101495 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2527 2023-04-13 18:35:06.099931 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/check.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1769 2023-04-13 18:35:06.103040 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/exmail.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1181 2023-04-13 18:35:06.100834 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/send.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/check.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/exmail.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/send.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.091226 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.097076 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      192 2023-04-13 18:35:06.094908 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1138 2023-04-13 18:35:06.091580 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/auth.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3012 2023-04-13 18:35:06.096953 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/gdrive.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      190 2023-04-13 18:35:06.094074 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/sheets.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      984 2023-04-13 18:35:06.093093 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/values.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/auth.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3199 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/gdrive.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/sheets.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      861 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/values.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.112495 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.113942 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      191 2023-04-13 18:35:06.113245 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      911 2023-04-13 18:35:06.112663 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/io.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      246 2023-04-13 18:35:06.113813 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/visualize.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/io.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/visualize.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.103764 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106224 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      189 2023-04-13 18:35:06.104099 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3940 2023-04-13 18:35:06.104914 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/b64_transfer.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1457 2023-04-13 18:35:06.106096 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/pdf_analyzer.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/b64_transfer.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/pdf_analyzer.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.114606 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.117410 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.116483 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3082 2023-04-13 18:35:06.115980 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/cos.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1666 2023-04-13 18:35:06.117308 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/sms.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1410 2023-04-13 18:35:06.114796 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/cos.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/sms.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/translate.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.079586 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.081196 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.079784 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2201 2023-04-13 18:35:06.081043 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/alexacn.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/alexacn.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.081908 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.082700 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      191 2023-04-13 18:35:06.082593 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1595 2023-04-13 18:35:06.082089 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/snap.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/snap.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.119284 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.122414 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      194 2023-04-13 18:35:06.120181 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      406 2023-04-13 18:35:06.120794 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/chanify.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4061 2023-04-13 18:35:06.122307 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/feishu.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4888 2023-04-13 18:35:06.119530 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/work_weixin.cpython-39.pyc
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/chanify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/feishu.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/work_weixin.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.171711 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:35:06.155256 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1540 2023-04-13 18:35:06.169425 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 18:35:06.155670 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 18:35:06.156164 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/requires.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        9 2023-04-13 18:35:06.156406 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/top_level.txt
```

### Comparing `comwares-0.1.2/comwares.egg-info/SOURCES.txt` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 README.md
 setup.py
+comwares/__init__.py
 comwares.egg-info/PKG-INFO
 comwares.egg-info/SOURCES.txt
 comwares.egg-info/dependency_links.txt
 comwares.egg-info/requires.txt
 comwares.egg-info/top_level.txt
-middlewares/__init__.py
-middlewares/captcha/__init__.py
-middlewares/captcha/captcha_dev.py
-middlewares/captcha/icredit_captcha.py
-middlewares/captcha/slider.py
-middlewares/commons/__init__.py
-middlewares/commons/logger.py
-middlewares/commons/md5.py
-middlewares/commons/path_funcs.py
-middlewares/commons/sorting.py
-middlewares/commons/string_funcs.py
-middlewares/commons/time_funcs.py
-middlewares/crawler/__init__.py
-middlewares/crawler/user_agents.py
-middlewares/data/__init__.py
-middlewares/data/loaders.py
-middlewares/data/mongo_to_pg.py
-middlewares/data/pandas_utils.py
-middlewares/data/pg_utils.py
-middlewares/decorators/__init__.py
-middlewares/decorators/batchify.py
-middlewares/decorators/time.py
-middlewares/e-mail/__init__.py
-middlewares/e-mail/check.py
-middlewares/e-mail/exmail.py
-middlewares/e-mail/send.py
-middlewares/google/__init__.py
-middlewares/google/auth.py
-middlewares/google/gdrive.py
-middlewares/google/sheets.py
-middlewares/google/values.py
-middlewares/image/__init__.py
-middlewares/image/io.py
-middlewares/image/visualize.py
-middlewares/pdf/__init__.py
-middlewares/pdf/b64_transfer.py
-middlewares/pdf/pdf_analyzer.py
-middlewares/tencent/__init__.py
-middlewares/tencent/cos.py
-middlewares/tencent/sms.py
-middlewares/tencent/translate.py
-middlewares/traffic/__init__.py
-middlewares/traffic/alexacn.py
-middlewares/video/__init__.py
-middlewares/video/snap.py
-middlewares/webhooks/__init__.py
-middlewares/webhooks/chanify.py
-middlewares/webhooks/feishu.py
-middlewares/webhooks/work_weixin.py
+comwares/captcha/__init__.py
+comwares/captcha/captcha_dev.py
+comwares/captcha/icredit_captcha.py
+comwares/captcha/slider.py
+comwares/commons/__init__.py
+comwares/commons/logger.py
+comwares/commons/md5.py
+comwares/commons/path_funcs.py
+comwares/commons/sorting.py
+comwares/commons/string_funcs.py
+comwares/commons/time_funcs.py
+comwares/crawler/__init__.py
+comwares/crawler/user_agents.py
+comwares/data/__init__.py
+comwares/data/loaders.py
+comwares/data/mongo_to_pg.py
+comwares/data/pandas_utils.py
+comwares/data/pg_utils.py
+comwares/decorators/__init__.py
+comwares/decorators/batchify.py
+comwares/decorators/time.py
+comwares/e-mail/__init__.py
+comwares/e-mail/check.py
+comwares/e-mail/exmail.py
+comwares/e-mail/send.py
+comwares/google/__init__.py
+comwares/google/auth.py
+comwares/google/gdrive.py
+comwares/google/sheets.py
+comwares/google/values.py
+comwares/image/__init__.py
+comwares/image/io.py
+comwares/image/visualize.py
+comwares/pdf/__init__.py
+comwares/pdf/b64_transfer.py
+comwares/pdf/pdf_analyzer.py
+comwares/tencent/__init__.py
+comwares/tencent/cos.py
+comwares/tencent/sms.py
+comwares/tencent/translate.py
+comwares/traffic/__init__.py
+comwares/traffic/alexacn.py
+comwares/video/__init__.py
+comwares/video/snap.py
+comwares/webhooks/__init__.py
+comwares/webhooks/chanify.py
+comwares/webhooks/feishu.py
+comwares/webhooks/work_weixin.py
```

### Comparing `comwares-0.1.2/middlewares/captcha/captcha_dev.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/captcha_dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cv2.cv2 as cv2
 import numpy as np
 from matplotlib import pyplot as plt
-from middlewares import change_to_root_dir, recognize_captcha_in_line
+from comwares import change_to_root_dir, recognize_captcha_in_line
 import time
 import os
 from PIL import Image
 
 
 def plot_in_grey_scale(img):
     plt.imshow(img, cmap='gray', interpolation='none')
```

### Comparing `comwares-0.1.2/middlewares/captcha/icredit_captcha.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/icredit_captcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import urllib.parse as parse
 import base64
 import os
-from middlewares import change_to_root_dir
+from comwares import change_to_root_dir
 from PIL import Image
 
 
 def verify_captcha(img_filename, appcode=None):
     endpoint = 'https://codevirify.market.alicloudapi.com/icredit_ai_image/verify_code/v1'
     appcode = appcode or os.environ.get('icredit_appcode')
     if appcode is None:
```

### Comparing `comwares-0.1.2/middlewares/captcha/slider.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/slider.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/commons/logger.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/logger.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/commons/path_funcs.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/path_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/commons/time_funcs.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/time_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/data/mongo_to_pg.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/mongo_to_pg.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/data/pandas_utils.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/data/pg_utils.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pg_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/decorators/batchify.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/batchify.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/decorators/time.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/time.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/e-mail/check.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/check.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/e-mail/exmail.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/exmail.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/e-mail/send.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/send.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/google/auth.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/auth.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/google/gdrive.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/gdrive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os.path
 from googleapiclient.http import MediaIoBaseDownload
 from googleapiclient.discovery import build
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 import os
 import io
-from middlewares.google.auth import update_token
+from comwares.google.auth import update_token
 
 
-def build_service(service_type, version, path='middlewares/google/creds/'):
+def build_service(service_type, version, path='comwares/google/creds/'):
     os.environ['HTTPS_PROXY'] = 'http://127.0.0.1:1087'
     creds = None
     if os.path.exists(path + 'token.pickle'):
         with open(path + 'token.pickle', 'rb') as token:
             creds = pickle.load(token)
     if not creds or not creds.valid:
         print('No creds found or creds is not valid, update oauth token first.')
```

### Comparing `comwares-0.1.2/middlewares/google/values.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/values.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from middlewares.google.auth import *
+from comwares.google.auth import *
 from googleapiclient.discovery import build
 import os
 
 
-def get_sheet_values(sheet_id, range, path='middlewares/google/creds/'):
+def get_sheet_values(sheet_id, range, path='comwares/google/creds/'):
     if os.path.exists(path + 'token.pickle'):
         with open(path + 'token.pickle', 'rb') as token:
             creds = pickle.load(token)
         if not creds.valid:
             creds = update_token(path=path)
     else:
         creds = update_token(path=path)
```

### Comparing `comwares-0.1.2/middlewares/image/io.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/io.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/pdf/b64_transfer.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/b64_transfer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/pdf/pdf_analyzer.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/pdf_analyzer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/tencent/cos.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/cos.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/tencent/sms.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/sms.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/tencent/translate.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/translate.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/traffic/alexacn.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/alexacn.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/video/snap.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/snap.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/webhooks/feishu.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/feishu.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.2/middlewares/webhooks/work_weixin.py` & `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/work_weixin.py`

 * *Files identical despite different names*

