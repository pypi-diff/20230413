# Comparing `tmp/happydomain-0.0.4.tar.gz` & `tmp/happydomain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.4.tar", last modified: Thu Apr 13 02:11:51 2023, max compression
+gzip compressed data, was "happydomain-0.0.5.tar", last modified: Thu Apr 13 04:58:27 2023, max compression
```

## Comparing `happydomain-0.0.4.tar` & `happydomain-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:11:51.625641 happydomain-0.0.4/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 02:11:39.000000 happydomain-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 02:11:51.621641 happydomain-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 02:11:39.000000 happydomain-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:11:51.597642 happydomain-0.0.4/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/admin.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/api.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/authuser.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/domain.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/error.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/provider.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/service.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-04-13 02:11:39.000000 happydomain-0.0.4/happydomain/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:11:51.617642 happydomain-0.0.4/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 02:11:50.000000 happydomain-0.0.4/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 02:11:51.000000 happydomain-0.0.4/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 02:11:50.000000 happydomain-0.0.4/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 02:11:50.000000 happydomain-0.0.4/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 02:11:50.000000 happydomain-0.0.4/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 02:11:39.000000 happydomain-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 02:11:51.625641 happydomain-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 02:11:39.000000 happydomain-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.995183 happydomain-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 04:57:37.000000 happydomain-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 04:58:26.991183 happydomain-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 04:57:37.000000 happydomain-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.979184 happydomain-0.0.5/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-04-13 04:57:37.000000 happydomain-0.0.5/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:58:26.991183 happydomain-0.0.5/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 04:58:26.000000 happydomain-0.0.5/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 04:57:37.000000 happydomain-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 04:58:26.995183 happydomain-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 04:57:37.000000 happydomain-0.0.5/setup.py
```

### Comparing `happydomain-0.0.4/LICENSE` & `happydomain-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.4/PKG-INFO` & `happydomain-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.4/happydomain/__init__.py` & `happydomain-0.0.5/happydomain/__init__.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.4/happydomain/admin.py` & `happydomain-0.0.5/happydomain/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if val is not None:
             from .authuser import AuthUser
             for au in val:
                 ret.append(AuthUser(self, **au))
 
         return ret
 
