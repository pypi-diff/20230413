# Comparing `tmp/deterrersapi-0.1.tar.gz` & `tmp/deterrersapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrersapi-0.1.tar", last modified: Thu Apr 13 19:48:38 2023, max compression
+gzip compressed data, was "deterrersapi-0.2.tar", last modified: Thu Apr 13 19:53:54 2023, max compression
```

## Comparing `deterrersapi-0.1.tar` & `deterrersapi-0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:48:38.068896 deterrersapi-0.1/
--rw-r--r--   0 lars      (1000) lars      (1000)      976 2023-04-13 19:48:38.068896 deterrersapi-0.1/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      707 2023-04-13 19:48:03.000000 deterrersapi-0.1/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:48:38.068896 deterrersapi-0.1/deterrersapi/
--rw-r--r--   0 lars      (1000) lars      (1000)     5271 2023-04-13 16:50:35.000000 deterrersapi-0.1/deterrersapi/__init__.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:48:38.068896 deterrersapi-0.1/deterrersapi.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)      976 2023-04-13 19:48:37.000000 deterrersapi-0.1/deterrersapi.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      222 2023-04-13 19:48:37.000000 deterrersapi-0.1/deterrersapi.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 19:48:37.000000 deterrersapi-0.1/deterrersapi.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:48:37.000000 deterrersapi-0.1/deterrersapi.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 19:48:37.000000 deterrersapi-0.1/deterrersapi.egg-info/top_level.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 19:48:38.068896 deterrersapi-0.1/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      686 2023-04-13 19:37:21.000000 deterrersapi-0.1/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:53:54.283289 deterrersapi-0.2/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrersapi-0.2/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrersapi-0.2/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     1067 2023-04-13 19:53:54.283289 deterrersapi-0.2/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      798 2023-04-13 19:52:22.000000 deterrersapi-0.2/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:53:54.283289 deterrersapi-0.2/deterrersapi/
+-rw-r--r--   0 lars      (1000) lars      (1000)     5271 2023-04-13 16:50:35.000000 deterrersapi-0.2/deterrersapi/__init__.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 19:53:54.283289 deterrersapi-0.2/deterrersapi.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1067 2023-04-13 19:53:54.000000 deterrersapi-0.2/deterrersapi.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      259 2023-04-13 19:53:54.000000 deterrersapi-0.2/deterrersapi.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 19:53:54.000000 deterrersapi-0.2/deterrersapi.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:53:54.000000 deterrersapi-0.2/deterrersapi.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 19:53:54.000000 deterrersapi-0.2/deterrersapi.egg-info/top_level.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrersapi-0.2/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 19:53:54.283289 deterrersapi-0.2/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      686 2023-04-13 19:53:46.000000 deterrersapi-0.2/setup.py
```

### Comparing `deterrersapi-0.1/PKG-INFO` & `deterrersapi-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: deterrersapi
-Version: 0.1
+Version: 0.2
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrersapi
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Python API client for DETERRERS
 
 This library makes it easy to interact with the DETERRERS perimeter firewall
 portal to automate registration, and configuration of IP addresses and firewall
 profiles.
 
+## Installation
+
+Use pip to install the latest version:
+
+```
+pip install deterrersapi
+```
+
 ## Example
 
 ```python
 import deterrersapi
 
 
 deterrers = deterrersapi.Deterrers('https://deterrers.example.com', '<api-token>')
```

### Comparing `deterrersapi-0.1/README.md` & `deterrersapi-0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Python API client for DETERRERS
 
 This library makes it easy to interact with the DETERRERS perimeter firewall
 portal to automate registration, and configuration of IP addresses and firewall
 profiles.
 
+## Installation
+
+Use pip to install the latest version:
+
+```
+pip install deterrersapi
+```
+
 ## Example
 
 ```python
 import deterrersapi
 
 
 deterrers = deterrersapi.Deterrers('https://deterrers.example.com', '<api-token>')
```

### Comparing `deterrersapi-0.1/deterrersapi/__init__.py` & `deterrersapi-0.2/deterrersapi/__init__.py`

 * *Files identical despite different names*

### Comparing `deterrersapi-0.1/deterrersapi.egg-info/PKG-INFO` & `deterrersapi-0.2/deterrersapi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: deterrersapi
-Version: 0.1
+Version: 0.2
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrersapi
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Python API client for DETERRERS
 
 This library makes it easy to interact with the DETERRERS perimeter firewall
 portal to automate registration, and configuration of IP addresses and firewall
 profiles.
 
+## Installation
+
+Use pip to install the latest version:
+
+```
+pip install deterrersapi
+```
+
 ## Example
 
 ```python
 import deterrersapi
 
 
 deterrers = deterrersapi.Deterrers('https://deterrers.example.com', '<api-token>')
```

### Comparing `deterrersapi-0.1/setup.py` & `deterrersapi-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrersapi',
-    version='0.1',
+    version='0.2',
     description='Python API client for DETERRERS',
     url='https://github.com/virtUOS/deterrersapi',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrersapi'],
     license_files=('LICENSE'),
```

