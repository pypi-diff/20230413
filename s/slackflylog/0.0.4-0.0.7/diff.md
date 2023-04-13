# Comparing `tmp/slackflylog-0.0.4.tar.gz` & `tmp/slackflylog-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-0.0.4.tar", last modified: Wed Apr 12 12:14:42 2023, max compression
+gzip compressed data, was "dist/slackflylog-0.0.7.tar", last modified: Thu Apr 13 02:16:02 2023, max compression
```

## Comparing `slackflylog-0.0.4.tar` & `slackflylog-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/agent/backends/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/agent.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/log.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/api/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/client.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/log_handler.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-12 12:14:31.000000 slackflylog-0.0.4/setup.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:14:42.000000 slackflylog-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 12:14:42.000000 slackflylog-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog/agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog/agent/backends/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/agent.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/log.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/agent/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog/api/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/api/client.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/api/log_handler.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-13 02:08:31.000000 slackflylog-0.0.7/slackflylog/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 02:16:02.000000 slackflylog-0.0.7/slackflylog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-13 02:16:02.000000 slackflylog-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      656 2023-04-13 02:15:59.000000 slackflylog-0.0.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-13 02:16:02.000000 slackflylog-0.0.7/PKG-INFO
```

### Comparing `slackflylog-0.0.4/slackflylog/agent/backends/send_slack.py` & `slackflylog-0.0.7/slackflylog/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.4/slackflylog/agent/agent.py` & `slackflylog-0.0.7/slackflylog/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.4/slackflylog/agent/utils.py` & `slackflylog-0.0.7/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.4/slackflylog/api/client.py` & `slackflylog-0.0.7/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.4/slackflylog/api/log_handler.py` & `slackflylog-0.0.7/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.4/setup.py` & `slackflylog-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 import sys
 
-PY2 = sys.version_info[0] == 2
 
 # 基於flylog, slack-client處理
+
+PY2 = sys.version_info[0] == 2
 if PY2:
-    require_pack = ['slackclient==1.3.2']
-    pack_version = '0.0.4'
+    REQUIRE_PACK = ['slackclient==1.3.2']
+    __version__ = "0.0.7"
+
 else:
-    require_pack = ['slack_sdk==3.19.5']
-    pack_version = '1.0.4'
+    REQUIRE_PACK = ['slack_sdk==3.19.5']
+    __version__ = "3.0.7"
+
+
+
 
 setup(
     name='slackflylog',
-    version=pack_version,
+    version=__version__,
     author="dkxx00",
     author_email="hymanxx6@gmail.com",
     description="基于flylog的Slack日志发送",
     license="MIT",
     packages=find_packages(),
-    install_requires =require_pack,
+    install_requires =REQUIRE_PACK,
     url="https://github.com/dkxx00/slackflylog"
 )
```

