# Comparing `tmp/freechatgpt-1.3.3.tar.gz` & `tmp/freechatgpt-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/freechatgpt-1.3.3.tar", last modified: Tue Apr 11 16:29:20 2023, max compression
+gzip compressed data, was "dist/freechatgpt-1.3.4.tar", last modified: Thu Apr 13 07:31:17 2023, max compression
```

## Comparing `freechatgpt-1.3.3.tar` & `freechatgpt-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt/
--rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.3/freechatgpt/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4919 2023-04-11 16:28:11.000000 freechatgpt-1.3.3/freechatgpt/free_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.3/README.md
--rw-r--r--   0 admin      (501) staff       (20)     1361 2023-04-11 16:28:51.000000 freechatgpt-1.3.3/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      244 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       33 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/freechatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-11 16:29:20.000000 freechatgpt-1.3.3/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.4/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/freechatgpt/
+-rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.4/freechatgpt/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     5103 2023-04-13 07:23:05.000000 freechatgpt-1.3.4/freechatgpt/free_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)      435 2023-04-12 04:56:51.000000 freechatgpt-1.3.4/freechatgpt/ip_util.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/freechatgpt.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      267 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       33 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1361 2023-04-13 07:30:52.000000 freechatgpt-1.3.4/setup.py
```

### Comparing `freechatgpt-1.3.3/PKG-INFO` & `freechatgpt-1.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.3
+Version: 1.3.4
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

### Comparing `freechatgpt-1.3.3/freechatgpt/free_chatgpt.py` & `freechatgpt-1.3.4/freechatgpt/free_chatgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from abc import ABCMeta
 from json import JSONDecodeError
 
 import requests
 import retrying
 from requests import ReadTimeout
 
+from freechatgpt.ip_util import IpTool
+
 
 def retry_if_timeout_error(excep):
     return isinstance(excep, ReadTimeout)
 
 
 class FreeChatgpt(object):
 
@@ -82,15 +84,16 @@
         pass
 
 
 class PlatformGptStore(BasePlatform):
     def _get_chat_res(self) -> str:
         url = "http://free-gpt.fun/chatgpt.php"
         msg = urllib.parse.quote(self.question)
-        payload = f'message={msg}&mychat_ip=121.78.25.14&user_uuid=CHAT-APIGPT-oj3uoj-gxhg-3u9ut-oj6q'
+        ip = IpTool.get_host_ip() or '121.78.25.14'
+        payload = f'message={msg}&mychat_ip={ip}&user_uuid=CHAT-APIGPT-oj3uoj-gxhg-3u9ut-oj6q'
         headers = {
             'Accept': '*/*',
             'Accept-Encoding': 'gzip, deflate',
             'Accept-Language': 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7',
             'Connection': 'keep-alive',
             'Content-Length': '83',
             'Content-Type': 'application/x-www-form-urlencoded',
@@ -108,10 +111,13 @@
 
 
 if __name__ == '__main__':
     # r = FreeChatgpt.ask(question='帮我优化这段话:pandas快速替换所有字符中的特殊字符')
     # print(r)
     # t = FreeChatgpt.ask(question='中国文化的特点是什么？')
     # print(t)
-    q = '根据我的预算2000元,风险偏好中等风险,预期收益率1.3%,请为我提供一种个人理财方案'
-    s = FreeChatgpt.ask(question=q)
-    print(s)
+    # q = '根据我的预算6000元,风险偏好中等风险,预期收益率1.3%,请为我提供一种个人理财方案'
+    # s = FreeChatgpt.ask(question=q)
+    # print(s)
+
+    r = FreeChatgpt.ask(question='帮我创作一个广告视频OPPO卖点？')
+    print(r)
```

### Comparing `freechatgpt-1.3.3/setup.py` & `freechatgpt-1.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author abo123456789
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='freechatgpt',
-    version='1.3.3',
+    version='1.3.4',
     description=(
         'free chatgpt api, not need token'
     ),
     keywords=(
         "chatgpt,free"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `freechatgpt-1.3.3/freechatgpt.egg-info/PKG-INFO` & `freechatgpt-1.3.4/freechatgpt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.3
+Version: 1.3.4
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

