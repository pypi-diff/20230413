# Comparing `tmp/yourtools-0.3.5.tar.gz` & `tmp/yourtools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yourtools-0.3.5.tar", last modified: Tue Mar 21 05:33:33 2023, max compression
+gzip compressed data, was "yourtools-0.3.6.tar", last modified: Thu Apr 13 07:37:03 2023, max compression
```

## Comparing `yourtools-0.3.5.tar` & `yourtools-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-03-21 05:33:33.803170 yourtools-0.3.5/
--rw-r--r--   0 zfang      (501) staff       (20)     2621 2023-03-21 05:33:33.802820 yourtools-0.3.5/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)     2232 2023-03-21 03:46:15.000000 yourtools-0.3.5/README.md
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-03-15 10:24:28.000000 yourtools-0.3.5/requirements.txt
--rw-r--r--   0 zfang      (501) staff       (20)       38 2023-03-21 05:33:33.803310 yourtools-0.3.5/setup.cfg
--rw-r--r--   0 zfang      (501) staff       (20)     1561 2023-03-21 04:20:56.000000 yourtools-0.3.5/setup.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-03-21 05:33:33.797968 yourtools-0.3.5/test/
--rw-r--r--   0 zfang      (501) staff       (20)     2978 2023-03-15 09:31:29.000000 yourtools-0.3.5/test/test.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-03-21 05:33:33.799276 yourtools-0.3.5/yourtools/
--rw-r--r--   0 zfang      (501) staff       (20)     2893 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/WeChat.py
--rw-r--r--   0 zfang      (501) staff       (20)      445 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/__init__.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-03-21 05:33:33.802367 yourtools-0.3.5/yourtools/db/
--rw-r--r--   0 zfang      (501) staff       (20)      347 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/db/__init__.py
--rw-r--r--   0 zfang      (501) staff       (20)      739 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/db/dbutils.py
--rw-r--r--   0 zfang      (501) staff       (20)     2122 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/db/hive.py
--rw-r--r--   0 zfang      (501) staff       (20)     2416 2023-03-15 10:23:48.000000 yourtools-0.3.5/yourtools/db/mysql.py
-drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-03-21 05:33:33.800986 yourtools-0.3.5/yourtools.egg-info/
--rw-r--r--   0 zfang      (501) staff       (20)     2621 2023-03-21 05:33:33.000000 yourtools-0.3.5/yourtools.egg-info/PKG-INFO
--rw-r--r--   0 zfang      (501) staff       (20)      346 2023-03-21 05:33:33.000000 yourtools-0.3.5/yourtools.egg-info/SOURCES.txt
--rw-r--r--   0 zfang      (501) staff       (20)        1 2023-03-21 05:33:33.000000 yourtools-0.3.5/yourtools.egg-info/dependency_links.txt
--rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-03-21 05:33:33.000000 yourtools-0.3.5/yourtools.egg-info/requires.txt
--rw-r--r--   0 zfang      (501) staff       (20)       10 2023-03-21 05:33:33.000000 yourtools-0.3.5/yourtools.egg-info/top_level.txt
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.037879 yourtools-0.3.6/
+-rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:37:03.037594 yourtools-0.3.6/PKG-INFO
+-rw-r--r--   0 zfang      (501) staff       (20)     2232 2023-04-07 10:28:09.000000 yourtools-0.3.6/README.md
+-rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-07 10:28:09.000000 yourtools-0.3.6/requirements.txt
+-rw-r--r--   0 zfang      (501) staff       (20)       38 2023-04-13 07:37:03.037965 yourtools-0.3.6/setup.cfg
+-rw-r--r--   0 zfang      (501) staff       (20)     1577 2023-04-07 10:28:09.000000 yourtools-0.3.6/setup.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.032829 yourtools-0.3.6/yourtools/
+-rw-r--r--   0 zfang      (501) staff       (20)     3842 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/Azkaban.py
+-rw-r--r--   0 zfang      (501) staff       (20)      542 2023-04-13 07:35:46.000000 yourtools-0.3.6/yourtools/Time.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2893 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/WeChat.py
+-rw-r--r--   0 zfang      (501) staff       (20)      465 2023-04-13 07:35:46.000000 yourtools-0.3.6/yourtools/__init__.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.037215 yourtools-0.3.6/yourtools/db/
+-rw-r--r--   0 zfang      (501) staff       (20)      347 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/__init__.py
+-rw-r--r--   0 zfang      (501) staff       (20)      739 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/dbutils.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2122 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/hive.py
+-rw-r--r--   0 zfang      (501) staff       (20)     2416 2023-04-07 10:28:09.000000 yourtools-0.3.6/yourtools/db/mysql.py
+drwxr-xr-x   0 zfang      (501) staff       (20)        0 2023-04-13 07:37:03.035347 yourtools-0.3.6/yourtools.egg-info/
+-rw-r--r--   0 zfang      (501) staff       (20)     2658 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/PKG-INFO
+-rw-r--r--   0 zfang      (501) staff       (20)      372 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zfang      (501) staff       (20)        1 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zfang      (501) staff       (20)     1075 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/requires.txt
+-rw-r--r--   0 zfang      (501) staff       (20)       10 2023-04-13 07:37:02.000000 yourtools-0.3.6/yourtools.egg-info/top_level.txt
```

### Comparing `yourtools-0.3.5/PKG-INFO` & `yourtools-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Python tools
@@ -105,7 +107,9 @@
     "enable_id_trans": 0,
     "enable_duplicate_check": 0,
     "duplicate_check_interval": 1800
 }
 send_statu = qw.send_msg(data)
 print(send_statu)
 ```
+
+
```

### Comparing `yourtools-0.3.5/README.md` & `yourtools-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/requirements.txt` & `yourtools-0.3.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/setup.py` & `yourtools-0.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import re
 
-with open('version') as f:
+with open('VERSION') as f:
     version_str = f.read()
 
 
 def get_version():
     # 从版本号字符串中提取三个数字并将它们转换为整数类型
     match = re.search(r"(\d+)\.(\d+)\.(\d+)", version_str)
     major = int(match.group(1))
@@ -47,14 +47,14 @@
     ],
     python_requires='>=3.6',
     install_requires=required,
 )
 
 
 def write_now_version():
-    print("Current version:", get_version())
-    with open("version", "w") as f:
-        f.write(get_version())
+    print("Current VERSION:", get_version())
+    with open("VERSION", "w") as version_f:
+        version_f.write(get_version())
 
 
 # 将新的版本号字符串回写入文件中
 write_now_version()
```

### Comparing `yourtools-0.3.5/yourtools/WeChat.py` & `yourtools-0.3.6/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/yourtools/db/dbutils.py` & `yourtools-0.3.6/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/yourtools/db/hive.py` & `yourtools-0.3.6/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/yourtools/db/mysql.py` & `yourtools-0.3.6/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.3.5/yourtools.egg-info/PKG-INFO` & `yourtools-0.3.6/yourtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Python tools
@@ -105,7 +107,9 @@
     "enable_id_trans": 0,
     "enable_duplicate_check": 0,
     "duplicate_check_interval": 1800
 }
 send_statu = qw.send_msg(data)
 print(send_statu)
 ```
+
+
```

### Comparing `yourtools-0.3.5/yourtools.egg-info/requires.txt` & `yourtools-0.3.6/yourtools.egg-info/requires.txt`

 * *Files identical despite different names*

