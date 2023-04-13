# Comparing `tmp/optumi-core-3.15.3.tar.gz` & `tmp/optumi-core-3.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-core-3.15.3.tar", last modified: Sat Mar 18 18:51:05 2023, max compression
+gzip compressed data, was "optumi-core-3.15.4.tar", last modified: Wed Apr 12 20:24:30 2023, max compression
```

## Comparing `optumi-core-3.15.3.tar` & `optumi-core-3.15.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-03-18 18:51:05.949510 optumi-core-3.15.3/
--rw-rw-r--   0 denis     (1001) denis     (1001)      280 2023-02-25 13:43:26.000000 optumi-core-3.15.3/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       16 2023-02-25 13:43:26.000000 optumi-core-3.15.3/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-03-18 18:51:05.949510 optumi-core-3.15.3/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-02-25 13:43:26.000000 optumi-core-3.15.3/README.md
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-03-18 18:51:05.949510 optumi-core-3.15.3/optumi_core/
--rw-rw-r--   0 denis     (1001) denis     (1001)      408 2023-02-25 13:43:26.000000 optumi-core-3.15.3/optumi_core/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-03-17 16:38:04.000000 optumi-core-3.15.3/optumi_core/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    39799 2023-03-14 21:57:23.000000 optumi-core-3.15.3/optumi_core/core.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1520 2023-03-17 16:38:04.000000 optumi-core-3.15.3/optumi_core/exceptions.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1043 2023-03-14 21:57:23.000000 optumi-core-3.15.3/optumi_core/logging.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    13980 2023-03-17 16:38:05.000000 optumi-core-3.15.3/optumi_core/login.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3407 2023-03-17 16:38:05.000000 optumi-core-3.15.3/optumi_core/sessions.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2359 2023-03-14 21:57:23.000000 optumi-core-3.15.3/optumi_core/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-03-18 18:51:05.949510 optumi-core-3.15.3/optumi_core.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      429 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       25 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       12 2023-03-18 18:51:05.000000 optumi-core-3.15.3/optumi_core.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-03-18 18:51:05.949510 optumi-core-3.15.3/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     1932 2023-03-14 21:57:23.000000 optumi-core-3.15.3/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.680214 optumi-core-3.15.4/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      280 2023-04-03 21:07:54.000000 optumi-core-3.15.4/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       34 2023-04-03 21:07:54.000000 optumi-core-3.15.4/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-12 20:24:30.676214 optumi-core-3.15.4/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-03 21:07:54.000000 optumi-core-3.15.4/README.md
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.676214 optumi-core-3.15.4/optumi_core/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      408 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-07 16:00:16.000000 optumi-core-3.15.4/optumi_core/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    39799 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/core.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1520 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/exceptions.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1043 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/logging.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    14139 2023-04-04 21:44:37.000000 optumi-core-3.15.4/optumi_core/login.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3407 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/sessions.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2359 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.676214 optumi-core-3.15.4/optumi_core.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      429 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       25 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       12 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-12 20:24:30.680214 optumi-core-3.15.4/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     1932 2023-04-03 21:07:54.000000 optumi-core-3.15.4/setup.py
```

### Comparing `optumi-core-3.15.3/PKG-INFO` & `optumi-core-3.15.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-core
-Version: 3.15.3
+Version: 3.15.4
 Summary: Optumi core library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-core-3.15.3/optumi_core/core.py` & `optumi-core-3.15.4/optumi_core/core.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.3/optumi_core/exceptions.py` & `optumi-core-3.15.4/optumi_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.3/optumi_core/logging.py` & `optumi-core-3.15.4/optumi_core/logging.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.3/optumi_core/login.py` & `optumi-core-3.15.4/optumi_core/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,21 +184,21 @@
 def login_rest_server(
     login_domain,
     login_port,
     token=None,
     login_type="oauth",
     save_token=False,
 ):
+    session = get_session()
     try:
         if check_login(login_domain, login_port):
             return 1, get_session()._domain_and_port
 
         start_time = None
         last_domain_and_port = None
-        session = get_session()
         while True:
             if start_time == None:
                 start_time = time.time()
             elif time.time() - start_time > 600:  # 10 minute timeout
                 session._domain_and_port = get_portal_domain_and_port()
                 return -1, "Timed out"
             # If we want to move back to using a devserver certificate we need to check for devserver.optumi.com explicitly
@@ -373,10 +373,16 @@
         if remove_token:
             TOKEN_FILE = get_token_file()
             try:
                 os.remove(TOKEN_FILE)
                 print("Removed connection token")
             except OSError:
                 pass
+        # Silently remove cookies
+        COOKIE_FILE = get_cookie_file()
+        try:
+            os.remove(COOKIE_FILE)
+        except OSError:
+            pass
         return get_session().get(URL, timeout=120)
     except HTTPError as e:
         return e
```

### Comparing `optumi-core-3.15.3/optumi_core/sessions.py` & `optumi-core-3.15.4/optumi_core/sessions.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.3/optumi_core/utils.py` & `optumi-core-3.15.4/optumi_core/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.3/optumi_core.egg-info/PKG-INFO` & `optumi-core-3.15.4/optumi_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-core
-Version: 3.15.3
+Version: 3.15.4
 Summary: Optumi core library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-core-3.15.3/setup.py` & `optumi-core-3.15.4/setup.py`

 * *Files identical despite different names*

