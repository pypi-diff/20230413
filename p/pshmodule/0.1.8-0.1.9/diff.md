# Comparing `tmp/pshmodule-0.1.8.tar.gz` & `tmp/pshmodule-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pshmodule-0.1.8.tar", last modified: Wed May  4 08:47:46 2022, max compression
+gzip compressed data, was "pshmodule-0.1.9.tar", last modified: Wed May  4 08:55:16 2022, max compression
```

## Comparing `pshmodule-0.1.8.tar` & `pshmodule-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.890907 pshmodule-0.1.8/
--rwxrwxrwx   0     1024 users      (100)     1743 2022-05-04 08:47:46.889907 pshmodule-0.1.8/PKG-INFO
--rwxrwxr-x   0     1024 users      (100)      903 2022-05-03 09:57:26.000000 pshmodule-0.1.8/README.md
--rwxrwxrwx   0     1024 users      (100)       38 2022-05-04 08:47:46.890907 pshmodule-0.1.8/setup.cfg
--rwxrwxr-x   0     1024 users      (100)     1029 2022-05-04 08:46:45.000000 pshmodule-0.1.8/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.864907 pshmodule-0.1.8/src/
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.870907 pshmodule-0.1.8/src/pshmodule/
--rwxrwxrwx   0     1024 users      (100)       21 2022-05-04 08:47:32.000000 pshmodule-0.1.8/src/pshmodule/__init__.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.880907 pshmodule-0.1.8/src/pshmodule/db/
--rwxrwxrwx   0     1024 users      (100)        0 2022-05-03 01:47:25.000000 pshmodule-0.1.8/src/pshmodule/db/__init__.py
--rwxrwxrwx   0     1024 users      (100)     3367 2022-05-04 08:18:44.000000 pshmodule-0.1.8/src/pshmodule/db/alchemy.py
--rwxrwxrwx   0     1024 users      (100)      675 2022-05-04 08:18:48.000000 pshmodule-0.1.8/src/pshmodule/db/config.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.882907 pshmodule-0.1.8/src/pshmodule/processing/
--rwxrwxrwx   0     1024 users      (100)       37 2022-05-04 08:46:02.000000 pshmodule-0.1.8/src/pshmodule/processing/__init__.py
--rwxrwxrwx   0     1024 users      (100)     5950 2022-05-04 08:44:59.000000 pshmodule-0.1.8/src/pshmodule/processing/processing.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.885907 pshmodule-0.1.8/src/pshmodule/selenium/
--rwxrwxr-x   0     1024 users      (100)       26 2022-05-04 05:40:08.000000 pshmodule-0.1.8/src/pshmodule/selenium/__init__.py
--rwxrwxr-x   0     1024 users      (100)     3563 2022-05-04 08:19:14.000000 pshmodule-0.1.8/src/pshmodule/selenium/helper.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.887907 pshmodule-0.1.8/src/pshmodule/utils/
--rwxrwxrwx   0     1024 users      (100)       39 2022-05-04 07:40:02.000000 pshmodule-0.1.8/src/pshmodule/utils/__init__.py
--rwxrwxrwx   0     1024 users      (100)     2013 2022-05-04 08:35:31.000000 pshmodule-0.1.8/src/pshmodule/utils/filemanager.py
-drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:47:46.876907 pshmodule-0.1.8/src/pshmodule.egg-info/
--rwxrwxrwx   0     1024 users      (100)     1743 2022-05-04 08:47:46.000000 pshmodule-0.1.8/src/pshmodule.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      523 2022-05-04 08:47:46.000000 pshmodule-0.1.8/src/pshmodule.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2022-05-04 08:47:46.000000 pshmodule-0.1.8/src/pshmodule.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       38 2022-05-04 08:47:46.000000 pshmodule-0.1.8/src/pshmodule.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       10 2022-05-04 08:47:46.000000 pshmodule-0.1.8/src/pshmodule.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.809924 pshmodule-0.1.9/
+-rwxrwxrwx   0     1024 users      (100)     1743 2022-05-04 08:55:16.809924 pshmodule-0.1.9/PKG-INFO
+-rwxrwxr-x   0     1024 users      (100)      903 2022-05-03 09:57:26.000000 pshmodule-0.1.9/README.md
+-rwxrwxrwx   0     1024 users      (100)       38 2022-05-04 08:55:16.810925 pshmodule-0.1.9/setup.cfg
+-rwxrwxr-x   0     1024 users      (100)     1029 2022-05-04 08:54:56.000000 pshmodule-0.1.9/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.778925 pshmodule-0.1.9/src/
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.783925 pshmodule-0.1.9/src/pshmodule/
+-rwxrwxrwx   0     1024 users      (100)       21 2022-05-04 08:54:58.000000 pshmodule-0.1.9/src/pshmodule/__init__.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.796925 pshmodule-0.1.9/src/pshmodule/db/
+-rwxrwxrwx   0     1024 users      (100)        0 2022-05-03 01:47:25.000000 pshmodule-0.1.9/src/pshmodule/db/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     3367 2022-05-04 08:18:44.000000 pshmodule-0.1.9/src/pshmodule/db/alchemy.py
+-rwxrwxrwx   0     1024 users      (100)      675 2022-05-04 08:18:48.000000 pshmodule-0.1.9/src/pshmodule/db/config.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.799924 pshmodule-0.1.9/src/pshmodule/processing/
+-rwxrwxrwx   0     1024 users      (100)       37 2022-05-04 08:52:09.000000 pshmodule-0.1.9/src/pshmodule/processing/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     5950 2022-05-04 08:44:59.000000 pshmodule-0.1.9/src/pshmodule/processing/processing.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.803925 pshmodule-0.1.9/src/pshmodule/selenium/
+-rwxrwxr-x   0     1024 users      (100)       26 2022-05-04 05:40:08.000000 pshmodule-0.1.9/src/pshmodule/selenium/__init__.py
+-rwxrwxr-x   0     1024 users      (100)     3563 2022-05-04 08:19:14.000000 pshmodule-0.1.9/src/pshmodule/selenium/helper.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.807925 pshmodule-0.1.9/src/pshmodule/utils/
+-rwxrwxrwx   0     1024 users      (100)       39 2022-05-04 07:40:02.000000 pshmodule-0.1.9/src/pshmodule/utils/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     2013 2022-05-04 08:35:31.000000 pshmodule-0.1.9/src/pshmodule/utils/filemanager.py
+drwxrwxrwx   0     1024 users      (100)        0 2022-05-04 08:55:16.791925 pshmodule-0.1.9/src/pshmodule.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     1743 2022-05-04 08:55:16.000000 pshmodule-0.1.9/src/pshmodule.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      523 2022-05-04 08:55:16.000000 pshmodule-0.1.9/src/pshmodule.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2022-05-04 08:55:16.000000 pshmodule-0.1.9/src/pshmodule.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2022-05-04 08:55:16.000000 pshmodule-0.1.9/src/pshmodule.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       10 2022-05-04 08:55:16.000000 pshmodule-0.1.9/src/pshmodule.egg-info/top_level.txt
```

### Comparing `pshmodule-0.1.8/PKG-INFO` & `pshmodule-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pshmodule
-Version: 0.1.8
+Version: 0.1.9
 Summary: Modules related to preprocessing, crawling, collection, database, data load & save 
 Home-page: https://github.com/hipster4020/package-module
 Author: shpark610
 Author-email: hipster4020@gmail.com
 License: UNKNOWN
 Description: # 🤖 AI Module
