# Comparing `tmp/slackflylog-1.0.3.tar.gz` & `tmp/slackflylog-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-1.0.3.tar", last modified: Thu Apr 13 05:34:58 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.3.tar", last modified: Thu Apr 13 06:05:13 2023, max compression
```

## Comparing `slackflylog-1.0.3.tar` & `slackflylog-3.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog/agent/
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog/agent/backends/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     2041 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     3537 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/agent.py
--rw-r--r--   0 user_xh   (1001) users      (100)      123 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/log.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1795 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/agent/utils.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog/api/
--rw-r--r--   0 user_xh   (1001) users      (100)       23 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/api/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1174 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/api/client.py
--rw-r--r--   0 user_xh   (1001) users      (100)     1599 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/api/log_handler.py
--rw-r--r--   0 user_xh   (1001) users      (100)      281 2023-04-13 04:23:35.000000 slackflylog-1.0.3/slackflylog/__init__.py
--rw-r--r--   0 user_xh   (1001) users      (100)      182 2023-04-13 02:08:31.000000 slackflylog-1.0.3/slackflylog/constants.py
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 04:23:35.000000 slackflylog-1.0.3/slackflylog/setup.py
-drwxr-xr-x   0 user_xh   (1001) users      (100)        0 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)      526 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1001) users      (100)        1 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       26 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1001) users      (100)       12 2023-04-13 05:34:58.000000 slackflylog-1.0.3/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 user_xh   (1001) users      (100)      639 2023-04-13 05:34:47.000000 slackflylog-1.0.3/setup.py
--rw-r--r--   0 user_xh   (1001) users      (100)      246 2023-04-13 05:34:58.000000 slackflylog-1.0.3/PKG-INFO
--rw-r--r--   0 user_xh   (1001) users      (100)       38 2023-04-13 05:34:58.000000 slackflylog-1.0.3/setup.cfg
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

### Comparing `slackflylog-1.0.3/slackflylog/agent/backends/send_slack.py` & `slackflylog-3.0.3/slackflylog/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog/agent/agent.py` & `slackflylog-3.0.3/slackflylog/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog/agent/utils.py` & `slackflylog-3.0.3/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog/api/client.py` & `slackflylog-3.0.3/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog/api/log_handler.py` & `slackflylog-3.0.3/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog/setup.py` & `slackflylog-3.0.3/slackflylog/setup.py`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/slackflylog.egg-info/SOURCES.txt` & `slackflylog-3.0.3/slackflylog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slackflylog-1.0.3/setup.py` & `slackflylog-3.0.3/setup.py`

 * *Files identical despite different names*

