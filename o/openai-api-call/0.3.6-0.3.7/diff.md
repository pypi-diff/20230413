# Comparing `tmp/openai_api_call-0.3.6.tar.gz` & `tmp/openai_api_call-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.6.tar", last modified: Thu Apr 13 08:14:43 2023, max compression
+gzip compressed data, was "openai_api_call-0.3.7.tar", last modified: Thu Apr 13 08:30:29 2023, max compression
```

## Comparing `openai_api_call-0.3.6.tar` & `openai_api_call-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:14:43.953670 openai_api_call-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:14:43.953670 openai_api_call-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:14:43.953670 openai_api_call-0.3.6/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:14:43.953670 openai_api_call-0.3.6/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:14:43.000000 openai_api_call-0.3.6/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:14:43.953670 openai_api_call-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:14:35.000000 openai_api_call-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/setup.py
```

### Comparing `openai_api_call-0.3.6/LICENSE` & `openai_api_call-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.6/PKG-INFO` & `openai_api_call-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.6
+Version: 0.3.7
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.3.6/README.md` & `openai_api_call-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.6/openai_api_call/__init__.py` & `openai_api_call-0.3.7/openai_api_call/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 import os
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
```

### Comparing `openai_api_call-0.3.6/openai_api_call/chattool.py` & `openai_api_call-0.3.7/openai_api_call/chattool.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             self._chat_log = []
         elif isinstance(msg, str):
             if openai_api_call.default_prompt is None:
                 self._chat_log = [{"role": "user", "content": msg}]
             else:
                 self._chat_log = openai_api_call.default_prompt(msg)
         elif isinstance(msg, list):
-            self._chat_log = msg
+            self._chat_log = msg.copy() # avoid changing the original list
         else:
             raise ValueError("msg should be a list of dict, a string or None")
         if api_key is None:
             self._api_key = openai_api_call.api_key
     
     @property
     def api_key(self):
```

### Comparing `openai_api_call-0.3.6/openai_api_call/proxy.py` & `openai_api_call-0.3.7/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.6/openai_api_call/request.py` & `openai_api_call-0.3.7/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.6/openai_api_call/response.py` & `openai_api_call-0.3.7/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.6/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.3.7/openai_api_call.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.6
+Version: 0.3.7
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.3.6/setup.py` & `openai_api_call-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.6'
+VERSION = '0.3.7'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

