# Comparing `tmp/starlette_web-0.1.1.tar.gz` & `tmp/starlette_web-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_web-0.1.1.tar", last modified: Sun Apr  2 21:40:47 2023, max compression
+gzip compressed data, was "starlette_web-0.1.2.tar", last modified: Thu Apr 13 19:30:56 2023, max compression
```

## Comparing `starlette_web-0.1.1.tar` & `starlette_web-0.1.2.tar`

### file list

```diff
@@ -1,587 +1,260 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.685367 starlette_web-0.1.1/
--rw-rw-rw-   0        0        0     1092 2022-04-25 19:06:18.000000 starlette_web-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       49 2023-03-27 17:02:23.000000 starlette_web-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3245 2023-04-02 21:40:47.685367 starlette_web-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.1/README.md
--rw-rw-rw-   0        0        0     1840 2023-04-02 21:40:47.686371 starlette_web-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-04-25 19:06:18.000000 starlette_web-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.250145 starlette_web-0.1.1/starlette_web/
--rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.1/starlette_web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.254160 starlette_web-0.1.1/starlette_web/__pycache__/
--rw-rw-rw-   0        0        0      165 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      163 2022-12-29 14:35:19.000000 starlette_web-0.1.1/starlette_web/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.261044 starlette_web-0.1.1/starlette_web/common/
--rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.1/starlette_web/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.265035 starlette_web-0.1.1/starlette_web/common/__pycache__/
--rw-rw-rw-   0        0        0      207 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      205 2022-04-30 17:23:58.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6520 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/app.cpython-310.pyc
--rw-rw-rw-   0        0        0     4243 2022-10-26 19:12:05.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/app.cpython-39.pyc
--rw-rw-rw-   0        0        0     4301 2022-05-03 15:41:29.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/db_utils.cpython-39.pyc
--rw-rw-rw-   0        0        0     4231 2022-05-03 15:41:29.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/models.cpython-39.pyc
--rw-rw-rw-   0        0        0     3034 2022-05-03 15:41:29.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/redis.cpython-39.pyc
--rw-rw-rw-   0        0        0     4704 2022-05-02 16:12:21.000000 starlette_web-0.1.1/starlette_web/common/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/app.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.267029 starlette_web-0.1.1/starlette_web/common/authorization/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.1/starlette_web/common/authorization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.276809 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/
--rw-rw-rw-   0        0        0      165 2022-12-31 10:47:35.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1448 2023-03-25 15:08:24.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/backends.cpython-310.pyc
--rw-rw-rw-   0        0        0     1467 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/backends.cpython-39.pyc
--rw-rw-rw-   0        0        0      751 2023-03-25 15:08:21.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/base_user.cpython-310.pyc
--rw-rw-rw-   0        0        0      787 2022-05-02 13:11:13.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/base_user.cpython-39.pyc
--rw-rw-rw-   0        0        0     4526 2023-03-25 15:08:24.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/permissions.cpython-310.pyc
--rw-rw-rw-   0        0        0     4642 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/common/authorization/__pycache__/permissions.cpython-39.pyc
--rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.1/starlette_web/common/authorization/backends.py
--rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.1/starlette_web/common/authorization/base_user.py
--rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.1/starlette_web/common/authorization/permissions.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.279806 starlette_web-0.1.1/starlette_web/common/caches/
--rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.1/starlette_web/common/caches/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.286181 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/
--rw-rw-rw-   0        0        0      230 2023-03-17 16:10:53.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      244 2022-05-14 20:12:19.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3167 2023-03-25 15:08:07.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     3199 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/base.cpython-39.pyc
--rw-rw-rw-   0        0        0     2747 2023-04-01 08:02:26.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/base_lock.cpython-310.pyc
--rw-rw-rw-   0        0        0     1366 2023-03-17 16:10:53.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/cache_handler.cpython-310.pyc
--rw-rw-rw-   0        0        0     2318 2022-09-03 11:52:06.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/cache_handler.cpython-39.pyc
--rw-rw-rw-   0        0        0     6204 2023-03-24 16:48:39.000000 starlette_web-0.1.1/starlette_web/common/caches/__pycache__/local_memory.cpython-310.pyc
--rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.1/starlette_web/common/caches/base.py
--rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.1/starlette_web/common/caches/base_lock.py
--rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.1/starlette_web/common/caches/cache_handler.py
--rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.1/starlette_web/common/caches/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.292555 starlette_web-0.1.1/starlette_web/common/channels/
--rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/common/channels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.297296 starlette_web-0.1.1/starlette_web/common/channels/__pycache__/
--rw-rw-rw-   0        0        0      160 2023-03-12 19:57:34.000000 starlette_web-0.1.1/starlette_web/common/channels/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4640 2023-04-01 19:06:28.000000 starlette_web-0.1.1/starlette_web/common/channels/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0      914 2023-03-12 19:57:34.000000 starlette_web-0.1.1/starlette_web/common/channels/__pycache__/event.cpython-310.pyc
--rw-rw-rw-   0        0        0      523 2023-03-22 16:40:06.000000 starlette_web-0.1.1/starlette_web/common/channels/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.1/starlette_web/common/channels/base.py
--rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/common/channels/event.py
--rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.1/starlette_web/common/channels/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.298296 starlette_web-0.1.1/starlette_web/common/channels/layers/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.300289 starlette_web-0.1.1/starlette_web/common/channels/layers/__pycache__/
--rw-rw-rw-   0        0        0      167 2023-03-12 19:57:34.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1512 2023-03-12 19:57:34.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     2268 2023-03-12 19:57:34.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/__pycache__/local_memory.cpython-310.pyc
--rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/base.py
--rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.1/starlette_web/common/channels/layers/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.304305 starlette_web-0.1.1/starlette_web/common/conf/
--rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.311570 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/
--rw-rw-rw-   0        0        0     2114 2023-03-30 21:28:00.000000 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1917 2022-09-03 11:52:05.000000 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2647 2023-03-26 18:27:45.000000 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/app_manager.cpython-310.pyc
--rw-rw-rw-   0        0        0      707 2023-03-03 20:07:25.000000 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/base_app_config.cpython-310.pyc
--rw-rw-rw-   0        0        0     1337 2023-03-31 19:13:32.000000 starlette_web-0.1.1/starlette_web/common/conf/__pycache__/global_settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2945 2023-03-26 18:25:01.000000 starlette_web-0.1.1/starlette_web/common/conf/app_manager.py
--rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/common/conf/base_app_config.py
--rw-rw-rw-   0        0        0     1637 2023-03-31 19:10:54.000000 starlette_web-0.1.1/starlette_web/common/conf/global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.314928 starlette_web-0.1.1/starlette_web/common/database/
--rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/common/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.328097 starlette_web-0.1.1/starlette_web/common/database/__pycache__/
--rw-rw-rw-   0        0        0      560 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      558 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1481 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/columns.cpython-310.pyc
--rw-rw-rw-   0        0        0     1471 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/columns.cpython-39.pyc
--rw-rw-rw-   0        0        0      236 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/model_base.cpython-310.pyc
--rw-rw-rw-   0        0        0      234 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/model_base.cpython-39.pyc
--rw-rw-rw-   0        0        0     7721 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/model_mixin.cpython-310.pyc
--rw-rw-rw-   0        0        0     7672 2022-08-19 14:29:48.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/model_mixin.cpython-39.pyc
--rw-rw-rw-   0        0        0     1338 2023-02-18 10:07:24.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/session_maker.cpython-310.pyc
--rw-rw-rw-   0        0        0      643 2022-10-09 18:04:23.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/session_maker.cpython-39.pyc
--rw-rw-rw-   0        0        0     2791 2023-02-18 12:47:18.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/types.cpython-310.pyc
--rw-rw-rw-   0        0        0     2781 2022-10-06 18:22:50.000000 starlette_web-0.1.1/starlette_web/common/database/__pycache__/types.cpython-39.pyc
--rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/common/database/columns.py
--rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/common/database/model_base.py
--rw-rw-rw-   0        0        0     9166 2022-08-19 14:16:41.000000 starlette_web-0.1.1/starlette_web/common/database/model_mixin.py
--rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.1/starlette_web/common/database/session_maker.py
--rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.1/starlette_web/common/database/types.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.330094 starlette_web-0.1.1/starlette_web/common/email/
--rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.1/starlette_web/common/email/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.338366 starlette_web-0.1.1/starlette_web/common/email/__pycache__/
--rw-rw-rw-   0        0        0      337 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      335 2022-05-22 18:29:58.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2142 2023-03-28 17:00:28.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/base_sender.cpython-310.pyc
--rw-rw-rw-   0        0        0     1979 2022-06-05 10:59:02.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/base_sender.cpython-39.pyc
--rw-rw-rw-   0        0        0     2149 2023-03-28 16:49:47.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/email_manager.cpython-310.pyc
--rw-rw-rw-   0        0        0     1921 2022-09-03 11:52:07.000000 starlette_web-0.1.1/starlette_web/common/email/__pycache__/email_manager.cpython-39.pyc
--rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.1/starlette_web/common/email/base_sender.py
--rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.1/starlette_web/common/email/email_manager.py
--rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/email/smtp.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.339367 starlette_web-0.1.1/starlette_web/common/files/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.1/starlette_web/common/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.341360 starlette_web-0.1.1/starlette_web/common/files/__pycache__/
--rw-rw-rw-   0        0        0      157 2023-03-23 18:11:39.000000 starlette_web-0.1.1/starlette_web/common/files/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     7350 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/common/files/__pycache__/cache.cpython-310.pyc
--rw-rw-rw-   0        0        0     3612 2023-04-01 08:12:18.000000 starlette_web-0.1.1/starlette_web/common/files/__pycache__/filelock.cpython-310.pyc
--rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/files/cache.py
--rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.1/starlette_web/common/files/filelock.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.343354 starlette_web-0.1.1/starlette_web/common/files/storages/
--rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.1/starlette_web/common/files/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.345648 starlette_web-0.1.1/starlette_web/common/files/storages/__pycache__/
--rw-rw-rw-   0        0        0      287 2023-03-30 20:41:25.000000 starlette_web-0.1.1/starlette_web/common/files/storages/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     8034 2023-03-31 18:52:49.000000 starlette_web-0.1.1/starlette_web/common/files/storages/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     5935 2023-04-01 16:31:49.000000 starlette_web-0.1.1/starlette_web/common/files/storages/__pycache__/filesystem.cpython-310.pyc
--rw-rw-rw-   0        0        0     4434 2023-03-30 15:59:56.000000 starlette_web-0.1.1/starlette_web/common/files/storages/__pycache__/filesystem_lock.cpython-310.pyc
--rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.1/starlette_web/common/files/storages/base.py
--rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.1/starlette_web/common/files/storages/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.355390 starlette_web-0.1.1/starlette_web/common/http/
--rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.1/starlette_web/common/http/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.370277 starlette_web-0.1.1/starlette_web/common/http/__pycache__/
--rw-rw-rw-   0        0        0      156 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      154 2022-05-03 08:52:46.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5798 2023-03-26 10:30:10.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/base_endpoint.cpython-310.pyc
--rw-rw-rw-   0        0        0     5330 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/base_endpoint.cpython-39.pyc
--rw-rw-rw-   0        0        0     5390 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/exception_handlers.cpython-310.pyc
--rw-rw-rw-   0        0        0     5388 2022-10-06 18:58:48.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/exception_handlers.cpython-39.pyc
--rw-rw-rw-   0        0        0     5275 2023-03-30 21:28:00.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0     4105 2022-09-03 11:52:05.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/exceptions.cpython-39.pyc
--rw-rw-rw-   0        0        0     1549 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/renderers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1527 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/renderers.cpython-39.pyc
--rw-rw-rw-   0        0        0      437 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/responses.cpython-310.pyc
--rw-rw-rw-   0        0        0      435 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/responses.cpython-39.pyc
--rw-rw-rw-   0        0        0     1099 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/schemas.cpython-310.pyc
--rw-rw-rw-   0        0        0     1101 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/schemas.cpython-39.pyc
--rw-rw-rw-   0        0        0     1152 2023-03-15 20:40:20.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/statuses.cpython-310.pyc
--rw-rw-rw-   0        0        0     1002 2022-09-04 14:01:21.000000 starlette_web-0.1.1/starlette_web/common/http/__pycache__/statuses.cpython-39.pyc
--rw-rw-rw-   0        0        0     6474 2023-03-26 10:02:27.000000 starlette_web-0.1.1/starlette_web/common/http/base_endpoint.py
--rw-rw-rw-   0        0        0     4338 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/common/http/exception_handlers.py
--rw-rw-rw-   0        0        0     4287 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/http/exceptions.py
--rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/common/http/renderers.py
--rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/common/http/responses.py
--rw-rw-rw-   0        0        0      829 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/common/http/schemas.py
--rw-rw-rw-   0        0        0      942 2023-03-14 17:15:47.000000 starlette_web-0.1.1/starlette_web/common/http/statuses.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.370277 starlette_web-0.1.1/starlette_web/common/i18n/
--rw-rw-rw-   0        0        0      163 2022-09-03 15:11:31.000000 starlette_web-0.1.1/starlette_web/common/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.371554 starlette_web-0.1.1/starlette_web/common/i18n/__pycache__/
--rw-rw-rw-   0        0        0      363 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/common/i18n/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      356 2022-09-04 15:53:59.000000 starlette_web-0.1.1/starlette_web/common/i18n/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.373552 starlette_web-0.1.1/starlette_web/common/management/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.1/starlette_web/common/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.377541 starlette_web-0.1.1/starlette_web/common/management/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-12-31 10:47:35.000000 starlette_web-0.1.1/starlette_web/common/management/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1032 2023-03-26 12:11:02.000000 starlette_web-0.1.1/starlette_web/common/management/__pycache__/admin_util.cpython-310.pyc
--rw-rw-rw-   0        0        0     6285 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/common/management/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     4668 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/common/management/__pycache__/base.cpython-39.pyc
--rw-rw-rw-   0        0        0     1489 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/management/admin_util.py
--rw-rw-rw-   0        0        0     6020 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/management/base.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.378538 starlette_web-0.1.1/starlette_web/common/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.1/starlette_web/common/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.384695 starlette_web-0.1.1/starlette_web/common/management/commands/__pycache__/
--rw-rw-rw-   0        0        0      171 2023-03-28 16:49:43.000000 starlette_web-0.1.1/starlette_web/common/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1043 2023-03-28 18:58:33.000000 starlette_web-0.1.1/starlette_web/common/management/commands/__pycache__/test_email.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0      934 2023-03-28 18:56:19.000000 starlette_web-0.1.1/starlette_web/common/management/commands/__pycache__/test_email.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.387689 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/__init__.py
--rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/admin.py
--rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/apps.py
--rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/models.py
--rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/routes.py
--rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_app_defaults/views.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.390705 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/__init__.py
--rw-rw-rw-   0        0        0      439 2023-04-02 10:38:48.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/asgi.py
--rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/command.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.391702 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.392699 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/__pycache__/
--rw-rw-rw-   0        0        0      221 2022-05-03 15:41:29.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/__pycache__/database.cpython-39.pyc
--rw-rw-rw-   0        0        0      884 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/routes.py
--rw-rw-rw-   0        0        0     3330 2023-03-30 19:15:27.000000 starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/settings.py
--rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/management/commands/startapp.py
--rw-rw-rw-   0        0        0     3673 2023-04-01 16:41:06.000000 starlette_web-0.1.1/starlette_web/common/management/commands/startproject.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.404795 starlette_web-0.1.1/starlette_web/common/utils/
--rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.1/starlette_web/common/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.421899 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/
--rw-rw-rw-   0        0        0      742 2023-04-01 19:37:22.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      640 2022-10-26 19:12:06.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3771 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/choices.cpython-310.pyc
--rw-rw-rw-   0        0        0     3795 2022-09-04 14:01:21.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/choices.cpython-39.pyc
--rw-rw-rw-   0        0        0     1495 2023-03-18 14:43:26.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/crypto.cpython-310.pyc
--rw-rw-rw-   0        0        0     1493 2022-05-21 09:42:07.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/crypto.cpython-39.pyc
--rw-rw-rw-   0        0        0      422 2023-04-01 19:36:02.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/encoding.cpython-310.pyc
--rw-rw-rw-   0        0        0      740 2023-02-18 10:07:24.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/importing.cpython-310.pyc
--rw-rw-rw-   0        0        0      760 2022-06-05 10:59:00.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/importing.cpython-39.pyc
--rw-rw-rw-   0        0        0     1029 2023-03-30 21:28:00.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/inspect.cpython-310.pyc
--rw-rw-rw-   0        0        0     2176 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/json.cpython-310.pyc
--rw-rw-rw-   0        0        0     2176 2022-05-09 11:55:14.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/json.cpython-39.pyc
--rw-rw-rw-   0        0        0     1641 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/regex.cpython-310.pyc
--rw-rw-rw-   0        0        0     3038 2023-03-25 15:08:07.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/serializers.cpython-310.pyc
--rw-rw-rw-   0        0        0     2653 2022-10-26 19:12:06.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/serializers.cpython-39.pyc
--rw-rw-rw-   0        0        0      566 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/singleton.cpython-310.pyc
--rw-rw-rw-   0        0        0      562 2022-05-09 11:55:14.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/singleton.cpython-39.pyc
--rw-rw-rw-   0        0        0      380 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0      378 2022-10-06 18:58:47.000000 starlette_web-0.1.1/starlette_web/common/utils/__pycache__/urls.cpython-39.pyc
--rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.1/starlette_web/common/utils/choices.py
--rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.1/starlette_web/common/utils/crypto.py
--rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.1/starlette_web/common/utils/encoding.py
--rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.1/starlette_web/common/utils/importing.py
--rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/utils/inspect.py
--rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/common/utils/json.py
--rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/common/utils/regex.py
--rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.1/starlette_web/common/utils/serializers.py
--rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/common/utils/singleton.py
--rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/common/utils/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.422876 starlette_web-0.1.1/starlette_web/common/ws/
--rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.1/starlette_web/common/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.424871 starlette_web-0.1.1/starlette_web/common/ws/__pycache__/
--rw-rw-rw-   0        0        0      154 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/common/ws/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      152 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/common/ws/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6256 2023-03-15 20:40:28.000000 starlette_web-0.1.1/starlette_web/common/ws/__pycache__/base_endpoint.cpython-310.pyc
--rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.1/starlette_web/common/ws/base_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.424871 starlette_web-0.1.1/starlette_web/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.428581 starlette_web-0.1.1/starlette_web/contrib/__pycache__/
--rw-rw-rw-   0        0        0      152 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      150 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/contrib/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.433685 starlette_web-0.1.1/starlette_web/contrib/admin/
--rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.436677 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/
--rw-rw-rw-   0        0        0      343 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3624 2023-03-25 15:08:25.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/admin.cpython-310.pyc
--rw-rw-rw-   0        0        0      873 2023-03-03 20:07:29.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0     2702 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/auth_provider.cpython-310.pyc
--rw-rw-rw-   0        0        0     4061 2023-03-19 16:56:53.000000 starlette_web-0.1.1/starlette_web/contrib/admin/__pycache__/middleware.cpython-310.pyc
--rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.1/starlette_web/contrib/admin/admin.py
--rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/admin/apps.py
--rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/admin/auth_provider.py
--rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.1/starlette_web/contrib/admin/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.439668 starlette_web-0.1.1/starlette_web/contrib/apispec/
--rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.449759 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/
--rw-rw-rw-   0        0        0      160 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      158 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1402 2023-03-08 06:45:38.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0     4010 2023-03-03 20:07:28.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/introspection.cpython-310.pyc
--rw-rw-rw-   0        0        0     3932 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/introspection.cpython-39.pyc
--rw-rw-rw-   0        0        0      414 2023-02-16 20:09:57.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/routes.cpython-310.pyc
--rw-rw-rw-   0        0        0      395 2022-10-26 19:12:07.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/routes.cpython-39.pyc
--rw-rw-rw-   0        0        0     1743 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     1824 2022-10-26 19:13:18.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/__pycache__/views.cpython-39.pyc
--rw-rw-rw-   0        0        0     1524 2023-03-04 19:50:46.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/apps.py
--rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/introspection.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.450756 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/
--rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.453748 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__pycache__/
--rw-rw-rw-   0        0        0      553 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      549 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1756 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__pycache__/converters.cpython-310.pyc
--rw-rw-rw-   0        0        0     1750 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/__pycache__/converters.cpython-39.pyc
--rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/converters.py
--rw-rw-rw-   0        0        0      269 2023-02-16 20:03:10.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/routes.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.214099 starlette_web-0.1.1/starlette_web/contrib/apispec/static/
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.453748 starlette_web-0.1.1/starlette_web/contrib/apispec/static/apispec/
--rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/static/apispec/redoc.js
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.216786 starlette_web-0.1.1/starlette_web/contrib/apispec/templates/
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.455733 starlette_web-0.1.1/starlette_web/contrib/apispec/templates/apispec/
--rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/templates/apispec/redoc.html
--rw-rw-rw-   0        0        0     1535 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/apispec/views.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.466470 starlette_web-0.1.1/starlette_web/contrib/auth/
--rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.486063 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/
--rw-rw-rw-   0        0        0      157 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      155 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3762 2023-02-26 21:37:01.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/admin.cpython-310.pyc
--rw-rw-rw-   0        0        0      629 2023-03-17 21:18:30.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0     3871 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/backend.cpython-310.pyc
--rw-rw-rw-   0        0        0     3283 2022-09-04 14:01:22.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/backend.cpython-39.pyc
--rw-rw-rw-   0        0        0     4641 2023-03-25 15:08:21.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/hashers.cpython-310.pyc
--rw-rw-rw-   0        0        0     4596 2022-09-03 11:52:05.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/hashers.cpython-39.pyc
--rw-rw-rw-   0        0        0     4080 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/models.cpython-310.pyc
--rw-rw-rw-   0        0        0     4018 2022-05-21 09:42:07.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/models.cpython-39.pyc
--rw-rw-rw-   0        0        0     3724 2023-03-19 16:56:52.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/password_validation.cpython-310.pyc
--rw-rw-rw-   0        0        0     1000 2023-02-26 15:50:45.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/permissions.cpython-310.pyc
--rw-rw-rw-   0        0        0      994 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/permissions.cpython-39.pyc
--rw-rw-rw-   0        0        0      672 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/routes.cpython-310.pyc
--rw-rw-rw-   0        0        0      670 2022-05-09 11:57:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/routes.cpython-39.pyc
--rw-rw-rw-   0        0        0     3495 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/schemas.cpython-310.pyc
--rw-rw-rw-   0        0        0     3497 2022-10-01 11:05:14.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/schemas.cpython-39.pyc
--rw-rw-rw-   0        0        0     1630 2023-03-19 16:56:52.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     1572 2022-09-03 11:52:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0    16028 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    15818 2022-10-06 18:58:49.000000 starlette_web-0.1.1/starlette_web/contrib/auth/__pycache__/views.cpython-39.pyc
--rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.1/starlette_web/contrib/auth/admin.py
--rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.1/starlette_web/contrib/auth/apps.py
--rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/auth/backend.py
--rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.1/starlette_web/contrib/auth/hashers.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.487060 starlette_web-0.1.1/starlette_web/contrib/auth/management/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.488058 starlette_web-0.1.1/starlette_web/contrib/auth/management/__pycache__/
--rw-rw-rw-   0        0        0      168 2023-02-26 15:51:03.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1633 2023-03-16 18:41:05.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/__pycache__/auth_command_mixin.cpython-310.pyc
--rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/auth_command_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.493406 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.497078 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/__pycache__/
--rw-rw-rw-   0        0        0      177 2023-02-26 15:51:03.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1536 2023-03-16 18:41:05.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/__pycache__/changepassword.cpython-310.pyc
--rw-rw-rw-   0        0        0     1509 2023-03-16 18:41:18.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/__pycache__/createsuperuser.cpython-310.pyc
--rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/changepassword.py
--rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/createsuperuser.py
--rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.1/starlette_web/contrib/auth/models.py
--rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.1/starlette_web/contrib/auth/password_validation.py
--rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.1/starlette_web/contrib/auth/permissions.py
--rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/contrib/auth/routes.py
--rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.1/starlette_web/contrib/auth/schemas.py
--rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.1/starlette_web/contrib/auth/utils.py
--rw-rw-rw-   0        0        0    18290 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/contrib/auth/views.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.500072 starlette_web-0.1.1/starlette_web/contrib/camel_case/
--rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.511195 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/
--rw-rw-rw-   0        0        0      433 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      431 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      785 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/parser.cpython-310.pyc
--rw-rw-rw-   0        0        0      779 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/parser.cpython-39.pyc
--rw-rw-rw-   0        0        0      656 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/renderer.cpython-310.pyc
--rw-rw-rw-   0        0        0      652 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/renderer.cpython-39.pyc
--rw-rw-rw-   0        0        0     3401 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     3401 2022-10-06 18:58:48.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0      374 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/parser.py
--rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/renderer.py
--rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.1/starlette_web/contrib/camel_case/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.511195 starlette_web-0.1.1/starlette_web/contrib/constance/
--rw-rw-rw-   0        0        0     2887 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/contrib/constance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.513192 starlette_web-0.1.1/starlette_web/contrib/constance/__pycache__/
--rw-rw-rw-   0        0        0     2762 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/contrib/constance/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2767 2023-02-20 10:53:40.000000 starlette_web-0.1.1/starlette_web/contrib/constance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.514189 starlette_web-0.1.1/starlette_web/contrib/constance/backends/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.516184 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__pycache__/
--rw-rw-rw-   0        0        0      171 2023-03-12 19:57:38.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      172 2023-02-20 10:53:40.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1830 2023-03-17 16:10:58.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     1812 2023-02-20 10:53:40.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/__pycache__/base.cpython-39.pyc
--rw-rw-rw-   0        0        0     1291 2023-03-16 18:44:56.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/base.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.518178 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/
--rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.525147 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/
--rw-rw-rw-   0        0        0     2362 2023-03-12 19:57:38.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2348 2023-02-20 10:53:40.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      458 2023-03-03 20:07:29.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0      776 2023-03-12 19:57:38.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/models.cpython-310.pyc
--rw-rw-rw-   0        0        0      775 2023-02-20 10:53:40.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__pycache__/models.cpython-39.pyc
--rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/apps.py
--rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/models.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.526050 starlette_web-0.1.1/starlette_web/contrib/postgres/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/contrib/postgres/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.527761 starlette_web-0.1.1/starlette_web/contrib/postgres/__pycache__/
--rw-rw-rw-   0        0        0      161 2023-03-12 19:57:35.000000 starlette_web-0.1.1/starlette_web/contrib/postgres/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4113 2023-04-02 21:14:35.000000 starlette_web-0.1.1/starlette_web/contrib/postgres/__pycache__/channel_layers.cpython-310.pyc
--rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.1/starlette_web/contrib/postgres/channel_layers.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.529757 starlette_web-0.1.1/starlette_web/contrib/redis/
--rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.533748 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/
--rw-rw-rw-   0        0        0      297 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      295 2022-05-14 20:12:19.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5049 2023-04-01 19:37:23.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/cache.cpython-310.pyc
--rw-rw-rw-   0        0        0     5148 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/cache.cpython-39.pyc
--rw-rw-rw-   0        0        0     2747 2023-04-01 19:42:43.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/channel_layers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1447 2023-03-27 18:38:56.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/redislock.cpython-310.pyc
--rw-rw-rw-   0        0        0      957 2022-05-14 20:12:19.000000 starlette_web-0.1.1/starlette_web/contrib/redis/__pycache__/redislock.cpython-39.pyc
--rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.1/starlette_web/contrib/redis/cache.py
--rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.1/starlette_web/contrib/redis/channel_layers.py
--rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.1/starlette_web/contrib/redis/redislock.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.541214 starlette_web-0.1.1/starlette_web/contrib/scheduler/
--rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.542844 starlette_web-0.1.1/starlette_web/contrib/scheduler/__pycache__/
--rw-rw-rw-   0        0        0      162 2023-03-08 06:45:38.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2326 2023-03-08 06:45:38.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/__pycache__/app_settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1510 2023-03-08 06:45:38.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/app_settings.py
--rw-rw-rw-   0        0        0     1641 2023-03-07 06:16:21.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.544838 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/
--rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.546834 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__pycache__/
--rw-rw-rw-   0        0        0      983 2023-03-31 19:13:32.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4965 2023-03-18 14:48:21.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__pycache__/base.cpython-310.pyc
--rw-rw-rw-   0        0        0     5765 2023-03-31 19:15:41.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__pycache__/win32.cpython-310.pyc
--rw-rw-rw-   0        0        0     3889 2023-03-18 14:46:09.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/base.py
--rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/posix.py
--rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.546834 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.549688 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-03-31 19:13:32.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.550690 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.553707 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/__pycache__/
--rw-rw-rw-   0        0        0      182 2023-03-31 19:13:32.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1598 2023-03-31 19:15:41.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/__pycache__/scheduler.cpython-310.pyc
--rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.556832 starlette_web-0.1.1/starlette_web/contrib/staticfiles/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.557404 starlette_web-0.1.1/starlette_web/contrib/staticfiles/__pycache__/
--rw-rw-rw-   0        0        0      164 2023-03-03 20:07:26.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      426 2023-03-03 20:07:26.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.558404 starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.559401 starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.564126 starlette_web-0.1.1/starlette_web/tests/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.1/starlette_web/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.576431 starlette_web-0.1.1/starlette_web/tests/__pycache__/
--rw-rw-rw-   0        0        0      150 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      148 2022-04-30 17:23:58.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      462 2023-03-03 20:07:29.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/apps.cpython-310.pyc
--rw-rw-rw-   0        0        0     6082 2023-03-30 20:59:05.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/conftest.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     5686 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/conftest.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     5634 2022-12-29 14:35:19.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     4064 2023-02-26 14:24:12.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/helpers.cpython-310.pyc
--rw-rw-rw-   0        0        0     4019 2022-05-13 05:58:54.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/helpers.cpython-39.pyc
--rw-rw-rw-   0        0        0     1948 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/mocks.cpython-310.pyc
--rw-rw-rw-   0        0        0     1944 2022-05-14 20:12:19.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/mocks.cpython-39.pyc
--rw-rw-rw-   0        0        0     1393 2023-03-30 19:27:52.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/routes.cpython-310.pyc
--rw-rw-rw-   0        0        0     3219 2023-03-30 20:41:24.000000 starlette_web-0.1.1/starlette_web/tests/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.1/starlette_web/tests/apps.py
--rw-rw-rw-   0        0        0     5416 2023-03-30 20:54:17.000000 starlette_web-0.1.1/starlette_web/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.582002 starlette_web-0.1.1/starlette_web/tests/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.598335 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/
--rw-rw-rw-   0        0        0      158 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      156 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5865 2023-03-30 19:24:17.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_apispec.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     5971 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_apispec.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     5973 2022-10-06 18:58:48.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_apispec.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0    35603 2023-03-30 19:24:17.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_auth.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2932 2022-12-29 14:47:29.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_camel_case.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2932 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_camel_case.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     2960 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_camel_case.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     7108 2023-04-01 18:52:21.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_channels.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2597 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_constance.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2597 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_constance.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     2595 2022-12-29 14:35:22.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_constance.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     2384 2023-03-17 21:18:30.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_password_validators.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     3032 2023-03-28 18:43:45.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_redis_cache.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     3564 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_redis_cache.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     3550 2022-05-14 20:12:19.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_redis_cache.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     1824 2023-03-12 19:57:35.000000 starlette_web-0.1.1/starlette_web/tests/contrib/__pycache__/test_websocket_chat.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0    16358 2023-03-30 19:24:14.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_apispec.py
--rw-rw-rw-   0        0        0    27613 2023-03-30 19:24:14.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_auth.py
--rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_camel_case.py
--rw-rw-rw-   0        0        0     6443 2023-04-01 18:50:52.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_channels.py
--rw-rw-rw-   0        0        0     1139 2022-10-11 21:53:33.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_constance.py
--rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_password_validators.py
--rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.1/starlette_web/tests/contrib/test_redis_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.607222 starlette_web-0.1.1/starlette_web/tests/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.1/starlette_web/tests/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.615659 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/
--rw-rw-rw-   0        0        0      155 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      153 2022-04-30 17:23:59.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     7423 2023-02-26 21:37:01.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_auth_backends.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     7492 2022-12-29 14:45:49.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_auth_backends.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     7414 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_auth_backends.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     9624 2023-03-30 19:23:45.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_base.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2713 2023-03-27 18:38:56.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_base_caches.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1866 2023-03-30 19:24:18.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_service.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1762 2023-03-23 18:13:40.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_settings.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1761 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_settings.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     1767 2022-09-03 11:52:06.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_settings.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0    11469 2023-03-16 18:16:15.000000 starlette_web-0.1.1/starlette_web/tests/core/__pycache__/test_websocket_endpoint.cpython-310-pytest-6.2.5.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.618741 starlette_web-0.1.1/starlette_web/tests/core/helpers/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.1/starlette_web/tests/core/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.620440 starlette_web-0.1.1/starlette_web/tests/core/helpers/__pycache__/
--rw-rw-rw-   0        0        0      163 2023-03-23 18:11:35.000000 starlette_web-0.1.1/starlette_web/tests/core/helpers/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4854 2023-03-30 21:28:01.000000 starlette_web-0.1.1/starlette_web/tests/core/helpers/__pycache__/base_cache_tester.cpython-310.pyc
--rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.1/starlette_web/tests/core/helpers/base_cache_tester.py
--rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.1/starlette_web/tests/core/test_auth_backends.py
--rw-rw-rw-   0        0        0     4741 2022-12-29 14:13:54.000000 starlette_web-0.1.1/starlette_web/tests/core/test_base.py
--rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.1/starlette_web/tests/core/test_base_caches.py
--rw-rw-rw-   0        0        0      867 2023-03-30 19:24:14.000000 starlette_web-0.1.1/starlette_web/tests/core/test_service.py
--rw-rw-rw-   0        0        0      528 2023-03-23 18:13:37.000000 starlette_web-0.1.1/starlette_web/tests/core/test_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.621440 starlette_web-0.1.1/starlette_web/tests/database/
--rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.1/starlette_web/tests/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.625338 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/
--rw-rw-rw-   0        0        0      159 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      157 2022-05-03 16:04:25.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9426 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/test_model_mixin.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     9426 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/test_model_mixin.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     9516 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/test_model_mixin.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     1968 2023-02-26 21:37:01.000000 starlette_web-0.1.1/starlette_web/tests/database/__pycache__/test_nested_transaction.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/tests/database/test_model_mixin.py
--rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.1/starlette_web/tests/database/test_nested_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.627552 starlette_web-0.1.1/starlette_web/tests/files/
--rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.1/starlette_web/tests/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.634986 starlette_web-0.1.1/starlette_web/tests/files/__pycache__/
--rw-rw-rw-   0        0        0      156 2023-03-29 22:19:04.000000 starlette_web-0.1.1/starlette_web/tests/files/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    10028 2023-03-31 18:52:49.000000 starlette_web-0.1.1/starlette_web/tests/files/__pycache__/test_filesystem_storage.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2700 2023-03-30 20:41:25.000000 starlette_web-0.1.1/starlette_web/tests/files/__pycache__/test_media_storage.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.1/starlette_web/tests/files/test_filesystem_storage.py
--rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.1/starlette_web/tests/files/test_media_storage.py
--rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.1/starlette_web/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.238429 starlette_web-0.1.1/starlette_web/tests/management/
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.637979 starlette_web-0.1.1/starlette_web/tests/management/commands/
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.657425 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/
--rw-rw-rw-   0        0        0      784 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_call_command.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0      784 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_call_command.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0      675 2023-02-19 12:39:59.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_call_command.cpython-310.pyc
--rw-rw-rw-   0        0        0      776 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_call_command.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0      667 2022-05-09 11:58:34.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_call_command.cpython-39.pyc
--rw-rw-rw-   0        0        0     1721 2023-03-12 19:57:35.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_channels_publisher.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1612 2023-03-12 19:58:10.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_channels_publisher.cpython-310.pyc
--rw-rw-rw-   0        0        0     1813 2023-03-12 19:57:35.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_channels_subscriber.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1704 2023-03-12 19:58:10.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_channels_subscriber.cpython-310.pyc
--rw-rw-rw-   0        0        0     1133 2023-02-03 14:23:08.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_db.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1113 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_db.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     1024 2023-02-19 12:40:08.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_db.cpython-310.pyc
--rw-rw-rw-   0        0        0     1101 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_db.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     1144 2023-03-26 12:19:31.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_parser.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1144 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_parser.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     1035 2023-03-26 12:19:25.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_parser.cpython-310.pyc
--rw-rw-rw-   0        0        0     1136 2022-05-03 14:51:40.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_parser.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     1027 2022-05-03 18:21:53.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_parser.cpython-39.pyc
--rw-rw-rw-   0        0        0     1235 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_redis.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0      789 2022-05-13 05:46:14.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_redis.cpython-39.pyc
--rw-rw-rw-   0        0        0      956 2023-03-03 21:53:04.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/__pycache__/test_write.cpython-310.pyc
--rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/test_call_command.py
--rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/test_channels_publisher.py
--rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/test_channels_subscriber.py
--rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/test_db.py
--rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.1/starlette_web/tests/management/commands/test_parser.py
--rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.1/starlette_web/tests/mocks.py
--rw-rw-rw-   0        0        0     1640 2023-03-30 19:27:49.000000 starlette_web-0.1.1/starlette_web/tests/routes.py
--rw-rw-rw-   0        0        0     4649 2023-03-30 20:25:32.000000 starlette_web-0.1.1/starlette_web/tests/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.664406 starlette_web-0.1.1/starlette_web/tests/utils/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.1/starlette_web/tests/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.673383 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/
--rw-rw-rw-   0        0        0      156 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      154 2022-04-30 17:24:00.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5897 2023-03-19 16:56:53.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_auth_hasher.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     5897 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_auth_hasher.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     6055 2022-05-21 09:42:08.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_auth_hasher.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     1618 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_json.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     1618 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_json.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     1622 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_json.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     4722 2023-03-23 18:11:35.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_redis_pattern_matcher.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2792 2022-12-29 14:47:30.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_serializers.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2792 2022-12-29 14:45:50.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_serializers.cpython-310-pytest-7.2.0.pyc
--rw-rw-rw-   0        0        0     2812 2022-05-13 05:58:55.000000 starlette_web-0.1.1/starlette_web/tests/utils/__pycache__/test_serializers.cpython-39-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.1/starlette_web/tests/utils/test_auth_hasher.py
--rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/tests/utils/test_json.py
--rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.1/starlette_web/tests/utils/test_redis_pattern_matcher.py
--rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.1/starlette_web/tests/utils/test_serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.675377 starlette_web-0.1.1/starlette_web/tests/views/
--rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.1/starlette_web/tests/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.681362 starlette_web-0.1.1/starlette_web/tests/views/__pycache__/
--rw-rw-rw-   0        0        0      542 2023-03-23 18:11:39.000000 starlette_web-0.1.1/starlette_web/tests/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2278 2023-03-23 18:11:39.000000 starlette_web-0.1.1/starlette_web/tests/views/__pycache__/http.cpython-310.pyc
--rw-rw-rw-   0        0        0     7916 2023-03-26 09:54:57.000000 starlette_web-0.1.1/starlette_web/tests/views/__pycache__/websocket.cpython-310.pyc
--rw-rw-rw-   0        0        0     2098 2023-03-23 18:10:52.000000 starlette_web-0.1.1/starlette_web/tests/views/http.py
--rw-rw-rw-   0        0        0     6815 2023-03-26 09:54:37.000000 starlette_web-0.1.1/starlette_web/tests/views/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.684353 starlette_web-0.1.1/starlette_web/tests/websockets/
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.685367 starlette_web-0.1.1/starlette_web/tests/websockets/__pycache__/
--rw-rw-rw-   0        0        0     1827 2023-03-30 19:23:45.000000 starlette_web-0.1.1/starlette_web/tests/websockets/__pycache__/test_websocket_chat.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0    11475 2023-03-30 19:23:45.000000 starlette_web-0.1.1/starlette_web/tests/websockets/__pycache__/test_websocket_endpoint.cpython-310-pytest-6.2.5.pyc
--rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.1/starlette_web/tests/websockets/test_websocket_chat.py
--rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.1/starlette_web/tests/websockets/test_websocket_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:40:47.253137 starlette_web-0.1.1/starlette_web.egg-info/
--rw-rw-rw-   0        0        0     3245 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    29226 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      789 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-02 21:40:47.000000 starlette_web-0.1.1/starlette_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2022-04-25 19:06:18.000000 starlette_web-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       75 2023-04-13 19:30:53.000000 starlette_web-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3245 2023-04-13 19:30:56.476963 starlette_web-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1870 2023-04-13 19:30:56.476963 starlette_web-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       75 2022-04-25 19:06:18.000000 starlette_web-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/
+-rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/common/
+-rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/common/__init__.py
+-rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/app.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/common/authorization/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.2/starlette_web/common/authorization/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/backends.py
+-rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/base_user.py
+-rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/permissions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.327060 starlette_web-0.1.2/starlette_web/common/caches/
+-rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.2/starlette_web/common/caches/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/caches/base.py
+-rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.2/starlette_web/common/caches/base_lock.py
+-rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.2/starlette_web/common/caches/cache_handler.py
+-rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.2/starlette_web/common/caches/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/channels/
+-rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.2/starlette_web/common/channels/base.py
+-rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/event.py
+-rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.2/starlette_web/common/channels/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/channels/layers/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/base.py
+-rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/conf/
+-rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/conf/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.2/starlette_web/common/conf/app_manager.py
+-rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/common/conf/base_app_config.py
+-rw-rw-rw-   0        0        0     1752 2023-04-06 19:27:41.000000 starlette_web-0.1.2/starlette_web/common/conf/global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/database/
+-rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/database/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/common/database/columns.py
+-rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/database/model_base.py
+-rw-rw-rw-   0        0        0     9279 2023-04-09 22:15:24.000000 starlette_web-0.1.2/starlette_web/common/database/model_mixin.py
+-rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.2/starlette_web/common/database/session_maker.py
+-rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.2/starlette_web/common/database/types.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/email/
+-rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.2/starlette_web/common/email/__init__.py
+-rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.2/starlette_web/common/email/base_sender.py
+-rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.2/starlette_web/common/email/email_manager.py
+-rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/email/smtp.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/files/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/common/files/__init__.py
+-rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/files/cache.py
+-rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.2/starlette_web/common/files/filelock.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/files/storages/
+-rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.2/starlette_web/common/files/storages/__init__.py
+-rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.2/starlette_web/common/files/storages/base.py
+-rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.2/starlette_web/common/files/storages/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/http/
+-rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.2/starlette_web/common/http/__init__.py
+-rw-rw-rw-   0        0        0     6474 2023-03-26 10:02:27.000000 starlette_web-0.1.2/starlette_web/common/http/base_endpoint.py
+-rw-rw-rw-   0        0        0     4338 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/common/http/exception_handlers.py
+-rw-rw-rw-   0        0        0     4287 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/http/exceptions.py
+-rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/http/renderers.py
+-rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/http/responses.py
+-rw-rw-rw-   0        0        0      829 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/http/schemas.py
+-rw-rw-rw-   0        0        0      942 2023-03-14 17:15:47.000000 starlette_web-0.1.2/starlette_web/common/http/statuses.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/i18n/
+-rw-rw-rw-   0        0        0      163 2022-09-03 15:11:31.000000 starlette_web-0.1.2/starlette_web/common/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/management/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.2/starlette_web/common/management/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/management/admin_util.py
+-rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.2/starlette_web/common/management/alembic_mixin.py
+-rw-rw-rw-   0        0        0     6023 2023-04-13 17:02:30.000000 starlette_web-0.1.2/starlette_web/common/management/base.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.367331 starlette_web-0.1.2/starlette_web/common/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.2/starlette_web/common/management/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.367331 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/admin.py
+-rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/apps.py
+-rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/models.py
+-rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/routes.py
+-rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/views.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.377349 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-04-03 20:19:20.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/asgi.py
+-rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/command.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.377349 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-04-13 18:30:43.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/routes.py
+-rw-rw-rw-   0        0        0     3441 2023-04-06 18:51:17.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-04-06 16:46:50.000000 starlette_web-0.1.2/starlette_web/common/management/commands/makemigrations.py
+-rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.2/starlette_web/common/management/commands/migrate.py
+-rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/management/commands/startapp.py
+-rw-rw-rw-   0        0        0     3800 2023-04-06 16:47:27.000000 starlette_web-0.1.2/starlette_web/common/management/commands/startproject.py
+-rw-rw-rw-   0        0        0     2019 2023-04-08 06:35:50.000000 starlette_web-0.1.2/starlette_web/common/management/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/common/utils/
+-rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.2/starlette_web/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.2/starlette_web/common/utils/choices.py
+-rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.2/starlette_web/common/utils/crypto.py
+-rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.2/starlette_web/common/utils/encoding.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.2/starlette_web/common/utils/importing.py
+-rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/utils/inspect.py
+-rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/utils/json.py
+-rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/utils/regex.py
+-rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.2/starlette_web/common/utils/serializers.py
+-rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/utils/singleton.py
+-rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/utils/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/common/ws/
+-rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/common/ws/__init__.py
+-rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.2/starlette_web/common/ws/base_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/admin/
+-rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/admin/__init__.py
+-rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.2/starlette_web/contrib/admin/admin.py
+-rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/admin/apps.py
+-rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/admin/auth_provider.py
+-rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/admin/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/
+-rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-04-03 20:01:29.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/apps.py
+-rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/introspection.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/
+-rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/__init__.py
+-rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/converters.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.287172 starlette_web-0.1.2/starlette_web/contrib/apispec/static/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/
+-rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/redoc.js
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.297397 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/
+-rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/redoc.html
+-rw-rw-rw-   0        0        0     1889 2023-04-13 18:25:49.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/views.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.407376 starlette_web-0.1.2/starlette_web/contrib/auth/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.2/starlette_web/contrib/auth/__init__.py
+-rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.2/starlette_web/contrib/auth/admin.py
+-rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.2/starlette_web/contrib/auth/apps.py
+-rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/backend.py
+-rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.2/starlette_web/contrib/auth/hashers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/auth/management/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/auth_command_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/changepassword.py
+-rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/createsuperuser.py
+-rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/contrib/auth/models.py
+-rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/auth/password_validation.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/contrib/auth/permissions.py
+-rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/contrib/auth/routes.py
+-rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.2/starlette_web/contrib/auth/schemas.py
+-rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/auth/utils.py
+-rw-rw-rw-   0        0        0    18290 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/contrib/auth/views.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/camel_case/
+-rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/parser.py
+-rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/renderer.py
+-rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/constance/
+-rw-rw-rw-   0        0        0     3754 2023-04-06 19:52:27.000000 starlette_web-0.1.2/starlette_web/contrib/constance/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-06 20:13:04.000000 starlette_web-0.1.2/starlette_web/contrib/constance/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/constance/backends/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/base.py
+-rw-rw-rw-   0        0        0     1656 2023-04-06 20:18:43.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/caching_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/
+-rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/apps.py
+-rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/models.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/postgres/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/contrib/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.2/starlette_web/contrib/postgres/channel_layers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/redis/
+-rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.2/starlette_web/contrib/redis/__init__.py
+-rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.2/starlette_web/contrib/redis/cache.py
+-rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.2/starlette_web/contrib/redis/channel_layers.py
+-rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.2/starlette_web/contrib/redis/redislock.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/scheduler/
+-rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/app_settings.py
+-rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/
+-rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/__init__.py
+-rw-rw-rw-   0        0        0     3867 2023-04-09 17:22:30.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/base.py
+-rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/posix.py
+-rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.447104 starlette_web-0.1.2/starlette_web/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/tests/apps.py
+-rw-rw-rw-   0        0        0     5474 2023-04-06 20:04:06.000000 starlette_web-0.1.2/starlette_web/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/contrib/__init__.py
+-rw-rw-rw-   0        0        0    16572 2023-04-13 18:40:01.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_apispec.py
+-rw-rw-rw-   0        0        0    27613 2023-03-30 19:24:14.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_auth.py
+-rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_camel_case.py
+-rw-rw-rw-   0        0        0     7677 2023-04-05 19:51:46.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_channels.py
+-rw-rw-rw-   0        0        0     1141 2023-04-06 19:30:04.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_constance.py
+-rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_password_validators.py
+-rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_redis_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/core/helpers/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/tests/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/tests/core/helpers/base_cache_tester.py
+-rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/tests/core/test_auth_backends.py
+-rw-rw-rw-   0        0        0     4741 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/tests/core/test_base.py
+-rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.2/starlette_web/tests/core/test_base_caches.py
+-rw-rw-rw-   0        0        0      867 2023-03-30 19:24:14.000000 starlette_web-0.1.2/starlette_web/tests/core/test_service.py
+-rw-rw-rw-   0        0        0      528 2023-03-23 18:13:37.000000 starlette_web-0.1.2/starlette_web/tests/core/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/database/
+-rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.2/starlette_web/tests/database/__init__.py
+-rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/database/test_model_mixin.py
+-rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/tests/database/test_nested_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.467066 starlette_web-0.1.2/starlette_web/tests/files/
+-rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.2/starlette_web/tests/files/__init__.py
+-rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.2/starlette_web/tests/files/test_filesystem_storage.py
+-rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.2/starlette_web/tests/files/test_media_storage.py
+-rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.2/starlette_web/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.307223 starlette_web-0.1.2/starlette_web/tests/management/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.467066 starlette_web-0.1.2/starlette_web/tests/management/commands/
+-rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_call_command.py
+-rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_publisher.py
+-rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_subscriber.py
+-rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_db.py
+-rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_parser.py
+-rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.2/starlette_web/tests/mocks.py
+-rw-rw-rw-   0        0        0     1641 2023-04-13 18:29:48.000000 starlette_web-0.1.2/starlette_web/tests/routes.py
+-rw-rw-rw-   0        0        0     4689 2023-04-06 19:58:52.000000 starlette_web-0.1.2/starlette_web/tests/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/utils/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_auth_hasher.py
+-rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_json.py
+-rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_redis_pattern_matcher.py
+-rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/views/
+-rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.2/starlette_web/tests/views/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-03-23 18:10:52.000000 starlette_web-0.1.2/starlette_web/tests/views/http.py
+-rw-rw-rw-   0        0        0     6815 2023-03-26 09:54:37.000000 starlette_web-0.1.2/starlette_web/tests/views/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/websockets/
+-rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_chat.py
+-rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web.egg-info/
+-rw-rw-rw-   0        0        0     3245 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9087 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      817 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/top_level.txt
```

### Comparing `starlette_web-0.1.1/LICENSE` & `starlette_web-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/PKG-INFO` & `starlette_web-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: starlette_web
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Home-page: https://github.com/dolamroth/starlette-web
 Author: Sergey Sayamov
 Author-email: dolamroth@mail.ru
 License: MIT License
-Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.2.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
```

### Comparing `starlette_web-0.1.1/README.md` & `starlette_web-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/setup.cfg` & `starlette_web-0.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7461 726c 6574 7465 5f77 6562   = starlette_web
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
+00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
 00000040: 2041 7379 6e63 6872 6f6e 6f75 7320 7765   Asynchronous we
 00000050: 6220 6672 616d 6577 6f72 6b2c 2062 6173  b framework, bas
 00000060: 6564 206f 6e20 5374 6172 6c65 7474 6520  ed on Starlette 
 00000070: 616e 6420 696e 7370 6972 6564 2062 7920  and inspired by 
 00000080: 446a 616e 676f 0d0a 6c6f 6e67 5f64 6573  Django..long_des
 00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
 000000a0: 2052 4541 444d 452e 6d64 0d0a 7572 6c20   README.md..url 
@@ -16,15 +16,15 @@
 000000f0: 7961 6d6f 760d 0a61 7574 686f 725f 656d  yamov..author_em
 00000100: 6169 6c20 3d20 646f 6c61 6d72 6f74 6840  ail = dolamroth@
 00000110: 6d61 696c 2e72 750d 0a64 6f77 6e6c 6f61  mail.ru..downloa
 00000120: 645f 7572 6c20 3d20 6874 7470 733a 2f2f  d_url = https://
 00000130: 6769 7468 7562 2e63 6f6d 2f64 6f6c 616d  github.com/dolam
 00000140: 726f 7468 2f73 7461 726c 6574 7465 2d77  roth/starlette-w
 00000150: 6562 2f61 7263 6869 7665 2f72 6566 732f  eb/archive/refs/
