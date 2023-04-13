# Comparing `tmp/recursive_size-1.1.tar.gz` & `tmp/recursive_size-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recursive_size-1.1.tar", last modified: Sun Feb 21 20:43:00 2021, max compression
+gzip compressed data, was "recursive_size-1.2.tar", last modified: Thu Apr 13 11:52:41 2023, max compression
```

## Comparing `recursive_size-1.1.tar` & `recursive_size-1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-21 20:43:00.531962 recursive_size-1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2021-02-21 20:43:00.531962 recursive_size-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      221 2021-02-21 20:42:50.000000 recursive_size-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-21 20:43:00.531962 recursive_size-1.1/recursive_size/
--rw-r--r--   0 runner    (1001) docker     (116)     1759 2021-02-21 20:42:50.000000 recursive_size-1.1/recursive_size/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-21 20:43:00.531962 recursive_size-1.1/recursive_size.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2021-02-21 20:43:00.000000 recursive_size-1.1/recursive_size.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      197 2021-02-21 20:43:00.000000 recursive_size-1.1/recursive_size.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-21 20:43:00.000000 recursive_size-1.1/recursive_size.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2021-02-21 20:43:00.000000 recursive_size-1.1/recursive_size.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-21 20:43:00.531962 recursive_size-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1337 2021-02-21 20:42:50.000000 recursive_size-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:52:41.742820 recursive_size-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-13 11:52:27.000000 recursive_size-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-13 11:52:41.742820 recursive_size-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 11:52:27.000000 recursive_size-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:52:41.742820 recursive_size-1.2/recursive_size/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-13 11:52:27.000000 recursive_size-1.2/recursive_size/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:52:41.742820 recursive_size-1.2/recursive_size.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-13 11:52:41.000000 recursive_size-1.2/recursive_size.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 11:52:41.000000 recursive_size-1.2/recursive_size.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:52:41.000000 recursive_size-1.2/recursive_size.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 11:52:41.000000 recursive_size-1.2/recursive_size.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:52:41.742820 recursive_size-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-13 11:52:27.000000 recursive_size-1.2/setup.py
```

### Comparing `recursive_size-1.1/PKG-INFO` & `recursive_size-1.2/recursive_size.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
-Name: recursive_size
-Version: 1.1
+Name: recursive-size
+Version: 1.2
 Summary: Recursively get the size of folder
 Home-page: https://github.com/deuteronomy-works/recursive_size
 Author: Deuteronomy Works
 Author-email: deutworks@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/deuteronomy-works/recursive_size/issues
 Project-URL: Documentation, https://github.com/deuteronomy-works/recursive_size/wiki
 Project-URL: Source Code, https://github.com/deuteronomy-works/recursive_size
-Description: # recursive_size
-         Recursively calculate the size of a folder or file
-        
-        
-        ## Install
-        ```pip install recursive-size```
-        
-        ## Usage
-        ```python
-        from recursive_size import get_size
-        size = get_size('path/to/folder')
-        print(size)
-        ```
-        
 Keywords: size,get_size,get size,recursive size,recursive_size
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# recursive_size
+ Recursively calculate the size of a folder or file. Works with docker directories.
+
+
+## Install
+```pip install recursive-size```
+
+## Usage
+```python
+from recursive_size import get_size
+size = get_size('path/to/folder')
+print(size)
+```
```

### Comparing `recursive_size-1.1/recursive_size/__init__.py` & `recursive_size-1.2/recursive_size/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 
 
 def handle_single_or_except(path_name, except_value):
 
     except_type = sys.exc_info()[0]
 
     if except_type == NotADirectoryError:
+
         try:
             return os.stat(path_name).st_size
 
         except Exception as exc:
             # Still couldn't read, still send error to user
             raise RuntimeError(f'Unable to read {path_name}') from exc
 
     elif except_type == FileNotFoundError:
         if len(path_name) > MAXIMUM_FILE_PATH_LENGTH:
             # won't be able to read
             print(f'ERROR - FILE NAME TOO LONG: {path_name}')
             return 0
 
         else:
+
             try:
                 with open(path_name, 'rb') as long_file:
                     # successful read
                     return len(long_file.read())
 
             except FileNotFoundError:
                 # Fix this Errno 2
@@ -42,21 +44,29 @@
 
     else:
         # Send early error back to user
         raise RuntimeError(f'Unable to read {path_name}') from except_value
 
 
 def looper(path_name):
-    try:
-        _ = os.listdir(path_name)
 
-    except Exception as exc:
-        handle_single_or_except(path_name, exc)
+    if os.path.islink(path_name):
+        # this is a symbolic link, we should not traverse these due 
+        # to loop risks and ultimately a failure
+        return 0
+
+    else:
+
+        try:
+            _ = os.listdir(path_name)
+
+        except Exception as exc:
+            handle_single_or_except(path_name, exc)
 
-    return get_size(path_name)
+        return get_size(path_name)
 
 
 def get_size(folder_name):
     total = 0
 
     try:
         conts = os.listdir(folder_name)
```

### Comparing `recursive_size-1.1/recursive_size.egg-info/PKG-INFO` & `recursive_size-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
-Name: recursive-size
-Version: 1.1
+Name: recursive_size
+Version: 1.2
 Summary: Recursively get the size of folder
 Home-page: https://github.com/deuteronomy-works/recursive_size
 Author: Deuteronomy Works
 Author-email: deutworks@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/deuteronomy-works/recursive_size/issues
 Project-URL: Documentation, https://github.com/deuteronomy-works/recursive_size/wiki
 Project-URL: Source Code, https://github.com/deuteronomy-works/recursive_size
-Description: # recursive_size
-         Recursively calculate the size of a folder or file
-        
-        
-        ## Install
-        ```pip install recursive-size```
-        
-        ## Usage
-        ```python
-        from recursive_size import get_size
-        size = get_size('path/to/folder')
-        print(size)
-        ```
-        
 Keywords: size,get_size,get size,recursive size,recursive_size
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# recursive_size
+ Recursively calculate the size of a folder or file. Works with docker directories.
+
+
+## Install
+```pip install recursive-size```
+
+## Usage
+```python
+from recursive_size import get_size
+size = get_size('path/to/folder')
+print(size)
+```
```

### Comparing `recursive_size-1.1/setup.py` & `recursive_size-1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     desc = r_file.read()
 
 LICENSE_TEXT = "License :: OSI Approved :: "
 LICENSE_TEXT += "GNU Library or Lesser General Public License (LGPL)"
 
 setup(
     name="recursive_size",
-    version="1.1",
+    version="1.2",
     packages=find_packages(),
 
     author="Deuteronomy Works",
     author_email="deutworks@gmail.com",
     description="Recursively get the size of folder",
     long_description=desc,
     long_description_content_type="text/markdown",
```

