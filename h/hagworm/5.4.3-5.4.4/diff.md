# Comparing `tmp/hagworm-5.4.3.tar.gz` & `tmp/hagworm-5.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.4.3.tar", last modified: Thu Apr 13 08:36:48 2023, max compression
+gzip compressed data, was "hagworm-5.4.4.tar", last modified: Thu Apr 13 09:18:36 2023, max compression
```

## Comparing `hagworm-5.4.3.tar` & `hagworm-5.4.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.329413 hagworm-5.4.3/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.3/LICENSE
--rw-rw-rw-   0        0        0     7509 2023-04-13 08:36:48.328413 hagworm-5.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.215415 hagworm-5.4.3/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.3/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.219413 hagworm-5.4.3/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.225413 hagworm-5.4.3/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.228413 hagworm-5.4.3/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.230413 hagworm-5.4.3/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.231413 hagworm-5.4.3/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.3/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.233414 hagworm-5.4.3/hagworm/
--rw-rw-rw-   0        0        0      510 2023-04-13 03:26:46.000000 hagworm-5.4.3/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.272413 hagworm-5.4.3/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.297413 hagworm-5.4.3/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.3/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.3/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.3/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.3/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.3/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    10611 2023-04-11 07:37:23.000000 hagworm-5.4.3/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.3/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.3/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.3/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.3/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.3/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.3/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14422 2023-04-13 08:33:22.000000 hagworm-5.4.3/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.3/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.3/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.3/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.302413 hagworm-5.4.3/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.309413 hagworm-5.4.3/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.3/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.312413 hagworm-5.4.3/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.314413 hagworm-5.4.3/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.318413 hagworm-5.4.3/hagworm/third/aliyun/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/aliyun/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/aliyun/logging.py
--rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.3/hagworm/third/aliyun/rocketmq.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.321413 hagworm-5.4.3/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.326413 hagworm-5.4.3/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.3/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.3/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.3/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:36:48.241413 hagworm-5.4.3/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7509 2023-04-13 08:36:47.000000 hagworm-5.4.3/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2262 2023-04-13 08:36:48.000000 hagworm-5.4.3/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:36:47.000000 hagworm-5.4.3/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      707 2023-04-13 08:36:47.000000 hagworm-5.4.3/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 08:36:47.000000 hagworm-5.4.3/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 08:36:48.329413 hagworm-5.4.3/setup.cfg
--rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.453160 hagworm-5.4.4/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.4/LICENSE
+-rw-rw-rw-   0        0        0     7509 2023-04-13 09:18:36.452159 hagworm-5.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.339657 hagworm-5.4.4/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.4/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.342657 hagworm-5.4.4/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.349719 hagworm-5.4.4/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.352717 hagworm-5.4.4/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.354718 hagworm-5.4.4/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.356160 hagworm-5.4.4/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.357159 hagworm-5.4.4/hagworm/
+-rw-rw-rw-   0        0        0      510 2023-04-13 09:17:44.000000 hagworm-5.4.4/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.395160 hagworm-5.4.4/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.422159 hagworm-5.4.4/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.4/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.4/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.4/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.4/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.4/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    10611 2023-04-11 07:37:23.000000 hagworm-5.4.4/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.4/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.4/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.4/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.4/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.4/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.4/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14859 2023-04-13 09:17:30.000000 hagworm-5.4.4/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.4/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.4/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.4/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.426159 hagworm-5.4.4/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.433159 hagworm-5.4.4/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.4/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.436159 hagworm-5.4.4/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.438159 hagworm-5.4.4/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.442159 hagworm-5.4.4/hagworm/third/aliyun/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/aliyun/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/aliyun/logging.py
+-rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.4/hagworm/third/aliyun/rocketmq.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.445161 hagworm-5.4.4/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.451159 hagworm-5.4.4/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.4/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.4/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.364160 hagworm-5.4.4/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7509 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2262 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      707 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:18:36.453160 hagworm-5.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.4/setup.py
```

### Comparing `hagworm-5.4.3/LICENSE` & `hagworm-5.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/PKG-INFO` & `hagworm-5.4.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.3
+Version: 5.4.4
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.3/README.md` & `hagworm-5.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/c_extend/math.c` & `hagworm-5.4.4/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.4.4/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/example/fastapi_demo/main.py` & `hagworm-5.4.4/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/example/fastapi_demo/service/__init__.py` & `hagworm-5.4.4/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/example/fastapi_demo/setting.py` & `hagworm-5.4.4/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/example/main_test.py` & `hagworm-5.4.4/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/base.py` & `hagworm-5.4.4/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/buffer.py` & `hagworm-5.4.4/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/command.py` & `hagworm-5.4.4/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/event.py` & `hagworm-5.4.4/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/file.py` & `hagworm-5.4.4/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/future.py` & `hagworm-5.4.4/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/mail.py` & `hagworm-5.4.4/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/mongo.py` & `hagworm-5.4.4/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/mysql.py` & `hagworm-5.4.4/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/net.py` & `hagworm-5.4.4/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/ntp.py` & `hagworm-5.4.4/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/pool.py` & `hagworm-5.4.4/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/redis.py` & `hagworm-5.4.4/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/socket.py` & `hagworm-5.4.4/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/task.py` & `hagworm-5.4.4/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/transaction.py` & `hagworm-5.4.4/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/asyncio/zmq.py` & `hagworm-5.4.4/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/base.py` & `hagworm-5.4.4/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/cache.py` & `hagworm-5.4.4/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/compile.py` & `hagworm-5.4.4/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/config.py` & `hagworm-5.4.4/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/crypto.py` & `hagworm-5.4.4/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/error.py` & `hagworm-5.4.4/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/event.py` & `hagworm-5.4.4/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/igraph.py` & `hagworm-5.4.4/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/interface.py` & `hagworm-5.4.4/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/logging.py` & `hagworm-5.4.4/hagworm/extend/logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,19 +72,20 @@
         )
 
 
 class _BaseSink:
     """基础日志投递基类
     """
 
