# Comparing `tmp/occe_api-1.0.0.tar.gz` & `tmp/occe_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "occe_api-1.0.0.tar", last modified: Thu Apr 13 02:11:46 2023, max compression
+gzip compressed data, was "occe_api-1.0.1.tar", last modified: Thu Apr 13 03:07:53 2023, max compression
```

## Comparing `occe_api-1.0.0.tar` & `occe_api-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 02:11:46.911511 occe_api-1.0.0/
--rw-r--r--   0 sleb      (1000) sleb      (1000)     1084 2023-04-11 11:01:21.000000 occe_api-1.0.0/LICENSE
--rw-r--r--   0 sleb      (1000) sleb      (1000)     1412 2023-04-13 02:11:46.911511 occe_api-1.0.0/PKG-INFO
--rw-r--r--   0 sleb      (1000) sleb      (1000)      957 2023-04-11 14:05:00.000000 occe_api-1.0.0/README.md
-drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 02:11:46.895511 occe_api-1.0.0/occe_api/
--rw-r--r--   0 sleb      (1000) sleb      (1000)        0 2023-04-13 01:44:33.000000 occe_api-1.0.0/occe_api/__init__.py
--rw-r--r--   0 sleb      (1000) sleb      (1000)    20754 2023-04-13 01:24:53.000000 occe_api-1.0.0/occe_api/main.py
-drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 02:11:46.911511 occe_api-1.0.0/occe_api.egg-info/
--rw-r--r--   0 sleb      (1000) sleb      (1000)     1412 2023-04-13 02:11:46.000000 occe_api-1.0.0/occe_api.egg-info/PKG-INFO
--rw-r--r--   0 sleb      (1000) sleb      (1000)      233 2023-04-13 02:11:46.000000 occe_api-1.0.0/occe_api.egg-info/SOURCES.txt
--rw-r--r--   0 sleb      (1000) sleb      (1000)        1 2023-04-13 02:11:46.000000 occe_api-1.0.0/occe_api.egg-info/dependency_links.txt
--rw-r--r--   0 sleb      (1000) sleb      (1000)       17 2023-04-13 02:11:46.000000 occe_api-1.0.0/occe_api.egg-info/requires.txt
--rw-r--r--   0 sleb      (1000) sleb      (1000)        9 2023-04-13 02:11:46.000000 occe_api-1.0.0/occe_api.egg-info/top_level.txt
--rw-r--r--   0 sleb      (1000) sleb      (1000)       38 2023-04-13 02:11:46.915511 occe_api-1.0.0/setup.cfg
--rw-r--r--   0 sleb      (1000) sleb      (1000)      771 2023-04-13 01:58:19.000000 occe_api-1.0.0/setup.py
+drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 03:07:53.143249 occe_api-1.0.1/
+-rw-r--r--   0 sleb      (1000) sleb      (1000)     1084 2023-04-11 11:01:21.000000 occe_api-1.0.1/LICENSE
+-rw-r--r--   0 sleb      (1000) sleb      (1000)     1616 2023-04-13 03:07:53.147249 occe_api-1.0.1/PKG-INFO
+-rw-r--r--   0 sleb      (1000) sleb      (1000)     1167 2023-04-13 03:06:39.000000 occe_api-1.0.1/README.md
+drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 03:07:53.143249 occe_api-1.0.1/occe-api/
+-rw-r--r--   0 sleb      (1000) sleb      (1000)        0 2023-04-13 02:46:29.000000 occe_api-1.0.1/occe-api/__init__.py
+-rw-r--r--   0 sleb      (1000) sleb      (1000)    20754 2023-04-13 01:24:53.000000 occe_api-1.0.1/occe-api/api.py
+drwxr-xr-x   0 sleb      (1000) sleb      (1000)        0 2023-04-13 03:07:53.143249 occe_api-1.0.1/occe_api.egg-info/
+-rw-r--r--   0 sleb      (1000) sleb      (1000)     1616 2023-04-13 03:07:52.000000 occe_api-1.0.1/occe_api.egg-info/PKG-INFO
+-rw-r--r--   0 sleb      (1000) sleb      (1000)      232 2023-04-13 03:07:52.000000 occe_api-1.0.1/occe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sleb      (1000) sleb      (1000)        1 2023-04-13 03:07:52.000000 occe_api-1.0.1/occe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sleb      (1000) sleb      (1000)       17 2023-04-13 03:07:52.000000 occe_api-1.0.1/occe_api.egg-info/requires.txt
+-rw-r--r--   0 sleb      (1000) sleb      (1000)        9 2023-04-13 03:07:52.000000 occe_api-1.0.1/occe_api.egg-info/top_level.txt
+-rw-r--r--   0 sleb      (1000) sleb      (1000)       38 2023-04-13 03:07:53.147249 occe_api-1.0.1/setup.cfg
+-rw-r--r--   0 sleb      (1000) sleb      (1000)      771 2023-04-13 03:03:59.000000 occe_api-1.0.1/setup.py
```

### Comparing `occe_api-1.0.0/LICENSE` & `occe_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `occe_api-1.0.0/PKG-INFO` & `occe_api-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: occe_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for occe.io stock
 Home-page: http://occe.io/
 Author: surugh
 Author-email: surugh@gmail.com
 Project-URL: Documentation, http://occe.io/info#api
 Keywords: occe python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# occe_api_v3
+# occe_api_v3  
+pip install occe-api  
+  
+from occe_api import api  
+occe = api.Occe(access_key=TRADE_ACCESS, secret_key=TRADE_SECRET)  
+occe_cashier = api.Occe(access_key=CASHIER_ACCESS, secret_key=CASHIER_SECRET)  
+
 [Occe.io](http://occe.io/) API v3 python wrapper
   
 [Документация | Documentation](http://occe.io/info#api)  
 [Телеграм | Telegram](https://t.me/occeio)
   
 Примеры использования находятся в example.py,  
 не забудьте указать свои API ключи в файле .env
```

