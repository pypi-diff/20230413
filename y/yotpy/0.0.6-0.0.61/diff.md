# Comparing `tmp/yotpy-0.0.6.tar.gz` & `tmp/yotpy-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.6.tar", last modified: Wed Apr 12 23:05:18 2023, max compression
+gzip compressed data, was "yotpy-0.0.61.tar", last modified: Wed Apr 12 23:16:04 2023, max compression
```

## Comparing `yotpy-0.0.6.tar` & `yotpy-0.0.61.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      762 2023-04-12 22:08:19.101801 yotpy-0.0.6/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.6/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.6/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.6/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.6/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.6/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.6/docs/yotpy.html
--rw-r--r--   0        0        0     1883 2023-04-12 22:50:16.599595 yotpy-0.0.6/exceptions.py
--rw-r--r--   0        0        0      830 2023-04-12 22:19:29.450917 yotpy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    30802 2023-04-12 22:57:51.962214 yotpy-0.0.6/yotpy.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 yotpy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.61/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.61/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.61/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.61/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 23:07:55.942421 yotpy-0.0.61/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.61/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.61/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.61/docs/yotpy.html
+-rw-r--r--   0        0        0     1883 2023-04-12 22:50:16.599595 yotpy-0.0.61/exceptions.py
+-rw-r--r--   0        0        0      830 2023-04-12 22:19:29.450917 yotpy-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0    30803 2023-04-12 23:08:26.829890 yotpy-0.0.61/yotpy.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.61/PKG-INFO
```

### Comparing `yotpy-0.0.6/LICENSE` & `yotpy-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.6/docs/search.js` & `yotpy-0.0.61/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.6/docs/yotpy.html` & `yotpy-0.0.61/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.6/exceptions.py` & `yotpy-0.0.61/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.6/pyproject.toml` & `yotpy-0.0.61/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.6/yotpy.py` & `yotpy-0.0.61/yotpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 """
 
-__version__ = "0.0.6"
+__version__ = "0.0.61"
 
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
```

### Comparing `yotpy-0.0.6/PKG-INFO` & `yotpy-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.6
+Version: 0.0.61
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