-    def __init__(self, buffer_maxsize=0xffff, bulk_maxsize=0x800):
+    def __init__(self, buffer_maxsize: int = 0xffff, bulk_maxsize: int = 0x800, write_max_delay: int = 5):
 
         self._buffer = queue.Queue(buffer_maxsize)
 
         self._bulk_maxsize = bulk_maxsize
+        self._write_max_delay = write_max_delay
         self._closed = False
 
         self._task = Thread(target=self._do_task)
         self._task.start()
 
     def write(self, message):
 
@@ -109,32 +110,32 @@
         except Exception as err:
 
             sys.stderr.write(f'{str(err)}\n')
 
     def close(self):
 
         self._closed = True
-        self._task.join(10)
+        self._task.join(self._write_max_delay * 2)
 
     def _do_task(self):
 
         messages = []
 
         while not self._closed:
 
             try:
 
                 messages.append(self._buffer.get(block=True))
 
-                for _ in range(5):
+                for _idx in range(self._write_max_delay):
 
                     for _ in range(min(self._buffer.qsize(), self._bulk_maxsize - len(messages))):
                         messages.append(self._buffer.get_nowait())
 
-                    if len(messages) < self._bulk_maxsize:
+                    if len(messages) < self._bulk_maxsize and (_idx + 1) < self._write_max_delay:
                         time.sleep(1)
                     else:
                         break
 
                 self._write_logs(messages)
 
             except Exception as err:
@@ -150,32 +151,40 @@
         raise NotImplementedError()
 
 
 class QueuedFileSink(_BaseSink, FileSink):
     """日志文件队列
     """
 
-    def __init__(self, path, *, buffer_maxsize=0xffff, bulk_maxsize=0x800, **kwargs):
+    def __init__(
+            self, path, *,
+            buffer_maxsize: int = 0xffff, bulk_maxsize: int = 0x800, write_max_delay: int = 5,
+            **kwargs
+    ):
 
