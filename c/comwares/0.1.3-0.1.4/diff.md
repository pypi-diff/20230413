# Comparing `tmp/comwares-0.1.3.macosx-10.15-x86_64.tar.gz` & `tmp/comwares-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kevinzhu/PycharmProjects/comwares/dist/comwares-0.1.3.macosx-10.15-x86_64.tar", last modified: Thu Apr 13 18:35:06 2023, max compression
+gzip compressed data, was "dist/comwares-0.1.4.tar", last modified: Thu Apr 13 18:36:35 2023, max compression
```

## Comparing `comwares-0.1.3.macosx-10.15-x86_64.tar` & `comwares-0.1.4.tar`

### file list

```diff
@@ -1,141 +1,74 @@
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.050607 ./
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.050893 ./Users/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051162 ./Users/kevinzhu/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051420 ./Users/kevinzhu/PycharmProjects/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051690 ./Users/kevinzhu/PycharmProjects/comwares/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.051911 ./Users/kevinzhu/PycharmProjects/comwares/venv/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.052155 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.052432 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.169885 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106647 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      219 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106947 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      392 2023-04-13 18:35:06.106832 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.107274 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.111994 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.107451 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4155 2023-04-13 18:35:06.111888 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/captcha_dev.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1638 2023-04-13 18:35:06.108366 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/icredit_captcha.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     5781 2023-04-13 18:35:06.110341 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/__pycache__/slider.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3942 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/captcha_dev.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1440 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/icredit_captcha.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/slider.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.085270 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.090264 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.085970 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      998 2023-04-13 18:35:06.086730 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      719 2023-04-13 18:35:06.088943 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/md5.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      931 2023-04-13 18:35:06.090048 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/path_funcs.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      796 2023-04-13 18:35:06.085450 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/sorting.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      502 2023-04-13 18:35:06.088275 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/string_funcs.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1964 2023-04-13 18:35:06.087639 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/__pycache__/time_funcs.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/logger.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/md5.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/path_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/sorting.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/string_funcs.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/time_funcs.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.097467 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.098488 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.097661 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      384 2023-04-13 18:35:06.098371 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/__pycache__/user_agents.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/crawler/user_agents.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.122950 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.126494 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      190 2023-04-13 18:35:06.125169 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      428 2023-04-13 18:35:06.124674 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/loaders.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2811 2023-04-13 18:35:06.126384 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/mongo_to_pg.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      972 2023-04-13 18:35:06.123124 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/pandas_utils.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2030 2023-04-13 18:35:06.124093 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/__pycache__/pg_utils.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/loaders.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/mongo_to_pg.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pandas_utils.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pg_utils.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.083194 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.084806 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      196 2023-04-13 18:35:06.084701 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1433 2023-04-13 18:35:06.084209 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/batchify.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      977 2023-04-13 18:35:06.083363 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/__pycache__/time.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/batchify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/time.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.099711 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.103181 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      192 2023-04-13 18:35:06.101495 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2527 2023-04-13 18:35:06.099931 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/check.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1769 2023-04-13 18:35:06.103040 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/exmail.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1181 2023-04-13 18:35:06.100834 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/__pycache__/send.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/check.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/exmail.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/send.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.091226 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.097076 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      192 2023-04-13 18:35:06.094908 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1138 2023-04-13 18:35:06.091580 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3012 2023-04-13 18:35:06.096953 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/gdrive.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      190 2023-04-13 18:35:06.094074 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/sheets.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      984 2023-04-13 18:35:06.093093 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/__pycache__/values.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/auth.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3199 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/gdrive.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/sheets.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)      861 2023-04-13 17:21:15.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/values.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.112495 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.113942 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      191 2023-04-13 18:35:06.113245 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      911 2023-04-13 18:35:06.112663 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/io.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      246 2023-04-13 18:35:06.113813 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/__pycache__/visualize.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/io.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/visualize.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.103764 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.106224 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      189 2023-04-13 18:35:06.104099 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3940 2023-04-13 18:35:06.104914 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/b64_transfer.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1457 2023-04-13 18:35:06.106096 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/pdf_analyzer.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/b64_transfer.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/pdf_analyzer.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.114606 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.117410 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.116483 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     3082 2023-04-13 18:35:06.115980 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/cos.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1666 2023-04-13 18:35:06.117308 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/sms.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1410 2023-04-13 18:35:06.114796 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/cos.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/sms.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/translate.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.079586 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.081196 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      193 2023-04-13 18:35:06.079784 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2201 2023-04-13 18:35:06.081043 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/__pycache__/alexacn.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/alexacn.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.081908 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.082700 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      191 2023-04-13 18:35:06.082593 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1595 2023-04-13 18:35:06.082089 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/__pycache__/snap.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/snap.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.119284 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/
--rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__init__.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.122414 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      194 2023-04-13 18:35:06.120181 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      406 2023-04-13 18:35:06.120794 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/chanify.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4061 2023-04-13 18:35:06.122307 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/feishu.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4888 2023-04-13 18:35:06.119530 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/__pycache__/work_weixin.cpython-39.pyc
--rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/chanify.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/feishu.py
--rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/work_weixin.py
-drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:35:06.171711 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/
--rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:35:06.155256 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 kevinzhu   (501) staff       (20)     1540 2023-04-13 18:35:06.169425 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 18:35:06.155670 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 18:35:06.156164 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/requires.txt
--rw-r--r--   0 kevinzhu   (501) staff       (20)        9 2023-04-13 18:35:06.156406 ./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.520939 comwares-0.1.4/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:36:35.520358 comwares-0.1.4/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      244 2023-04-13 04:53:05.000000 comwares-0.1.4/README.md
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.485500 comwares-0.1.4/comwares/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      219 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/__init__.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.490157 comwares-0.1.4/comwares/captcha/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-06-30 06:17:49.000000 comwares-0.1.4/comwares/captcha/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3942 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/captcha/captcha_dev.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1440 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/captcha/icredit_captcha.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     7815 2021-03-25 02:37:08.000000 comwares-0.1.4/comwares/captcha/slider.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.495625 comwares-0.1.4/comwares/commons/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:09:53.000000 comwares-0.1.4/comwares/commons/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1088 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/commons/logger.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      408 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/md5.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      516 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/path_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      444 2022-11-25 08:03:36.000000 comwares-0.1.4/comwares/commons/sorting.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      278 2022-10-20 06:41:29.000000 comwares-0.1.4/comwares/commons/string_funcs.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1711 2023-04-13 04:28:04.000000 comwares-0.1.4/comwares/commons/time_funcs.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.496753 comwares-0.1.4/comwares/crawler/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:11:49.000000 comwares-0.1.4/comwares/crawler/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      208 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/crawler/user_agents.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.500622 comwares-0.1.4/comwares/data/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-12 22:12:47.000000 comwares-0.1.4/comwares/data/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      143 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/data/loaders.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2831 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/data/mongo_to_pg.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      771 2023-04-13 04:53:05.000000 comwares-0.1.4/comwares/data/pandas_utils.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1794 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/data/pg_utils.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.503050 comwares-0.1.4/comwares/decorators/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-04-26 10:04:51.000000 comwares-0.1.4/comwares/decorators/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1270 2021-08-07 17:39:01.000000 comwares-0.1.4/comwares/decorators/batchify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      623 2021-04-26 10:04:51.000000 comwares-0.1.4/comwares/decorators/time.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.505889 comwares-0.1.4/comwares/e-mail/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/e-mail/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3557 2023-04-13 01:16:42.000000 comwares-0.1.4/comwares/e-mail/check.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1586 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/e-mail/exmail.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1107 2023-04-12 22:51:38.000000 comwares-0.1.4/comwares/e-mail/send.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.508669 comwares-0.1.4/comwares/google/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1097 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/auth.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     3199 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/google/gdrive.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/google/sheets.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      861 2023-04-13 17:21:15.000000 comwares-0.1.4/comwares/google/values.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.510347 comwares-0.1.4/comwares/image/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-07-13 11:02:07.000000 comwares-0.1.4/comwares/image/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      613 2023-04-12 22:30:10.000000 comwares-0.1.4/comwares/image/io.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       52 2022-01-09 12:26:53.000000 comwares-0.1.4/comwares/image/visualize.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.512593 comwares-0.1.4/comwares/pdf/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-11 06:05:59.000000 comwares-0.1.4/comwares/pdf/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4293 2023-02-05 18:23:25.000000 comwares-0.1.4/comwares/pdf/b64_transfer.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1650 2023-04-13 04:12:03.000000 comwares-0.1.4/comwares/pdf/pdf_analyzer.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.515188 comwares-0.1.4/comwares/tencent/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2020-12-08 07:56:30.000000 comwares-0.1.4/comwares/tencent/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2638 2023-04-13 07:51:54.000000 comwares-0.1.4/comwares/tencent/cos.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     6431 2023-04-13 04:10:06.000000 comwares-0.1.4/comwares/tencent/sms.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2023-01-16 08:01:41.000000 comwares-0.1.4/comwares/tencent/translate.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.516317 comwares-0.1.4/comwares/traffic/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-03-26 02:45:31.000000 comwares-0.1.4/comwares/traffic/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     2129 2021-09-22 09:21:25.000000 comwares-0.1.4/comwares/traffic/alexacn.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.517251 comwares-0.1.4/comwares/video/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2023-04-13 04:11:00.000000 comwares-0.1.4/comwares/video/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1786 2022-01-10 15:36:27.000000 comwares-0.1.4/comwares/video/snap.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.519588 comwares-0.1.4/comwares/webhooks/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        0 2021-09-12 01:50:08.000000 comwares-0.1.4/comwares/webhooks/__init__.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      188 2021-09-12 01:59:13.000000 comwares-0.1.4/comwares/webhooks/chanify.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     4714 2022-01-23 05:01:17.000000 comwares-0.1.4/comwares/webhooks/feishu.py
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     5395 2022-10-30 04:17:29.000000 comwares-0.1.4/comwares/webhooks/work_weixin.py
+drwxr-xr-x   0 kevinzhu   (501) staff       (20)        0 2023-04-13 18:36:35.487539 comwares-0.1.4/comwares.egg-info/
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      325 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/PKG-INFO
+-rw-r--r--   0 kevinzhu   (501) staff       (20)     1540 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        1 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      221 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/requires.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)        9 2023-04-13 18:36:35.000000 comwares-0.1.4/comwares.egg-info/top_level.txt
+-rw-r--r--   0 kevinzhu   (501) staff       (20)       38 2023-04-13 18:36:35.521044 comwares-0.1.4/setup.cfg
+-rw-r--r--   0 kevinzhu   (501) staff       (20)      897 2023-04-13 18:36:05.000000 comwares-0.1.4/setup.py
```

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/captcha_dev.py` & `comwares-0.1.4/comwares/captcha/captcha_dev.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/icredit_captcha.py` & `comwares-0.1.4/comwares/captcha/icredit_captcha.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/captcha/slider.py` & `comwares-0.1.4/comwares/captcha/slider.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/logger.py` & `comwares-0.1.4/comwares/commons/logger.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/path_funcs.py` & `comwares-0.1.4/comwares/commons/path_funcs.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/commons/time_funcs.py` & `comwares-0.1.4/comwares/commons/time_funcs.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/mongo_to_pg.py` & `comwares-0.1.4/comwares/data/mongo_to_pg.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pandas_utils.py` & `comwares-0.1.4/comwares/data/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/data/pg_utils.py` & `comwares-0.1.4/comwares/data/pg_utils.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/batchify.py` & `comwares-0.1.4/comwares/decorators/batchify.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/decorators/time.py` & `comwares-0.1.4/comwares/decorators/time.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/check.py` & `comwares-0.1.4/comwares/e-mail/check.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/exmail.py` & `comwares-0.1.4/comwares/e-mail/exmail.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/e-mail/send.py` & `comwares-0.1.4/comwares/e-mail/send.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/auth.py` & `comwares-0.1.4/comwares/google/auth.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/gdrive.py` & `comwares-0.1.4/comwares/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/google/values.py` & `comwares-0.1.4/comwares/google/values.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/image/io.py` & `comwares-0.1.4/comwares/image/io.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/__pycache__/b64_transfer.cpython-39.pyc` & `comwares-0.1.4/comwares/pdf/b64_transfer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,247 +1,269 @@
-00000000: 610d 0d0a 0000 0000 1df4 df63 c510 0000  a..........c....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
-00000030: 6401 6c00 5a00 6407 6403 6404 8401 5a01  d.l.Z.d.d.d...Z.
-00000040: 6502 6405 6b02 7226 6406 5a03 6501 6503  e.d.k.r&d.Z.e.e.
-00000050: 8301 0100 6401 5300 2908 e900 0000 004e  ....d.S.)......N
-00000060: fa07 746d 702e 7064 6663 0200 0000 0000  ..tmp.pdfc......
-00000070: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-00000080: 0000 734c 0000 0074 007c 0164 0183 028f  ..sL...t.|.d....
-00000090: 2e7d 027c 02a0 0174 02a0 037c 00a1 01a1  .}.|...t...|....
-000000a0: 0101 0074 0464 027c 019b 009d 0283 0101  ...t.d.|........
-000000b0: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-000000c0: 0073 3e30 0001 0001 0001 0059 0001 0064  .s>0.......Y...d
-000000d0: 0053 0029 034e da02 7762 7a19 5361 7665  .S.).N..wbz.Save
-000000e0: 6420 6261 7365 3634 2063 6f6e 7465 6e74  d base64 content
-000000f0: 2074 6f3a 2029 05da 046f 7065 6eda 0577   to: )...open..w
-00000100: 7269 7465 da06 6261 7365 3634 da09 6236  rite..base64..b6
-00000110: 3464 6563 6f64 65da 0570 7269 6e74 2903  4decode..print).
-00000120: 5a0a 6236 345f 7374 7269 6e67 da08 6669  Z.b64_string..fi
-00000130: 6c65 6e61 6d65 da01 66a9 0072 0b00 0000  lename..f..r....
-00000140: fa66 2f55 7365 7273 2f6b 6576 696e 7a68  .f/Users/kevinzh
-00000150: 752f 5079 6368 6172 6d50 726f 6a65 6374  u/PycharmProject
-00000160: 732f 636f 6d77 6172 6573 2f76 656e 762f  s/comwares/venv/
-00000170: 6c69 622f 7079 7468 6f6e 332e 392f 7369  lib/python3.9/si
-00000180: 7465 2d70 6163 6b61 6765 732f 636f 6d77  te-packages/comw
-00000190: 6172 6573 2f70 6466 2f62 3634 5f74 7261  ares/pdf/b64_tra
-000001a0: 6e73 6665 722e 7079 da16 7361 7665 5f62  nsfer.py..save_b
-000001b0: 3634 5f73 7472 696e 675f 6173 5f70 6466  64_string_as_pdf
-000001c0: 0400 0000 7306 0000 0000 010c 0110 0172  ....s..........r
-000001d0: 0d00 0000 da08 5f5f 6d61 696e 5f5f 612c  ......__main__a,
-000001e0: 0d00 004a 5642 4552 6930 784c 6a51 4b4a  ...JVBERi0xLjQKJ
-000001f0: 654c 6a7a 394d 4b4e 4341 7749 4739 6961  eLjz9MKNCAwIG9ia
-00000200: 676f 3850 4339 4d5a 5735 6e64 4767 674e  go8PC9MZW5ndGggN
-00000210: 6a49 794c 305a 7062 4852 6c63 6939 4762  jIyL0ZpbHRlci9Gb
-00000220: 4746 305a 5552 6c59 3239 6b5a 5434 2b63  GF0ZURlY29kZT4+c
-00000230: 3352 795a 5746 7443 6e69 636e 5a58 4e62  3RyZWFtCnicnZXNb
-00000240: 7470 4145 4d64 5850 666f 7052 756f 6c71  tpAEMdXPfopRuolq
-00000250: 5a72 4e37 7670 6a31 3977 6f48 7847 7063  ZrN7vpj19woHxGpc
-00000260: 424b 386c 4354 4b78 5149 4858 4945 4a42  BK8lCTKxQIHXIEJB
-00000270: 7052 6a48 3642 5348 3747 5030 5675 6c7a  pRjH6BSH7GP0Vulz
-00000280: 686f 4843 4348 426a 6132 5664 3262 482f  hoHCCHBja2Vd2bH/
-00000290: 3939 346d 4631 6d31 6777 3439 5878 6765  994mF1m1gw49Xxge
-000002a0: 4f4e 4567 6d31 5433 7766 4f66 6572 3630  ONEgm1T3wfOfer60
-000002b0: 4a2f 4136 6655 3968 2f6f 5572 7177 7261  J/A6fU9h/oUrqwra
-000002c0: 325a 3930 5259 446f 577a 7167 6835 5944  2Z90RYDoWzqgh5YD
-000002d0: 5a30 377a 5242 776a 6974 6e4f 4d63 5176  Z07zRBwjitnOMcQv
-000002e0: 7049 4472 696a 6a49 4679 5032 6737 6f69  pIDrijjIFyP2g7oi
-000002f0: 5858 6152 4238 4466 592f 684f 724d 5974  XXaRB8DfY/hOrMYt
-00000300: 6330 466a 7862 4c58 2b69 6346 5a4e 7361  c0FjxbLX+icFZNsa
-00000310: 4232 4663 546f 4150 6130 6336 2b2f 6f48  B2FcToAPa0c6+/oH
-00000320: 6549 7762 7943 4259 7a79 4344 324d 6468  eIwbyCBYzyCD2Mdh
-00000330: 7a4c 7868 5057 3371 6675 4a51 6258 6467  zLxhPW3qfuJQbXdg
-00000340: 4172 306f 6952 397a 4a4c 6861 4148 744b  Ar0oiR9zJLhaAHtK
-00000350: 4f76 4830 524b 2b52 6f76 524f 4937 5476  OvH0RK+RovROI7Tv
-00000360: 626e 7355 4732 336f 4c34 4e71 3962 7279  bnsUG23oL4Nq9bry
-00000370: 4249 4b65 7646 3841 5466 545a 5471 457a  BIKevF8ATfTZTqEz
-00000380: 7141 4d51 4869 6c41 4c57 5776 6b46 434c  qAMQHilALWWvkFCL
-00000390: 526f 6e44 3945 6953 3649 7932 6c79 5730  RonD9EiS6Iy2lyW0
-000003a0: 6735 3156 5a74 5331 6170 6c52 4a6b 716c  g51VZtS1aplRJkql
-000003b0: 2f42 464e 3941 646b 334d 3361 4f6c 4748  /BFN9Adk3M3aOlGH
-000003c0: 584a 4b2b 4a37 666e 776e 7134 344e 7a30  XJK+J7fnwnq44Nz0
-000003d0: 384e 4641 3669 7442 6843 6568 3532 2b4e  8NFA6itBhCeh52+N
-000003e0: 3475 6d77 7830 6d42 4f4f 434d 3778 7137  4umwx0mBOOCM7xq7
-000003f0: 3848 4c2f 494e 6454 6e33 316a 4836 5963  8HL/INdTn31jH6Yc
-00000400: 6b44 596f 3767 7a6c 554d 6c66 3058 334e  kDYo7gzlUMlf0X3N
-00000410: 6e6e 412b 766c 4332 485a 4a53 5674 5277  nnA+vlC2HZJSVtRw
-00000420: 5665 6972 3268 656a 715a 706a 4b70 3352  Veir2hejqZpjKp3R
-00000430: 3637 4437 3435 4275 7336 4a53 626f 6377  67D745Bus6JSbocw
-00000440: 4d65 4f63 6a46 7a50 414b 4b59 6f68 6441  MeOcjFzPAKKYohdA
-00000450: 4f6d 5367 4c53 494a 6731 534a 3042 436e  OmSgLSIJg1SJ0BCn
-00000460: 4656 7a4b 3051 4c66 767a 3639 7266 6b74  FVzK0QLfvz69rfkt
-00000470: 7768 7a7a 4468 7166 6467 4964 4f32 676d  whzzDhqfdgIdO2gm
-00000480: 6968 3853 396f 3472 6c48 6343 5376 2f49  ih8S9o4rlHcCSv/I
-00000490: 3632 6f63 702b 5535 5937 774a 636e 496c  62ocp+U5Y7wJcnIl
-000004a0: 417a 496b 7654 4a41 7155 4445 7045 4a69  AzIkvTJAqUDEpEJi
-000004b0: 5846 5777 5645 6a49 3178 5079 427a 584a  XFWwVEjI1xPyBzXJ
-000004c0: 7267 7952 3938 5550 576b 526c 614c 662b  rgyR98UPWkRlaLf+
-000004d0: 4469 4233 7365 6676 2f73 6667 6a2f 6b4d  DiB3sefv/sfgj/kM
-000004e0: 376e 5969 636a 5867 302b 456d 6e73 7238  7nYicjXg0+Emnsr8
-000004f0: 5530 6255 386d 5564 4c46 4473 6265 6f6b  U0bU8mUdLFDsbeok
-00000500: 2f63 6773 7746 336e 6852 5579 6349 6357  /cgswF3nhRUycIcW
-00000510: 2b48 4c53 4c50 7a2b 535a 795a 6535 4763  +HLSLPz+SZyZe5Gc
-00000520: 7370 7449 7949 6445 376b 7973 536c 6653  sptIyIdE7kysSlfS
-00000530: 4b49 4739 7a61 424b 334d 642b 4561 6468  KIG9zaBK3Md+Eadh
-00000540: 5642 6d79 7771 3537 6862 3065 6339 4c33  VBmywq57hb0ec9L3
-00000550: 5132 3350 3330 4e58 5266 424e 6639 6951  Q23P30NXRfBNf9iQ
-00000560: 6b71 7162 436a 514a 3855 7a69 7848 2f44  kqqbCjQJ8UzixH/D
-00000570: 3574 5561 596b 4b5a 5735 6b63 3352 795a  5tUaYkKZW5kc3RyZ
-00000580: 5746 7443 6d56 755a 4739 6961 676f 3249  WFtCmVuZG9iago2I
-00000590: 4441 6762 324a 7143 6a77 384c 3152 3563  DAgb2JqCjw8L1R5c
-000005a0: 4755 7655 4746 6e5a 5339 4e5a 5752 7059  GUvUGFnZS9NZWRpY
-000005b0: 554a 7665 4673 7749 4441 674d 6a67 7a4c  UJveFswIDAgMjgzL
-000005c0: 6a55 674d 6a67 7a4c 6a56 644c 314a 6c63  jUgMjgzLjVdL1Jlc
-000005d0: 3239 3163 6d4e 6c63 7a77 384c 305a 7662  291cmNlczw8L0Zvb
-000005e0: 6e51 3850 4339 474d 5341 7849 4441 6755  nQ8PC9GMSAxIDAgU
-000005f0: 6939 474d 6941 7a49 4441 6755 6a34 2b4c  i9GMiAzIDAgUj4+L
-00000600: 3168 5059 6d70 6c59 3351 3850 4339 595a  1hPYmplY3Q8PC9YZ
-00000610: 6a45 674d 6941 7749 4649 2b50 6a34 2b4c  jEgMiAwIFI+Pj4+L
-00000620: 304e 7662 6e52 6c62 6e52 7a49 4451 674d  0NvbnRlbnRzIDQgM
-00000630: 4342 534c 3142 6863 6d56 7564 4341 3149  CBSL1BhcmVudCA1I
-00000640: 4441 6755 6a34 2b43 6d56 755a 4739 6961  DAgUj4+CmVuZG9ia
-00000650: 676f 7849 4441 6762 324a 7143 6a77 384c  goxIDAgb2JqCjw8L
-00000660: 3152 3563 4755 7652 6d39 7564 4339 5464  1R5cGUvRm9udC9Td
-00000670: 574a 3065 5842 6c4c 3152 3563 4755 784c  WJ0eXBlL1R5cGUxL
-00000680: 304a 6863 3256 4762 3235 304c 3068 6c62  0Jhc2VGb250L0hlb
-00000690: 485a 6c64 476c 6a59 5339 4662 6d4e 765a  HZldGljYS9FbmNvZ
-000006a0: 476c 755a 7939 5861 5735 4262 6e4e 7052  GluZy9XaW5BbnNpR
-000006b0: 5735 6a62 3252 7062 6d63 2b50 6770 6c62  W5jb2Rpbmc+Pgplb
-000006c0: 6d52 7659 6d6f 4b4e 7941 7749 4739 6961  mRvYmoKNyAwIG9ia
-000006d0: 676f 3850 4339 5565 5842 6c4c 305a 7662  go8PC9UeXBlL0Zvb
-000006e0: 6e52 455a 584e 6a63 6d6c 7764 4739 794c  nREZXNjcmlwdG9yL
-000006f0: 3046 7a59 3256 7564 4341 344f 4441 7651  0FzY2VudCA4ODAvQ
-00000700: 3246 7753 4756 705a 3268 3049 4467 344d  2FwSGVpZ2h0IDg4M
-00000710: 4339 455a 584e 6a5a 5735 3049 4330 784d  C9EZXNjZW50IC0xM
-00000720: 6a41 7652 6d78 685a 334d 674e 6939 4762  jAvRmxhZ3MgNi9Gb
-00000730: 3235 3051 6b4a 7665 4342 624c 5449 3149  250QkJveCBbLTI1I
-00000740: 4330 794e 5451 674d 5441 774d 4341 344f  C0yNTQgMTAwMCA4O
-00000750: 4442 644c 305a 7662 6e52 4f59 5731 6c4c  DBdL0ZvbnROYW1lL
-00000760: 314e 5555 3239 755a 7931 4d61 5764 6f64  1NUU29uZy1MaWdod
-00000770: 4339 4a64 4746 7361 574e 4262 6d64 735a  C9JdGFsaWNBbmdsZ
-00000780: 5341 774c 314e 305a 5731 5749 446b 7a4c  SAwL1N0ZW1WIDkzL
-00000790: 314e 3065 5778 6c50 4477 7655 4746 7562  1N0eWxlPDwvUGFub
-000007a0: 334e 6c4b 4145 4641 6749 4541 4141 4141  3NlKAEFAgIEAAAAA
-000007b0: 4141 4141 436b 2b50 6a34 2b43 6d56 755a  AAAACk+Pj4+CmVuZ
-000007c0: 4739 6961 676f 3449 4441 6762 324a 7143  G9iago4IDAgb2JqC
-000007d0: 6a77 384c 3152 3563 4755 7652 6d39 7564  jw8L1R5cGUvRm9ud
-000007e0: 4339 5464 574a 3065 5842 6c4c 304e 4a52  C9TdWJ0eXBlL0NJR
-000007f0: 455a 7662 6e52 5565 5842 6c4d 4339 4359  EZvbnRUeXBlMC9CY
-00000800: 584e 6c52 6d39 7564 4339 5456 464e 7662  XNlRm9udC9TVFNvb
-00000810: 6d63 7454 476c 6e61 4851 7652 6d39 7564  mctTGlnaHQvRm9ud
-00000820: 4552 6c63 324e 7961 5842 3062 3349 674e  ERlc2NyaXB0b3IgN
-00000830: 7941 7749 4649 7656 7942 624d 5673 794d  yAwIFIvVyBbMVsyM
-00000840: 4464 644d 544e 624d 6a4d 3458 5445 3157  DddMTNbMjM4XTE1W
-00000850: 7a49 7a4f 4630 784f 4673 304e 6a4a 644d  zIzOF0xOFs0NjJdM
-00000860: 6a46 624e 4459 7958 5449 3357 7a49 7a4f  jFbNDYyXTI3WzIzO
-00000870: 4630 7a4e 4673 324f 4452 644d 7a5a 624e  F0zNFs2ODRdMzZbN
-00000880: 6a6b 3149 4463 7a4f 5341 314e 6a4d 674e  jk1IDczOSA1NjMgN
-00000890: 5445 7858 5451 7957 7a4d 784f 4630 304e  TExXTQyWzMxOF00N
-000008a0: 6c73 344f 5459 674e 7a55 3449 4463 334d  ls4OTYgNzU4IDc3M
-000008b0: 6941 314e 4452 644e 544a 624e 4459 3149  iA1NDRdNTJbNDY1I
-000008c0: 4459 774e 7941 334e 544e 644e 5464 624e  DYwNyA3NTNdNTdbN
-000008d0: 6a51 3358 5455 3557 7a59 774e 3130 324e  jQ3XTU5WzYwN102N
-000008e0: 6c73 304d 5464 644e 6a68 624e 4449 3349  ls0MTddNjhbNDI3I
-000008f0: 4455 794f 5341 304d 5456 644e 7a4e 624e  DUyOSA0MTVdNzNbN
-00000900: 5445 3449 4449 304d 5630 334f 4673 334f  TE4IDI0MV03OFs3O
-00000910: 544d 674e 5449 3349 4455 794e 4630 344d  TMgNTI3IDUyNF04M
-00000920: 3173 7a4d 7a67 674d 7a4d 3249 4449 334e  1szMzggMzM2IDI3N
-00000930: 7941 314d 5464 6458 5339 4556 7941 784d  yA1MTddXS9EVyAxM
-00000940: 4441 774c 304e 4a52 464e 3563 3352 6c62  DAwL0NJRFN5c3Rlb
-00000950: 556c 755a 6d38 3850 4339 535a 5764 7063  UluZm88PC9SZWdpc
-00000960: 3352 7965 5368 425a 4739 695a 536b 7654  3RyeShBZG9iZSkvT
-00000970: 334a 6b5a 584a 7062 6d63 6f52 3049 784b  3JkZXJpbmcoR0IxK
-00000980: 5339 5464 5842 7762 4756 745a 5735 3049  S9TdXBwbGVtZW50I
-00000990: 4451 2b50 6a34 2b43 6d56 755a 4739 6961  DQ+Pj4+CmVuZG9ia
-000009a0: 676f 7a49 4441 6762 324a 7143 6a77 384c  gozIDAgb2JqCjw8L
-000009b0: 3152 3563 4755 7652 6d39 7564 4339 5464  1R5cGUvRm9udC9Td
-000009c0: 574a 3065 5842 6c4c 3152 3563 4755 774c  WJ0eXBlL1R5cGUwL
-000009d0: 304a 6863 3256 4762 3235 304c 314e 5555  0Jhc2VGb250L1NUU
-000009e0: 3239 755a 7931 4d61 5764 6f64 4331 5662  29uZy1MaWdodC1Vb
-000009f0: 6d6c 4851 6931 5651 314d 794c 5567 7652  mlHQi1VQ1MyLUgvR
-00000a00: 5735 6a62 3252 7062 6d63 7656 5735 7052  W5jb2RpbmcvVW5pR
-00000a10: 3049 7456 554e 544d 6931 494c 3052 6c63  0ItVUNTMi1IL0Rlc
-00000a20: 324e 6c62 6d52 6862 6e52 4762 3235 3063  2NlbmRhbnRGb250c
-00000a30: 3173 3449 4441 6755 6c30 2b50 6770 6c62  1s4IDAgUl0+Pgplb
-00000a40: 6d52 7659 6d6f 4b4d 6941 7749 4739 6961  mRvYmoKMiAwIG9ia
-00000a50: 676f 3850 4339 5565 5842 6c4c 3168 5059  go8PC9UeXBlL1hPY
-00000a60: 6d70 6c59 3351 7655 3356 6964 486c 775a  mplY3QvU3VidHlwZ
-00000a70: 5339 4762 334a 744c 314a 6c63 3239 3163  S9Gb3JtL1Jlc291c
-00000a80: 6d4e 6c63 7a77 3850 6a34 7651 6b4a 7665  mNlczw8Pj4vQkJve
-00000a90: 4673 7749 4441 674d 5449 304c 6a67 674d  FswIDAgMTI0LjggM
-00000aa0: 6a52 644c 305a 7663 6d31 5565 5842 6c49  jRdL0Zvcm1UeXBlI
-00000ab0: 4445 7654 5746 3063 6d6c 3449 4673 7849  DEvTWF0cml4IFsxI
-00000ac0: 4441 674d 4341 7849 4441 674d 4630 7654  DAgMCAxIDAgMF0vT
-00000ad0: 4756 755a 3352 6f49 4445 344f 4339 4761  GVuZ3RoIDE4OC9Ga
-00000ae0: 5778 305a 5849 7652 6d78 6864 4756 455a  Wx0ZXIvRmxhdGVEZ
-00000af0: 574e 765a 4755 2b50 6e4e 3063 6d56 6862  WNvZGU+PnN0cmVhb
-00000b00: 5170 346e 4931 534f 784b 4549 417a 7450  Qp4nI1SOxKEIAztP
-00000b10: 5955 6e79 4351 6842 446a 5172 7233 334c  YUnyCQhBDjQrr33L
-00000b20: 3161 4547 6379 7a32 6248 5146 3379 664a  1aEGcyz2bHQF3yfJ
-00000b30: 5044 4f31 334d 6557 3338 4a2b 6136 326e  PDO13MeW38J+a62n
-00000b40: 3539 4e79 666f 4231 596e 742b 6e72 6943  59NyfoB1Ynt+nriC
-00000b50: 6c67 3030 4d58 6a61 5345 6f4e 4f71 4537  lg00MXjaSEoNOqE7
-00000b60: 6a4c 3968 6d47 3679 7250 6764 3246 4a4a  jL9hmG6yrPgd2FJJ
-00000b70: 6f5a 494b 5946 6f79 6852 5470 4f48 7936  oZIKYFoyhRTpOHy6
-00000b80: 4949 6874 6b55 504b 7841 726f 326e 5757  IIhtkUPKxAro2nWW
-00000b90: 3246 5273 6b64 5949 6259 4c78 542f 6367  2FRskdYIbYLxT/cg
-00000ba0: 6f50 4851 4957 4258 3943 7752 4c6e 536f  oPHQIWBX9CwRLnSo
-00000bb0: 4f6d 4b68 7456 416f 6349 7132 3031 596f  OmKhtVAocIq201Yo
-00000bc0: 3239 6a73 4374 6a63 3977 324d 2b41 454b  29jsCtjc9w2M+AEK
-00000bd0: 5951 7a72 7078 6664 3059 4557 574c 5176  YQzrpxfd0YEWWLQv
-00000be0: 7367 5936 416f 6a4b 7169 734c 3365 6439  sgY6AojKqisL3ed9
-00000bf0: 2f56 502f 4e31 2b31 5565 5961 6770 6c62  /VP/N1+1UeYagplb
-00000c00: 6d52 7a64 484a 6c59 5730 4b5a 5735 6b62  mRzdHJlYW0KZW5kb
-00000c10: 324a 7143 6a55 674d 4342 7659 6d6f 4b50  2JqCjUgMCBvYmoKP
-00000c20: 4477 7656 486c 775a 5339 5159 5764 6c63  DwvVHlwZS9QYWdlc
-00000c30: 7939 4462 3356 7564 4341 784c 3074 705a  y9Db3VudCAxL0tpZ
-00000c40: 484e 624e 6941 7749 464a 6450 6a34 4b5a  HNbNiAwIFJdPj4KZ
-00000c50: 5735 6b62 324a 7143 6a6b 674d 4342 7659  W5kb2JqCjkgMCBvY
-00000c60: 6d6f 4b50 4477 7656 486c 775a 5339 4459  moKPDwvVHlwZS9DY
-00000c70: 5852 6862 4739 6e4c 3142 685a 3256 7a49  XRhbG9nL1BhZ2VzI
-00000c80: 4455 674d 4342 5350 6a34 4b5a 5735 6b62  DUgMCBSPj4KZW5kb
-00000c90: 324a 7143 6a45 7749 4441 6762 324a 7143  2JqCjEwIDAgb2JqC
-00000ca0: 6a77 384c 3142 7962 3252 3159 3256 794b  jw8L1Byb2R1Y2VyK
-00000cb0: 436b 7651 334a 6c59 5852 7062 3235 4559  CkvQ3JlYXRpb25EY
-00000cc0: 5852 6c4b 4551 364d 6a41 794d 4445 794d  XRlKEQ6MjAyMDEyM
-00000cd0: 5441 784e 6a45 314e 5463 724d 4467 6e4d  TAxNjE1NTcrMDgnM
-00000ce0: 4441 6e4b 5339 4e62 3252 4559 5852 6c4b  DAnKS9Nb2REYXRlK
-00000cf0: 4551 364d 6a41 794d 4445 794d 5441 784e  EQ6MjAyMDEyMTAxN
-00000d00: 6a45 314e 5463 724d 4467 6e4d 4441 6e4b  jE1NTcrMDgnMDAnK
-00000d10: 5434 2b43 6d56 755a 4739 6961 6770 3463  T4+CmVuZG9iagp4c
-00000d20: 6d56 6d43 6a41 674d 5445 4b4d 4441 774d  mVmCjAgMTEKMDAwM
-00000d30: 4441 774d 4441 774d 4341 324e 5455 7a4e  DAwMDAwMCA2NTUzN
-00000d40: 5342 6d49 416f 774d 4441 774d 4441 774f  SBmIAowMDAwMDAwO
-00000d50: 4455 7849 4441 774d 4441 7749 4734 6743  DUxIDAwMDAwIG4gC
-00000d60: 6a41 774d 4441 774d 4445 324d 5445 674d  jAwMDAwMDE2MTEgM
-00000d70: 4441 774d 4441 6762 6941 4b4d 4441 774d  DAwMDAgbiAKMDAwM
-00000d80: 4441 774d 5451 344e 7941 774d 4441 774d  DAwMTQ4NyAwMDAwM
-00000d90: 4342 7549 416f 774d 4441 774d 4441 774d  CBuIAowMDAwMDAwM
-00000da0: 4445 3149 4441 774d 4441 7749 4734 6743  DE1IDAwMDAwIG4gC
-00000db0: 6a41 774d 4441 774d 4445 354e 5463 674d  jAwMDAwMDE5NTcgM
-00000dc0: 4441 774d 4441 6762 6941 4b4d 4441 774d  DAwMDAgbiAKMDAwM
-00000dd0: 4441 774d 4463 774e 4341 774d 4441 774d  DAwMDcwNCAwMDAwM
-00000de0: 4342 7549 416f 774d 4441 774d 4441 774f  CBuIAowMDAwMDAwO
-00000df0: 544d 3549 4441 774d 4441 7749 4734 6743  TM5IDAwMDAwIG4gC
-00000e00: 6a41 774d 4441 774d 4445 784d 7a41 674d  jAwMDAwMDExMzAgM
-00000e10: 4441 774d 4441 6762 6941 4b4d 4441 774d  DAwMDAgbiAKMDAwM
-00000e20: 4441 774d 6a41 774f 4341 774d 4441 774d  DAwMjAwOCAwMDAwM
-00000e30: 4342 7549 416f 774d 4441 774d 4441 794d  CBuIAowMDAwMDAyM
-00000e40: 4455 7a49 4441 774d 4441 7749 4734 6743  DUzIDAwMDAwIG4gC
-00000e50: 6e52 7959 576c 735a 5849 4b50 4477 7655  nRyYWlsZXIKPDwvU
-00000e60: 326c 365a 5341 784d 5339 5362 3239 3049  2l6ZSAxMS9Sb290I
-00000e70: 446b 674d 4342 534c 306c 755a 6d38 674d  DkgMCBSL0luZm8gM
-00000e80: 5441 674d 4342 534c 306c 4549 4673 384d  TAgMCBSL0lEIFs8M
-00000e90: 4755 334e 6a4a 6c4e 6a59 3159 5745 7a5a  GU3NjJlNjY1YWEzZ
-00000ea0: 4745 794e 6a41 344d 5442 6c5a 6a41 794d  GEyNjA4MTBlZjAyM
-00000eb0: 544a 694e 6a56 6d4e 4759 2b50 4442 6c4e  TJiNjVmNGY+PDBlN
-00000ec0: 7a59 795a 5459 324e 5746 684d 3252 684d  zYyZTY2NWFhM2RhM
-00000ed0: 6a59 774f 4445 775a 5759 774d 6a45 7959  jYwODEwZWYwMjEyY
-00000ee0: 6a59 315a 6a52 6d50 6c30 2b50 676f 6c4c  jY1ZjRmPl0+PgolL
-00000ef0: 5170 7a64 4746 7964 4868 795a 5759 4b4d  QpzdGFydHhyZWYKM
-00000f00: 6a45 314e 676f 6c4a 5556 5052 676f 3d29  jE1NgolJUVPRgo=)
-00000f10: 0172 0200 0000 2904 7206 0000 0072 0d00  .r....).r....r..
-00000f20: 0000 da08 5f5f 6e61 6d65 5f5f 5a07 6236  ....__name__Z.b6
-00000f30: 345f 7374 7272 0b00 0000 720b 0000 0072  4_strr....r....r
-00000f40: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00000f50: 6c65 3e01 0000 0073 0800 0000 0803 0a06  le>....s........
-00000f60: 0801 0422                                ..."
+00000000: 696d 706f 7274 2062 6173 6536 340a 0a0a  import base64...
+00000010: 6465 6620 7361 7665 5f62 3634 5f73 7472  def save_b64_str
+00000020: 696e 675f 6173 5f70 6466 2862 3634 5f73  ing_as_pdf(b64_s
+00000030: 7472 696e 672c 2066 696c 656e 616d 653d  tring, filename=
+00000040: 2774 6d70 2e70 6466 2729 3a0a 2020 2020  'tmp.pdf'):.    
+00000050: 7769 7468 206f 7065 6e28 6669 6c65 6e61  with open(filena
+00000060: 6d65 2c20 2777 6227 2920 6173 2066 3a0a  me, 'wb') as f:.
+00000070: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00000080: 6261 7365 3634 2e62 3634 6465 636f 6465  base64.b64decode
+00000090: 2862 3634 5f73 7472 696e 6729 290a 2020  (b64_string)).  
+000000a0: 2020 2020 2020 7072 696e 7428 6627 5361        print(f'Sa
+000000b0: 7665 6420 6261 7365 3634 2063 6f6e 7465  ved base64 conte
+000000c0: 6e74 2074 6f3a 207b 6669 6c65 6e61 6d65  nt to: {filename
+000000d0: 7d27 290a 0a0a 6966 205f 5f6e 616d 655f  }')...if __name_
+000000e0: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
+000000f0: 0a20 2020 2062 3634 5f73 7472 203d 2027  .    b64_str = '
+00000100: 4a56 4245 5269 3078 4c6a 514b 4a65 4c6a  JVBERi0xLjQKJeLj
+00000110: 7a39 4d4b 4e43 4177 4947 3969 6167 6f38  z9MKNCAwIG9iago8
+00000120: 5043 394d 5a57 356e 6447 6767 4e6a 4979  PC9MZW5ndGggNjIy
+00000130: 4c30 5a70 6248 526c 6369 3947 6247 4630  L0ZpbHRlci9GbGF0
+00000140: 5a55 526c 5932 396b 5a54 342b 6333 5279  ZURlY29kZT4+c3Ry
+00000150: 5a57 4674 436e 6963 6e5a 584e 6274 7041  ZWFtCnicnZXNbtpA
+00000160: 454d 6458 5027 205c 0a20 2020 2020 2020  EMdXP' \.       
+00000170: 2020 2020 2020 2027 666f 7052 756f 6c71         'fopRuolq
+00000180: 5a72 4e37 7670 6a31 3977 6f48 7847 7063  ZrN7vpj19woHxGpc
+00000190: 424b 386c 4354 4b78 5149 4858 4945 4a42  BK8lCTKxQIHXIEJB
+000001a0: 7052 6a48 3642 5348 3747 5030 5675 6c7a  pRjH6BSH7GP0Vulz
+000001b0: 686f 4843 4348 426a 6132 5664 3262 482f  hoHCCHBja2Vd2bH/
+000001c0: 3939 346d 4631 6d31 6777 3439 5878 6765  994mF1m1gw49Xxge
+000001d0: 4f4e 4567 6d31 5433 7766 4f66 6572 2720  ONEgm1T3wfOfer' 
+000001e0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+000001f0: 2736 304a 2f41 3666 5539 682f 6f55 7271  '60J/A6fU9h/oUrq
+00000200: 7772 6132 5a39 3052 5944 6f57 7a71 6768  wra2Z90RYDoWzqgh
+00000210: 3559 445a 3037 7a52 4277 6a69 746e 4f4d  5YDZ07zRBwjitnOM
+00000220: 6351 7670 4944 7269 6a6a 4946 7950 3267  cQvpIDrijjIFyP2g
+00000230: 376f 6958 5861 5242 3844 6659 2f68 4f72  7oiXXaRB8DfY/hOr
+00000240: 4d59 7463 3046 6a78 624c 582b 6963 465a  MYtc0FjxbLX+icFZ
+00000250: 4e73 6142 3227 205c 0a20 2020 2020 2020  NsaB2' \.       
+00000260: 2020 2020 2020 2027 4663 546f 4150 6130         'FcToAPa0
+00000270: 6336 2b2f 6f48 6549 7762 7943 4259 7a79  c6+/oHeIwbyCBYzy
+00000280: 4344 324d 6468 7a4c 7868 5057 3371 6675  CD2MdhzLxhPW3qfu
+00000290: 4a51 6258 6467 4172 306f 6952 397a 4a4c  JQbXdgAr0oiR9zJL
+000002a0: 6861 4148 744b 4f76 4830 524b 2b52 6f76  haAHtKOvH0RK+Rov
+000002b0: 524f 4937 5476 626e 7355 4732 336f 4c34  ROI7TvbnsUG23oL4
+000002c0: 4e71 3962 7279 4249 4b65 7646 3827 205c  Nq9bryBIKevF8' \
+000002d0: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+000002e0: 4154 6654 5a54 7145 7a71 414d 5148 696c  ATfTZTqEzqAMQHil
+000002f0: 414c 5757 766b 4643 4c52 6f6e 4439 4569  ALWWvkFCLRonD9Ei
+00000300: 5336 4979 326c 7957 3067 3531 565a 7453  S6Iy2lyW0g51VZtS
+00000310: 3161 706c 524a 6b71 6c2f 4246 4e39 4164  1aplRJkql/BFN9Ad
+00000320: 6b33 4d33 614f 6c47 4858 4a4b 2b4a 3766  k3M3aOlGHXJK+J7f
+00000330: 6e77 6e71 3434 4e7a 3038 4e46 4136 6974  nwnq44Nz08NFA6it
+00000340: 4268 4365 6827 205c 0a20 2020 2020 2020  BhCeh' \.       
+00000350: 2020 2020 2020 2027 3532 2b4e 3475 6d77         '52+N4umw
+00000360: 7830 6d42 4f4f 434d 3778 7137 3848 4c2f  x0mBOOCM7xq78HL/
+00000370: 494e 6454 6e33 316a 4836 5963 6b44 596f  INdTn31jH6YckDYo
+00000380: 3767 7a6c 554d 6c66 3058 334e 6e6e 412b  7gzlUMlf0X3NnnA+
+00000390: 766c 4332 485a 4a53 5674 5277 5665 6972  vlC2HZJSVtRwVeir
+000003a0: 3268 656a 715a 706a 4b70 3352 3637 4437  2hejqZpjKp3R67D7
+000003b0: 3435 4275 7336 4a53 626f 6377 4d65 2720  45Bus6JSbocwMe' 
+000003c0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+000003d0: 274f 636a 467a 5041 4b4b 596f 6864 414f  'OcjFzPAKKYohdAO
+000003e0: 6d53 674c 5349 4a67 3153 4a30 4243 6e46  mSgLSIJg1SJ0BCnF
+000003f0: 567a 4b30 514c 6676 7a36 3972 666b 7477  VzK0QLfvz69rfktw
+00000400: 687a 7a44 6871 6664 6749 644f 3267 6d69  hzzDhqfdgIdO2gmi
+00000410: 6838 5339 6f34 726c 4863 4353 762f 4936  h8S9o4rlHcCSv/I6
+00000420: 326f 6370 2b55 3559 3777 4a63 6e49 6c41  2ocp+U5Y7wJcnIlA
+00000430: 7a49 6b76 544a 4127 205c 0a20 2020 2020  zIkvTJA' \.     
+00000440: 2020 2020 2020 2020 2027 7155 4445 7045           'qUDEpE
+00000450: 4a69 5846 5777 5645 6a49 3178 5079 427a  JiXFWwVEjI1xPyBz
+00000460: 584a 7267 7952 3938 5550 576b 526c 614c  XJrgyR98UPWkRlaL
+00000470: 662b 4469 4233 7365 6676 2f73 6667 6a2f  f+DiB3sefv/sfgj/
+00000480: 6b4d 376e 5969 636a 5867 302b 456d 6e73  kM7nYicjXg0+Emns
+00000490: 7238 5530 6255 386d 5564 4c46 4473 6265  r8U0bU8mUdLFDsbe
+000004a0: 6f6b 2f63 6773 7746 336e 6852 5579 6349  ok/cgswF3nhRUycI
+000004b0: 6327 205c 0a20 2020 2020 2020 2020 2020  c' \.           
+000004c0: 2020 2027 572b 484c 534c 507a 2b53 5a79     'W+HLSLPz+SZy
+000004d0: 5a65 3547 6373 7074 4979 4964 4537 6b79  Ze5GcsptIyIdE7ky
+000004e0: 7353 6c66 534b 4947 397a 6142 4b33 4d64  sSlfSKIG9zaBK3Md
+000004f0: 2b45 6164 6856 426d 7977 7135 3768 6230  +EadhVBmywq57hb0
+00000500: 6563 394c 3351 3233 5033 304e 5852 6642  ec9L3Q23P30NXRfB
+00000510: 4e66 3969 516b 7171 6243 6a51 4a38 557a  Nf9iQkqqbCjQJ8Uz
+00000520: 6978 482f 4435 7455 6159 6b27 205c 0a20  ixH/D5tUaYk' \. 
+00000530: 2020 2020 2020 2020 2020 2020 2027 4b5a               'KZ
+00000540: 5735 6b63 3352 795a 5746 7443 6d56 755a  W5kc3RyZWFtCmVuZ
+00000550: 4739 6961 676f 3249 4441 6762 324a 7143  G9iago2IDAgb2JqC
+00000560: 6a77 384c 3152 3563 4755 7655 4746 6e5a  jw8L1R5cGUvUGFnZ
+00000570: 5339 4e5a 5752 7059 554a 7665 4673 7749  S9NZWRpYUJveFswI
+00000580: 4441 674d 6a67 7a4c 6a55 674d 6a67 7a4c  DAgMjgzLjUgMjgzL
+00000590: 6a56 644c 314a 6c63 3239 3163 6d4e 6c63  jVdL1Jlc291cmNlc
+000005a0: 7a77 384c 2720 5c0a 2020 2020 2020 2020  zw8L' \.        
+000005b0: 2020 2020 2020 2730 5a76 626e 5138 5043        '0ZvbnQ8PC
+000005c0: 3947 4d53 4178 4944 4167 5569 3947 4d69  9GMSAxIDAgUi9GMi
+000005d0: 417a 4944 4167 556a 342b 4c31 6850 596d  AzIDAgUj4+L1hPYm
+000005e0: 706c 5933 5138 5043 3959 5a6a 4567 4d69  plY3Q8PC9YZjEgMi
+000005f0: 4177 4946 492b 506a 342b 4c30 4e76 626e  AwIFI+Pj4+L0Nvbn
+00000600: 526c 626e 527a 4944 5167 4d43 4253 4c31  RlbnRzIDQgMCBSL1
+00000610: 4268 636d 5675 6443 4131 4944 4127 205c  BhcmVudCA1IDA' \
+00000620: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+00000630: 6755 6a34 2b43 6d56 755a 4739 6961 676f  gUj4+CmVuZG9iago
+00000640: 7849 4441 6762 324a 7143 6a77 384c 3152  xIDAgb2JqCjw8L1R
+00000650: 3563 4755 7652 6d39 7564 4339 5464 574a  5cGUvRm9udC9TdWJ
+00000660: 3065 5842 6c4c 3152 3563 4755 784c 304a  0eXBlL1R5cGUxL0J
+00000670: 6863 3256 4762 3235 304c 3068 6c62 485a  hc2VGb250L0hlbHZ
+00000680: 6c64 476c 6a59 5339 4662 6d4e 765a 476c  ldGljYS9FbmNvZGl
+00000690: 755a 7939 5861 2720 5c0a 2020 2020 2020  uZy9Xa' \.      
+000006a0: 2020 2020 2020 2020 2757 3542 626e 4e70          'W5BbnNp
+000006b0: 5257 356a 6232 5270 626d 632b 5067 706c  RW5jb2Rpbmc+Pgpl
+000006c0: 626d 5276 596d 6f4b 4e79 4177 4947 3969  bmRvYmoKNyAwIG9i
+000006d0: 6167 6f38 5043 3955 6558 426c 4c30 5a76  ago8PC9UeXBlL0Zv
+000006e0: 626e 5245 5a58 4e6a 636d 6c77 6447 3979  bnREZXNjcmlwdG9y
+000006f0: 4c30 467a 5932 5675 6443 4134 4f44 4176  L0FzY2VudCA4ODAv
+00000700: 5132 4677 5347 5670 5a32 6830 4944 6727  Q2FwSGVpZ2h0IDg'
+00000710: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00000720: 2027 344d 4339 455a 584e 6a5a 5735 3049   '4MC9EZXNjZW50I
+00000730: 4330 784d 6a41 7652 6d78 685a 334d 674e  C0xMjAvRmxhZ3MgN
+00000740: 6939 4762 3235 3051 6b4a 7665 4342 624c  i9Gb250QkJveCBbL
+00000750: 5449 3149 4330 794e 5451 674d 5441 774d  TI1IC0yNTQgMTAwM
+00000760: 4341 344f 4442 644c 305a 7662 6e52 4f59  CA4ODBdL0ZvbnROY
+00000770: 5731 6c4c 314e 5555 3239 755a 7931 4d61  W1lL1NUU29uZy1Ma
+00000780: 5764 6f64 4339 4a64 4727 205c 0a20 2020  WdodC9JdG' \.   
+00000790: 2020 2020 2020 2020 2020 2027 4673 6157             'FsaW
+000007a0: 4e42 626d 6473 5a53 4177 4c31 4e30 5a57  NBbmdsZSAwL1N0ZW
+000007b0: 3157 4944 6b7a 4c31 4e30 6557 786c 5044  1WIDkzL1N0eWxlPD
+000007c0: 7776 5547 4675 6233 4e6c 4b41 4546 4167  wvUGFub3NlKAEFAg
+000007d0: 4945 4141 4141 4141 4141 4143 6b2b 506a  IEAAAAAAAAACk+Pj
+000007e0: 342b 436d 5675 5a47 3969 6167 6f34 4944  4+CmVuZG9iago4ID
+000007f0: 4167 6232 4a71 436a 7738 4c31 5235 6347  Agb2JqCjw8L1R5cG
+00000800: 5527 205c 0a20 2020 2020 2020 2020 2020  U' \.           
+00000810: 2020 2027 7652 6d39 7564 4339 5464 574a     'vRm9udC9TdWJ
+00000820: 3065 5842 6c4c 304e 4a52 455a 7662 6e52  0eXBlL0NJREZvbnR
+00000830: 5565 5842 6c4d 4339 4359 584e 6c52 6d39  UeXBlMC9CYXNlRm9
+00000840: 7564 4339 5456 464e 7662 6d63 7454 476c  udC9TVFNvbmctTGl
+00000850: 6e61 4851 7652 6d39 7564 4552 6c63 324e  naHQvRm9udERlc2N
+00000860: 7961 5842 3062 3349 674e 7941 7749 4649  yaXB0b3IgNyAwIFI
+00000870: 7656 7942 624d 5673 7927 205c 0a20 2020  vVyBbMVsy' \.   
+00000880: 2020 2020 2020 2020 2020 2027 4d44 6464             'MDdd
+00000890: 4d54 4e62 4d6a 4d34 5854 4531 577a 497a  MTNbMjM4XTE1WzIz
+000008a0: 4f46 3078 4f46 7330 4e6a 4a64 4d6a 4662  OF0xOFs0NjJdMjFb
+000008b0: 4e44 5979 5854 4933 577a 497a 4f46 307a  NDYyXTI3WzIzOF0z
+000008c0: 4e46 7332 4f44 5264 4d7a 5a62 4e6a 6b31  NFs2ODRdMzZbNjk1
+000008d0: 4944 637a 4f53 4131 4e6a 4d67 4e54 4578  IDczOSA1NjMgNTEx
+000008e0: 5854 5179 577a 4d78 4f46 3030 4e6c 7334  XTQyWzMxOF00Nls4
+000008f0: 4f27 205c 0a20 2020 2020 2020 2020 2020  O' \.           
+00000900: 2020 2027 5459 674e 7a55 3449 4463 334d     'TYgNzU4IDc3M
+00000910: 6941 314e 4452 644e 544a 624e 4459 3149  iA1NDRdNTJbNDY1I
+00000920: 4459 774e 7941 334e 544e 644e 5464 624e  DYwNyA3NTNdNTdbN
+00000930: 6a51 3358 5455 3557 7a59 774e 3130 324e  jQ3XTU5WzYwN102N
+00000940: 6c73 304d 5464 644e 6a68 624e 4449 3349  ls0MTddNjhbNDI3I
+00000950: 4455 794f 5341 304d 5456 644e 7a4e 624e  DUyOSA0MTVdNzNbN
+00000960: 5445 3449 4449 304d 5630 2720 5c0a 2020  TE4IDI0MV0' \.  
+00000970: 2020 2020 2020 2020 2020 2020 2733 4f46              '3OF
+00000980: 7333 4f54 4d67 4e54 4933 4944 5579 4e46  s3OTMgNTI3IDUyNF
+00000990: 3034 4d31 737a 4d7a 6767 4d7a 4d32 4944  04M1szMzggMzM2ID
+000009a0: 4933 4e79 4131 4d54 6464 5853 3945 5679  I3NyA1MTddXS9EVy
+000009b0: 4178 4d44 4177 4c30 4e4a 5246 4e35 6333  AxMDAwL0NJRFN5c3
+000009c0: 526c 6255 6c75 5a6d 3838 5043 3953 5a57  RlbUluZm88PC9SZW
+000009d0: 6470 6333 5279 6553 6842 5a47 3969 5a53  dpc3RyeShBZG9iZS
+000009e0: 6b76 5427 205c 0a20 2020 2020 2020 2020  kvT' \.         
+000009f0: 2020 2020 2027 334a 6b5a 584a 7062 6d63       '3JkZXJpbmc
+00000a00: 6f52 3049 784b 5339 5464 5842 7762 4756  oR0IxKS9TdXBwbGV
+00000a10: 745a 5735 3049 4451 2b50 6a34 2b43 6d56  tZW50IDQ+Pj4+CmV
+00000a20: 755a 4739 6961 676f 7a49 4441 6762 324a  uZG9iagozIDAgb2J
+00000a30: 7143 6a77 384c 3152 3563 4755 7652 6d39  qCjw8L1R5cGUvRm9
+00000a40: 7564 4339 5464 574a 3065 5842 6c4c 3152  udC9TdWJ0eXBlL1R
+00000a50: 3563 4755 774c 304a 6863 3227 205c 0a20  5cGUwL0Jhc2' \. 
+00000a60: 2020 2020 2020 2020 2020 2020 2027 5647               'VG
+00000a70: 6232 3530 4c31 4e55 5532 3975 5a79 314d  b250L1NUU29uZy1M
+00000a80: 6157 646f 6443 3156 626d 6c48 5169 3156  aWdodC1VbmlHQi1V
+00000a90: 5131 4d79 4c55 6776 5257 356a 6232 5270  Q1MyLUgvRW5jb2Rp
+00000aa0: 626d 6376 5657 3570 5230 4974 5655 4e54  bmcvVW5pR0ItVUNT
+00000ab0: 4d69 3149 4c30 526c 6332 4e6c 626d 5268  Mi1IL0Rlc2NlbmRh
+00000ac0: 626e 5247 6232 3530 6331 7334 4944 4167  bnRGb250c1s4IDAg
+00000ad0: 556c 302b 2720 5c0a 2020 2020 2020 2020  Ul0+' \.        
+00000ae0: 2020 2020 2020 2750 6770 6c62 6d52 7659        'PgplbmRvY
+00000af0: 6d6f 4b4d 6941 7749 4739 6961 676f 3850  moKMiAwIG9iago8P
+00000b00: 4339 5565 5842 6c4c 3168 5059 6d70 6c59  C9UeXBlL1hPYmplY
+00000b10: 3351 7655 3356 6964 486c 775a 5339 4762  3QvU3VidHlwZS9Gb
+00000b20: 334a 744c 314a 6c63 3239 3163 6d4e 6c63  3JtL1Jlc291cmNlc
+00000b30: 7a77 3850 6a34 7651 6b4a 7665 4673 7749  zw8Pj4vQkJveFswI
+00000b40: 4441 674d 5449 304c 6a67 674d 6a27 205c  DAgMTI0LjggMj' \
+00000b50: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+00000b60: 5264 4c30 5a76 636d 3155 6558 426c 4944  RdL0Zvcm1UeXBlID
+00000b70: 4576 5457 4630 636d 6c34 4946 7378 4944  EvTWF0cml4IFsxID
+00000b80: 4167 4d43 4178 4944 4167 4d46 3076 5447  AgMCAxIDAgMF0vTG
+00000b90: 5675 5a33 526f 4944 4534 4f43 3947 6157  VuZ3RoIDE4OC9GaW
+00000ba0: 7830 5a58 4976 526d 7868 6447 5645 5a57  x0ZXIvRmxhdGVEZW
+00000bb0: 4e76 5a47 552b 506e 4e30 636d 5668 6251  NvZGU+PnN0cmVhbQ
+00000bc0: 7034 6e49 3153 2720 5c0a 2020 2020 2020  p4nI1S' \.      
+00000bd0: 2020 2020 2020 2020 274f 784b 4549 417a          'OxKEIAz
+00000be0: 7450 5955 6e79 4351 6842 446a 5172 7233  tPYUnyCQhBDjQrr3
+00000bf0: 334c 3161 4547 6379 7a32 6248 5146 3379  3L1aEGcyz2bHQF3y
+00000c00: 664a 5044 4f31 334d 6557 3338 4a2b 6136  fJPDO13MeW38J+a6
+00000c10: 326e 3539 4e79 666f 4231 596e 742b 6e72  2n59NyfoB1Ynt+nr
+00000c20: 6943 6c67 3030 4d58 6a61 5345 6f4e 4f71  iClg00MXjaSEoNOq
+00000c30: 4537 6a4c 3968 6d47 3679 7250 6764 3227  E7jL9hmG6yrPgd2'
+00000c40: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00000c50: 2027 464a 4a6f 5a49 4b59 466f 7968 5254   'FJJoZIKYFoyhRT
+00000c60: 704f 4879 3649 4968 746b 5550 4b78 4172  pOHy6IIhtkUPKxAr
+00000c70: 6f32 6e57 5732 4652 736b 6459 4962 594c  o2nWW2FRskdYIbYL
+00000c80: 7854 2f63 676f 5048 5149 5742 5839 4377  xT/cgoPHQIWBX9Cw
+00000c90: 524c 6e53 6f4f 6d4b 6874 5641 6f63 4971  RLnSoOmKhtVAocIq
+00000ca0: 3230 3159 6f32 396a 7343 746a 6339 7732  201Yo29jsCtjc9w2
+00000cb0: 4d2b 4145 4b59 517a 2720 5c0a 2020 2020  M+AEKYQz' \.    
+00000cc0: 2020 2020 2020 2020 2020 2772 7078 6664            'rpxfd
+00000cd0: 3059 4557 574c 5176 7367 5936 416f 6a4b  0YEWWLQvsgY6AojK
+00000ce0: 7169 734c 3365 6439 2f56 502f 4e31 2b31  qisL3ed9/VP/N1+1
+00000cf0: 5565 5961 6770 6c62 6d52 7a64 484a 6c59  UeYagplbmRzdHJlY
+00000d00: 5730 4b5a 5735 6b62 324a 7143 6a55 674d  W0KZW5kb2JqCjUgM
+00000d10: 4342 7659 6d6f 4b50 4477 7656 486c 775a  CBvYmoKPDwvVHlwZ
+00000d20: 5339 5159 5764 6c63 7939 4462 3356 7564  S9QYWdlcy9Db3Vud
+00000d30: 4327 205c 0a20 2020 2020 2020 2020 2020  C' \.           
+00000d40: 2020 2027 4178 4c30 7470 5a48 4e62 4e69     'AxL0tpZHNbNi
+00000d50: 4177 4946 4a64 506a 344b 5a57 356b 6232  AwIFJdPj4KZW5kb2
+00000d60: 4a71 436a 6b67 4d43 4276 596d 6f4b 5044  JqCjkgMCBvYmoKPD
+00000d70: 7776 5648 6c77 5a53 3944 5958 5268 6247  wvVHlwZS9DYXRhbG
+00000d80: 396e 4c31 4268 5a32 567a 4944 5567 4d43  9nL1BhZ2VzIDUgMC
+00000d90: 4253 506a 344b 5a57 356b 6232 4a71 436a  BSPj4KZW5kb2JqCj
+00000da0: 4577 4944 4167 6232 4a71 2720 5c0a 2020  EwIDAgb2Jq' \.  
+00000db0: 2020 2020 2020 2020 2020 2020 2743 6a77              'Cjw
+00000dc0: 384c 3142 7962 3252 3159 3256 794b 436b  8L1Byb2R1Y2VyKCk
+00000dd0: 7651 334a 6c59 5852 7062 3235 4559 5852  vQ3JlYXRpb25EYXR
+00000de0: 6c4b 4551 364d 6a41 794d 4445 794d 5441  lKEQ6MjAyMDEyMTA
+00000df0: 784e 6a45 314e 5463 724d 4467 6e4d 4441  xNjE1NTcrMDgnMDA
+00000e00: 6e4b 5339 4e62 3252 4559 5852 6c4b 4551  nKS9Nb2REYXRlKEQ
+00000e10: 364d 6a41 794d 4445 794d 5441 784e 6a45  6MjAyMDEyMTAxNjE
+00000e20: 314e 2720 5c0a 2020 2020 2020 2020 2020  1N' \.          
+00000e30: 2020 2020 2754 6372 4d44 676e 4d44 416e      'TcrMDgnMDAn
+00000e40: 4b54 342b 436d 5675 5a47 3969 6167 7034  KT4+CmVuZG9iagp4
+00000e50: 636d 566d 436a 4167 4d54 454b 4d44 4177  cmVmCjAgMTEKMDAw
+00000e60: 4d44 4177 4d44 4177 4d43 4132 4e54 557a  MDAwMDAwMCA2NTUz
+00000e70: 4e53 426d 4941 6f77 4d44 4177 4d44 4177  NSBmIAowMDAwMDAw
+00000e80: 4f44 5578 4944 4177 4d44 4177 4947 3467  ODUxIDAwMDAwIG4g
+00000e90: 436a 4177 4d44 4177 4d44 4527 205c 0a20  CjAwMDAwMDE' \. 
+00000ea0: 2020 2020 2020 2020 2020 2020 2027 324d               '2M
+00000eb0: 5445 674d 4441 774d 4441 6762 6941 4b4d  TEgMDAwMDAgbiAKM
+00000ec0: 4441 774d 4441 774d 5451 344e 7941 774d  DAwMDAwMTQ4NyAwM
+00000ed0: 4441 774d 4342 7549 416f 774d 4441 774d  DAwMCBuIAowMDAwM
+00000ee0: 4441 774d 4445 3149 4441 774d 4441 7749  DAwMDE1IDAwMDAwI
+00000ef0: 4734 6743 6a41 774d 4441 774d 4445 354e  G4gCjAwMDAwMDE5N
+00000f00: 5463 674d 4441 774d 4441 6762 6941 4b4d  TcgMDAwMDAgbiAKM
+00000f10: 4441 7727 205c 0a20 2020 2020 2020 2020  DAw' \.         
+00000f20: 2020 2020 2027 4d44 4177 4d44 6377 4e43       'MDAwMDcwNC
+00000f30: 4177 4d44 4177 4d43 4275 4941 6f77 4d44  AwMDAwMCBuIAowMD
+00000f40: 4177 4d44 4177 4f54 4d35 4944 4177 4d44  AwMDAwOTM5IDAwMD
+00000f50: 4177 4947 3467 436a 4177 4d44 4177 4d44  AwIG4gCjAwMDAwMD
+00000f60: 4578 4d7a 4167 4d44 4177 4d44 4167 6269  ExMzAgMDAwMDAgbi
+00000f70: 414b 4d44 4177 4d44 4177 4d6a 4177 4f43  AKMDAwMDAwMjAwOC
+00000f80: 4177 4d44 4177 4d43 4275 4941 2720 5c0a  AwMDAwMCBuIA' \.
+00000f90: 2020 2020 2020 2020 2020 2020 2020 276f                'o
+00000fa0: 774d 4441 774d 4441 794d 4455 7a49 4441  wMDAwMDAyMDUzIDA
+00000fb0: 774d 4441 7749 4734 6743 6e52 7959 576c  wMDAwIG4gCnRyYWl
+00000fc0: 735a 5849 4b50 4477 7655 326c 365a 5341  sZXIKPDwvU2l6ZSA
+00000fd0: 784d 5339 5362 3239 3049 446b 674d 4342  xMS9Sb290IDkgMCB
+00000fe0: 534c 306c 755a 6d38 674d 5441 674d 4342  SL0luZm8gMTAgMCB
+00000ff0: 534c 306c 4549 4673 384d 4755 334e 6a4a  SL0lEIFs8MGU3NjJ
+00001000: 6c4e 6a59 2720 5c0a 2020 2020 2020 2020  lNjY' \.        
+00001010: 2020 2020 2020 2731 5957 457a 5a47 4579        '1YWEzZGEy
+00001020: 4e6a 4134 4d54 426c 5a6a 4179 4d54 4a69  NjA4MTBlZjAyMTJi
+00001030: 4e6a 566d 4e47 592b 5044 426c 4e7a 5979  NjVmNGY+PDBlNzYy
+00001040: 5a54 5932 4e57 4668 4d32 5268 4d6a 5977  ZTY2NWFhM2RhMjYw
+00001050: 4f44 4577 5a57 5977 4d6a 4579 596a 5931  ODEwZWYwMjEyYjY1
+00001060: 5a6a 526d 506c 302b 5067 6f6c 4c51 707a  ZjRmPl0+PgolLQpz
+00001070: 6447 4679 6448 6879 5a57 594b 4d27 205c  dGFydHhyZWYKM' \
+00001080: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+00001090: 6a45 314e 676f 6c4a 5556 5052 676f 3d27  jE1NgolJUVPRgo='
+000010a0: 0a20 2020 2073 6176 655f 6236 345f 7374  .    save_b64_st
+000010b0: 7269 6e67 5f61 735f 7064 6628 6236 345f  ring_as_pdf(b64_
+000010c0: 7374 7229 0a                             str).
```

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/pdf/pdf_analyzer.py` & `comwares-0.1.4/comwares/pdf/pdf_analyzer.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/cos.py` & `comwares-0.1.4/comwares/tencent/cos.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/sms.py` & `comwares-0.1.4/comwares/tencent/sms.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/tencent/translate.py` & `comwares-0.1.4/comwares/tencent/translate.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/traffic/alexacn.py` & `comwares-0.1.4/comwares/traffic/alexacn.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/video/snap.py` & `comwares-0.1.4/comwares/video/snap.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/feishu.py` & `comwares-0.1.4/comwares/webhooks/feishu.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares/webhooks/work_weixin.py` & `comwares-0.1.4/comwares/webhooks/work_weixin.py`

 * *Files identical despite different names*

### Comparing `./Users/kevinzhu/PycharmProjects/comwares/venv/lib/python3.9/site-packages/comwares-0.1.3-py3.9.egg-info/SOURCES.txt` & `comwares-0.1.4/comwares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