-00000160: 7461 6773 2f30 2e31 2e31 2e74 6172 2e67  tags/0.1.1.tar.g
+00000160: 7461 6773 2f30 2e31 2e32 2e74 6172 2e67  tags/0.1.2.tar.g
 00000170: 7a0d 0a6c 6963 656e 7365 203d 204d 4954  z..license = MIT
 00000180: 204c 6963 656e 7365 0d0a 636c 6173 7369   License..classi
 00000190: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
 000001a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000001b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
 000001c0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
@@ -62,54 +62,56 @@
 000003d0: 332c 3c30 2e32 340d 0a09 7079 7468 6f6e  3,<0.24...python
 000003e0: 2d64 6f74 656e 763e 3d30 2e32 312c 3c30  -dotenv>=0.21,<0
 000003f0: 2e32 320d 0a09 7472 6163 6562 6163 6b2d  .22...traceback-
 00000400: 7769 7468 2d76 6172 6961 626c 6573 3e3d  with-variables>=
 00000410: 322e 302e 342c 3c32 2e31 0d0a 0961 696f  2.0.4,<2.1...aio
 00000420: 736d 7470 6c69 623e 3d32 2e30 2e31 2c3c  smtplib>=2.0.1,<
 00000430: 322e 310d 0a09 6669 6c65 6c6f 636b 3e3d  2.1...filelock>=
