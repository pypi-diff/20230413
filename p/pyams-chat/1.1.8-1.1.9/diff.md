# Comparing `tmp/pyams_chat-1.1.8.tar.gz` & `tmp/pyams_chat-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_chat-1.1.8.tar", last modified: Tue May 17 08:44:20 2022, max compression
+gzip compressed data, was "dist/pyams_chat-1.1.9.tar", last modified: Thu Apr 13 13:01:01 2023, max compression
```

## Comparing `pyams_chat-1.1.8.tar` & `pyams_chat-1.1.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3373 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/docs/
--rwxrwxrwx   0 root         (0) root         (0)      953 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1126 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2647 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/
--rw-rw-rw-   0 root         (0) root         (0)      871 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/api/
--rw-rw-rw-   0 root         (0) root         (0)     5517 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10751 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/handler/
--rw-rw-rw-   0 root         (0) root         (0)      550 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/handler/login.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/include.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2319 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.mo
--rw-rw-rw-   0 root         (0) root         (0)     3595 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.po
--rw-rw-rw-   0 root         (0) root         (0)     2969 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/locales/pyams_chat.pot
--rw-rw-rw-   0 root         (0) root         (0)     6213 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      796 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    15040 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/chat-sw.js
--rw-rw-rw-   0 root         (0) root         (0)     3444 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/pyams_chat.js
--rw-rw-rw-   0 root         (0) root         (0)     1466 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/pyams_chat.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2291 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/templates/notifications.pt
--rw-rw-rw-   0 root         (0) root         (0)     1224 2022-05-17 08:44:05.000000 pyams_chat-1.1.8/src/pyams_chat/zmi/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3373 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1269 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      242 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-05-17 08:44:20.000000 pyams_chat-1.1.8/src/pyams_chat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2647 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/api/
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10786 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/handler/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/handler/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.po
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/locales/pyams_chat.pot
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    15040 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/chat-sw.js
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/pyams_chat.js
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/pyams_chat.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/templates/notifications.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-04-13 13:00:39.000000 pyams_chat-1.1.9/src/pyams_chat/zmi/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-13 13:01:01.000000 pyams_chat-1.1.9/src/pyams_chat.egg-info/top_level.txt
```

### Comparing `pyams_chat-1.1.8/docs/HISTORY.txt` & `pyams_chat-1.1.9/docs/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+1.1.9
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+ - added support for Python 3.11
+
 1.1.8
 -----
  - added CORS validators and OPTIONS handler to REST services
 
 1.1.7
 -----
  - PyAMS_security interfaces refactoring
```

### Comparing `pyams_chat-1.1.8/docs/README.txt` & `pyams_chat-1.1.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/setup.py` & `pyams_chat-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 from setuptools import setup, find_packages
 
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
-README = os.path.join(DOCS, 'README.txt')
-HISTORY = os.path.join(DOCS, 'HISTORY.txt')
+README = os.path.join(DOCS, 'README.rst')
+HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.1.8'
+version = '1.1.9'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'fakeredis',
     'pyams_auth_http',
     'pyams_zmi',
     'pyramid_zcml',
```

### Comparing `pyams_chat-1.1.8/src/pyams_chat/__init__.py` & `pyams_chat-1.1.9/src/pyams_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/client.py` & `pyams_chat-1.1.9/src/pyams_chat/client.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/doctests/README.rst` & `pyams_chat-1.1.9/src/pyams_chat/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     >>> cache_regions.update({'short': {'type': 'memory', 'expire': 0}})
     >>> cache_regions.update({'long': {'type': 'memory', 'expire': 0}})
 
     >>> from pyramid_zodbconn import includeme as include_zodbconn
     >>> include_zodbconn(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
+    >>> from cornice_swagger import includeme as include_swagger
+    >>> include_swagger(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_security import includeme as include_security
     >>> include_security(config)
     >>> from pyams_auth_http import includeme as include_auth_http
     >>> include_auth_http(config)
     >>> from pyams_chat import includeme as include_chat
@@ -92,23 +94,23 @@
 
 A REST API is available to get chat context; this context is used to filter chat messages:
 
     >>> from pyams_chat.api import get_chat_context
     >>> pprint.pprint(get_chat_context(request))
     {'context': {'*': ['user.login']},
      'principal': {'id': 'system:admin',
-                   'principals': (...'system:admin'...),
+                   'principals': [...'system:admin'...],
                    'title': '__unknown__'},
      'status': 'success'}
 
 We can also get chat messages:
 
     >>> from pyams_chat.api import get_notifications
     >>> pprint.pprint(get_notifications(request))
-    {'notifications': [], 'timestamp': ...}
+    {'notifications': [], 'timestamp': '...T...'}
 
 The notifications list is actually empty because the Redis list is filled by the websocket
 server only when notifications are actually dispatched.
 
     >>> with request.redis_client as redis:
     ...     redis.lrange(f'chat:notifications::{request.host_url}', 0, -1)
     []
@@ -187,15 +189,14 @@
                         'channel': 'chat:main',
                         'host': 'http://example.com',
                         'image': None,
                         'message': '__unknown__ logged in...',
                         'source': {'id': 'test:user',
                                    'title': 'MissingPrincipal: test:user'},
                         'status': 'info',
-                        'target': {'principals': ['system:admin']},
                         'timestamp': '...T...',
                         'title': 'User login',
                         'url': None}],
      'timestamp': ...}
 
 
 Chat notifications viewlet
