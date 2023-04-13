# Comparing `tmp/deng-2023.4.13.1.tar.gz` & `tmp/deng-2023.4.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deng-2023.4.13.1.tar", last modified: Thu Apr 13 07:02:20 2023, max compression
+gzip compressed data, was "dist\deng-2023.4.13.2.tar", last modified: Thu Apr 13 11:26:57 2023, max compression
```

## Comparing `deng-2023.4.13.1.tar` & `deng-2023.4.13.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:02:20.000000 deng-2023.4.13.1/
--rw-rw-rw-   0        0        0     3101 2023-04-13 07:02:20.000000 deng-2023.4.13.1/PKG-INFO
--rw-rw-rw-   0        0        0     2496 2022-05-09 08:35:59.000000 deng-2023.4.13.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng/
--rw-rw-rw-   0        0        0     8253 2023-04-13 07:02:05.000000 deng-2023.4.13.1/deng/__init__.py
--rw-rw-rw-   0        0        0   100410 2020-04-08 06:30:19.000000 deng-2023.4.13.1/deng/addressinfo.py
--rw-rw-rw-   0        0        0      942 2022-02-18 02:47:48.000000 deng-2023.4.13.1/deng/baidu.py
--rw-rw-rw-   0        0        0   194860 2020-04-08 06:30:19.000000 deng-2023.4.13.1/deng/bankinfo.py
--rw-rw-rw-   0        0        0     8005 2022-07-21 05:47:30.000000 deng-2023.4.13.1/deng/cache.py
--rw-rw-rw-   0        0        0      471 2022-02-10 07:57:34.000000 deng-2023.4.13.1/deng/colors.py
--rw-rw-rw-   0        0        0     4519 2023-03-15 05:47:04.000000 deng-2023.4.13.1/deng/encrypt.py
--rw-rw-rw-   0        0        0     3309 2022-06-06 09:10:41.000000 deng-2023.4.13.1/deng/feishu.py
--rw-rw-rw-   0        0        0    16715 2022-06-30 02:58:31.000000 deng-2023.4.13.1/deng/file.py
--rw-rw-rw-   0        0        0    12174 2022-06-22 11:46:42.000000 deng-2023.4.13.1/deng/flow.py
--rw-rw-rw-   0        0        0    17479 2023-03-27 09:31:27.000000 deng-2023.4.13.1/deng/git.py
--rw-rw-rw-   0        0        0    12712 2022-05-11 11:23:10.000000 deng-2023.4.13.1/deng/gitea.py
--rw-rw-rw-   0        0        0     7940 2023-02-28 12:04:19.000000 deng-2023.4.13.1/deng/http.py
--rw-rw-rw-   0        0        0     1645 2020-09-14 04:03:41.000000 deng-2023.4.13.1/deng/image.py
--rw-rw-rw-   0        0        0      912 2022-02-10 07:57:34.000000 deng-2023.4.13.1/deng/message.py
--rw-rw-rw-   0        0        0     4258 2022-08-19 03:05:41.000000 deng-2023.4.13.1/deng/net.py
--rw-rw-rw-   0        0        0     5577 2022-02-10 07:57:34.000000 deng-2023.4.13.1/deng/samba.py
--rw-rw-rw-   0        0        0      530 2020-04-08 06:30:19.000000 deng-2023.4.13.1/deng/singleton.py
--rw-rw-rw-   0        0        0    23336 2022-07-06 07:42:51.000000 deng-2023.4.13.1/deng/testdata.py
--rw-rw-rw-   0        0        0     2170 2022-07-21 09:20:45.000000 deng-2023.4.13.1/deng/time.py
--rw-rw-rw-   0        0        0    10574 2023-02-01 06:53:41.000000 deng-2023.4.13.1/deng/utils.py
--rw-rw-rw-   0        0        0     8531 2022-06-24 08:12:38.000000 deng-2023.4.13.1/deng/windows.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/
--rw-rw-rw-   0        0        0     3101 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-13 07:02:20.000000 deng-2023.4.13.1/deng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 07:02:20.000000 deng-2023.4.13.1/setup.cfg
--rw-rw-rw-   0        0        0     1210 2022-05-17 08:25:37.000000 deng-2023.4.13.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:26:57.000000 deng-2023.4.13.2/
+-rw-rw-rw-   0        0        0     3101 2023-04-13 11:26:57.000000 deng-2023.4.13.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2496 2022-05-09 08:35:59.000000 deng-2023.4.13.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng/
+-rw-rw-rw-   0        0        0     8253 2023-04-13 11:26:49.000000 deng-2023.4.13.2/deng/__init__.py
+-rw-rw-rw-   0        0        0   100410 2020-04-08 06:30:19.000000 deng-2023.4.13.2/deng/addressinfo.py
+-rw-rw-rw-   0        0        0      942 2022-02-18 02:47:48.000000 deng-2023.4.13.2/deng/baidu.py
+-rw-rw-rw-   0        0        0   194860 2020-04-08 06:30:19.000000 deng-2023.4.13.2/deng/bankinfo.py
+-rw-rw-rw-   0        0        0     8005 2022-07-21 05:47:30.000000 deng-2023.4.13.2/deng/cache.py
+-rw-rw-rw-   0        0        0      471 2022-02-10 07:57:34.000000 deng-2023.4.13.2/deng/colors.py
+-rw-rw-rw-   0        0        0     4519 2023-03-15 05:47:04.000000 deng-2023.4.13.2/deng/encrypt.py
+-rw-rw-rw-   0        0        0     3309 2022-06-06 09:10:41.000000 deng-2023.4.13.2/deng/feishu.py
+-rw-rw-rw-   0        0        0    16715 2022-06-30 02:58:31.000000 deng-2023.4.13.2/deng/file.py
+-rw-rw-rw-   0        0        0    12174 2022-06-22 11:46:42.000000 deng-2023.4.13.2/deng/flow.py
+-rw-rw-rw-   0        0        0    17479 2023-03-27 09:31:27.000000 deng-2023.4.13.2/deng/git.py
+-rw-rw-rw-   0        0        0    12712 2022-05-11 11:23:10.000000 deng-2023.4.13.2/deng/gitea.py
+-rw-rw-rw-   0        0        0     7962 2023-04-13 11:26:33.000000 deng-2023.4.13.2/deng/http.py
+-rw-rw-rw-   0        0        0     1645 2020-09-14 04:03:41.000000 deng-2023.4.13.2/deng/image.py
+-rw-rw-rw-   0        0        0      912 2022-02-10 07:57:34.000000 deng-2023.4.13.2/deng/message.py
+-rw-rw-rw-   0        0        0     4258 2022-08-19 03:05:41.000000 deng-2023.4.13.2/deng/net.py
+-rw-rw-rw-   0        0        0     5577 2022-02-10 07:57:34.000000 deng-2023.4.13.2/deng/samba.py
+-rw-rw-rw-   0        0        0      530 2020-04-08 06:30:19.000000 deng-2023.4.13.2/deng/singleton.py
+-rw-rw-rw-   0        0        0    23336 2022-07-06 07:42:51.000000 deng-2023.4.13.2/deng/testdata.py
+-rw-rw-rw-   0        0        0     2170 2022-07-21 09:20:45.000000 deng-2023.4.13.2/deng/time.py
+-rw-rw-rw-   0        0        0    10574 2023-02-01 06:53:41.000000 deng-2023.4.13.2/deng/utils.py
+-rw-rw-rw-   0        0        0     8531 2022-06-24 08:12:38.000000 deng-2023.4.13.2/deng/windows.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/
+-rw-rw-rw-   0        0        0     3101 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-13 11:26:57.000000 deng-2023.4.13.2/deng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:26:57.000000 deng-2023.4.13.2/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2022-05-17 08:25:37.000000 deng-2023.4.13.2/setup.py
```

### Comparing `deng-2023.4.13.1/PKG-INFO` & `deng-2023.4.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deng
-Version: 2023.4.13.1
+Version: 2023.4.13.2
 Summary: Personal method encapsulation
 Home-page: https://github.com/Deng2016/deng
 Author: dengqingyong
 Author-email: yu12377@163.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deng-2023.4.13.1/README.md` & `deng-2023.4.13.2/README.md`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/__init__.py` & `deng-2023.4.13.2/deng/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import logging
 import logging.handlers
 from typing import List, Union
 from pathlib import Path
 
 
-__version__ = "2023.4.13.1"
+__version__ = "2023.4.13.2"
 log_format = logging.Formatter(
     "[%(asctime)s] %(name)s/%(filename)s/%(lineno)s/%(funcName)s/%(levelname)s: %(message)s"
 )
 
 # 日志句柄
 logger = logging.getLogger("DengUtils")
 # 此处必须为DEBUG，否则在UiBot中多次加载时会覆盖configure_logger中level配置
```