### Comparing `occe_api-1.0.0/README.md` & `occe_api-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# occe_api_v3
+# occe_api_v3  
+pip install occe-api  
+  
+from occe_api import api  
+occe = api.Occe(access_key=TRADE_ACCESS, secret_key=TRADE_SECRET)  
+occe_cashier = api.Occe(access_key=CASHIER_ACCESS, secret_key=CASHIER_SECRET)  
+
 [Occe.io](http://occe.io/) API v3 python wrapper
   
 [Документация | Documentation](http://occe.io/info#api)  
 [Телеграм | Telegram](https://t.me/occeio)
   
 Примеры использования находятся в example.py,  
 не забудьте указать свои API ключи в файле .env
```

### Comparing `occe_api-1.0.0/occe_api/main.py` & `occe_api-1.0.1/occe-api/api.py`

 * *Files identical despite different names*

### Comparing `occe_api-1.0.0/occe_api.egg-info/PKG-INFO` & `occe_api-1.0.1/occe_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: occe-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for occe.io stock
 Home-page: http://occe.io/
 Author: surugh
 Author-email: surugh@gmail.com
 Project-URL: Documentation, http://occe.io/info#api
 Keywords: occe python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# occe_api_v3
+# occe_api_v3  
+pip install occe-api  
+  
+from occe_api import api  
+occe = api.Occe(access_key=TRADE_ACCESS, secret_key=TRADE_SECRET)  
+occe_cashier = api.Occe(access_key=CASHIER_ACCESS, secret_key=CASHIER_SECRET)  
+
 [Occe.io](http://occe.io/) API v3 python wrapper
   
 [Документация | Documentation](http://occe.io/info#api)  
 [Телеграм | Telegram](https://t.me/occeio)
   
 Примеры использования находятся в example.py,  
 не забудьте указать свои API ключи в файле .env
```

### Comparing `occe_api-1.0.0/setup.py` & `occe_api-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='occe_api',
-    version='1.0.0',
+    version='1.0.1',
     author='surugh',
     author_email='surugh@gmail.com',
     description='Python wrapper for occe.io stock',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='http://occe.io/',
     packages=find_packages(),
```