-00000440: 332e 3130 2e37 2c3c 332e 3131 0d0a 0d0a  3.10.7,<3.11....
-00000450: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000460: 732e 6669 6e64 5d0d 0a65 7863 6c75 6465  s.find]..exclude
-00000470: 203d 200d 0a09 7465 7374 730d 0a0d 0a5b   = ...tests....[
-00000480: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000490: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000004a0: 6372 6970 7473 203d 200d 0a09 7374 6172  cripts = ...star
-000004b0: 6c65 7474 652d 7765 622d 6164 6d69 6e20  lette-web-admin 
-000004c0: 3d20 7374 6172 6c65 7474 655f 7765 622e  = starlette_web.
-000004d0: 636f 6d6d 6f6e 2e6d 616e 6167 656d 656e  common.managemen
-000004e0: 742e 6164 6d69 6e5f 7574 696c 3a6d 6169  t.admin_util:mai
-000004f0: 6e0d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  n....[options.ex
-00000500: 7472 6173 5f72 6571 7569 7265 5d0d 0a61  tras_require]..a
-00000510: 7069 7370 6563 203d 200d 0a09 6170 6973  pispec = ...apis
-00000520: 7065 633e 3d36 2e30 2c3c 362e 310d 0a09  pec>=6.0,<6.1...
-00000530: 7079 7961 6d6c 3e3d 362e 302c 3c36 2e31  pyyaml>=6.0,<6.1
-00000540: 0d0a 096f 7065 6e61 7069 2d73 7065 632d  ...openapi-spec-
-00000550: 7661 6c69 6461 746f 723e 3d30 2e35 2e35  validator>=0.5.5
-00000560: 2c3c 302e 360d 0a61 646d 696e 203d 200d  ,<0.6..admin = .
-00000570: 0a09 7374 6172 6c65 7474 652d 6164 6d69  ..starlette-admi
-00000580: 6e3e 3d30 2e37 2e30 2c3c 302e 380d 0a61  n>=0.7.0,<0.8..a
-00000590: 7574 6820 3d20 0d0a 0950 794a 5754 3e3d  uth = ...PyJWT>=
-000005a0: 322e 362c 3c32 2e37 0d0a 706f 7374 6772  2.6,<2.7..postgr
-000005b0: 6573 203d 200d 0a09 6173 796e 6370 673e  es = ...asyncpg>
-000005c0: 3d30 2e32 372c 3c30 2e32 380d 0a72 6564  =0.27,<0.28..red
-000005d0: 6973 203d 200d 0a09 7265 6469 733e 3d34  is = ...redis>=4
-000005e0: 2e35 2e34 2c3c 342e 360d 0a73 6368 6564  .5.4,<4.6..sched
-000005f0: 756c 6572 203d 200d 0a09 6372 6f6e 6974  uler = ...cronit
-00000600: 6572 3e3d 312e 332e 382c 3c31 2e34 0d0a  er>=1.3.8,<1.4..
-00000610: 0970 792d 7769 6e2d 7461 736b 2d73 6368  .py-win-task-sch
-00000620: 6564 756c 6572 3d3d 302e 312e 303b 2073  eduler==0.1.0; s
-00000630: 7973 5f70 6c61 7466 6f72 6d20 3d3d 2027  ys_platform == '
-00000640: 7769 6e33 3227 0d0a 6465 706c 6f79 203d  win32'..deploy =
-00000650: 200d 0a09 6775 6e69 636f 726e 3e3d 3230   ...gunicorn>=20
-00000660: 2e31 2e30 2c3c 3230 2e32 0d0a 6465 7665  .1.0,<20.2..deve
-00000670: 6c6f 7020 3d20 0d0a 0962 6c61 636b 7e3d  lop = ...black~=
-00000680: 3232 2e31 302e 300d 0a74 6573 7469 6e67  22.10.0..testing
-00000690: 203d 200d 0a09 7079 7465 7374 3e3d 362e   = ...pytest>=6.
-000006a0: 322c 3c36 2e33 0d0a 0963 6f76 6572 6167  2,<6.3...coverag
-000006b0: 653e 3d36 2e32 2c3c 362e 330d 0a09 7073  e>=6.2,<6.3...ps
-000006c0: 7963 6f70 6732 2d62 696e 6172 793e 3d32  ycopg2-binary>=2
-000006d0: 2e39 2c3c 322e 3130 0d0a 0972 6571 7565  .9,<2.10...reque
-000006e0: 7374 733e 3d32 2e32 382c 3c32 2e32 390d  sts>=2.28,<2.29.
-000006f0: 0a09 666c 616b 6538 3e3d 342e 302c 3c34  ..flake8>=4.0,<4
-00000700: 2e31 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .1....[egg_info]
-00000710: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000720: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000440: 332e 3130 2e37 2c3c 332e 3131 0d0a 096d  3.10.7,<3.11...m
+00000450: 6172 7368 6d61 6c6c 6f77 3e3d 332e 3139  arshmallow>=3.19
+00000460: 2e30 2c3c 332e 3230 0d0a 0d0a 5b6f 7074  .0,<3.20....[opt
+00000470: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000480: 6e64 5d0d 0a65 7863 6c75 6465 203d 200d  nd]..exclude = .
+00000490: 0a09 7465 7374 730d 0a0d 0a5b 6f70 7469  ..tests....[opti
+000004a0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000004b0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+000004c0: 7473 203d 200d 0a09 7374 6172 6c65 7474  ts = ...starlett
+000004d0: 652d 7765 622d 6164 6d69 6e20 3d20 7374  e-web-admin = st
+000004e0: 6172 6c65 7474 655f 7765 622e 636f 6d6d  arlette_web.comm
+000004f0: 6f6e 2e6d 616e 6167 656d 656e 742e 6164  on.management.ad
+00000500: 6d69 6e5f 7574 696c 3a6d 6169 6e0d 0a0d  min_util:main...
+00000510: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000520: 5f72 6571 7569 7265 5d0d 0a61 7069 7370  _require]..apisp
+00000530: 6563 203d 200d 0a09 6170 6973 7065 633e  ec = ...apispec>
+00000540: 3d36 2e33 2e30 2c3c 362e 340d 0a09 7079  =6.3.0,<6.4...py
+00000550: 7961 6d6c 3e3d 362e 302c 3c36 2e31 0d0a  yaml>=6.0,<6.1..
+00000560: 096f 7065 6e61 7069 2d73 7065 632d 7661  .openapi-spec-va
+00000570: 6c69 6461 746f 723e 3d30 2e35 2e36 2c3c  lidator>=0.5.6,<
+00000580: 302e 360d 0a61 646d 696e 203d 200d 0a09  0.6..admin = ...
+00000590: 7374 6172 6c65 7474 652d 6164 6d69 6e3e  starlette-admin>
+000005a0: 3d30 2e37 2e30 2c3c 302e 390d 0a61 7574  =0.7.0,<0.9..aut
+000005b0: 6820 3d20 0d0a 0950 794a 5754 3e3d 322e  h = ...PyJWT>=2.
+000005c0: 362c 3c32 2e37 0d0a 706f 7374 6772 6573  6,<2.7..postgres
+000005d0: 203d 200d 0a09 6173 796e 6370 673e 3d30   = ...asyncpg>=0
+000005e0: 2e32 372c 3c30 2e32 380d 0a72 6564 6973  .27,<0.28..redis
+000005f0: 203d 200d 0a09 7265 6469 733e 3d34 2e35   = ...redis>=4.5
+00000600: 2e34 2c3c 342e 360d 0a73 6368 6564 756c  .4,<4.6..schedul
+00000610: 6572 203d 200d 0a09 6372 6f6e 6974 6572  er = ...croniter
+00000620: 3e3d 312e 332e 382c 3c31 2e34 0d0a 0970  >=1.3.8,<1.4...p
+00000630: 792d 7769 6e2d 7461 736b 2d73 6368 6564  y-win-task-sched
+00000640: 756c 6572 3d3d 302e 312e 303b 2073 7973  uler==0.1.0; sys
+00000650: 5f70 6c61 7466 6f72 6d20 3d3d 2027 7769  _platform == 'wi
+00000660: 6e33 3227 0d0a 6465 706c 6f79 203d 200d  n32'..deploy = .
+00000670: 0a09 6775 6e69 636f 726e 3e3d 3230 2e31  ..gunicorn>=20.1
+00000680: 2e30 2c3c 3230 2e32 0d0a 6465 7665 6c6f  .0,<20.2..develo
+00000690: 7020 3d20 0d0a 0962 6c61 636b 7e3d 3232  p = ...black~=22
+000006a0: 2e31 302e 300d 0a74 6573 7469 6e67 203d  .10.0..testing =
+000006b0: 200d 0a09 7079 7465 7374 3e3d 362e 322c   ...pytest>=6.2,
+000006c0: 3c36 2e33 0d0a 0963 6f76 6572 6167 653e  <6.3...coverage>
+000006d0: 3d36 2e32 2c3c 362e 330d 0a09 7073 7963  =6.2,<6.3...psyc
+000006e0: 6f70 6732 2d62 696e 6172 793e 3d32 2e39  opg2-binary>=2.9
+000006f0: 2c3c 322e 3130 0d0a 0972 6571 7565 7374  ,<2.10...request
+00000700: 733e 3d32 2e32 382c 3c32 2e32 390d 0a09  s>=2.28,<2.29...
+00000710: 666c 616b 6538 3e3d 342e 302c 3c34 2e31  flake8>=4.0,<4.1
+00000720: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000730: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000740: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `starlette_web-0.1.1/starlette_web/common/app.py` & `starlette_web-0.1.2/starlette_web/common/app.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/authorization/backends.py` & `starlette_web-0.1.2/starlette_web/common/authorization/backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/authorization/permissions.py` & `starlette_web-0.1.2/starlette_web/common/authorization/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/caches/base.py` & `starlette_web-0.1.2/starlette_web/common/caches/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/caches/base_lock.py` & `starlette_web-0.1.2/starlette_web/common/caches/base_lock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/caches/cache_handler.py` & `starlette_web-0.1.2/starlette_web/common/caches/cache_handler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/caches/local_memory.py` & `starlette_web-0.1.2/starlette_web/common/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/channels/base.py` & `starlette_web-0.1.2/starlette_web/common/channels/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/channels/layers/base.py` & `starlette_web-0.1.2/starlette_web/common/channels/layers/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/channels/layers/local_memory.py` & `starlette_web-0.1.2/starlette_web/common/channels/layers/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/conf/__init__.py` & `starlette_web-0.1.2/starlette_web/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/conf/app_manager.py` & `starlette_web-0.1.2/starlette_web/common/conf/app_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections import OrderedDict
 from importlib import import_module
 
 from starlette_web.common.conf import settings
 from starlette_web.common.conf.base_app_config import BaseAppConfig
 from starlette_web.common.http.exceptions import ImproperlyConfigured
-from starlette_web.common.utils.importing import import_string
 
 
 class AppManager:
     """
     A project-wide manager for installed modules (apps, in django terminology).
     Dynamically introspects %module_name%/apps.py and runs apps' own
     initializations and checks. Called at Starlette app initialization.
@@ -20,19 +19,30 @@
         self._apps_registered = False
 
     def register_apps(self):
         if self._apps_registered:
             return
 
         for installed_app in settings.INSTALLED_APPS:
+            _module = import_module(installed_app)
+            if not _module.__file__:
+                raise ImproperlyConfigured(
+                    details=f"App {installed_app} must contain an __init__.py file."
+                )
+
+            try:
+                _app_module = import_module(installed_app + ".apps")
+            except (SystemError, ImportError) as exc:
+                raise ImproperlyConfigured(details=str(exc)) from exc
+
             try:
-                AppConfig = import_string(installed_app + ".apps.AppConfig")
+                AppConfig = getattr(_app_module, "AppConfig")
                 if BaseAppConfig not in AppConfig.__mro__:
                     raise AssertionError
-            except (SystemError, ImportError, AssertionError) as exc:
+            except (AttributeError, AssertionError) as exc:
                 raise ImproperlyConfigured(
                     details=f"App {installed_app} must define apps.AppConfig class, inherited "
                     f"from starlette_web.common.conf.base_app_config.BaseAppConfig"
                 ) from exc
 
             app_config: BaseAppConfig = AppConfig()
             if app_config.app_name in self.app_names.keys():
```

### Comparing `starlette_web-0.1.1/starlette_web/common/conf/global_settings.py` & `starlette_web-0.1.2/starlette_web/common/conf/global_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,10 +56,16 @@
 # see https://pyjwt.readthedocs.io/en/latest/algorithms.html for details
 AUTH_JWT_EXPIRES_IN = 300  # 5 min
 AUTH_JWT_REFRESH_EXPIRES_IN = 30 * 24 * 3600  # 30 days
 AUTH_JWT_ALGORITHM = "HS512"
 AUTH_INVITE_LINK_EXPIRES_IN = 3 * 24 * 3600  # 3 day
 AUTH_RESET_PASSWORD_LINK_EXPIRES_IN = 3 * 3600  # 3 hours
 
+# Contrib.constance
+
+CONSTANCE_CONFIG = {}
+CONSTANCE_DATABASE_CACHE_BACKEND = None
+CONSTANCE_BACKEND = None
+
 # Contrib.scheduler
 
 PERIODIC_JOBS_BACKEND = None
```

### Comparing `starlette_web-0.1.1/starlette_web/common/database/columns.py` & `starlette_web-0.1.2/starlette_web/common/database/columns.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/database/model_mixin.py` & `starlette_web-0.1.2/starlette_web/common/database/model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,16 @@
                 filters.append(getattr(cls, field) > filter_value)
             elif criteria == "lt":
                 filters.append(getattr(cls, field) < filter_value)
             elif criteria == "is":
                 filters.append(getattr(cls, field).is_(filter_value))
             elif criteria == "in":
                 filters.append(getattr(cls, field).in_(filter_value))
+            elif criteria == "notin":
+                filters.append(getattr(cls, field).notin_(filter_value))
             elif criteria == "inarr":
                 filters.append(getattr(cls, field).contains([filter_value]))
             elif criteria == "icontains":
                 filters.append(getattr(cls, field).ilike(f"%{filter_value}%"))
             elif criteria == "ne":
                 filters.append(getattr(cls, field) != filter_value)
             else:
```

### Comparing `starlette_web-0.1.1/starlette_web/common/database/session_maker.py` & `starlette_web-0.1.2/starlette_web/common/database/session_maker.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/database/types.py` & `starlette_web-0.1.2/starlette_web/common/database/types.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/email/base_sender.py` & `starlette_web-0.1.2/starlette_web/common/email/base_sender.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/email/email_manager.py` & `starlette_web-0.1.2/starlette_web/common/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/email/smtp.py` & `starlette_web-0.1.2/starlette_web/common/email/smtp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/files/cache.py` & `starlette_web-0.1.2/starlette_web/common/files/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/files/filelock.py` & `starlette_web-0.1.2/starlette_web/common/files/filelock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/files/storages/base.py` & `starlette_web-0.1.2/starlette_web/common/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/files/storages/filesystem.py` & `starlette_web-0.1.2/starlette_web/common/files/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/base_endpoint.py` & `starlette_web-0.1.2/starlette_web/common/http/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/exception_handlers.py` & `starlette_web-0.1.2/starlette_web/common/http/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/exceptions.py` & `starlette_web-0.1.2/starlette_web/common/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/renderers.py` & `starlette_web-0.1.2/starlette_web/common/http/renderers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/schemas.py` & `starlette_web-0.1.2/starlette_web/common/http/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/http/statuses.py` & `starlette_web-0.1.2/starlette_web/common/http/statuses.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/management/admin_util.py` & `starlette_web-0.1.2/starlette_web/common/management/admin_util.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/management/base.py` & `starlette_web-0.1.2/starlette_web/common/management/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,20 +100,20 @@
             found_local_module = module_info.name
 
     app_path = app.replace(".", os.sep)
 
     if not found_local_module:
         try:
             venv_module = __import__(module_name)
-            prefix = os.path.dirname(venv_module.__path__[0]).strip(os.sep)
+            prefix = os.path.dirname(venv_module.__path__[0]).rstrip(os.sep)
         except (OSError, SystemError, ImportError, IndexError):
             prefix = ""
 
         if prefix:
-            app_path = prefix.strip(os.sep) + os.sep + app_path.strip(os.sep)
+            app_path = prefix.rstrip(os.sep) + os.sep + app_path.lstrip(os.sep)
 
     return app_path
 
 
 def list_commands() -> Dict[str, str]:
     command_files = {}
```

### Comparing `starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/command.py` & `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/command.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/routes.py` & `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 
 from starlette.routing import Mount, Route, WebSocketRoute
 from starlette.staticfiles import StaticFiles
 
 from starlette_web.common.conf import settings
-from starlette_web.contrib.apispec.routes import routes as apispec_routes
+from starlette_web.contrib.apispec.views import OpenApiView
 from starlette_web.contrib.admin import admin, AdminMount
 
 
 routes = [
     Mount(
         settings.STATIC["URL"],
         app=StaticFiles(directory=settings.STATIC["ROOT_DIR"]),
@@ -21,9 +21,9 @@
     ),
 
     # Admin-panel is not yet integral part of the framework,
     # so it requires a bit of hacking with custom mount class,
     # to manage static files right
     AdminMount("/admin", app=admin.get_app(), name="admin"),
 
-    Mount("/openapi", routes=apispec_routes),
+    Route("/openapi", OpenApiView, include_in_schema=False),
 ]
```

### Comparing `starlette_web-0.1.1/starlette_web/common/management/commands/_project_defaults/core/settings.py` & `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 
 APP_DEBUG = config("APP_DEBUG", cast=bool, default=False)
 SECRET_KEY = config("SECRET_KEY", cast=Secret, default="project-secret")
 SITE_URL = "https://web.project.com"
 
 INSTALLED_APPS = [
     "starlette_web.contrib.staticfiles",
-    "starlette_web.contrib.apispec",
-    "starlette_web.contrib.auth",
-    "starlette_web.contrib.admin",
+
+    # Following contrib modules require extra dependencies.
+    # "starlette_web.contrib.apispec",
+    # "starlette_web.contrib.auth",
+    # "starlette_web.contrib.admin",
+    # "starlette_web.contrib.constance",
     # "starlette_web.contrib.constance.backends.database",
     # "starlette_web.contrib.scheduler",
 ]
 
 DB_ECHO = config("DB_ECHO", cast=bool, default=False)
 DB_NAME = config("DB_NAME", default="web_project")
```

### Comparing `starlette_web-0.1.1/starlette_web/common/management/commands/startapp.py` & `starlette_web-0.1.2/starlette_web/common/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/management/commands/startproject.py` & `starlette_web-0.1.2/starlette_web/common/management/commands/startproject.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import shutil
 from pathlib import Path
 
-from alembic.config import main as alembic_main
-
+from starlette_web.common.management.alembic_mixin import AlembicMixin
 from starlette_web.common.management.base import BaseCommand, CommandError, CommandParser
 from starlette_web.common.utils import get_random_string
 
 
-class Command(BaseCommand):
+class Command(BaseCommand, AlembicMixin):
     help = "Initialize directory with project files"
     _alembic_directory_name = "alembic"
 
     def add_arguments(self, parser: CommandParser):
         parser.add_argument("project_name", type=str)
 
     async def handle(self, **options):
@@ -75,22 +74,23 @@
         # Setup base directories
 
         (project_dir / "static").mkdir()
         (project_dir / "templates").mkdir()
 
         # Setup alembic
         os.chdir(project_dir)
-        alembic_main(["init", "-t", "async", self._alembic_directory_name])
+        await self.run_alembic_main(["init", "-t", "async", self._alembic_directory_name])
         with open(project_dir / self._alembic_directory_name / "env.py", "rt") as file:
             lines = []
             for line in file:
                 if line.strip() == "target_metadata = None":
                     lines += [
-                        "from starlette_web.common.database.model_base import ModelBase\n",
+                        "from starlette_web.common.conf import settings\n",
                         "from starlette_web.common.conf.app_manager import app_manager\n",
+                        "from starlette_web.common.database.model_base import ModelBase\n",
                         "app_manager.import_models()\n"
                         "target_metadata = ModelBase.metadata\n",
                     ]
                 else:
                     lines.append(line)
 
         with open(project_dir / self._alembic_directory_name / "env.py", "wt") as file:
```

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/choices.py` & `starlette_web-0.1.2/starlette_web/common/utils/choices.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/crypto.py` & `starlette_web-0.1.2/starlette_web/common/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/importing.py` & `starlette_web-0.1.2/starlette_web/common/utils/importing.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/inspect.py` & `starlette_web-0.1.2/starlette_web/common/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/json.py` & `starlette_web-0.1.2/starlette_web/common/utils/json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/regex.py` & `starlette_web-0.1.2/starlette_web/common/utils/regex.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/utils/serializers.py` & `starlette_web-0.1.2/starlette_web/common/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/common/ws/base_endpoint.py` & `starlette_web-0.1.2/starlette_web/common/ws/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/admin/admin.py` & `starlette_web-0.1.2/starlette_web/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/admin/apps.py` & `starlette_web-0.1.2/starlette_web/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/admin/auth_provider.py` & `starlette_web-0.1.2/starlette_web/contrib/admin/auth_provider.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/admin/middleware.py` & `starlette_web-0.1.2/starlette_web/contrib/admin/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/apispec/apps.py` & `starlette_web-0.1.2/starlette_web/contrib/apispec/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-from openapi_spec_validator import validate_spec
-from openapi_spec_validator.validation.exceptions import (
-    OpenAPIValidationError,
-    OpenAPISpecValidatorError,
-)
 from traceback_with_variables import format_exc
 
 from starlette_web.common.conf import settings
 from starlette_web.common.conf.base_app_config import BaseAppConfig
 from starlette_web.common.http.exceptions import ImproperlyConfigured
 from starlette_web.common.utils import import_string
 from starlette_web.contrib.apispec.views import schemas
 
 
 class AppConfig(BaseAppConfig):
     app_name = "apispec"
 
+    def initialize(self):
+        try:
+            __import__("openapi_spec_validator")
+        except (SystemError, ImportError):
+            raise ImproperlyConfigured(
+                details=(
+                    "Extra dependency 'openapi_spec_validator' is required"
+                    " for starlette_web.contrib.apispec "
+                    "Install it via 'pip install starlette-web[apispec]'."
+                )
+            )
+
     def perform_checks(self):
+        from openapi_spec_validator import validate_spec
+        from openapi_spec_validator.validation.exceptions import (
+            OpenAPIValidationError,
+            OpenAPISpecValidatorError,
+        )
+
         routes = import_string(settings.ROUTES)
 
         try:
             # This check mostly fails on invalid indentation
             # or partially missing properties.
             api_spec = schemas.get_schema(routes)
         except Exception as exc:  # noqa
```

### Comparing `starlette_web-0.1.1/starlette_web/contrib/apispec/introspection.py` & `starlette_web-0.1.2/starlette_web/contrib/apispec/introspection.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/apispec/marshmallow/converters.py` & `starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/apispec/static/apispec/redoc.js` & `starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/redoc.js`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/apispec/templates/apispec/redoc.html` & `starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/redoc.html`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/admin.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/backend.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/backend.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/hashers.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/management/auth_command_mixin.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/management/auth_command_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/changepassword.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/changepassword.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/management/commands/createsuperuser.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/models.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/models.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/password_validation.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/password_validation.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/permissions.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/routes.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/schemas.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/utils.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/auth/views.py` & `starlette_web-0.1.2/starlette_web/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/camel_case/utils.py` & `starlette_web-0.1.2/starlette_web/contrib/camel_case/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/constance/__init__.py` & `starlette_web-0.1.2/starlette_web/contrib/constance/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Any, List, Dict
 
+from starlette_web.common.conf import settings
 from starlette_web.common.http.exceptions import (
     NotSupportedError,
     BaseApplicationError,
     UnexpectedError,
+    ImproperlyConfigured,
 )
 from starlette_web.common.utils import import_string
 from starlette_web.contrib.constance.backends.base import BaseConstanceBackend
-
-from starlette_web.common.conf import settings
+from starlette_web.contrib.constance.backends.caching_mixin import ConstanceCacheMixin
 
 
 # TODO: some kind of validation system, much like django.checks
 # TODO: _validate method
 class LazyConstance:
     _backend: BaseConstanceBackend
     _is_setup: bool
@@ -68,28 +69,48 @@
             for key, value in return_list.items()
         }
 
     def _postprocess_value(self, key, value):
         if key not in settings.CONSTANCE_CONFIG:
             raise NotSupportedError
 
