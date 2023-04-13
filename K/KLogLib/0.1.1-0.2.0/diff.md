# Comparing `tmp/KLogLib-0.1.1.tar.gz` & `tmp/KLogLib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.1.1.tar", last modified: Wed Apr 12 16:13:00 2023, max compression
+gzip compressed data, was "KLogLib-0.2.0.tar", last modified: Thu Apr 13 14:55:54 2023, max compression
```

## Comparing `KLogLib-0.1.1.tar` & `KLogLib-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.794055 KLogLib-0.1.1/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793174 KLogLib-0.1.1/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.1.1/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.1.1/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.1.1/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793423 KLogLib-0.1.1/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.1.1/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.1.1/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793876 KLogLib-0.1.1/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.1.1/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:13:00.794140 KLogLib-0.1.1/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.1.1/README.md
--rw-r--r--   0 javier     (501) staff       (20)      191 2023-04-12 16:13:00.794391 KLogLib-0.1.1/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      710 2023-04-12 16:12:50.000000 KLogLib-0.1.1/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-13 14:55:54.062704 KLogLib-0.2.0/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-13 14:55:54.061824 KLogLib-0.2.0/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.2.0/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.2.0/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3701 2023-04-13 14:40:54.000000 KLogLib-0.2.0/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-13 14:55:54.062085 KLogLib-0.2.0/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.2.0/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.2.0/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-13 14:55:54.062571 KLogLib-0.2.0/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)     2411 2023-04-13 14:55:54.000000 KLogLib-0.2.0/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-13 14:55:54.000000 KLogLib-0.2.0/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-13 14:55:54.000000 KLogLib-0.2.0/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-13 14:55:54.000000 KLogLib-0.2.0/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.2.0/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)     2411 2023-04-13 14:55:54.062772 KLogLib-0.2.0/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2232 2023-04-13 14:53:05.000000 KLogLib-0.2.0/README.md
+-rw-r--r--   0 javier     (501) staff       (20)      191 2023-04-13 14:55:54.062996 KLogLib-0.2.0/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      710 2023-04-13 14:55:49.000000 KLogLib-0.2.0/setup.py
```

### Comparing `KLogLib-0.1.1/Handlers/files_handler.py` & `KLogLib-0.2.0/Handlers/files_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os 
 import Handlers.byte
 from zipfile import ZipFile
 from datetime import datetime
 import tempfile
+import glob
 
 """
     Check if file exists
 
     Arguments:
     file:   string  |   Log file path
 """
