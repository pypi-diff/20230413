# Comparing `tmp/pyams_chat_ws-1.1.5.tar.gz` & `tmp/pyams_chat_ws-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_chat_ws-1.1.5.tar", last modified: Wed Oct 27 20:54:35 2021, max compression
+gzip compressed data, was "dist/pyams_chat_ws-1.1.7.tar", last modified: Thu Apr 13 13:22:06 2023, max compression
```

## Comparing `pyams_chat_ws-1.1.5.tar` & `pyams_chat_ws-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/
--rw-rw-rw-   0 root         (0) root         (0)      104 2021-10-02 13:35:41.000000 pyams_chat_ws-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2707 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/PKG-INFO
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/docs/
--rwxrwxrwx   0 root         (0) root         (0)      443 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1191 2021-10-02 13:35:41.000000 pyams_chat_ws-1.1.5/docs/README.txt
--rw-rw-rw-   0 root         (0) root         (0)    59032 2021-10-02 13:35:41.000000 pyams_chat_ws-1.1.5/docs/chat.png
--rw-rw-rw-   0 root         (0) root         (0)     1245 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/docs/chat.puml
--rw-rw-rw-   0 root         (0) root         (0)      554 2021-10-20 07:29:16.000000 pyams_chat_ws-1.1.5/docs/config.json
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2213 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/setup.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/
--rw-rw-rw-   0 root         (0) root         (0)      741 2021-10-02 13:35:41.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6299 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/app.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2021-10-27 20:53:18.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2021-10-17 17:26:03.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws/webapp.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2707 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      557 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       69 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-10-27 20:54:35.000000 pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    59032 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/docs/chat.png
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/docs/chat.puml
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/docs/config.json
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2213 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6321 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2023-04-13 13:21:50.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws/webapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      565 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 13:22:06.000000 pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/top_level.txt
```

### Comparing `pyams_chat_ws-1.1.5/docs/README.txt` & `pyams_chat_ws-1.1.7/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/docs/chat.png` & `pyams_chat_ws-1.1.7/docs/chat.png`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/docs/chat.puml` & `pyams_chat_ws-1.1.7/docs/chat.puml`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/docs/config.json` & `pyams_chat_ws-1.1.7/docs/config.json`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/setup.py` & `pyams_chat_ws-1.1.7/setup.py`

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
 
-version = '1.1.5'
+version = '1.1.7'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
 ]
 
 setup(name='pyams_chat_ws',
       version=version,
```

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/__init__.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/app.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,26 +124,26 @@
         if isinstance(message, (str, bytes)):
             try:
                 message = json.loads(message)
             except ValueError:
                 return
         if message:
             async with self.sessions_lock:
+                principals = set(message.pop('target', {}).get('principals', []))
                 for session in self.sessions.values():
                     LOGGER.debug(f"  > checking session: {session}")
                     # don't send messages to other hosts
                     if session['host'] != message.get('host'):
                         continue
                     # don't send messages to message emitter
                     if session['principal_id'] == message.get('source', {}).get('id'):
                         continue
                     # filter message targets
                     try:
-                        if (set(session['context']['principal']['principals']) &
-                                set(message['target']['principals'])):
+                        if set(session['context']['principal']['principals']) & principals:
                             LOGGER.debug(f"  > sending message: {message}")
                             await session['ws'].send_json(message)
                     except KeyError:
                         continue
             # update Redis notifications queue
             cache_key = self.config.get('notifications_key')
             if cache_key:
```

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/auth.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/auth.py`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/chat.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/chat.py`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/monitor.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/monitor.py`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws/webapp.py` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws/webapp.py`

 * *Files identical despite different names*

### Comparing `pyams_chat_ws-1.1.5/src/pyams_chat_ws.egg-info/SOURCES.txt` & `pyams_chat_ws-1.1.7/src/pyams_chat_ws.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 docs/chat.png
 docs/chat.puml
 docs/config.json
 src/pyams_chat_ws/__init__.py
 src/pyams_chat_ws/app.py
 src/pyams_chat_ws/auth.py
 src/pyams_chat_ws/chat.py
```

