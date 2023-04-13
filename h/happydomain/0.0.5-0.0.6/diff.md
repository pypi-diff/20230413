# Comparing `tmp/happydomain-0.0.5.tar.gz` & `tmp/happydomain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.5.tar", last modified: Thu Apr 13 04:58:27 2023, max compression
+gzip compressed data, was "happydomain-0.0.6.tar", last modified: Thu Apr 13 15:19:58 2023, max compression
```

## Comparing `happydomain-0.0.5.tar` & `happydomain-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.995183 happydomain-0.0.5/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 04:57:37.000000 happydomain-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 04:58:26.991183 happydomain-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 04:57:37.000000 happydomain-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.979184 happydomain-0.0.5/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/admin.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/api.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/authuser.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/domain.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/error.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/provider.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/service.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.991183 happydomain-0.0.5/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 04:57:37.000000 happydomain-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 04:58:26.995183 happydomain-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 04:57:37.000000 happydomain-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.805650 happydomain-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 15:19:50.000000 happydomain-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 15:19:58.805650 happydomain-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 15:19:50.000000 happydomain-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.793651 happydomain-0.0.6/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.801650 happydomain-0.0.6/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 15:19:50.000000 happydomain-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 15:19:58.805650 happydomain-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 15:19:50.000000 happydomain-0.0.6/setup.py
```

### Comparing `happydomain-0.0.5/LICENSE` & `happydomain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/PKG-INFO` & `happydomain-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.5
+Version: 0.0.6
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.5/happydomain/__init__.py` & `happydomain-0.0.6/happydomain/__init__.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/happydomain/admin.py` & `happydomain-0.0.6/happydomain/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if r.status_code != 200:
             raise HappyError(r.status_code, **r.json())
 
         from .authuser import AuthUser
         u = AuthUser(self, **r.json())
 
         u.Password = u.ResetPassword(password)
-        return
+        return u
 
     def authuser_delete(self, Id):
         r = self.session.delete("http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id))
 
         if r.status_code != 200:
             raise HappyError(r.status_code, **r.json())
```

### Comparing `happydomain-0.0.5/happydomain/api.py` & `happydomain-0.0.6/happydomain/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,60 @@
-"""Handle administration tasks through happyDomain's admin API"""
-
-from datetime import datetime
 import json
-import os
-from urllib.parse import quote_plus
-
-import requests
+from urllib.parse import quote
 
 from .error import HappyError
 from .domain import Domain
-from .provider import Provider
-
-COOKIE_NAME = "happydomain_session"
 
-class HappyDomain:
+class Provider:
 
-    def __init__(self, scheme="http", host="127.0.0.1", port=8081, baseurl="", token=None):
-        self.session = requests.Session()
-        self.baseurl = scheme + "://" + host + ":" + str(port) + baseurl
-        self.token = token
+    def __init__(self, _session, _srctype, _id, _ownerid, _comment, Provider={}):
+        self._session = _session
 
-    def login(self, username, password):
-        r = self.session.post(
-            self.baseurl + "/api/auth",
+        self._srctype = _srctype
+        self._id = _id
+        self._ownerid = _ownerid
+        self._comment = _comment
+        self.args = Provider
+
+    def _dumps(self):
+        return json.dumps({
+            "_srctype": self._srctype,
+            "_id": self._id,
+            "_ownerid": self._ownerid,
+            "_comment": self._comment,
+            "Provider": self.args,
+        })
+
+    def domain_add(self, dn):
+        r = self._session.session.post(
+            self._session.baseurl + "/api/domains",
             data=json.dumps({
-                "email": username,
-                "password": password,
+                "domain": dn,
+                "id_provider": self._id,
             })
         )
 
         if r.status_code != 200:
-            raise HappyError(r.status_code, **json.loads(r.text))
-
-        self.token = r.cookies[COOKIE_NAME]
-
-        return json.loads(r.text)
+            raise HappyError(r.status_code, **r.json())
 
-    # Domains
+        return Domain(self._session, **r.json())
 
-    def domain_list(self):
-        r = self.session.get(
-            self.baseurl + "/api/domains",
+    def delete(self):
+        r = self._session.session.delete(
+            self._session.baseurl + "/api/providers/" + quote(self._id),
         )
 
-        if r.status_code != 200:
-            raise HappyError(r.status_code, **json.loads(r.text))
-
-        ret = []
-        val = json.loads(r.text)
-
-        if val is not None:
-            for au in val:
-                ret.append(Domain(self, **au))
+        if r.status_code > 300:
+            raise HappyError(r.status_code, **r.json())
 
-        return ret
+        return r.json()
 
-    # Providers
-
-    def provider_list(self):
-        r = self.session.get(
-            self.baseurl + "/api/providers",
+    def update(self):
+        r = self._session.session.put(
+            self._session.baseurl + "/api/providers/" + quote(self._id),
+            data=self._dumps(),
         )
 
-        if r.status_code != 200:
-            raise HappyError(r.status_code, **json.loads(r.text))
-
-        ret = []
-        val = json.loads(r.text)
-
-        if val is not None:
-            for au in val:
-                ret.append(Provider(self, **au))
-
-        return ret
-
-    def provider_add(self, type, name, data):
-        r = self.session.post(
-            self.baseurl + "/api/providers",
-            data=json.dumps({
-                "Provider": data,
-                "_comment": name,
-                "_srctype": type,
-            })
-        )
-
-        if r.status_code != 200:
-            raise HappyError(r.status_code, **json.loads(r.text))
+        if r.status_code > 300:
+            raise HappyError(r.status_code, **r.json())
 
-        return Provider(self, **json.loads(r.text))
+        return r.json()
```

### Comparing `happydomain-0.0.5/happydomain/authuser.py` & `happydomain-0.0.6/happydomain/authuser.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/happydomain/domain.py` & `happydomain-0.0.6/happydomain/domain.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/happydomain/service.py` & `happydomain-0.0.6/happydomain/service.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/happydomain/zone.py` & `happydomain-0.0.6/happydomain/zone.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.5/happydomain.egg-info/PKG-INFO` & `happydomain-0.0.6/happydomain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.5
+Version: 0.0.6
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.5/pyproject.toml` & `happydomain-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.5/setup.py` & `happydomain-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.0.5"
+version = "0.0.6"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