@@ -40,14 +41,15 @@
 """
 def write(log_model):
     try:
         log_file = os.path.join(log_model.folder, log_model.log_name)
         
         if(log_model.is_zip == True):
             zip_log(log_file=log_file, max_size=log_model.max_size, log_folder=log_model.folder)
+            delete_oldest_zip(log_folder=log_model.folder, max_zips=log_model.max_zip)
 
         file_exists(log_file)
 
         with open(log_file, "a+") as f:
             f.write(f"{log_model.time}\t\t{log_model.where}\t\t{log_model.severity}\t\t{log_model.msg}")
             f.write("\n")
             f.close()
@@ -91,26 +93,42 @@
             f.close()
         
         zip_name = datetime.now().isoformat(sep=" ", timespec="seconds").replace('/', ':')
 
         with ZipFile(f"{log_folder}/{zip_name}.zip", "w") as log_zip:
             log_zip.write(temp_log_file.name, os.path.basename(temp_log_file.name))
             temp_log_file.close()
-        
-        delete_file(log_file=temp_log_file.name)
+
         delete_file(log_file=log_file)
 
     except:
         raise Exception("Error creating temp file")
     
 """
     This method delete the log file
 
     Arguments:
     temp_log_file:  string  |   Path to the temp log
 """
 def delete_file(log_file):
     try:
-        if os.path.exists(log_file):
-            os.remove(log_file)
+        if log_file != None:
+            if os.path.exists(log_file):
+                os.remove(log_file)
+    except:
+        raise Exception("Error deleting temp log")
+    
+"""
+    This method delete the oldest zip file
+
+    Arguments:
+
+"""
+def delete_oldest_zip(log_folder, max_zips):
+    try:
+        if os.path.exists(log_folder):
+            os.chdir(log_folder)
+            zip_files = glob.glob("*.zip")
+            if len(zip_files) > max_zips:
+                delete_file(sorted( zip_files, key = lambda file: os.path.getctime(file))[0])
     except:
-        raise Exception("Error deleting temp log")
+        raise Exception("Error deleting the oldest zip file")
```

### Comparing `KLogLib-0.1.1/KLog/KLog.py` & `KLogLib-0.2.0/KLog/KLog.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.1.1/KLogLib.egg-info/PKG-INFO` & `KLogLib-0.2.0/KLogLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KLogLib
-Version: 0.1.1
-Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.1
+Version: 0.2.0
+Home-page: https://github.com/javifriasj/KLog/releases/tag/0.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KLog
 
 KLog is a library which aims to bring easy logging in Python
 
@@ -71,8 +71,15 @@
 - severity: Log line type, can be one of those:
   - <img alt="Warning" src="https://img.shields.io/badge/WARNING-yellow"/>
   - <img alt="Warning" src="https://img.shields.io/badge/DEBUG-green"/>
   - <img alt="Warning" src="https://img.shields.io/badge/ERROR-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/CRITICAL-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/INFO-blue"/>
 
+<hr>
+
+Example of deleting zips
+
+
+
+https://user-images.githubusercontent.com/17411934/231798446-a4187172-878c-423a-9abd-1cf40e6c58bb.mov
```

### Comparing `KLogLib-0.1.1/LICENSE` & `KLogLib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.1.1/PKG-INFO` & `KLogLib-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KLogLib
-Version: 0.1.1
-Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.1
+Version: 0.2.0
+Home-page: https://github.com/javifriasj/KLog/releases/tag/0.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KLog
 
 KLog is a library which aims to bring easy logging in Python
 
@@ -71,8 +71,15 @@
 - severity: Log line type, can be one of those:
   - <img alt="Warning" src="https://img.shields.io/badge/WARNING-yellow"/>
   - <img alt="Warning" src="https://img.shields.io/badge/DEBUG-green"/>
   - <img alt="Warning" src="https://img.shields.io/badge/ERROR-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/CRITICAL-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/INFO-blue"/>
 
+<hr>
+
+Example of deleting zips
+
+
+
+https://user-images.githubusercontent.com/17411934/231798446-a4187172-878c-423a-9abd-1cf40e6c58bb.mov
```

### Comparing `KLogLib-0.1.1/README.md` & `KLogLib-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,8 +64,15 @@
 - severity: Log line type, can be one of those:
   - <img alt="Warning" src="https://img.shields.io/badge/WARNING-yellow"/>
   - <img alt="Warning" src="https://img.shields.io/badge/DEBUG-green"/>
   - <img alt="Warning" src="https://img.shields.io/badge/ERROR-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/CRITICAL-red"/>
   - <img alt="Warning" src="https://img.shields.io/badge/INFO-blue"/>
 
+<hr>
+
+Example of deleting zips
+
+
+
+https://user-images.githubusercontent.com/17411934/231798446-a4187172-878c-423a-9abd-1cf40e6c58bb.mov
```

### Comparing `KLogLib-0.1.1/setup.py` & `KLogLib-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 PACKAGE_NAME =  'KLogLib'
 AUTHOR = 'Javier Frias Jimenez'
 AUTHOR_EMAIL = 'javifriasj@gmail.com'
-URL = 'https://github.com/javifriasj/KLog/releases/tag/0.1.1'
+URL = 'https://github.com/javifriasj/KLog/releases/tag/0.2.0'
 LICENSE = 'MIT license'
 DESCRIPTION = 'Simple Log library'
 LONG_DESCRIPTION = ''
 LONG_DESC_TYPE = "text/markdown"
 INSTALL_REQUIRES = [
 
 ]
```

