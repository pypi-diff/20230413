# Comparing `tmp/gpt-api-0.1.1.tar.gz` & `tmp/gpt-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-api-0.1.1.tar", last modified: Thu Apr 13 02:23:57 2023, max compression
+gzip compressed data, was "gpt-api-0.1.2.tar", last modified: Thu Apr 13 09:31:33 2023, max compression
```

## Comparing `gpt-api-0.1.1.tar` & `gpt-api-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.857870 gpt-api-0.1.1/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 02:23:57.857556 gpt-api-0.1.1/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.854143 gpt-api-0.1.1/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.1/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     3762 2023-04-13 02:09:07.000000 gpt-api-0.1.1/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.857118 gpt-api-0.1.1/gpt_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-13 02:23:57.857995 gpt-api-0.1.1/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.1/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.239142 gpt-api-0.1.2/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 09:31:33.238877 gpt-api-0.1.2/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.236752 gpt-api-0.1.2/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.2/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     3757 2023-04-13 09:31:10.000000 gpt-api-0.1.2/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.238499 gpt-api-0.1.2/gpt_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-13 09:31:33.239241 gpt-api-0.1.2/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.2/setup.py
```

### Comparing `gpt-api-0.1.1/api/gpt.py` & `gpt-api-0.1.2/api/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 from pathlib import Path
 log = getLogger(__name__)
 log.setLevel(INFO)
 
 
 class GPT4(object):
-    def __init__(self, key=None, model='gpt-4-0314', temperature=0.8, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None):
+    def __init__(self, key=None, model='gpt-4', temperature=0.8, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None):
         if os.environ.get("OPENAI_API_KEY") is None:
             if key:
                 openai.api_key = key
         self.model = model
         self.temperature = temperature
         # 用于控制生成文本的随机性和创造性的参数。值越高，生成文本越随机和创造性；值越低，生成文本越可预测和保守
         self.top_p = top_p
```

### Comparing `gpt-api-0.1.1/setup.py` & `gpt-api-0.1.2/setup.py`

 * *Files identical despite different names*

