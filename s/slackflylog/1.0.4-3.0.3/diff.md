# Comparing `tmp/slackflylog-1.0.4.tar.gz` & `tmp/slackflylog-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-1.0.4.tar", last modified: Thu Apr 13 06:51:53 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.3.tar", last modified: Thu Apr 13 06:05:13 2023, max compression
```

## Comparing `slackflylog-1.0.4.tar` & `slackflylog-3.0.3.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 06:51:53.000000 slackflylog-1.0.4/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog/
--rw-r--r--   0 user_xh   (1001) users      (100)      281 2023-04-13 06:49:31.000000 slackflylog-1.0.4/slackflylog/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 06:49:31.000000 slackflylog-1.0.4/slackflylog/setup.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)      227 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1001) users      (100)        1 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       26 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       12 2023-04-13 06:51:53.000000 slackflylog-1.0.4/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 06:51:40.000000 slackflylog-1.0.4/setup.py
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 06:51:53.000000 slackflylog-1.0.4/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)       38 2023-04-13 06:51:53.000000 slackflylog-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.045209 slackflylog-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 06:05:13.045209 slackflylog-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 06:05:13.045209 slackflylog-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-13 06:04:05.000000 slackflylog-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.043208 slackflylog-3.0.3/slackflylog/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.044209 slackflylog-3.0.3/slackflylog/agent/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/agent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.044209 slackflylog-3.0.3/slackflylog/agent/backends/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/log.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/agent/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.045209 slackflylog-3.0.3/slackflylog/api/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/client.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/api/log_handler.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/constants.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-13 06:02:58.000000 slackflylog-3.0.3/slackflylog/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 06:05:13.043208 slackflylog-3.0.3/slackflylog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2023-04-13 06:05:13.000000 slackflylog-3.0.3/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 06:05:12.000000 slackflylog-3.0.3/slackflylog.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slackflylog-1.0.4/slackflylog/setup.py` & `slackflylog-3.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.4"
+    __version__ = "1.0.3"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.4"
+    __version__ = "3.0.3"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-1.0.4/setup.py` & `slackflylog-3.0.3/slackflylog/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.4"
+    __version__ = "1.0.0"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.4"
+    __version__ = "3.0.0"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

