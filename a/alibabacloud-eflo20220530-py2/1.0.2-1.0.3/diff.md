# Comparing `tmp/alibabacloud_eflo20220530_py2-1.0.2.tar.gz` & `tmp/alibabacloud_eflo20220530_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo20220530_py2-1.0.2.tar", last modified: Thu Mar 30 09:59:28 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo20220530_py2-1.0.3.tar", last modified: Thu Apr 13 08:26:18 2023, max compression
```

## Comparing `alibabacloud_eflo20220530_py2-1.0.2.tar` & `alibabacloud_eflo20220530_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40460 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530/client.py
--rw-r--r--   0 root         (0) root         (0)   233121 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-03-30 09:59:28.000000 alibabacloud_eflo20220530_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81750 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530/client.py
+-rw-r--r--   0 root         (0) root         (0)   451003 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-04-13 08:26:18.000000 alibabacloud_eflo20220530_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/LICENSE` & `alibabacloud_eflo20220530_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/PKG-INFO` & `alibabacloud_eflo20220530_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo20220530_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo (20220530) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/README-CN.md` & `alibabacloud_eflo20220530_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/README.md` & `alibabacloud_eflo20220530_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/alibabacloud_eflo20220530_py2.egg-info/PKG-INFO` & `alibabacloud_eflo20220530_py2-1.0.3/alibabacloud_eflo20220530_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo20220530-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo (20220530) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo20220530_py2-1.0.2/setup.py` & `alibabacloud_eflo20220530_py2-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo20220530_py2.
 
-Created on 30/03/2023
+Created on 13/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo20220530"
 NAME = "alibabacloud_eflo20220530_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo (20220530) SDK Library for Python2"
```

