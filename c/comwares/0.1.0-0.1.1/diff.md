# Comparing `tmp/comwares-0.1.0.tar.gz` & `tmp/comwares-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/comwares-0.1.0.tar", last modified: Thu Apr 13 05:36:50 2023, max compression
+gzip compressed data, was "dist/comwares-0.1.1.tar", last modified: Thu Apr 13 08:29:03 2023, max compression
```

## Comparing `comwares-0.1.0.tar` & `comwares-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.137159 comwares-0.1.0/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      259 2023-04-13 05:36:50.136797 comwares-0.1.0/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.0/README.md
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.092084 comwares-0.1.0/comwares.egg-info/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      259 2023-04-13 05:36:50.000000 comwares-0.1.0/comwares.egg-info/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1687 2023-04-13 05:36:50.000000 comwares-0.1.0/comwares.egg-info/SOURCES.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 05:36:50.000000 comwares-0.1.0/comwares.egg-info/dependency_links.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)      232 2023-04-13 05:36:50.000000 comwares-0.1.0/comwares.egg-info/requires.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)       12 2023-04-13 05:36:50.000000 comwares-0.1.0/comwares.egg-info/top_level.txt
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.092817 comwares-0.1.0/middlewares/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      237 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.096533 comwares-0.1.0/middlewares/captcha/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.0/middlewares/captcha/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3945 2020-06-30 03:37:40.000000 comwares-0.1.0/middlewares/captcha/captcha_dev.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1443 2020-06-30 07:43:25.000000 comwares-0.1.0/middlewares/captcha/icredit_captcha.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.0/middlewares/captcha/slider.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.102533 comwares-0.1.0/middlewares/commons/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.0/middlewares/commons/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/commons/logger.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.0/middlewares/commons/md5.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.0/middlewares/commons/path_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.0/middlewares/commons/sorting.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.0/middlewares/commons/string_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.0/middlewares/commons/time_funcs.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.103788 comwares-0.1.0/middlewares/crawler/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.0/middlewares/crawler/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/crawler/user_agents.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.108881 comwares-0.1.0/middlewares/data/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.0/middlewares/data/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/data/loaders.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/data/mongo_to_pg.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.0/middlewares/data/pandas_utils.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/data/pg_utils.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.111600 comwares-0.1.0/middlewares/decorators/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.0/middlewares/decorators/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.0/middlewares/decorators/batchify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.0/middlewares/decorators/time.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.114678 comwares-0.1.0/middlewares/e-mail/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/e-mail/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.0/middlewares/e-mail/check.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/e-mail/exmail.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.0/middlewares/e-mail/send.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.118355 comwares-0.1.0/middlewares/google/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/google/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/google/auth.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3205 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/google/gdrive.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/google/sheets.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      867 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/google/values.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.120491 comwares-0.1.0/middlewares/image/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.0/middlewares/image/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.0/middlewares/image/io.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.0/middlewares/image/visualize.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.123042 comwares-0.1.0/middlewares/pdf/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.0/middlewares/pdf/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.0/middlewares/pdf/b64_transfer.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.0/middlewares/pdf/pdf_analyzer.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.127760 comwares-0.1.0/middlewares/tencent/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.0/middlewares/tencent/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2285 2023-04-13 03:58:55.000000 comwares-0.1.0/middlewares/tencent/cos.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.0/middlewares/tencent/sms.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.0/middlewares/tencent/translate.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.128899 comwares-0.1.0/middlewares/traffic/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.0/middlewares/traffic/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.0/middlewares/traffic/alexacn.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.130078 comwares-0.1.0/middlewares/video/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.0/middlewares/video/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.0/middlewares/video/snap.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 05:36:50.135829 comwares-0.1.0/middlewares/webhooks/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.0/middlewares/webhooks/__init__.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.0/middlewares/webhooks/chanify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.0/middlewares/webhooks/feishu.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.0/middlewares/webhooks/work_weixin.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-13 05:36:50.137279 comwares-0.1.0/setup.cfg
--rw-r--r--   0 kevinzhu   (501) staff       (20)      843 2023-04-13 04:43:44.000000 comwares-0.1.0/setup.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.034278 comwares-0.1.1/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      259 2023-04-13 08:29:03.033664 comwares-0.1.1/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.1/README.md
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:02.997026 comwares-0.1.1/comwares.egg-info/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      259 2023-04-13 08:29:02.000000 comwares-0.1.1/comwares.egg-info/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1687 2023-04-13 08:29:02.000000 comwares-0.1.1/comwares.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 08:29:02.000000 comwares-0.1.1/comwares.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 08:29:02.000000 comwares-0.1.1/comwares.egg-info/requires.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       12 2023-04-13 08:29:02.000000 comwares-0.1.1/comwares.egg-info/top_level.txt
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:02.997393 comwares-0.1.1/middlewares/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      237 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:02.999700 comwares-0.1.1/middlewares/captcha/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.1/middlewares/captcha/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3945 2020-06-30 03:37:40.000000 comwares-0.1.1/middlewares/captcha/captcha_dev.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1443 2020-06-30 07:43:25.000000 comwares-0.1.1/middlewares/captcha/icredit_captcha.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.1/middlewares/captcha/slider.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.004850 comwares-0.1.1/middlewares/commons/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.1/middlewares/commons/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/commons/logger.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.1/middlewares/commons/md5.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.1/middlewares/commons/path_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.1/middlewares/commons/sorting.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.1/middlewares/commons/string_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.1/middlewares/commons/time_funcs.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.005963 comwares-0.1.1/middlewares/crawler/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.1/middlewares/crawler/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/crawler/user_agents.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.010516 comwares-0.1.1/middlewares/data/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.1/middlewares/data/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/data/loaders.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/data/mongo_to_pg.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.1/middlewares/data/pandas_utils.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/data/pg_utils.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.013107 comwares-0.1.1/middlewares/decorators/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.1/middlewares/decorators/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.1/middlewares/decorators/batchify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.1/middlewares/decorators/time.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.016555 comwares-0.1.1/middlewares/e-mail/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/e-mail/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.1/middlewares/e-mail/check.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/e-mail/exmail.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.1/middlewares/e-mail/send.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.020179 comwares-0.1.1/middlewares/google/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/google/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/google/auth.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3205 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/google/gdrive.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/google/sheets.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      867 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/google/values.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.022311 comwares-0.1.1/middlewares/image/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.1/middlewares/image/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.1/middlewares/image/io.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.1/middlewares/image/visualize.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.024659 comwares-0.1.1/middlewares/pdf/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.1/middlewares/pdf/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.1/middlewares/pdf/b64_transfer.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.1/middlewares/pdf/pdf_analyzer.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.028059 comwares-0.1.1/middlewares/tencent/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.1/middlewares/tencent/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 comwares-0.1.1/middlewares/tencent/cos.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.1/middlewares/tencent/sms.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.1/middlewares/tencent/translate.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.029205 comwares-0.1.1/middlewares/traffic/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.1/middlewares/traffic/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.1/middlewares/traffic/alexacn.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.030181 comwares-0.1.1/middlewares/video/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.1/middlewares/video/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.1/middlewares/video/snap.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 08:29:03.032898 comwares-0.1.1/middlewares/webhooks/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.1/middlewares/webhooks/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.1/middlewares/webhooks/chanify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.1/middlewares/webhooks/feishu.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.1/middlewares/webhooks/work_weixin.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-13 08:29:03.034385 comwares-0.1.1/setup.cfg
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      821 2023-04-13 08:26:51.000000 comwares-0.1.1/setup.py
```

### Comparing `comwares-0.1.0/comwares.egg-info/SOURCES.txt` & `comwares-0.1.1/comwares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/captcha/captcha_dev.py` & `comwares-0.1.1/middlewares/captcha/captcha_dev.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/captcha/icredit_captcha.py` & `comwares-0.1.1/middlewares/captcha/icredit_captcha.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/captcha/slider.py` & `comwares-0.1.1/middlewares/captcha/slider.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/commons/logger.py` & `comwares-0.1.1/middlewares/commons/logger.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/commons/path_funcs.py` & `comwares-0.1.1/middlewares/commons/path_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/commons/time_funcs.py` & `comwares-0.1.1/middlewares/commons/time_funcs.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/data/mongo_to_pg.py` & `comwares-0.1.1/middlewares/data/mongo_to_pg.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/data/pandas_utils.py` & `comwares-0.1.1/middlewares/data/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/data/pg_utils.py` & `comwares-0.1.1/middlewares/data/pg_utils.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/decorators/batchify.py` & `comwares-0.1.1/middlewares/decorators/batchify.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/decorators/time.py` & `comwares-0.1.1/middlewares/decorators/time.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/e-mail/check.py` & `comwares-0.1.1/middlewares/e-mail/check.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/e-mail/exmail.py` & `comwares-0.1.1/middlewares/e-mail/exmail.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/e-mail/send.py` & `comwares-0.1.1/middlewares/e-mail/send.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/google/auth.py` & `comwares-0.1.1/middlewares/google/auth.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/google/gdrive.py` & `comwares-0.1.1/middlewares/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/google/values.py` & `comwares-0.1.1/middlewares/google/values.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/image/io.py` & `comwares-0.1.1/middlewares/image/io.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/pdf/b64_transfer.py` & `comwares-0.1.1/middlewares/pdf/b64_transfer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/pdf/pdf_analyzer.py` & `comwares-0.1.1/middlewares/pdf/pdf_analyzer.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/tencent/cos.py` & `comwares-0.1.1/middlewares/tencent/cos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from qcloud_cos.cos_exception import *
-from middlewares.utils import change_to_root_dir
-import sys
-import logging
 import json
 
 
 # logging.basicConfig(level=logging.INFO, stream=sys.stdout)
 
 
 class CosOper:
 
