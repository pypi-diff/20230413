# Comparing `tmp/slackflylog-1.0.5.tar.gz` & `tmp/slackflylog-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-1.0.5.tar", last modified: Thu Apr 13 07:26:40 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.4.tar", last modified: Thu Apr 13 06:57:23 2023, max compression
```

## Comparing `slackflylog-1.0.5.tar` & `slackflylog-3.0.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog/agent/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog/agent/backends/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     2114 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     3640 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/agent.py
--rw-r--r--   0 user_xh   (1001) users      (100)      123 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/log.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1795 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/agent/utils.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog/api/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/api/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1174 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/api/client.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1599 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/api/log_handler.py
--rw-r--r--   0 user_xh   (1001) users      (100)      281 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)      182 2023-04-13 07:23:04.000000 slackflylog-1.0.5/slackflylog/constants.py
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 07:23:36.000000 slackflylog-1.0.5/slackflylog/setup.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)      526 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1001) users      (100)        1 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       26 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       12 2023-04-13 07:26:40.000000 slackflylog-1.0.5/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 07:26:13.000000 slackflylog-1.0.5/setup.py
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 07:26:40.000000 slackflylog-1.0.5/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)       38 2023-04-13 07:26:40.000000 slackflylog-1.0.5/setup.cfg
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

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slackflylog-1.0.5/slackflylog/agent/backends/send_slack.py` & `slackflylog-3.0.4/slackflylog/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.5/slackflylog/agent/agent.py` & `slackflylog-3.0.4/slackflylog/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.5/slackflylog/agent/utils.py` & `slackflylog-3.0.4/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.5/slackflylog/api/client.py` & `slackflylog-3.0.4/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.5/slackflylog/api/log_handler.py` & `slackflylog-3.0.4/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.5/slackflylog/setup.py` & `slackflylog-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.5"
+    __version__ = "1.0.4"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
     __version__ = "3.0.4"
```

### Comparing `slackflylog-1.0.5/slackflylog.egg-info/SOURCES.txt` & `slackflylog-3.0.4/slackflylog.egg-info/SOURCES.txt`

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

### Comparing `slackflylog-1.0.5/setup.py` & `slackflylog-3.0.4/slackflylog/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.5"
+    __version__ = "1.0.4"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
     __version__ = "3.0.4"
```

