# Comparing `tmp/happydomain-0.0.2.tar.gz` & `tmp/happydomain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.2.tar", last modified: Thu Apr 13 01:11:47 2023, max compression
+gzip compressed data, was "happydomain-0.0.3.tar", last modified: Thu Apr 13 02:08:11 2023, max compression
```

## Comparing `happydomain-0.0.2.tar` & `happydomain-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.806336 happydomain-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 01:11:39.000000 happydomain-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 01:11:47.802337 happydomain-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 01:11:39.000000 happydomain-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.790337 happydomain-0.0.2/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/admin.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/api.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/authuser.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/domain.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/error.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/provider.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/service.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-04-13 01:11:39.000000 happydomain-0.0.2/happydomain/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:11:47.802337 happydomain-0.0.2/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 01:11:47.000000 happydomain-0.0.2/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 01:11:39.000000 happydomain-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 01:11:47.806336 happydomain-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 01:11:39.000000 happydomain-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:08:11.089755 happydomain-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 02:08:00.000000 happydomain-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 02:08:11.089755 happydomain-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 02:08:00.000000 happydomain-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:08:11.073755 happydomain-0.0.3/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-04-13 02:08:00.000000 happydomain-0.0.3/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:08:11.085755 happydomain-0.0.3/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 02:08:10.000000 happydomain-0.0.3/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 02:08:10.000000 happydomain-0.0.3/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 02:08:10.000000 happydomain-0.0.3/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 02:08:10.000000 happydomain-0.0.3/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 02:08:10.000000 happydomain-0.0.3/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 02:08:00.000000 happydomain-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 02:08:11.093755 happydomain-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 02:08:00.000000 happydomain-0.0.3/setup.py
```

### Comparing `happydomain-0.0.2/LICENSE` & `happydomain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/PKG-INFO` & `happydomain-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.2/happydomain/__init__.py` & `happydomain-0.0.3/happydomain/__init__.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain/admin.py` & `happydomain-0.0.3/happydomain/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,28 +61,14 @@
         if val is not None:
             from .authuser import AuthUser
             for au in val:
                 ret.append(AuthUser(self, **au))
 
         return ret
 
-    def authuser_reset_password(self, Id, NewPassword):
-        r = self.session.post(
-            "http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id) + "/reset_password",
-            data=json.dumps({
-                "password": NewPassword,
-            })
-        )
-
-        if r.status_code != 200:
-            raise HappyError(r.status_code, **r.json())
-
-        from .authuser import AuthUser
-        return r.json()
-
     def authuser_udpate(self, Id, au):
         r = self.session.put(
             "http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id),
             data=json.dumps({
                 "Id": au.Id,
                 "Email": au.Email,
                 "EmailVerification": au.EmailVerification,
```

### Comparing `happydomain-0.0.2/happydomain/api.py` & `happydomain-0.0.3/happydomain/api.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain/authuser.py` & `happydomain-0.0.3/happydomain/authuser.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,11 +11,21 @@
         self.LastLoggedIn = LastLoggedIn
         self.AllowCommercials = AllowCommercials
 
     def Delete(self):
         self._session.authuser_delete(self.Id)
 
     def ResetPassword(self, *args, **kwargs):
-        self._session.authuser_reset_password(self.Id, *args, **kwargs)
+        r = self.session.post(
+            "http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id) + "/reset_password",
+            data=json.dumps({
+                "password": NewPassword,
+            })
+        )
+
+        if r.status_code != 200 and r.status_code != 406:
+            raise HappyError(r.status_code, **r.json())
+
+        return r.status_code == 200
 
     def Update(self):
         self._session.authuser_update(self.Id, self)
```

### Comparing `happydomain-0.0.2/happydomain/domain.py` & `happydomain-0.0.3/happydomain/domain.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain/provider.py` & `happydomain-0.0.3/happydomain/provider.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain/service.py` & `happydomain-0.0.3/happydomain/service.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain/zone.py` & `happydomain-0.0.3/happydomain/zone.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.2/happydomain.egg-info/PKG-INFO` & `happydomain-0.0.3/happydomain.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.2/pyproject.toml` & `happydomain-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.2/setup.py` & `happydomain-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.0.2"
+version = "0.0.3"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

