# Comparing `tmp/slackflylog-0.0.8.tar.gz` & `tmp/slackflylog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-0.0.8.tar", last modified: Thu Apr 13 03:10:09 2023, max compression
+gzip compressed data, was "dist/slackflylog-1.0.0.tar", last modified: Thu Apr 13 04:25:33 2023, max compression
```

## Comparing `slackflylog-0.0.8.tar` & `slackflylog-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/slackflylog/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/slackflylog/agent/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/slackflylog/agent/backends/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     2041 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     3537 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/agent.py
--rw-r--r--   0 user_xh   (1001) users      (100)      123 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/log.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1795 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/agent/utils.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/slackflylog/api/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/api/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1174 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/api/client.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1599 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/api/log_handler.py
--rw-r--r--   0 user_xh   (1001) users      (100)      193 2023-04-13 02:58:07.000000 slackflylog-0.0.8/slackflylog/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)      182 2023-04-13 02:08:31.000000 slackflylog-0.0.8/slackflylog/constants.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 03:10:09.000000 slackflylog-0.0.8/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 03:10:08.000000 slackflylog-0.0.8/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)      515 2023-04-13 03:10:08.000000 slackflylog-0.0.8/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1001) users      (100)        1 2023-04-13 03:10:08.000000 slackflylog-0.0.8/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       19 2023-04-13 03:10:08.000000 slackflylog-0.0.8/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       12 2023-04-13 03:10:08.000000 slackflylog-0.0.8/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 user_xh   (1001) users      (100)      100 2023-04-13 03:10:09.000000 slackflylog-0.0.8/setup.cfg
--rw-r--r--   0 user_xh   (1001) users      (100)      656 2023-04-13 02:58:07.000000 slackflylog-0.0.8/setup.py
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 03:10:09.000000 slackflylog-0.0.8/PKG-INFO
+drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 04:25:33.000000 slackflylog-1.0.0/
+drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 04:25:33.000000 slackflylog-1.0.0/agent/
+drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 04:25:33.000000 slackflylog-1.0.0/agent/backends/
+-rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/backends/__init__.py
+-rw-r--r--   0 user_xh   (1001) users      (100)     2041 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/backends/send_slack.py
+-rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/__init__.py
+-rw-r--r--   0 user_xh   (1001) users      (100)     3537 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/agent.py
+-rw-r--r--   0 user_xh   (1001) users      (100)      123 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/log.py
+-rw-r--r--   0 user_xh   (1001) users      (100)     1795 2023-04-13 02:08:31.000000 slackflylog-1.0.0/agent/utils.py
+drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 04:25:33.000000 slackflylog-1.0.0/api/
+-rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.0/api/__init__.py
+-rw-r--r--   0 user_xh   (1001) users      (100)     1174 2023-04-13 02:08:31.000000 slackflylog-1.0.0/api/client.py
+-rw-r--r--   0 user_xh   (1001) users      (100)     1599 2023-04-13 02:08:31.000000 slackflylog-1.0.0/api/log_handler.py
+drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/
+-rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 user_xh   (1001) users      (100)      348 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 user_xh   (1001) users      (100)        1 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 user_xh   (1001) users      (100)       26 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 user_xh   (1001) users      (100)       10 2023-04-13 04:25:33.000000 slackflylog-1.0.0/slackflylog.egg-info/top_level.txt
+-rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 04:23:35.000000 slackflylog-1.0.0/setup.py
+-rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 04:25:33.000000 slackflylog-1.0.0/PKG-INFO
+-rw-r--r--   0 user_xh   (1001) users      (100)       38 2023-04-13 04:25:33.000000 slackflylog-1.0.0/setup.cfg
```

### Comparing `slackflylog-0.0.8/slackflylog/agent/backends/send_slack.py` & `slackflylog-1.0.0/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.8/slackflylog/agent/agent.py` & `slackflylog-1.0.0/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.8/slackflylog/agent/utils.py` & `slackflylog-1.0.0/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.8/slackflylog/api/client.py` & `slackflylog-1.0.0/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.8/slackflylog/api/log_handler.py` & `slackflylog-1.0.0/api/log_handler.py`

 * *Files identical despite different names*

