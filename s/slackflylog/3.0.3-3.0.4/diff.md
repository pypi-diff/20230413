# Comparing `tmp/slackflylog-3.0.3.tar.gz` & `tmp/slackflylog-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-3.0.3.tar", last modified: Thu Apr 13 06:05:13 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.4.tar", last modified: Thu Apr 13 06:57:23 2023, max compression
```

## Comparing `slackflylog-3.0.3.tar` & `slackflylog-3.0.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.045209 slackflylog-3.0.3/
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 06:05:13.045209 slackflylog-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 06:05:13.045209 slackflylog-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      639 2023-04-13 06:04:05.000000 slackflylog-3.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.043208 slackflylog-3.0.3/slackflylog/
--rw-r--r--   0 root         (0) root         (0)      281 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.044209 slackflylog-3.0.3/slackflylog/agent/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/agent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.044209 slackflylog-3.0.3/slackflylog/agent/backends/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/log.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.045209 slackflylog-3.0.3/slackflylog/api/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/client.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/log_handler.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/constants.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.043208 slackflylog-3.0.3/slackflylog.egg-info/
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2023-04-13 06:05:13.000000 slackflylog-3.0.3/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/top_level.txt
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.918817 slackflylog-3.0.4/
+-rw-r--r--   0 user_xh   (1000) users      (100)     1063 2023-04-13 06:56:46.000000 slackflylog-3.0.4/LICENSE
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 06:57:23.917816 slackflylog-3.0.4/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)       13 2023-04-13 06:56:46.000000 slackflylog-3.0.4/README.md
+-rw-r--r--   0 user_xh   (1000) users      (100)       38 2023-04-13 06:57:23.918817 slackflylog-3.0.4/setup.cfg
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 06:57:05.000000 slackflylog-3.0.4/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.914816 slackflylog-3.0.4/slackflylog/
+-rw-r--r--   0 user_xh   (1000) users      (100)      281 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/__init__.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.916817 slackflylog-3.0.4/slackflylog/agent/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     3640 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/agent.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.917816 slackflylog-3.0.4/slackflylog/agent/backends/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     2114 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      123 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/log.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1795 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/utils.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.917816 slackflylog-3.0.4/slackflylog/api/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1174 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/client.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1599 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/log_handler.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      182 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/constants.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.915817 slackflylog-3.0.4/slackflylog.egg-info/
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)      544 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)        1 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       25 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       12 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/top_level.txt
```

### Comparing `slackflylog-3.0.3/setup.py` & `slackflylog-3.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.3"
+    __version__ = "1.0.4"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.3"
+    __version__ = "3.0.4"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.3/slackflylog/agent/agent.py` & `slackflylog-3.0.4/slackflylog/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,30 @@
 """
 用来作为接受log传递的agent
 通过udp通道。
 
 不使用 gevent，因为测试了 gevent 对 smtplib 似乎没法异步，还是会阻塞
 """
 
+
+import sys
 import json
-import SocketServer
 from thread import start_new_thread
 from collections import defaultdict
-
 from .utils import import_string
 from .log import logger
 
+PY2 = sys.version_info[0] == 2
+if PY2:
+    import SocketServer
+
+else:
+    import socketserver as SocketServer
+
+
 
 class Agent(object):
     debug = False
 
     backend_dict = None
 
     def __init__(self, config=None, debug=None):
```

### Comparing `slackflylog-3.0.3/slackflylog/agent/backends/send_slack.py` & `slackflylog-3.0.4/slackflylog/agent/backends/send_slack.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 
-from urllib2 import urlopen
-
 import copy
 import random
-# import telegramlog.constants
 from ..log import logger
+import sys
 
-# logger = logging.getLogger(telegramlog.constants.AGENT_LOGGER_NAME)
-#
-# MULTIPLE_CHANNEL_BOT_API = '1944182514:AAFeRKSO6S3TBRmPBxTZTO6JX-xh6BAWE5Y'
-# MULTIPLE_CHANNEL_USER_API = '@server_error_log'
+PY2 = sys.version_info[0] == 2
+if PY2:
+    from slackclient import SlackClient as SendClient
+else:
+    from slack_sdk import WebClient as SendClient
 
 
-class TelegramBackend(object):
+class SlackFlyLogBackend(object):
     """
     发送tele
     """
 
     def __init__(self, sender_list):
         """
         初始化
@@ -37,36 +36,49 @@
             random.shuffle(sender_list)
 
             # 取出最后一个
             params = sender_list.pop()
 
             try:
                 logger.error("params %s", params)
-                bot_api = params['bot_api']
-                user_api = params['user_api']
-                self._send_msg_to_telegram(bot_api, user_api, content, title)
+                channel_id = params['channel_id']
+                slack_token = params['slack_token']
+                self._send_msg_to_slack(channel_id, slack_token, content, title)
                 return True
             except:
                 logger.error('exc occur. params: %s', params, exc_info=True)
         else:
             # 就是循环完了，也没发送成功
             return False
 
-    def _send_msg_to_telegram(self, bot_api, user_api, send_msg, title):
+    def _send_msg_to_slack(self, channel_id, slack_token, send_msg, title):
         """
-        :param bot_api: 机器人密钥
-        :param user_api: 频道link
+        :param channel_id: 接收渠道ID
+        :param slack_token: slack_token
         :param send_msg: 发送内容
         :return:
         """
-        import urllib
 
-        if not send_msg:
+
+        if not send_msg and not title:
             return False
 
-        full_content = '\n\n'.join([title, send_msg])
-        logger.error("full_content [[[[[[[%s]]]]]]]", urllib.quote(full_content))
+        msg = '\n\n'.join([title, send_msg])
+        if '%0a' in msg:
+            msg = msg.replace('%0a', '\n')
+
+        if PY2:
+            sc = SendClient(slack_token)
+            # 发送消息
+            sc.api_call(
+                "chat.postMessage",
+                channel=channel_id,
+                text=msg
+            )
+
+        else:
+            # Python3 发送
+            sc = SendClient(token=slack_token)
+
+            sc.chat_postMessage(channel=channel_id, text=text)
 
-        url = "https://api.telegram.org/bot{0}/sendMessage?chat_id={1}&text={2}".format(bot_api, user_api, urllib.quote(full_content))
-        logger.error("url %s", url)
-        urlopen(url).close()
         return True
```

### Comparing `slackflylog-3.0.3/slackflylog/agent/utils.py` & `slackflylog-3.0.4/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.3/slackflylog/api/client.py` & `slackflylog-3.0.4/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.3/slackflylog/api/log_handler.py` & `slackflylog-3.0.4/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.3/slackflylog/setup.py` & `slackflylog-3.0.4/slackflylog/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.0"
+    __version__ = "1.0.4"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.0"
+    __version__ = "3.0.4"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.3/slackflylog.egg-info/SOURCES.txt` & `slackflylog-3.0.4/slackflylog.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 slackflylog/__init__.py
 slackflylog/constants.py
 slackflylog/setup.py
 slackflylog.egg-info/PKG-INFO
 slackflylog.egg-info/SOURCES.txt
 slackflylog.egg-info/dependency_links.txt
```