-    def __init__(self, secrets):
-        self._secret_id = secrets['secret_id']
-        self._secret_key = secrets['secret_key']
-        self.region = 'ap-shanghai'
-        self.proxies = None
-        self.token = None
-        self.scheme = 'https'
+    def __init__(self, config: dict):
         self.client = None
         self.buckets = None
-        self.create_cos_client()
+        self.create_cos_client(config)
         self.update_buckets()
 
-    def create_cos_client(self):
-        config = CosConfig(Region=self.region, SecretId=self._secret_id, SecretKey=self._secret_key,
-                           Token=self.token, Scheme=self.scheme, Proxies=self.proxies)
+    def create_cos_client(self, config: dict):
+        keys_must_have = ['secret_id', 'secret_key', 'region']
+        for key in keys_must_have:
+            if key not in config.keys():
+                raise ValueError(f"Must provide '{key}'")
+        config = CosConfig(SecretId=config['secret_id'],
+                           SecretKey=config['secret_key'],
+                           Region=config['region'],
+                           Token=config.get('token'),
+                           Scheme='https',
+                           Proxies=config.get('proxies'))
         client = CosS3Client(config)
         self.client = client
 
     def update_buckets(self):
         res = self.client.list_buckets()
         buckets = res.get('Buckets')
         if isinstance(buckets, dict):
