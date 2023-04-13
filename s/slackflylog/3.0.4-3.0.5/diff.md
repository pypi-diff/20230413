# Comparing `tmp/slackflylog-3.0.4.tar.gz` & `tmp/slackflylog-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-3.0.4.tar", last modified: Thu Apr 13 06:57:23 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.5.tar", last modified: Thu Apr 13 09:27:17 2023, max compression
```

## Comparing `slackflylog-3.0.4.tar` & `slackflylog-3.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.918817 slackflylog-3.0.4/
--rw-r--r--   0 user_xh   (1000) users      (100)     1063 2023-04-13 06:56:46.000000 slackflylog-3.0.4/LICENSE
--rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 06:57:23.917816 slackflylog-3.0.4/PKG-INFO
--rw-r--r--   0 user_xh   (1000) users      (100)       13 2023-04-13 06:56:46.000000 slackflylog-3.0.4/README.md
--rw-r--r--   0 user_xh   (1000) users      (100)       38 2023-04-13 06:57:23.918817 slackflylog-3.0.4/setup.cfg
--rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 06:57:05.000000 slackflylog-3.0.4/setup.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.914816 slackflylog-3.0.4/slackflylog/
--rw-r--r--   0 user_xh   (1000) users      (100)      281 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/__init__.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.916817 slackflylog-3.0.4/slackflylog/agent/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     3640 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/agent.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.917816 slackflylog-3.0.4/slackflylog/agent/backends/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     2114 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 user_xh   (1000) users      (100)      123 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/log.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1795 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/agent/utils.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.917816 slackflylog-3.0.4/slackflylog/api/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1174 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/client.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1599 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/api/log_handler.py
--rw-r--r--   0 user_xh   (1000) users      (100)      182 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/constants.py
--rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 06:56:46.000000 slackflylog-3.0.4/slackflylog/setup.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 06:57:23.915817 slackflylog-3.0.4/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1000) users      (100)      544 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1000) users      (100)        1 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1000) users      (100)       25 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1000) users      (100)       12 2023-04-13 06:57:23.000000 slackflylog-3.0.4/slackflylog.egg-info/top_level.txt
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.766273 slackflylog-3.0.5/
+-rw-r--r--   0 user_xh   (1000) users      (100)     1063 2023-04-13 09:26:46.000000 slackflylog-3.0.5/LICENSE
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 09:27:17.766273 slackflylog-3.0.5/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)       13 2023-04-13 09:26:46.000000 slackflylog-3.0.5/README.md
+-rw-r--r--   0 user_xh   (1000) users      (100)       38 2023-04-13 09:27:17.766273 slackflylog-3.0.5/setup.cfg
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 09:27:05.000000 slackflylog-3.0.5/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.763273 slackflylog-3.0.5/slackflylog/
+-rw-r--r--   0 user_xh   (1000) users      (100)      281 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/__init__.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/agent/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     3686 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/agent.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/agent/backends/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     2114 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      123 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/log.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1795 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/utils.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/api/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1174 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/client.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1599 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/log_handler.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      182 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/constants.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.764273 slackflylog-3.0.5/slackflylog.egg-info/
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)      544 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)        1 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       25 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       12 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/top_level.txt
```

### Comparing `slackflylog-3.0.4/LICENSE` & `slackflylog-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.4/setup.py` & `slackflylog-3.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.4"
+    __version__ = "1.0.5"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.4"
+    __version__ = "3.0.5"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.4/slackflylog/agent/agent.py` & `slackflylog-3.0.5/slackflylog/agent/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 不使用 gevent，因为测试了 gevent 对 smtplib 似乎没法异步，还是会阻塞
 """
 
 
 import sys
 import json
-from thread import start_new_thread
+
 from collections import defaultdict
 from .utils import import_string
 from .log import logger
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     import SocketServer
+    from thread import start_new_thread
 
 else:
     import socketserver as SocketServer
+    from _thread import start_new_thread
 
 
 
 class Agent(object):
     debug = False
 
     backend_dict = None
```

### Comparing `slackflylog-3.0.4/slackflylog/agent/backends/send_slack.py` & `slackflylog-3.0.5/slackflylog/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.4/slackflylog/agent/utils.py` & `slackflylog-3.0.5/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.4/slackflylog/api/client.py` & `slackflylog-3.0.5/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.4/slackflylog/api/log_handler.py` & `slackflylog-3.0.5/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.4/slackflylog/setup.py` & `slackflylog-3.0.5/slackflylog/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.4"
+    __version__ = "1.0.5"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.4"
+    __version__ = "3.0.5"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.4/slackflylog.egg-info/SOURCES.txt` & `slackflylog-3.0.5/slackflylog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

