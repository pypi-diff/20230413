# Comparing `tmp/time_util_wj-1.0.3.tar.gz` & `tmp/time_util_wj-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_util_wj-1.0.3.tar", last modified: Wed Apr 12 08:26:43 2023, max compression
+gzip compressed data, was "time_util_wj-1.0.4.tar", last modified: Thu Apr 13 13:27:45 2023, max compression
```

## Comparing `time_util_wj-1.0.3.tar` & `time_util_wj-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:26:43.689494 time_util_wj-1.0.3/
--rw-r--r--   0 wangjie    (501) staff       (20)     1314 2023-04-12 08:26:43.689400 time_util_wj-1.0.3/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 08:26:43.689526 time_util_wj-1.0.3/setup.cfg
--rw-r--r--   0 wangjie    (501) staff       (20)      976 2023-04-12 08:26:35.000000 time_util_wj-1.0.3/setup.py
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:26:43.689275 time_util_wj-1.0.3/time_util_wj.egg-info/
--rw-r--r--   0 wangjie    (501) staff       (20)     1314 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)      166 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/SOURCES.txt
--rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/dependency_links.txt
--rw-r--r--   0 wangjie    (501) staff       (20)       11 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/top_level.txt
--rw-r--r--   0 wangjie    (501) staff       (20)     5374 2023-04-12 08:03:30.000000 time_util_wj-1.0.3/time_utils.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-13 13:27:45.303046 time_util_wj-1.0.4/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1318 2023-04-13 13:27:45.302919 time_util_wj-1.0.4/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-13 13:27:45.303088 time_util_wj-1.0.4/setup.cfg
+-rw-r--r--   0 wangjie    (501) staff       (20)     1056 2023-04-13 13:26:58.000000 time_util_wj-1.0.4/setup.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-13 13:27:45.302753 time_util_wj-1.0.4/time_util_wj.egg-info/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1318 2023-04-13 13:27:45.000000 time_util_wj-1.0.4/time_util_wj.egg-info/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)      168 2023-04-13 13:27:45.000000 time_util_wj-1.0.4/time_util_wj.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-13 13:27:45.000000 time_util_wj-1.0.4/time_util_wj.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)       13 2023-04-13 13:27:45.000000 time_util_wj-1.0.4/time_util_wj.egg-info/top_level.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)     5376 2023-04-13 13:25:14.000000 time_util_wj-1.0.4/time_util_wj.py
```

### Comparing `time_util_wj-1.0.3/PKG-INFO` & `time_util_wj-1.0.4/time_util_wj.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: time_util_wj
-Version: 1.0.3
+Name: time-util-wj
+Version: 1.0.4
 Summary: 提供了各种时间转换的方法
 Home-page: https://github.com/wangjie-jason/time_utils
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 Description-Content-Type: text/markdown
 
 将 python 的 requests 代码转换成 curl 命令
 
 # 安装
 
 ```python
-pip install time_utils
+pip install time-util-wj
 ```
 
 # 使用
 
 ```python
-from time_utils import TimeUtil
+from time_util_wj import TimeUtil
 
 print(TimeUtil.get_current_time_str())  ###获取当前字符串格式化时间
 print(TimeUtil.get_current_time_unix())  ###获取当前时间戳
 print(TimeUtil.get_seven_days_ago_time_unix())
 print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
 print(TimeUtil.unix_time_to_str(1657197749260))
 print(TimeUtil.get_recently_day(-7, 'unix'))
```

### Comparing `time_util_wj-1.0.3/setup.py` & `time_util_wj-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_util_wj",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.3",  # 程序版本
-    py_modules=['time_utils'],
+    version="1.0.4",  # 程序版本
+    py_modules=['time_util_wj'], # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="WangJie",  # 项目作者
     author_email="1641540482@qq.com",  # 作者邮件
     description="提供了各种时间转换的方法",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/wangjie-jason/time_utils",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

### Comparing `time_util_wj-1.0.3/time_util_wj.egg-info/PKG-INFO` & `time_util_wj-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: time-util-wj
-Version: 1.0.3
+Name: time_util_wj
+Version: 1.0.4
 Summary: 提供了各种时间转换的方法
 Home-page: https://github.com/wangjie-jason/time_utils
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 Description-Content-Type: text/markdown
 
 将 python 的 requests 代码转换成 curl 命令
 
 # 安装
 
 ```python
-pip install time_utils
+pip install time-util-wj
 ```
 
 # 使用
 
 ```python
-from time_utils import TimeUtil
+from time_util_wj import TimeUtil
 
 print(TimeUtil.get_current_time_str())  ###获取当前字符串格式化时间
 print(TimeUtil.get_current_time_unix())  ###获取当前时间戳
 print(TimeUtil.get_seven_days_ago_time_unix())
 print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
 print(TimeUtil.unix_time_to_str(1657197749260))
 print(TimeUtil.get_recently_day(-7, 'unix'))
```

### Comparing `time_util_wj-1.0.3/time_utils.py` & `time_util_wj-1.0.4/time_util_wj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # !/usr/bin/python
 # -*- coding:utf-8 -*-
 # @Time : 2022/7/7 19:11
 # @Author : wangjie
-# @File : time_utils.py
+# @File : time_util_wj.py
 # @project : SensoroApi
 import datetime
 import time
 
 
 class TimeUtil:
```

