# Comparing `tmp/starkcore-0.0.9.tar.gz` & `tmp/starkcore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkcore-0.0.9.tar", last modified: Fri Oct  7 20:04:27 2022, max compression
+gzip compressed data, was "starkcore-0.1.0.tar", last modified: Thu Apr 13 17:31:34 2023, max compression
```

## Comparing `starkcore-0.0.9.tar` & `starkcore-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-10-07 20:04:27.172243 starkcore-0.0.9/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.0.9/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.0.9/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)      885 2022-10-07 20:04:27.172041 starkcore-0.0.9/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.0.9/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-10-07 20:04:27.172311 starkcore-0.0.9/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.0.9/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-10-07 20:04:27.078105 starkcore-0.0.9/starkcore/
--rw-r--r--   0 caiodottori   (501) staff       (20)      198 2022-10-07 20:02:47.000000 starkcore-0.0.9/starkcore/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.0.9/starkcore/environment.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/error.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/key.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-10-07 20:04:27.100016 starkcore-0.0.9/starkcore/user/
--rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.0.9/starkcore/user/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/user/__organization.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/user/__project.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.0.9/starkcore/user/__publicuser.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/user/__user.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-10-07 20:04:27.171460 starkcore-0.0.9/starkcore/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/api.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/cache.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/case.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.0.9/starkcore/utils/checks.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/compatibility.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/enum.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.0.9/starkcore/utils/host.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.0.9/starkcore/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2780 2022-09-07 13:21:49.000000 starkcore-0.0.9/starkcore/utils/request.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/resource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6803 2022-10-07 20:00:58.000000 starkcore-0.0.9/starkcore/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/subresource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      459 2022-05-11 20:37:59.000000 starkcore-0.0.9/starkcore/utils/url.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2022-10-07 20:04:27.084145 starkcore-0.0.9/starkcore.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)      885 2022-10-07 20:04:26.000000 starkcore-0.0.9/starkcore.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      798 2022-10-07 20:04:27.000000 starkcore-0.0.9/starkcore.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2022-10-07 20:04:26.000000 starkcore-0.0.9/starkcore.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-10-07 20:04:26.000000 starkcore-0.0.9/starkcore.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       16 2022-10-07 20:04:26.000000 starkcore-0.0.9/starkcore.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-13 17:31:34.455075 starkcore-0.1.0/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.1.0/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.1.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2023-04-13 17:31:34.454772 starkcore-0.1.0/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.1.0/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-04-13 17:31:34.455184 starkcore-0.1.0/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.1.0/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-13 17:31:34.341852 starkcore-0.1.0/starkcore/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      198 2023-04-13 17:30:51.000000 starkcore-0.1.0/starkcore/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.1.0/starkcore/environment.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/error.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/key.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-13 17:31:34.357427 starkcore-0.1.0/starkcore/user/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.1.0/starkcore/user/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/user/__organization.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/user/__project.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.1.0/starkcore/user/__publicuser.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/user/__user.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-13 17:31:34.454279 starkcore-0.1.0/starkcore/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/api.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/cache.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/case.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.1.0/starkcore/utils/checks.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/compatibility.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/enum.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.1.0/starkcore/utils/host.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.1.0/starkcore/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2780 2022-09-07 13:21:49.000000 starkcore-0.1.0/starkcore/utils/request.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/resource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7173 2023-04-13 17:28:43.000000 starkcore-0.1.0/starkcore/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/subresource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      459 2022-05-11 20:37:59.000000 starkcore-0.1.0/starkcore/utils/url.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-13 17:31:34.345185 starkcore-0.1.0/starkcore.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2023-04-13 17:31:34.000000 starkcore-0.1.0/starkcore.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      798 2023-04-13 17:31:34.000000 starkcore-0.1.0/starkcore.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-04-13 17:31:34.000000 starkcore-0.1.0/starkcore.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2023-04-13 17:31:34.000000 starkcore-0.1.0/starkcore.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       16 2023-04-13 17:31:34.000000 starkcore-0.1.0/starkcore.egg-info/top_level.txt
```

### Comparing `starkcore-0.0.9/LICENSE.txt` & `starkcore-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/PKG-INFO` & `starkcore-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.0.9
+Version: 0.1.0
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
-Description: # Stark Core Python SDK
-        
-        Welcome to the Stark Core Python SDK!
-        This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
-        
-        # Help and Feedback
-        
-        If you have any questions about our SDK, just send us an email.
-        We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
-        We also love feedback, so don't be shy about sharing your thoughts with us.
-        
-        Email: help@starkbank.com
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Stark Core Python SDK
+
+Welcome to the Stark Core Python SDK!
+This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
+
+# Help and Feedback
+
+If you have any questions about our SDK, just send us an email.
+We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
+We also love feedback, so don't be shy about sharing your thoughts with us.
+
+Email: help@starkbank.com
+
+
```

### Comparing `starkcore-0.0.9/setup.py` & `starkcore-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/error.py` & `starkcore-0.1.0/starkcore/error.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/key.py` & `starkcore-0.1.0/starkcore/key.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/user/__organization.py` & `starkcore-0.1.0/starkcore/user/__organization.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/user/__project.py` & `starkcore-0.1.0/starkcore/user/__project.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/utils/api.py` & `starkcore-0.1.0/starkcore/utils/api.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/utils/checks.py` & `starkcore-0.1.0/starkcore/utils/checks.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/utils/parse.py` & `starkcore-0.1.0/starkcore/utils/parse.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/utils/request.py` & `starkcore-0.1.0/starkcore/utils/request.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore/utils/rest.py` & `starkcore-0.1.0/starkcore/utils/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,7 +216,22 @@
         method=get,
         path=path,
         query=query,
         api_version=api_version,
         language=language,
         timeout=timeout,
     ).json()
+
+
+def post_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+    return fetch(
+        host=host,
+        sdk_version=sdk_version,
+        user=user,
+        method=post,
+        path=path,
+        payload=payload,
+        query=query,
+        api_version=api_version,
+        language=language,
+        timeout=timeout,
+    ).json()
```

### Comparing `starkcore-0.0.9/starkcore/utils/subresource.py` & `starkcore-0.1.0/starkcore/utils/subresource.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.0.9/starkcore.egg-info/PKG-INFO` & `starkcore-0.1.0/starkcore.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.0.9
+Version: 0.1.0
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
-Description: # Stark Core Python SDK
-        
-        Welcome to the Stark Core Python SDK!
-        This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
-        
-        # Help and Feedback
-        
-        If you have any questions about our SDK, just send us an email.
-        We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
-        We also love feedback, so don't be shy about sharing your thoughts with us.
-        
-        Email: help@starkbank.com
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Stark Core Python SDK
+
+Welcome to the Stark Core Python SDK!
+This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
+
+# Help and Feedback
+
+If you have any questions about our SDK, just send us an email.
+We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
+We also love feedback, so don't be shy about sharing your thoughts with us.
+
+Email: help@starkbank.com
+
+
```

### Comparing `starkcore-0.0.9/starkcore.egg-info/SOURCES.txt` & `starkcore-0.1.0/starkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