```

### Comparing `pyams_chat-1.1.8/src/pyams_chat/handler/__init__.py` & `pyams_chat-1.1.9/src/pyams_chat/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/handler/login.py` & `pyams_chat-1.1.9/src/pyams_chat/handler/login.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/include.py` & `pyams_chat-1.1.9/src/pyams_chat/include.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/interfaces.py` & `pyams_chat-1.1.9/src/pyams_chat/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.mo` & `pyams_chat-1.1.9/src/pyams_chat/locales/fr/LC_MESSAGES/pyams_chat.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,20 +9,14 @@
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.14\n"
 
 msgid "Attributes of the principal which emitted the notification"
 msgstr "Attributs tu mandataire ayant envoyé le message"
 
-msgid "Error message"
-msgstr "Message d'erreur"
-
-msgid "Forbidden access"
-msgstr "Accès interdit"
-
 msgid "Internal user data"
 msgstr "Données utilisateur spécifiques"
 
 msgid "Message action"
 msgstr "Action"
 
 msgid "Message category"
@@ -33,16 +27,19 @@
 
 msgid "Message content"
 msgstr "Contenu"
 
 msgid "Message host name"
 msgstr "Nom d'hôte"
 
+msgid "Message image URL"
+msgstr "URL de l'image associée au message"
+
 msgid "Message source"
-msgstr "Source"
+msgstr "Source du message"
 
 msgid "Message status"
 msgstr "Statut"
 
 msgid "Message target"
 msgstr "Cible"
 
@@ -51,47 +48,23 @@
 
 msgid "Message timestamp in ISO-8601 format"
 msgstr "Horodatage du message au format ISO 8601"
 
 msgid "Message title"
 msgstr "Titre"
 
-msgid "Missing arguments"
-msgstr "Arguments incorrects"
-
 msgid "Notification URL"
 msgstr "URL de notification"
 
 msgid "Notifications"
 msgstr "Notifications"
 
-msgid "Page not found"
-msgstr "Page non trouvée"
-
-msgid "Principal ID"
-msgstr "ID du mandataire"
-
-msgid "Response status"
-msgstr "Statut de la réponse"
-
-msgid "Service unavailable"
-msgstr "Service indisponible"
-
-msgid "Token accepted"
-msgstr "Jeton accepté"
-
 msgid "URL target of this message notification"
 msgstr "Cible du message de notification"
 
-msgid "Unauthorized"
-msgstr "Accès non autorisé"
-
-msgid "User context properties"
-msgstr "Propriétés du contexte de l'utilisateur"
-
 msgid ""
 "User data used for internal usage; these data are not sent in notifications "
 "contents"
 msgstr ""
 "Ces données internes peuvent être utilisées pour le traitement du message ; "
 "elles ne fon pas partie des données envoyées dans les notifications"