-    def authuser_udpate(self, Id, au):
+    def authuser_update(self, Id, au):
         r = self.session.put(
             "http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id),
             data=json.dumps({
                 "Id": au.Id,
                 "Email": au.Email,
                 "EmailVerification": au.EmailVerification,
                 "Password": au.Password,
```

### Comparing `happydomain-0.0.4/happydomain/api.py` & `happydomain-0.0.5/happydomain/api.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.4/happydomain/authuser.py` & `happydomain-0.0.5/happydomain/authuser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+from urllib.parse import quote
+
 class AuthUser:
 
     def __init__(self, _session, Id, Email, EmailVerification, Password, CreatedAt, LastLoggedIn, AllowCommercials):
         self._session = _session
 
         self.Id = Id
         self.Email = Email
@@ -10,17 +13,17 @@
         self.CreatedAt = CreatedAt
         self.LastLoggedIn = LastLoggedIn
         self.AllowCommercials = AllowCommercials
 
     def Delete(self):
         self._session.authuser_delete(self.Id)
 
-    def ResetPassword(self, Id, NewPassword):
-        r = self.session.post(
-            "http+unix://" + self.socket_path + "/api/auth/" + quote_plus(Id) + "/reset_password",
+    def ResetPassword(self, NewPassword):
+        r = self._session.session.post(
+            "http+unix://" + self._session.socket_path + "/api/auth/" + quote(self.Id) + "/reset_password",
             data=json.dumps({
                 "password": NewPassword,
             })
         )
 
         if r.status_code != 200 and r.status_code != 406:
             raise HappyError(r.status_code, **r.json())
```

### Comparing `happydomain-0.0.4/happydomain/domain.py` & `happydomain-0.0.5/happydomain/domain.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.4/happydomain/provider.py` & `happydomain-0.0.5/happydomain/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from urllib.parse import quote
 
 from .error import HappyError
 from .domain import Domain
 
 class Provider:
 
     def __init__(self, _session, _srctype, _id, _ownerid, _comment, **kwargs):
@@ -11,50 +12,49 @@
         self._srctype = _srctype
         self._id = _id
         self._ownerid = _ownerid
         self._comment = _comment
         self.args = kwargs
 
     def _dumps(self):
-        d = {
+        return json.dumps({
             "_srctype": self._srctype,
             "_id": self._id,
             "_ownerid": self._ownerid,
             "_comment": self._comment,
-        }
-        d.update(self.kwargs)
-        return json.dumps(d)
+            "Provider": self.args,
+        })
 
     def domain_add(self, dn):
         r = self._session.session.post(
             self._session.baseurl + "/api/domains",
             data=json.dumps({
                 "domain": dn,
                 "id_provider": self._id,
             })
         )
 
         if r.status_code != 200:
             raise HappyError(r.status_code, **r.json())
 
-        return Domain(self, **r.json())
+        return Domain(self._session, **r.json())
 
     def delete(self):
         r = self._session.session.delete(
-            self.baseurl + "/api/providers/" + quote(self._id),
+            self._session.baseurl + "/api/providers/" + quote(self._id),
         )
 
         if r.status_code > 300:
             raise HappyError(r.status_code, **r.json())
 
         return r.json()
 
     def update(self):
         r = self._session.session.put(
-            self.baseurl + "/api/providers/" + quote(self._id),
-            date=self._dumps(),
+            self._session.baseurl + "/api/providers/" + quote(self._id),
+            data=self._dumps(),
         )
 
         if r.status_code > 300:
             raise HappyError(r.status_code, **r.json())
 
         return r.json()
```

### Comparing `happydomain-0.0.4/happydomain/service.py` & `happydomain-0.0.5/happydomain/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from urllib.parse import quote
 
 from .error import HappyError
 
 class ServiceMeta:
 
     def __init__(self, _session, _svctype, _domain, _ttl, _id=None, _ownerid=None, _comment="", _mycomment="", _aliases=[], _tmp_hint_nb=0):
+        self._session = _session
+
         self._svctype = _svctype
         self._domain = _domain
         self._ttl = _ttl
         self._id = _id
         self._ownerid = _ownerid
         self._comment = _comment
         self._mycomment = _mycomment
@@ -38,29 +40,32 @@
         self._zoneid = _zoneid
         self.service = Service
 
     def _dumps(self):
         return json.dumps(self._flat())
 
     def _flat(self):
-        return {
+        d = {
             "_svctype": self._svctype,
             "_domain": self._domain,
             "_ttl": self._ttl,
-            "_id": self._id,
-            "_ownerid": self._ownerid,
             "_comment": self._comment,
             "_mycomment": self._mycomment,
             "_aliases": self._aliases,
             "_tmp_hint_nb": self._tmp_hint_nb,
             "Service": self.service,
         }
+        if self._id is not None:
+            d["_id"] = self._id
+        if self._ownerid is not None:
+            d["_ownerid"] = self._ownerid
+        return d
 
     def delete(self):
         r = self._session.session.delete(
-            self.baseurl + "/api/domains/" + quote(self._domainid) + "/zone/" + quote(self._zoneid) + "/" + quote(self._domain) + "/services/" + quote(self._id),
+            self._session.baseurl + "/api/domains/" + quote(self._domainid) + "/zone/" + quote(self._zoneid) + "/" + quote(self._domain) + "/services/" + quote(self._id),
         )
 
         if r.status_code > 300:
             raise HappyError(r.status_code, **r.json())
 
         return r.json()
```

### Comparing `happydomain-0.0.4/happydomain/zone.py` & `happydomain-0.0.5/happydomain/zone.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,53 +29,53 @@
             "commit_date": self.commit_date,
             "published": self.published,
         })
 
 
 class Zone(ZoneMeta):
 
-    def __init__(self, _session, _domainid, services, **kwargs):
-        super(Zone, self).__init__(_session, **kwargs)
-
+    def __init__(self, _session, _domainid, **kwargs):
         self._domainid = _domainid
-        self._load(services)
 
+        super(Zone, self).__init__(_session, **kwargs)
 
     def _load(self, services, **kwargs):
-        if "id" in kwargs:
-            super(Zone, self).__init__(**kwargs)
+        super(Zone, self)._load(**kwargs)
 
         self.services = {}
         if services is not None:
             for k in services:
                 self.services[k] = []
                 for s in services[k]:
-                    self.services[k].append(HService(_session, self._domainid, self.id, **s))
+                    self.services[k].append(HService(self._session, self._domainid, self.id, **s))
 
     def _svc_dumps(self):
         services = {}
 
         for k in self.services:
             services[k] = []
             for s in self.services[k]:
                 services[k].append(s._flat())
 
         return services
 
     def _dumps(self):
-        return json.dumps({
-            "id": self.id,
-            "id_author": self.id_author,
+        d = json.dumps({
             "default_ttl": self.default_ttl,
             "last_modified": self.last_modified,
             "commit_message": self.commit_message,
             "commit_date": self.commit_date,
             "published": self.published,
             "services": self._svc_dumps(),
         })
+        if self.id is not None:
+            d["id"] = self.id
+        if self.id_author is not None:
+            d["id_author"] = self.id_author
+        return d
 
     def add_zone_service(self, subdomain, svctype, svc):
         r = self._session.session.post(
             self._session.baseurl + "/api/domains/" + quote(self._domainid) + "/zone/" + quote(self.id) + "/" + quote(subdomain) + "/services",
             data=HService(self._session, self._domainid, self.id, Service=svc, _svctype=svctype, _domain=subdomain, _ttl=self.default_ttl)._dumps(),
         )
 
@@ -93,15 +93,23 @@
 
         if r.status_code > 300:
             raise HappyError(r.status_code, **r.json())
 
         return r.json()
 
     def apply_changes(self):
+        rdiff = self._session.session.post(
+            self._session.baseurl + "/api/domains/" + quote(self._domainid) + "/diff_zones/%40/" + quote(self.id),
+        )
+
+        if rdiff.status_code > 300:
+            raise HappyError(rdiff.status_code, **rdiff.json())
+
         r = self._session.session.post(
             self._session.baseurl + "/api/domains/" + quote(self._domainid) + "/zone/" + quote(self.id) + "/apply_changes",
+            data=rdiff.text
         )
 
         if r.status_code > 300:
             raise HappyError(r.status_code, **r.json())
 
-        return r.json()
+        return ZoneMeta(self._session, **r.json())
```

### Comparing `happydomain-0.0.4/happydomain.egg-info/PKG-INFO` & `happydomain-0.0.5/happydomain.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.4/pyproject.toml` & `happydomain-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.4/setup.py` & `happydomain-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.0.4"
+version = "0.0.5"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

