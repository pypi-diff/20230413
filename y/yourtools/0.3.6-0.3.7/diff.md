# Comparing `tmp/yourtools-0.3.6.tar.gz` & `tmp/yourtools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yourtools-0.3.6.tar", last modified: Thu Apr 13 07:37:03 2023, max compression
+gzip compressed data, was "yourtools-0.3.7.tar", last modified: Thu Apr 13 07:53:12 2023, max compression
```

## Comparing `yourtools-0.3.6.tar` & `yourtools-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.037879 yourtools-0.3.6/
--rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:37:03.037594 yourtools-0.3.6/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)     2232 2023-04-07 10:28:09.000000 yourtools-0.3.6/README.md
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-07 10:28:09.000000 yourtools-0.3.6/requirements.txt
--rw-r--r--   0 zfang      (501) staff       (20)       38 2023-04-13 07:37:03.037965 yourtools-0.3.6/setup.cfg
--rw-r--r--   0 zfang      (501) staff       (20)     1577 2023-04-07 10:28:09.000000 yourtools-0.3.6/setup.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.032829 yourtools-0.3.6/yourtools/
--rw-r--r--   0 zfang      (501) staff       (20)     3842 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/Azkaban.py
--rw-r--r--   0 zfang      (501) staff       (20)      542 2023-04-13 07:35:46.000000 yourtools-0.3.6/yourtools/Time.py
--rw-r--r--   0 zfang      (501) staff       (20)     2893 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/WeChat.py
--rw-r--r--   0 zfang      (501) staff       (20)      465 2023-04-13 07:35:46.000000 yourtools-0.3.6/yourtools/__init__.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.037215 yourtools-0.3.6/yourtools/db/
--rw-r--r--   0 zfang      (501) staff       (20)      347 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/__init__.py
--rw-r--r--   0 zfang      (501) staff       (20)      739 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/dbutils.py
--rw-r--r--   0 zfang      (501) staff       (20)     2122 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/hive.py
--rw-r--r--   0 zfang      (501) staff       (20)     2416 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/mysql.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.035347 yourtools-0.3.6/yourtools.egg-info/
--rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)      372 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/SOURCES.txt
--rw-r--r--   0 zfang      (501) staff       (20)        1 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/dependency_links.txt
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/requires.txt
--rw-r--r--   0 zfang      (501) staff       (20)       10 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/top_level.txt
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.077796 yourtools-0.3.7/
+-rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:53:12.077366 yourtools-0.3.7/PKG-INFO
+-rw-r--r--   0 zfang      (501) staff       (20)     2232 2023-04-07 10:28:09.000000 yourtools-0.3.7/README.md
+-rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-07 10:28:09.000000 yourtools-0.3.7/requirements.txt
+-rw-r--r--   0 zfang      (501) staff       (20)       38 2023-04-13 07:53:12.077883 yourtools-0.3.7/setup.cfg
+-rw-r--r--   0 zfang      (501) staff       (20)     1577 2023-04-07 10:28:09.000000 yourtools-0.3.7/setup.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.072602 yourtools-0.3.7/yourtools/
+-rw-r--r--   0 zfang      (501) staff       (20)     3842 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/Azkaban.py
+-rw-r--r--   0 zfang      (501) staff       (20)      574 2023-04-13 07:52:20.000000 yourtools-0.3.7/yourtools/Time.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2893 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/WeChat.py
+-rw-r--r--   0 zfang      (501) staff       (20)      465 2023-04-13 07:35:46.000000 yourtools-0.3.7/yourtools/__init__.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.076857 yourtools-0.3.7/yourtools/db/
+-rw-r--r--   0 zfang      (501) staff       (20)      347 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/__init__.py
+-rw-r--r--   0 zfang      (501) staff       (20)      739 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/dbutils.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2122 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/hive.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2416 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/mysql.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.074866 yourtools-0.3.7/yourtools.egg-info/
+-rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/PKG-INFO
+-rw-r--r--   0 zfang      (501) staff       (20)      372 2023-04-13 07:53:12.000000 yourtools-0.3.7/yourtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zfang      (501) staff       (20)        1 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/requires.txt
+-rw-r--r--   0 zfang      (501) staff       (20)       10 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/top_level.txt
```

### Comparing `yourtools-0.3.6/PKG-INFO` & `yourtools-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.3.6/README.md` & `yourtools-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/requirements.txt` & `yourtools-0.3.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/setup.py` & `yourtools-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools/Azkaban.py` & `yourtools-0.3.7/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools/Time.py` & `yourtools-0.3.7/yourtools/Time.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 @modify time: 2023/4/13 3:35 PM
 @describe   : 
 -------------------------------------------------
 """
 from time import strftime, localtime
 
 
-def curr_time(time_format=None):
-    if time_format:
-        return strftime(time_format, localtime())
-    else:
-        return strftime("%Y-%m-%d %H:%M:%S", localtime())
+class Time:
+    def curr_time(time_format=None):
+        if time_format:
+            return strftime(time_format, localtime())
+        else:
+            return strftime("%Y-%m-%d %H:%M:%S", localtime())
```

### Comparing `yourtools-0.3.6/yourtools/WeChat.py` & `yourtools-0.3.7/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools/db/dbutils.py` & `yourtools-0.3.7/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools/db/hive.py` & `yourtools-0.3.7/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools/db/mysql.py` & `yourtools-0.3.7/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.6/yourtools.egg-info/PKG-INFO` & `yourtools-0.3.7/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.3.6/yourtools.egg-info/requires.txt` & `yourtools-0.3.7/yourtools.egg-info/requires.txt`

 * *Files identical despite different names*