```

### Comparing `pyams_chat-1.1.8/src/pyams_chat/locales/pyams_chat.pot` & `pyams_chat-1.1.9/src/pyams_chat/locales/pyams_chat.pot`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,101 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2021-10-16 12:29+0200\n"
+"POT-Creation-Date: 2023-04-12 15:58+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Lingua 4.14\n"
+"Generated-By: Lingua 4.15.0\n"
 
-#: ./src/pyams_chat/interfaces.py:31
+#: ./src/pyams_chat/interfaces.py:34
 msgid "Message host name"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:33
+#: ./src/pyams_chat/interfaces.py:36
 msgid "Message channel"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:35
+#: ./src/pyams_chat/interfaces.py:38
 msgid "Message action"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:37
+#: ./src/pyams_chat/interfaces.py:40
 msgid "Message category"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:39
+#: ./src/pyams_chat/interfaces.py:42
 msgid "Message status"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:41
+#: ./src/pyams_chat/interfaces.py:44
 msgid "Message title"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:43
+#: ./src/pyams_chat/interfaces.py:46
 msgid "Message content"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:45
+#: ./src/pyams_chat/interfaces.py:48
+msgid "Message image URL"
+msgstr ""
+
+#: ./src/pyams_chat/interfaces.py:51
 msgid "Message source"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:46
+#: ./src/pyams_chat/interfaces.py:52
 msgid "Attributes of the principal which emitted the notification"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:50
+#: ./src/pyams_chat/interfaces.py:56
 msgid "Message target"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:51
+#: ./src/pyams_chat/interfaces.py:57
 msgid "Message targets can be principals, roles..."
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:54
+#: ./src/pyams_chat/interfaces.py:60
 msgid "Notification URL"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:55
+#: ./src/pyams_chat/interfaces.py:61
 msgid "URL target of this message notification"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:58
+#: ./src/pyams_chat/interfaces.py:64
 msgid "Message timestamp in ISO-8601 format"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:60
+#: ./src/pyams_chat/interfaces.py:66
 msgid "Internal user data"
 msgstr ""
 
-#: ./src/pyams_chat/interfaces.py:61
+#: ./src/pyams_chat/interfaces.py:67
 msgid ""
 "User data used for internal usage; these data are not sent in notifications "
 "contents"
 msgstr ""
 
-#: ./src/pyams_chat/api/__init__.py:43 ./src/pyams_chat/api/__init__.py:56
-msgid "Response status"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:50
-msgid "Principal ID"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:58
-msgid "Error message"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:63
-msgid "User context properties"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:64
-msgid "Token accepted"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:65
-msgid "Page not found"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:66
-msgid "Unauthorized"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:67
-msgid "Forbidden access"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:68
-msgid "Missing arguments"
-msgstr ""
-
-#: ./src/pyams_chat/api/__init__.py:69
-msgid "Service unavailable"
-msgstr ""
-
-#: ./src/pyams_chat/zmi/viewlet/templates/notifications.pt:19
-#: ./src/pyams_chat/zmi/viewlet/templates/notifications.pt:33
+#: ./src/pyams_chat/zmi/viewlet/templates/notifications.pt:23
+#: ./src/pyams_chat/zmi/viewlet/templates/notifications.pt:37
 msgid "Notifications"
 msgstr ""
 
-#: ./src/pyams_chat/handler/login.py:47
+#: ./src/pyams_chat/handler/login.py:48
 msgid "User login"
 msgstr ""
 
-#: ./src/pyams_chat/handler/login.py:48
+#: ./src/pyams_chat/handler/login.py:49
 #, python-format
 msgid "{} logged in..."
 msgstr ""
```

### Comparing `pyams_chat-1.1.8/src/pyams_chat/message.py` & `pyams_chat-1.1.9/src/pyams_chat/message.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/tests/__init__.py` & `pyams_chat-1.1.9/src/pyams_chat/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/tests/test_utilsdocs.py` & `pyams_chat-1.1.9/src/pyams_chat/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/tests/test_utilsdocstrings.py` & `pyams_chat-1.1.9/src/pyams_chat/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/__init__.py` & `pyams_chat-1.1.9/src/pyams_chat/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/chat-sw.js` & `pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/chat-sw.js`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/pyams_chat.js` & `pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/pyams_chat.js`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/resources/js/pyams_chat.min.js` & `pyams_chat-1.1.9/src/pyams_chat/zmi/resources/js/pyams_chat.min.js`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/__init__.py` & `pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/interfaces.py` & `pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/notifications.py` & `pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/notifications.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/viewlet/templates/notifications.pt` & `pyams_chat-1.1.9/src/pyams_chat/zmi/viewlet/templates/notifications.pt`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat/zmi/worker.py` & `pyams_chat-1.1.9/src/pyams_chat/zmi/worker.py`

 * *Files identical despite different names*

### Comparing `pyams_chat-1.1.8/src/pyams_chat.egg-info/SOURCES.txt` & `pyams_chat-1.1.9/src/pyams_chat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 src/pyams_chat/__init__.py
 src/pyams_chat/client.py
 src/pyams_chat/include.py
 src/pyams_chat/interfaces.py
 src/pyams_chat/message.py
 src/pyams_chat.egg-info/PKG-INFO
 src/pyams_chat.egg-info/SOURCES.txt
```