```

### Comparing `pshmodule-0.1.8/README.md` & `pshmodule-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/setup.py` & `pshmodule-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pshmodule",  # 프로젝트 이름
-    version="0.1.8",  # 프로젝트 버전
+    version="0.1.9",  # 프로젝트 버전
     description="Modules related to preprocessing, crawling, collection, database, data load & save ",  # 간단한 설명
     url="https://github.com/hipster4020/package-module",  # 프로젝트 주소
     author="shpark610",  # 작성자
     author_email="hipster4020@gmail.com",  # 작성자 이메일
     long_description=long_description,  # 프로젝트 설명, 보통 README.md로 관리
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `pshmodule-0.1.8/src/pshmodule/db/alchemy.py` & `pshmodule-0.1.9/src/pshmodule/db/alchemy.py`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/src/pshmodule/db/config.py` & `pshmodule-0.1.9/src/pshmodule/db/config.py`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/src/pshmodule/processing/processing.py` & `pshmodule-0.1.9/src/pshmodule/processing/processing.py`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/src/pshmodule/selenium/helper.py` & `pshmodule-0.1.9/src/pshmodule/selenium/helper.py`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/src/pshmodule/utils/filemanager.py` & `pshmodule-0.1.9/src/pshmodule/utils/filemanager.py`

 * *Files identical despite different names*

### Comparing `pshmodule-0.1.8/src/pshmodule.egg-info/PKG-INFO` & `pshmodule-0.1.9/src/pshmodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pshmodule
-Version: 0.1.8
+Version: 0.1.9
 Summary: Modules related to preprocessing, crawling, collection, database, data load & save 
 Home-page: https://github.com/hipster4020/package-module
 Author: shpark610
 Author-email: hipster4020@gmail.com
 License: UNKNOWN
 Description: # 🤖 AI Module
```

### Comparing `pshmodule-0.1.8/src/pshmodule.egg-info/SOURCES.txt` & `pshmodule-0.1.9/src/pshmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