-        if value is self._backend.empty:
+        if value == self._backend.empty:
             return settings.CONSTANCE_CONFIG[key][0]
 
         return value
 
     def _setup(self) -> None:
         if self._is_setup:
             return
 
         try:
-            _backend_kls = import_string(settings.CONSTANCE_BACKEND)
+            _import_path = settings.CONSTANCE_BACKEND
+            if _import_path is None:
+                _backend_kls = None
+            else:
+                _backend_kls = import_string(_import_path)
         except (AttributeError, BaseApplicationError):
             _backend_kls = None
+        except (ImportError, SystemError):
+            raise ImproperlyConfigured(
+                details=f"Invalid constance class: {settings.CONSTANCE_BACKEND}"
+            )
+
+        try:
+            _cache_key = settings.CONSTANCE_DATABASE_CACHE_BACKEND
+        except (AttributeError, BaseApplicationError):
+            _cache_key = None
 
         if _backend_kls:
-            self._backend = _backend_kls()
+            if _cache_key:
+                self._backend = type(
+                    _backend_kls.__name__,
+                    (ConstanceCacheMixin, _backend_kls),
+                    {"_cache_key": _cache_key},
+                )()
+            else:
+                self._backend = _backend_kls()
 
         self._is_setup = True
 
 
 config = LazyConstance()