### Comparing `deng-2023.4.13.1/deng/addressinfo.py` & `deng-2023.4.13.2/deng/addressinfo.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/baidu.py` & `deng-2023.4.13.2/deng/baidu.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/bankinfo.py` & `deng-2023.4.13.2/deng/bankinfo.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/cache.py` & `deng-2023.4.13.2/deng/cache.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/encrypt.py` & `deng-2023.4.13.2/deng/encrypt.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/feishu.py` & `deng-2023.4.13.2/deng/feishu.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/file.py` & `deng-2023.4.13.2/deng/file.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/flow.py` & `deng-2023.4.13.2/deng/flow.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/git.py` & `deng-2023.4.13.2/deng/git.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/gitea.py` & `deng-2023.4.13.2/deng/gitea.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/http.py` & `deng-2023.4.13.2/deng/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     """
     if response.status_code == 200:
         content_type = response.headers.get("content-type")
         if content_type and "json" in content_type:
             if not operate:
                 _info = caller_info or get_caller_info(2)
                 operate = f"调用{_info['output']})"
-            if response.json().get("code") == 0:
+            if response.json().get("code") in (0, 200, "200"):
                 status = True
-            elif response.json().get("success"):
+            elif response.json().get("success") is True:
                 status = True
             else:
                 msg = f"{operate}失败，错误详情：{response.text}"
                 if ignore_error:
                     status = False
                     logger.error(msg)
                 else:
```

### Comparing `deng-2023.4.13.1/deng/image.py` & `deng-2023.4.13.2/deng/image.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/message.py` & `deng-2023.4.13.2/deng/message.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/net.py` & `deng-2023.4.13.2/deng/net.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/samba.py` & `deng-2023.4.13.2/deng/samba.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/singleton.py` & `deng-2023.4.13.2/deng/singleton.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/testdata.py` & `deng-2023.4.13.2/deng/testdata.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/time.py` & `deng-2023.4.13.2/deng/time.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/utils.py` & `deng-2023.4.13.2/deng/utils.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng/windows.py` & `deng-2023.4.13.2/deng/windows.py`

 * *Files identical despite different names*

### Comparing `deng-2023.4.13.1/deng.egg-info/PKG-INFO` & `deng-2023.4.13.2/deng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deng
-Version: 2023.4.13.1
+Version: 2023.4.13.2
 Summary: Personal method encapsulation
 Home-page: https://github.com/Deng2016/deng
 Author: dengqingyong
 Author-email: yu12377@163.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deng-2023.4.13.1/setup.py` & `deng-2023.4.13.2/setup.py`

 * *Files identical despite different names*