@@ -69,7 +68,22 @@
         pass
 
     def delete_object(self):
         pass
 
     def gen_object_url(self, bucket_name, key):
         return 'https://' + bucket_name + '.' + self.client._conf._endpoint + '/' + key
+
+
+if __name__ == '__main__':
+
+    import os
+    from pprint import pprint
+
+    config = {
+        'secret_id': os.environ.get('TC_SECRET_ID'),
+        'secret_key': os.environ.get('TC_SECRET_KEY'),
+        'region': 'ap-shanghai'
+    }
+
+    cos = CosOper(config)
+    pprint(cos.buckets)
```

### Comparing `comwares-0.1.0/middlewares/tencent/sms.py` & `comwares-0.1.1/middlewares/tencent/sms.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/tencent/translate.py` & `comwares-0.1.1/middlewares/tencent/translate.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/traffic/alexacn.py` & `comwares-0.1.1/middlewares/traffic/alexacn.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/video/snap.py` & `comwares-0.1.1/middlewares/video/snap.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/webhooks/feishu.py` & `comwares-0.1.1/middlewares/webhooks/feishu.py`

 * *Files identical despite different names*

### Comparing `comwares-0.1.0/middlewares/webhooks/work_weixin.py` & `comwares-0.1.1/middlewares/webhooks/work_weixin.py`

 * *Files identical despite different names*