```

### Comparing `starlette_web-0.1.1/starlette_web/contrib/constance/backends/base.py` & `starlette_web-0.1.2/starlette_web/contrib/constance/backends/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,22 @@
     BytesSerializer,
     PickleSerializer,
     DeserializeError,
 )
 
 
 class BaseConstanceBackend:
-    empty = object()
     serializer_class: Type[BytesSerializer] = PickleSerializer
 
+    class EmptyValue:
+        def __eq__(self, other):
+            return self.__class__ == other.__class__
+
+    empty = EmptyValue()
+
     def __init__(self):
         self.serializer: BytesSerializer = self.serializer_class()
 
     def _preprocess_response(self, response: ByteString) -> Any:
         if response is None:
             return self.empty
```

### Comparing `starlette_web-0.1.1/starlette_web/contrib/constance/backends/database/__init__.py` & `starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/postgres/channel_layers.py` & `starlette_web-0.1.2/starlette_web/contrib/postgres/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/redis/cache.py` & `starlette_web-0.1.2/starlette_web/contrib/redis/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/redis/channel_layers.py` & `starlette_web-0.1.2/starlette_web/contrib/redis/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/redis/redislock.py` & `starlette_web-0.1.2/starlette_web/contrib/redis/redislock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/app_settings.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/app_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/apps.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/apps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import json
 