-        _BaseSink.__init__(self, buffer_maxsize, bulk_maxsize)
+        _BaseSink.__init__(self, buffer_maxsize, bulk_maxsize, write_max_delay)
         FileSink.__init__(self, path, **kwargs)
 
     def _write_logs(self, logs):
 
         for _log in logs:
             FileSink.write(self, _log)
 
 
 class KafkaSink(_BaseSink):
     """Kafka日志投递
     """
 
-    def __init__(self, servers, topic, *, buffer_maxsize=0xffff, bulk_maxsize=0x800, **kwargs):
+    def __init__(
+            self, servers, topic, *,
+            buffer_maxsize: int = 0xffff, bulk_maxsize: int = 0x800, write_max_delay: int = 5,
+            **kwargs
+    ):
 
-        super().__init__(buffer_maxsize, bulk_maxsize)
+        super().__init__(buffer_maxsize, bulk_maxsize, write_max_delay)
 
         kwargs[r'bootstrap.servers'] = servers
 
         self._producer = KFKProducer(kwargs)
 
         self._topic = topic
 
@@ -374,20 +383,20 @@
 
 class ElasticsearchSink(_BaseSink):
     """Elasticsearch日志投递
     """
 
     def __init__(
             self, hosts, index, *,
-            buffer_maxsize=0xffff, bulk_maxsize=0x800,
+            buffer_maxsize: int = 0xffff, bulk_maxsize: int = 0x800, write_max_delay: int = 5,
             rollover_max_age: str = r'1d', rollover_max_primary_shard_size: str = r'50gb',
             delete_min_age: str = r'30d',
             **kwargs):
 
-        super().__init__(buffer_maxsize, bulk_maxsize)
+        super().__init__(buffer_maxsize, bulk_maxsize, write_max_delay)
 
         self._elasticsearch = Elasticsearch(hosts, **kwargs)
 
         ElasticsearchDataStreamUtil(
             self._elasticsearch, index,
             rollover_max_age=rollover_max_age, rollover_max_primary_shard_size=rollover_max_primary_shard_size,
             delete_min_age=delete_min_age
```

### Comparing `hagworm-5.4.3/hagworm/extend/media.py` & `hagworm-5.4.4/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/metaclass.py` & `hagworm-5.4.4/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/process.py` & `hagworm-5.4.4/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/qrcode.py` & `hagworm-5.4.4/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/struct.py` & `hagworm-5.4.4/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/text.py` & `hagworm-5.4.4/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/trace.py` & `hagworm-5.4.4/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/transaction.py` & `hagworm-5.4.4/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/extend/validator.py` & `hagworm-5.4.4/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/fastapi/base.py` & `hagworm-5.4.4/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/fastapi/field.py` & `hagworm-5.4.4/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/fastapi/model.py` & `hagworm-5.4.4/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/fastapi/response.py` & `hagworm-5.4.4/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/gunicorn.py` & `hagworm-5.4.4/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/frame/stress_tests.py` & `hagworm-5.4.4/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/static/cacert.pem` & `hagworm-5.4.4/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/aliyun/logging.py` & `hagworm-5.4.4/hagworm/third/aliyun/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/aliyun/rocketmq.py` & `hagworm-5.4.4/hagworm/third/aliyun/rocketmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/consul/config.py` & `hagworm-5.4.4/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/rabbitmq/consume.py` & `hagworm-5.4.4/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/rabbitmq/publish.py` & `hagworm-5.4.4/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.4.4/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm.egg-info/PKG-INFO` & `hagworm-5.4.4/hagworm.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.3
+Version: 5.4.4
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.3/hagworm.egg-info/SOURCES.txt` & `hagworm-5.4.4/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/hagworm.egg-info/requires.txt` & `hagworm-5.4.4/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.3/setup.py` & `hagworm-5.4.4/setup.py`

 * *Files identical despite different names*

