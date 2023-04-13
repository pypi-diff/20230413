# Comparing `tmp/logkk-0.4.0.tar.gz` & `tmp/logkk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkk-0.4.0.tar", last modified: Fri Mar 31 03:16:10 2023, max compression
+gzip compressed data, was "logkk-0.5.0.tar", last modified: Thu Apr 13 03:07:10 2023, max compression
```

## Comparing `logkk-0.4.0.tar` & `logkk-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 03:16:10.731361 logkk-0.4.0/
--rw-rw-rw-   0        0        0     1267 2023-03-31 03:16:10.731361 logkk-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      833 2023-03-03 10:19:55.000000 logkk-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 03:16:10.699343 logkk-0.4.0/logkk/
--rw-rw-rw-   0        0        0       69 2023-03-03 04:07:46.000000 logkk-0.4.0/logkk/__init__.py
--rw-rw-rw-   0        0        0      206 2023-03-03 04:07:33.000000 logkk-0.4.0/logkk/errors.py
--rw-rw-rw-   0        0        0      884 2023-03-31 03:13:58.000000 logkk-0.4.0/logkk/handlers.py
--rw-rw-rw-   0        0        0      134 2023-03-01 03:30:08.000000 logkk-0.4.0/logkk/level.py
--rw-rw-rw-   0        0        0     2347 2023-03-03 09:07:54.000000 logkk-0.4.0/logkk/logger.py
--rw-rw-rw-   0        0        0     1739 2023-03-03 09:07:54.000000 logkk-0.4.0/logkk/manager.py
-drwxrwxrwx   0        0        0        0 2023-03-31 03:16:10.730361 logkk-0.4.0/logkk.egg-info/
--rw-rw-rw-   0        0        0     1267 2023-03-31 03:16:10.000000 logkk-0.4.0/logkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-03-31 03:16:10.000000 logkk-0.4.0/logkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 03:16:10.000000 logkk-0.4.0/logkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-31 03:16:10.000000 logkk-0.4.0/logkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 03:16:10.731361 logkk-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-03-31 03:14:09.000000 logkk-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.230152 logkk-0.5.0/
+-rw-rw-rw-   0        0        0     1267 2023-04-13 03:07:10.225179 logkk-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2023-03-03 10:19:55.000000 logkk-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.202143 logkk-0.5.0/logkk/
+-rw-rw-rw-   0        0        0       69 2023-03-03 04:07:46.000000 logkk-0.5.0/logkk/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-03-03 04:07:33.000000 logkk-0.5.0/logkk/errors.py
+-rw-rw-rw-   0        0        0      896 2023-04-13 03:03:46.000000 logkk-0.5.0/logkk/handlers.py
+-rw-rw-rw-   0        0        0      134 2023-03-01 03:30:08.000000 logkk-0.5.0/logkk/level.py
+-rw-rw-rw-   0        0        0     2347 2023-03-03 09:07:54.000000 logkk-0.5.0/logkk/logger.py
+-rw-rw-rw-   0        0        0     1739 2023-03-03 09:07:54.000000 logkk-0.5.0/logkk/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.223144 logkk-0.5.0/logkk.egg-info/
+-rw-rw-rw-   0        0        0     1267 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:07:10.230152 logkk-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-04-13 03:04:28.000000 logkk-0.5.0/setup.py
```

### Comparing `logkk-0.4.0/PKG-INFO` & `logkk-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkk
-Version: 0.4.0
+Version: 0.5.0
 Summary: 日志组件
 Home-page: https://github.com/olivetree/logkk
 Author: olivetree
 Author-email: olivetree123@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logkk-0.4.0/README.md` & `logkk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `logkk-0.4.0/logkk/handlers.py` & `logkk-0.5.0/logkk/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         pass
 
 
 class StreamHandler(Handler):
 
     def write(self, content):
         with stream_lock:
-            print(content)
+            print(content, flush=True)
 
 
 class FileHandler(Handler):
 
     def __init__(self, filepath, encoding="utf8"):
         self.filepath = filepath
         self.encoding = encoding
```

### Comparing `logkk-0.4.0/logkk/logger.py` & `logkk-0.5.0/logkk/logger.py`

 * *Files identical despite different names*

### Comparing `logkk-0.4.0/logkk/manager.py` & `logkk-0.5.0/logkk/manager.py`

 * *Files identical despite different names*

### Comparing `logkk-0.4.0/logkk.egg-info/PKG-INFO` & `logkk-0.5.0/logkk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkk
-Version: 0.4.0
+Version: 0.5.0
 Summary: 日志组件
 Home-page: https://github.com/olivetree/logkk
 Author: olivetree
 Author-email: olivetree123@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logkk-0.4.0/setup.py` & `logkk-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logkk",  # 模块名称
-    version="0.4.0",  # 当前版本
+    version="0.5.0",  # 当前版本
     author="olivetree",  # 作者
     author_email="olivetree123@163.com",  # 作者邮箱
     description="日志组件",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/olivetree/logkk",  # 模块github地址
     packages=["logkk"],  # 自动找到项目中导入的模块
```