-import croniter
-from croniter.croniter import CroniterError
-
 from starlette_web.common.conf import settings as project_settings
 from starlette_web.common.conf.base_app_config import BaseAppConfig
 from starlette_web.common.http.exceptions import ImproperlyConfigured
 from starlette_web.contrib.scheduler.app_settings import Settings
 from starlette_web.contrib.scheduler.backends.base import JobType
 
 
 class AppConfig(BaseAppConfig):
     app_name = "scheduler"
 
+    def initialize(self):
+        try:
+            __import__("croniter")
+        except (ImportError, SystemError):
+            raise ImproperlyConfigured(
+                details=(
+                    "Extra dependency 'croniter' is required for "
+                    "starlette_web.contrib.scheduler "
+                    "Install it via 'pip install starlette-web[scheduler]'."
+                )
+            )
+
     def perform_checks(self):
+        import croniter
+        from croniter.croniter import CroniterError
+
         jobs_list = Settings(project_settings).PERIODIC_JOBS
 
         for job in jobs_list:
             try:
                 json.JSONEncoder(sort_keys=True).encode(job)
             except (TypeError, ValueError) as exc:
                 raise ImproperlyConfigured(
```

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/__init__.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/base.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 import hashlib
 import logging
 import os
 import tempfile
-from typing import List, Dict, Tuple, TypeAlias, Union
+from typing import List, Dict, Tuple, Union
 
 import anyio
 from filelock import FileLock
 from traceback_with_variables import format_exc
 
 from starlette_web.common.conf import settings as project_settings
 
 # Scheduler is only supposed to be run as management-command
 from starlette_web.common.management.base import CommandError
 from starlette_web.common.utils.importing import import_string
 from starlette_web.contrib.scheduler.app_settings import Settings
 
 
 logger = logging.getLogger("starlette_web.contrib.scheduler")
-JSONType: TypeAlias = Union[
+JSONType = Union[
     Dict[str, "JSONType"],
     List["JSONType"],
     str,
     int,
     float,
     bool,
     None,
```

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/posix.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/posix.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/backends/win32.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/win32.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/scheduler/management/commands/scheduler.py` & `starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/contrib/staticfiles/management/commands/collectstatic.py` & `starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/conftest.py` & `starlette_web-0.1.2/starlette_web/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
             uuid.UUID("094eb5ff-01de-4985-afeb-22ebb9e76abf"),
             "Test constant uuid",
             uuid.UUID,
         ),
         "TEST_CONSTANT_DATETIME": (datetime(2000, 1, 1), "Test constant datetime", datetime),
     }
     settings.CONSTANCE_BACKEND = "starlette_web.contrib.constance.backends.database.DatabaseBackend"
