# Comparing `tmp/yourtools-0.3.7.tar.gz` & `tmp/yourtools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yourtools-0.3.7.tar", last modified: Thu Apr 13 07:53:12 2023, max compression
+gzip compressed data, was "dist/yourtools-0.3.9.tar", last modified: Thu Apr 13 08:42:49 2023, max compression
```

## Comparing `yourtools-0.3.7.tar` & `yourtools-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.077796 yourtools-0.3.7/
--rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:53:12.077366 yourtools-0.3.7/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)     2232 2023-04-07 10:28:09.000000 yourtools-0.3.7/README.md
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-07 10:28:09.000000 yourtools-0.3.7/requirements.txt
--rw-r--r--   0 zfang      (501) staff       (20)       38 2023-04-13 07:53:12.077883 yourtools-0.3.7/setup.cfg
--rw-r--r--   0 zfang      (501) staff       (20)     1577 2023-04-07 10:28:09.000000 yourtools-0.3.7/setup.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.072602 yourtools-0.3.7/yourtools/
--rw-r--r--   0 zfang      (501) staff       (20)     3842 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/Azkaban.py
--rw-r--r--   0 zfang      (501) staff       (20)      574 2023-04-13 07:52:20.000000 yourtools-0.3.7/yourtools/Time.py
--rw-r--r--   0 zfang      (501) staff       (20)     2893 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/WeChat.py
--rw-r--r--   0 zfang      (501) staff       (20)      465 2023-04-13 07:35:46.000000 yourtools-0.3.7/yourtools/__init__.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.076857 yourtools-0.3.7/yourtools/db/
--rw-r--r--   0 zfang      (501) staff       (20)      347 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/__init__.py
--rw-r--r--   0 zfang      (501) staff       (20)      739 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/dbutils.py
--rw-r--r--   0 zfang      (501) staff       (20)     2122 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/hive.py
--rw-r--r--   0 zfang      (501) staff       (20)     2416 2023-04-07 10:28:09.000000 yourtools-0.3.7/yourtools/db/mysql.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:53:12.074866 yourtools-0.3.7/yourtools.egg-info/
--rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)      372 2023-04-13 07:53:12.000000 yourtools-0.3.7/yourtools.egg-info/SOURCES.txt
--rw-r--r--   0 zfang      (501) staff       (20)        1 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/dependency_links.txt
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/requires.txt
--rw-r--r--   0 zfang      (501) staff       (20)       10 2023-04-13 07:53:11.000000 yourtools-0.3.7/yourtools.egg-info/top_level.txt
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 08:42:49.000000 yourtools-0.3.9/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2416 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      574 2023-04-13 07:52:20.000000 yourtools-0.3.9/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2893 2023-04-07 10:28:09.000000 yourtools-0.3.9/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      465 2023-04-13 07:35:46.000000 yourtools-0.3.9/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-13 08:42:49.000000 yourtools-0.3.9/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.3.9/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.3.9/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.3.9/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 08:42:49.000000 yourtools-0.3.9/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-13 08:42:49.000000 yourtools-0.3.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `yourtools-0.3.7/PKG-INFO` & `yourtools-0.3.9/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.7
+Version: 0.3.9
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.3.7/README.md` & `yourtools-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/setup.py` & `yourtools-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/Azkaban.py` & `yourtools-0.3.9/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/Time.py` & `yourtools-0.3.9/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/WeChat.py` & `yourtools-0.3.9/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/db/dbutils.py` & `yourtools-0.3.9/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/db/hive.py` & `yourtools-0.3.9/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools/db/mysql.py` & `yourtools-0.3.9/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.7/yourtools.egg-info/PKG-INFO` & `yourtools-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.7
+Version: 0.3.9
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