+    settings.CONSTANCE_DATABASE_CACHE_BACKEND = "locmem"
 
     base_config._setup()
     yield base_config
 
 
 @pytest.fixture(autouse=True, scope="session")
 def client() -> WebTestClient:
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_apispec.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_apispec.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,13 +389,18 @@
         },
         "securitySchemes": {"JWTAuth": {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"}},
     },
 }
 
 
 class TestOpenAPISchema(BaseTestAPIView):
-    url = "/openapi/schema/"
+    url = "/openapi"
 
-    def test_schema(self, client, user):
+    def test_schema(self, client):
         response = client.get(self.url)
         assert response.status_code == 200
         assert response.json() == REFERENCE_SCHEMA
+
+    def test_redoc(self, client):
+        response = client.get(self.url + "?format=redoc")
+        assert response.status_code == 200
+        assert b'<script src="/static/apispec/redoc.js"></script>' in response.content
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_auth.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_auth.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_camel_case.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_camel_case.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_channels.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_channels.py`

 * *Files 12% similar despite different names*

```diff
@@ -144,7 +144,35 @@
         )
         subscriber_3_flag = await_(
             default_cache.async_get(f"{test_group_name}-{subscriber_3}-done")
         )
         assert subscriber_1_flag == ["Message 0", "Message 1", "Message 2", "DONE"]
         assert subscriber_2_flag == ["Message 0", "Message 1", "Message 2", "DONE"]
         assert subscriber_3_flag == ["Message 0", "Message 1", "Message 2", "DONE"]
+
+    def test_immediate_subscriber_cleanup_on_exit(self):
+        async def task_coroutine():
+            _publisher_result = []
+
+            async def publisher_task(channel, _res):
+                await channel.publish("test_group", "Message")
+                await anyio.sleep(0.2)
+                _res.append(len(channel._subscribers))
+                _res.append(len(channel._channel_layer._subscribed))
+
+            async def subscriber_task(channel: Channel):
+                async with channel.subscribe("test_group") as subscriber:
+                    async for message in subscriber:
+                        # break immediately
+                        break
+
+            async with Channel(InMemoryChannelLayer()) as channels:
+                async with anyio.create_task_group() as task_group:
+                    task_group.start_soon(publisher_task, channels, _publisher_result)
+                    task_group.start_soon(subscriber_task, channels)
+                    task_group.start_soon(subscriber_task, channels)
+                    task_group.start_soon(subscriber_task, channels)
+
+            return _publisher_result
+
+        res = await_(task_coroutine())
+        assert res == [0, 0]
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_constance.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_constance.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 def test_constance_get_value(config):
     test_constant_1_value = await_(config.get("TEST_CONSTANT_1"))
     assert test_constant_1_value == 1
 
     all_values = await_(config.mget(["TEST_CONSTANT_1", "TEST_CONSTANT_2"]))
     assert all_values == {"TEST_CONSTANT_1": 1, "TEST_CONSTANT_2": 2}
 
+    test_constant_datetime = await_(config.get("TEST_CONSTANT_DATETIME"))
+    assert type(test_constant_datetime) == datetime.datetime
+
 
 def test_constance_set_value(config):
     new_value = uuid.uuid4()
     await_(config.set("TEST_CONSTANT_UUID", new_value))
     test_constant_uuid = await_(config.get("TEST_CONSTANT_UUID"))
     assert new_value == test_constant_uuid
 
 
 def test_constance_errors(config):
     new_value = uuid.uuid4()
     with pytest.raises(BaseApplicationError):
         await_(config.set("TEST_CONSTANT_DATETIME", new_value))
-    test_constant_datetime = await_(config.get("TEST_CONSTANT_DATETIME"))
-    assert type(test_constant_datetime) == datetime.datetime
 
     with pytest.raises(BaseApplicationError):
         await_(config.get("TEST_CONSTANT_NOT_EXISTING_KEY"))
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_password_validators.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_password_validators.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/contrib/test_redis_cache.py` & `starlette_web-0.1.2/starlette_web/tests/contrib/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/helpers/base_cache_tester.py` & `starlette_web-0.1.2/starlette_web/tests/core/helpers/base_cache_tester.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/test_auth_backends.py` & `starlette_web-0.1.2/starlette_web/tests/core/test_auth_backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/test_base.py` & `starlette_web-0.1.2/starlette_web/tests/core/test_base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/test_base_caches.py` & `starlette_web-0.1.2/starlette_web/tests/core/test_base_caches.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/test_service.py` & `starlette_web-0.1.2/starlette_web/tests/core/test_service.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/core/test_settings.py` & `starlette_web-0.1.2/starlette_web/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/database/test_model_mixin.py` & `starlette_web-0.1.2/starlette_web/tests/database/test_model_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/database/test_nested_transaction.py` & `starlette_web-0.1.2/starlette_web/tests/database/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/files/test_filesystem_storage.py` & `starlette_web-0.1.2/starlette_web/tests/files/test_filesystem_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/files/test_media_storage.py` & `starlette_web-0.1.2/starlette_web/tests/files/test_media_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/helpers.py` & `starlette_web-0.1.2/starlette_web/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/management/commands/test_channels_publisher.py` & `starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_publisher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/management/commands/test_channels_subscriber.py` & `starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_subscriber.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/management/commands/test_db.py` & `starlette_web-0.1.2/starlette_web/tests/management/commands/test_db.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/management/commands/test_parser.py` & `starlette_web-0.1.2/starlette_web/tests/management/commands/test_parser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/mocks.py` & `starlette_web-0.1.2/starlette_web/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/routes.py` & `starlette_web-0.1.2/starlette_web/tests/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from starlette.routing import Mount, Route, WebSocketRoute
 from starlette.staticfiles import StaticFiles
 
 from starlette_web.common.conf import settings
-from starlette_web.contrib.apispec.routes import routes as apispec_routes
+from starlette_web.contrib.apispec.views import OpenApiView
 from starlette_web.contrib.auth.routes import routes as auth_routes
 from starlette_web.contrib.admin import admin, AdminMount
 from starlette_web.tests.views import (
     HealthCheckAPIView,
     BaseWebsocketTestEndpoint,
     CancellationWebsocketTestEndpoint,
     AuthenticationWebsocketTestEndpoint,
@@ -15,15 +15,15 @@
     ChatWebsocketTestEndpoint,
 )
 
 
 # TODO: split auth and api
 routes = [
     Mount("/api", routes=auth_routes),
-    Mount("/openapi", routes=apispec_routes),
+    Route("/openapi", OpenApiView, include_in_schema=False),
     AdminMount("/admin", app=admin.get_app(), name="admin"),
     Mount("/static", app=StaticFiles(directory=settings.STATIC["ROOT_DIR"]), name="static"),
     Mount("/media", app=StaticFiles(directory=settings.MEDIA["ROOT_DIR"]), name="media"),
     Route("/health_check/", HealthCheckAPIView),
     WebSocketRoute("/ws/test_websocket_base", BaseWebsocketTestEndpoint),
     WebSocketRoute("/ws/test_websocket_cancel", CancellationWebsocketTestEndpoint),
     WebSocketRoute("/ws/test_websocket_auth", AuthenticationWebsocketTestEndpoint),
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/settings.py` & `starlette_web-0.1.2/starlette_web/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 TEST_MODE = True
 
 INSTALLED_APPS = [
     "starlette_web.contrib.staticfiles",
     "starlette_web.contrib.apispec",
     "starlette_web.contrib.auth",
     "starlette_web.contrib.admin",
+    "starlette_web.contrib.constance",
     "starlette_web.contrib.constance.backends.database",
     "starlette_web.contrib.scheduler",
     "starlette_web.tests",
 ]
 
 DB_ECHO = config("DB_ECHO", cast=bool, default=False)
 DB_NAME = config("DB_NAME_TEST", default="web_project_test")
```

### Comparing `starlette_web-0.1.1/starlette_web/tests/utils/test_auth_hasher.py` & `starlette_web-0.1.2/starlette_web/tests/utils/test_auth_hasher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/utils/test_json.py` & `starlette_web-0.1.2/starlette_web/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/utils/test_redis_pattern_matcher.py` & `starlette_web-0.1.2/starlette_web/tests/utils/test_redis_pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/utils/test_serializers.py` & `starlette_web-0.1.2/starlette_web/tests/utils/test_serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/views/http.py` & `starlette_web-0.1.2/starlette_web/tests/views/http.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/views/websocket.py` & `starlette_web-0.1.2/starlette_web/tests/views/websocket.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/websockets/test_websocket_chat.py` & `starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_chat.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web/tests/websockets/test_websocket_endpoint.py` & `starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.1/starlette_web.egg-info/PKG-INFO` & `starlette_web-0.1.2/starlette_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: starlette-web
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Home-page: https://github.com/dolamroth/starlette-web
 Author: Sergey Sayamov
 Author-email: dolamroth@mail.ru
 License: MIT License
-Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.2.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
```

### Comparing `starlette_web-0.1.1/starlette_web.egg-info/requires.txt` & `starlette_web-0.1.2/starlette_web.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 alembic<1.11,>=1.10.2
 Jinja2<3.2,>=3.1
 httpx<0.24,>=0.23.3
 python-dotenv<0.22,>=0.21
 traceback-with-variables<2.1,>=2.0.4
 aiosmtplib<2.1,>=2.0.1
 filelock<3.11,>=3.10.7
+marshmallow<3.20,>=3.19.0
 
 [admin]
-starlette-admin<0.8,>=0.7.0
+starlette-admin<0.9,>=0.7.0
 
 [apispec]
-apispec<6.1,>=6.0
+apispec<6.4,>=6.3.0
 pyyaml<6.1,>=6.0
-openapi-spec-validator<0.6,>=0.5.5
+openapi-spec-validator<0.6,>=0.5.6
 
 [auth]
 PyJWT<2.7,>=2.6
 
 [deploy]
 gunicorn<20.2,>=20.1.0
```

