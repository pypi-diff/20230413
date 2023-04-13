# Comparing `tmp/crabpy-0.9.0.tar.gz` & `tmp/crabpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crabpy-0.9.0.tar", last modified: Tue Mar 20 08:55:24 2018, max compression
+gzip compressed data, was "crabpy-1.0.0.tar", last modified: Thu Apr 13 12:57:59 2023, max compression
```

## Comparing `crabpy-0.9.0.tar` & `crabpy-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,31 @@
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     1089 2017-03-24 12:28:28.000000 crabpy-0.9.0/LICENSE
--rw-rw-r--   0 tinne     (1000) tinne     (1000)       76 2017-03-24 12:28:28.000000 crabpy-0.9.0/MANIFEST.in
--rw-rw-r--   0 tinne     (1000) tinne     (1000)      941 2017-03-24 12:28:28.000000 crabpy-0.9.0/README.rst
--rwxr-xr-x   0 tinne     (1000) tinne     (1000)     1402 2018-03-20 08:46:56.000000 crabpy-0.9.0/setup.py
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/
--rw-rw-r--   0 tinne     (1000) tinne     (1000)        1 2017-03-24 14:43:47.000000 crabpy-0.9.0/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 tinne     (1000) tinne     (1000)        1 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     8177 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 tinne     (1000) tinne     (1000)       50 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 tinne     (1000) tinne     (1000)       45 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/requires.txt
--rw-rw-r--   0 tinne     (1000) tinne     (1000)       13 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 tinne     (1000) tinne     (1000)      742 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy.egg-info/SOURCES.txt
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/tests/
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/tests/gateway/
--rw-r--r--   0 tinne     (1000) tinne     (1000)    70481 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/gateway/test_crab.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)    15245 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/gateway/test_capakey.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)      365 2017-03-24 12:28:28.000000 crabpy-0.9.0/tests/gateway/test_exception.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)     5996 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/gateway/test_capakey_cached.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)    24407 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/gateway/test_crab_cached.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)        0 2017-03-24 12:28:28.000000 crabpy-0.9.0/tests/gateway/__init__.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)      577 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/conftest.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)      904 2017-03-24 12:28:28.000000 crabpy-0.9.0/tests/test_wsa.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     1376 2017-03-24 12:28:28.000000 crabpy-0.9.0/tests/test_wsse.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)      741 2018-03-20 08:46:56.000000 crabpy-0.9.0/tests/test_client.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)      542 2017-03-24 12:28:28.000000 crabpy-0.9.0/tests/__init__.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)     8177 2018-03-20 08:55:24.000000 crabpy-0.9.0/PKG-INFO
--rw-r--r--   0 tinne     (1000) tinne     (1000)     5001 2018-03-20 08:46:56.000000 crabpy-0.9.0/CHANGES.rst
--rw-r--r--   0 tinne     (1000) tinne     (1000)       38 2018-03-20 08:55:24.000000 crabpy-0.9.0/setup.cfg
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy/
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     2693 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/wsse.py
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy/gateway/
--rw-r--r--   0 tinne     (1000) tinne     (1000)    27577 2018-03-20 08:46:56.000000 crabpy-0.9.0/crabpy/gateway/capakey.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     1013 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/gateway/exception.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)    87654 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/gateway/crab.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)        0 2017-03-27 09:27:23.000000 crabpy-0.9.0/crabpy/gateway/__init__.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)        0 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/__init__.py
--rw-rw-r--   0 tinne     (1000) tinne     (1000)     1104 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/wsa.py
--rw-r--r--   0 tinne     (1000) tinne     (1000)     1417 2018-03-20 08:46:56.000000 crabpy-0.9.0/crabpy/client.py
-drwxr-xr-x   0 tinne     (1000) tinne     (1000)        0 2018-03-20 08:55:24.000000 crabpy-0.9.0/crabpy/data/
--rw-rw-r--   0 tinne     (1000) tinne     (1000)   181018 2017-03-24 12:28:28.000000 crabpy-0.9.0/crabpy/data/deelgemeenten.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6333 2023-04-13 12:57:29.000000 crabpy-1.0.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.0.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.0.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7984 2023-04-13 12:57:59.740497 crabpy-1.0.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.0.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   118599 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      478 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      753 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    31167 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7984 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      551 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-04-13 12:57:59.740497 crabpy-1.0.0/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-04-13 12:57:29.000000 crabpy-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crabpy-0.9.0/LICENSE` & `crabpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-0.9.0/README.rst` & `crabpy-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-0.9.0/CHANGES.rst` & `crabpy-1.0.0/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,68 @@
+1.0.0 (13-04-2023)
+------------------
+
+- Naar v2 van adressenregister (#185)
+- File wordt niet geclosed (#133)
+- black, flake8, python2 weg en pre-commit (#195)
+- Uitbreidingen aan adressenregister model (#192)
+- pip install van crabpy installeert ook een "tests" met alle data van crabpy (#165)
+
+0.16.1 (29-03-2023)
+-------------------
+
+- Add user agent header to geo.api calls (#190)
+
+0.16.0 (29-03-2023)
+-------------------
+
+- Overschakelen naar nieuwe AGIV services (#183)
+
+0.15.0 (10-12-2021)
+-------------------
+
+- Methode list_straten kan meer data laden (#172)
+
+0.14.0 (18-11-2021)
+-------------------
+
+- Bounding box geeft strings ipv floats (#168)
+
+0.13.0 (14-09-2021)
+-------------------
+
+- Verwijderen python 2 support (#160)
+- Vervangen suds-jurko door suds-py (#160)
+- Upgraden requirements
+
+0.12.1 (28-01-2021)
+-------------------
+
+- Adres toegevoegd aan Perceel (#147)
+
+0.12.0 (24-06-2019)
+-------------------
+
+- Switchen naar v2 van de capakey REST-API (#120)
+- Mocken van calls naar externe url's bij testen (#118)
+- get_perceel_by_coordinates (#121)
+
+0.11.0 (03-01-2019)
+-------------------
+
+- Update deelgemeenten (#110, #116)
+- Fix travis tests (#112)
+- Update dependencies
+
+0.10.0 (17-07-2018)
+-------------------
+
+- Capakey service: change source base map (#95)
+- Capakey service: return full geometry (#96)
+
 0.9.0 (20-03-2018)
 ------------------
 
 - Remove the deprecated CapakeyGateway (#92)
 
 
 0.8.3 (07-12-2017)
```

### Comparing `crabpy-0.9.0/crabpy/wsse.py` & `crabpy-1.0.0/crabpy/wsse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 This module adds a :class:`UsernameDigestToken` for use with SOAP services.
 
 .. versionadded:: 0.2.0
-'''
+"""
 
-from __future__ import unicode_literals
-
-from base64 import b64encode
 
 import hashlib
-
+from base64 import b64encode
 from datetime import datetime
 
-from suds.wsse import UsernameToken, wssens, wsuns
-
 from suds.sax.element import Element
+from suds.wsse import UsernameToken
+from suds.wsse import wssens
+from suds.wsse import wsuns
 
 
 class UsernameDigestToken(UsernameToken):
     """
     Represents a basic WS-Security token with password digest
     """
 
     def __init__(self, username=None, password=None):
-        UsernameToken.__init__(
-            self,
-            username,
-            password
-        )
+        UsernameToken.__init__(self, username, password)
         utc = UsernameToken.utc()
         utc = datetime(
-            utc.year, utc.month, utc.day,
-            utc.hour, utc.minute, utc.second,
-            tzinfo=utc.tzinfo
+            utc.year,
+            utc.month,
+            utc.day,
+            utc.hour,
+            utc.minute,
+            utc.second,
+            tzinfo=utc.tzinfo,
         )
         self.setcreated(utc)
         self.setnonce()
 
     def setnonce(self, text=None):
         if text is None:
             s = []
-            s.append(self.username.encode('utf-8'))
-            s.append(self.password.encode('utf-8'))
-            s.append(str(datetime.utcnow()).encode('utf-8'))
+            s.append(self.username.encode("utf-8"))
+            s.append(self.password.encode("utf-8"))
+            s.append(str(datetime.utcnow()).encode("utf-8"))
             m = hashlib.md5()
-            m.update(':'.encode('utf-8').join(s))
-            self.nonce = m.hexdigest().encode('utf-8')
+            m.update(b":".join(s))
+            self.nonce = m.hexdigest().encode("utf-8")
         else:
             self.nonce = text
 
     @staticmethod
     def _print_datetime(dt):
         return "%.4d-%.2d-%.2dT%.2d:%.2d:%.2dZ" % (
-            dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second
+            dt.year,
+            dt.month,
+            dt.day,
+            dt.hour,
+            dt.minute,
+            dt.second,
         )
 
     def xml(self):
-        usernametoken = Element('UsernameToken', ns=wssens)
+        usernametoken = Element("UsernameToken", ns=wssens)
 
-        username = Element('Username', ns=wssens)
+        username = Element("Username", ns=wssens)
         username.setText(self.username)
         usernametoken.append(username)
 
-        password = Element('Password', ns=wssens)
+        password = Element("Password", ns=wssens)
         s = hashlib.sha1()
         s.update(self.nonce)
-        s.update(self._print_datetime(self.created).encode('utf-8'))
-        s.update(self.password.encode('utf-8'))
-        password.setText(b64encode(s.digest()).decode('utf-8'))
-        password.set('Type', 'http://docs.oasis-open.org/wss/2004/01/'
-                             'oasis-200401-wss-username-token-profile-1.0'
-                             '#PasswordDigest')
+        s.update(self._print_datetime(self.created).encode("utf-8"))
+        s.update(self.password.encode("utf-8"))
+        password.setText(b64encode(s.digest()).decode("utf-8"))
+        password.set(
+            "Type",
+            "http://docs.oasis-open.org/wss/2004/01/"
+            "oasis-200401-wss-username-token-profile-1.0"
+            "#PasswordDigest",
+        )
         usernametoken.append(password)
 
-        nonce = Element('Nonce', ns=wssens)
-        nonce.setText(b64encode(self.nonce).decode('utf-8'))
+        nonce = Element("Nonce", ns=wssens)
+        nonce.setText(b64encode(self.nonce).decode("utf-8"))
         nonce.set(
-            'EncodingType',
-            'http://docs.oasis-open.org/wss/2004'
-            '/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary'
+            "EncodingType",
+            "http://docs.oasis-open.org/wss/2004"
+            "/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary",
         )
         usernametoken.append(nonce)
 
-        created = Element('Created', ns=wsuns)
+        created = Element("Created", ns=wsuns)
         created.setText(self._print_datetime(self.created))
         usernametoken.append(created)
 
         return usernametoken
```

### Comparing `crabpy-0.9.0/crabpy/gateway/capakey.py` & `crabpy-1.0.0/crabpy/gateway/capakey.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,562 +1,586 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 This module contains an opionated gateway for the capakey webservice.
 
 .. versionadded:: 0.2.0
-'''
+"""
 
-from __future__ import unicode_literals
-import six
 import json
-
 import logging
-log = logging.getLogger(__name__)
-
-from crabpy.gateway.exception import (
-    GatewayRuntimeException,
-    GatewayResourceNotFoundException
-)
 
+import requests
 from dogpile.cache import make_region
 
-import requests
+from crabpy.gateway.exception import GatewayResourceNotFoundException
+from crabpy.gateway.exception import GatewayRuntimeException
+
+log = logging.getLogger(__name__)
 
 
 def capakey_rest_gateway_request(url, headers={}, params={}):
-    '''
+    """
     Utility function that helps making requests to the CAPAKEY REST service.
 
     :param string url: URL to request.
     :param dict headers: Headers to send with the URL.
     :param dict params: Parameters to send with the URL.
     :returns: Result of the call.
-    '''
+    """
     try:
+        # calls to geoservices give a 403 if the user-agent is not set
+        headers["user-agent"] = "*"
         res = requests.get(url, headers=headers, params=params)
         res.raise_for_status()
         return res
     except requests.ConnectionError as ce:
         raise GatewayRuntimeException(
-            'Could not execute request due to connection problems:\n%s' % repr(ce),
-            ce
+            "Could not execute request due to connection problems:\n%s" % repr(ce), ce
         )
-    except requests.HTTPError as he:
+    except requests.HTTPError:
         raise GatewayResourceNotFoundException()
     except requests.RequestException as re:
         raise GatewayRuntimeException(
-            'Could not execute request due to:\n%s' % repr(re),
-            re
+            "Could not execute request due to:\n%s" % repr(re), re
         )
 
 
-class CapakeyRestGateway(object):
-    '''
+class CapakeyRestGateway:
+    """
     A REST gateway to the capakey webservice.
 
     .. versionadded:: 0.8.0
-    '''
+    """
 
     caches = {}
 
     def __init__(self, **kwargs):
-        self.base_url = kwargs.get(
-            'base_url',
-            'https://geoservices.informatievlaanderen.be/capakey/api/v1'
-        )
-        self.base_headers = {
-            'Accept': 'application/json'
-        }
-        cache_regions = ['permanent', 'long', 'short']
+        self.base_url = kwargs.get("base_url", "https://geo.api.vlaanderen.be/capakey/v2")
+        self.base_headers = {"Accept": "application/json"}
+        cache_regions = ["permanent", "long", "short"]
         for cr in cache_regions:
             self.caches[cr] = make_region(key_mangler=str)
-        if 'cache_config' in kwargs:
+        if "cache_config" in kwargs:
             for cr in cache_regions:
-                if ('%s.backend' % cr) in kwargs['cache_config']:
-                    log.debug('Configuring %s region on CapakeyRestGateway', cr)
+                if ("%s.backend" % cr) in kwargs["cache_config"]:
+                    log.debug("Configuring %s region on CapakeyRestGateway", cr)
                     self.caches[cr].configure_from_config(
-                        kwargs['cache_config'],
-                        '%s.' % cr
+                        kwargs["cache_config"], "%s." % cr
                     )
 
     @staticmethod
     def _parse_centroid(center):
-        '''
+        """
         Parse response center from the CapakeyRestGateway to (CenterX, CenterY)
-        
+
         :param center: response center from the CapakeyRestGateway
         :return: (CenterX, CenterY)
-        '''
+        """
         coordinates = json.loads(center)["coordinates"]
         return coordinates[0], coordinates[1]
 
     @staticmethod
     def _parse_bounding_box(bounding_box):
-        '''
+        """
         Parse response bounding box from the CapakeyRestGateway to (MinimumX, MinimumY, MaximumX, MaximumY)
-        
+
         :param bounding_box: response bounding box from the CapakeyRestGateway
         :return: (MinimumX, MinimumY, MaximumX, MaximumY)
-        '''
+        """
         coordinates = json.loads(bounding_box)["coordinates"]
         x_coords = [x for x, y in coordinates[0]]
         y_coords = [y for x, y in coordinates[0]]
         return min(x_coords), min(y_coords), max(x_coords), max(y_coords)
 
     def list_gemeenten(self, sort=1):
-        '''
+        """
         List all `gemeenten` in Vlaanderen.
 
         :param integer sort: What field to sort on.
         :rtype: A :class:`list` of :class:`Gemeente`.
-        '''
+        """
+
         def creator():
-            url = self.base_url + '/municipality'
+            url = self.base_url + "/municipality"
             h = self.base_headers
-            p = {
-                'orderbyCode': sort == 1
-            }
+            p = {"orderbyCode": sort == 1}
             res = capakey_rest_gateway_request(url, h, p).json()
             return [
-                Gemeente(r['municipalityCode'], r['municipalityName'])
-                for r in res['municipalities']
+                Gemeente(r["municipalityCode"], r["municipalityName"])
+                for r in res["municipalities"]
             ]
-        if self.caches['permanent'].is_configured:
-            key = 'list_gemeenten_rest#%s' % sort
-            gemeente = self.caches['permanent'].get_or_create(key, creator)
+
+        if self.caches["permanent"].is_configured:
+            key = "list_gemeenten_rest#%s" % sort
+            gemeente = self.caches["permanent"].get_or_create(key, creator)
         else:
             gemeente = creator()
         for g in gemeente:
             g.set_gateway(self)
         return gemeente
 
     def get_gemeente_by_id(self, id):
-        '''
+        """
         Retrieve a `gemeente` by id (the NIScode).
 
         :rtype: :class:`Gemeente`
-        '''
+        """
+
         def creator():
-            url = self.base_url + '/municipality/%s' % id
+            url = self.base_url + "/municipality/%s" % id
             h = self.base_headers
-            p = {
-                'geometry': 'bbox',
-                'srs': '31370'
-            }
+            p = {"geometry": "full", "srs": "31370"}
             res = capakey_rest_gateway_request(url, h, p).json()
             return Gemeente(
-                res['municipalityCode'],
-                res['municipalityName'],
-                self._parse_centroid(res['geometry']['center']),
-                self._parse_bounding_box(res['geometry']['boundingBox'])
-            )
-        if self.caches['long'].is_configured:
-            key = 'get_gemeente_by_id_rest#%s' % id
-            gemeente = self.caches['long'].get_or_create(key, creator)
+                res["municipalityCode"],
+                res["municipalityName"],
+                self._parse_centroid(res["geometry"]["center"]),
+                self._parse_bounding_box(res["geometry"]["boundingBox"]),
+                res["geometry"]["shape"],
+            )
+
+        if self.caches["long"].is_configured:
+            key = "get_gemeente_by_id_rest#%s" % id
+            gemeente = self.caches["long"].get_or_create(key, creator)
         else:
             gemeente = creator()
         gemeente.set_gateway(self)
         return gemeente
 
     def list_kadastrale_afdelingen(self):
-        '''
+        """
         List all `kadastrale afdelingen` in Flanders.
 
         :param integer sort: Field to sort on.
         :rtype: A :class:`list` of :class:`Afdeling`.
-        '''
+        """
+
         def creator():
             gemeentes = self.list_gemeenten()
             res = []
             for g in gemeentes:
                 res += self.list_kadastrale_afdelingen_by_gemeente(g)
             return res
-        if self.caches['permanent'].is_configured:
-            key = 'list_afdelingen_rest'
-            afdelingen = self.caches['permanent'].get_or_create(key, creator)
+
+        if self.caches["permanent"].is_configured:
+            key = "list_afdelingen_rest"
+            afdelingen = self.caches["permanent"].get_or_create(key, creator)
         else:
             afdelingen = creator()
         return afdelingen
 
     def list_kadastrale_afdelingen_by_gemeente(self, gemeente, sort=1):
-        '''
+        """
         List all `kadastrale afdelingen` in a `gemeente`.
 
         :param gemeente: The :class:`Gemeente` for which the \
             `afdelingen` are wanted.
         :param integer sort: Field to sort on.
         :rtype: A :class:`list` of :class:`Afdeling`.
-        '''
+        """
         try:
             gid = gemeente.id
         except AttributeError:
             gid = gemeente
             gemeente = self.get_gemeente_by_id(gid)
         gemeente.clear_gateway()
 
         def creator():
-            url = self.base_url + '/municipality/%s/department' % gid
+            url = self.base_url + "/municipality/%s/department" % gid
             h = self.base_headers
-            p = {
-                'orderbyCode': sort == 1
-            }
+            p = {"orderbyCode": sort == 1}
             res = capakey_rest_gateway_request(url, h, p).json()
             return [
                 Afdeling(
-                    id=r['departmentCode'],
-                    naam=r['departmentName'],
-                    gemeente=gemeente
-                ) for r in res['departments']]
-        if self.caches['permanent'].is_configured:
-            key = 'list_kadastrale_afdelingen_by_gemeente_rest#%s#%s' % (gid, sort)
-            afdelingen = self.caches['permanent'].get_or_create(key, creator)
+                    id=r["departmentCode"], naam=r["departmentName"], gemeente=gemeente
+                )
+                for r in res["departments"]
+            ]
+
+        if self.caches["permanent"].is_configured:
+            key = f"list_kadastrale_afdelingen_by_gemeente_rest#{gid}#{sort}"
+            afdelingen = self.caches["permanent"].get_or_create(key, creator)
         else:
             afdelingen = creator()
         for a in afdelingen:
             a.set_gateway(self)
         return afdelingen
 
     def get_kadastrale_afdeling_by_id(self, aid):
-        '''
+        """
         Retrieve a 'kadastrale afdeling' by id.
 
         :param aid: An id of a `kadastrale afdeling`.
         :rtype: A :class:`Afdeling`.
-        '''
+        """
+
         def creator():
-            url = self.base_url + '/department/%s' % (aid)
+            url = self.base_url + "/department/%s" % (aid)
             h = self.base_headers
-            p = {
-                'geometry': 'bbox',
-                'srs': '31370'
-            }
+            p = {"geometry": "full", "srs": "31370"}
             res = capakey_rest_gateway_request(url, h, p).json()
             return Afdeling(
-                id=res['departmentCode'],
-                naam=res['departmentName'],
-                gemeente=Gemeente(res['municipalityCode'], res['municipalityName']),
-                centroid=self._parse_centroid(res['geometry']['center']),
-                bounding_box=self._parse_bounding_box(res['geometry']['boundingBox'])
-            )
-        if self.caches['long'].is_configured:
-            key = 'get_kadastrale_afdeling_by_id_rest#%s' % aid
-            afdeling = self.caches['long'].get_or_create(key, creator)
+                id=res["departmentCode"],
+                naam=res["departmentName"],
+                gemeente=Gemeente(res["municipalityCode"], res["municipalityName"]),
+                centroid=self._parse_centroid(res["geometry"]["center"]),
+                bounding_box=self._parse_bounding_box(res["geometry"]["boundingBox"]),
+                shape=res["geometry"]["shape"],
+            )
+
+        if self.caches["long"].is_configured:
+            key = "get_kadastrale_afdeling_by_id_rest#%s" % aid
+            afdeling = self.caches["long"].get_or_create(key, creator)
         else:
             afdeling = creator()
         afdeling.set_gateway(self)
         return afdeling
 
     def list_secties_by_afdeling(self, afdeling):
-        '''
+        """
         List all `secties` in a `kadastrale afdeling`.
 
         :param afdeling: The :class:`Afdeling` for which the `secties` are \
             wanted. Can also be the id of and `afdeling`.
         :rtype: A :class:`list` of `Sectie`.
-        '''
+        """
         try:
             aid = afdeling.id
             gid = afdeling.gemeente.id
         except AttributeError:
             aid = afdeling
             afdeling = self.get_kadastrale_afdeling_by_id(aid)
             gid = afdeling.gemeente.id
         afdeling.clear_gateway()
 
         def creator():
-            url = self.base_url + '/municipality/%s/department/%s/section' % (gid, aid)
+            url = self.base_url + f"/municipality/{gid}/department/{aid}/section"
             h = self.base_headers
             res = capakey_rest_gateway_request(url, h).json()
-            return [
-                Sectie(
-                    r['sectionCode'],
-                    afdeling
-                ) for r in res['sections']
-            ]
-        if self.caches['long'].is_configured:
-            key = 'list_secties_by_afdeling_rest#%s' % aid
-            secties = self.caches['long'].get_or_create(key, creator)
+            return [Sectie(r["sectionCode"], afdeling) for r in res["sections"]]
+
+        if self.caches["long"].is_configured:
+            key = "list_secties_by_afdeling_rest#%s" % aid
+            secties = self.caches["long"].get_or_create(key, creator)
         else:
             secties = creator()
         for s in secties:
             s.set_gateway(self)
         return secties
 
     def get_sectie_by_id_and_afdeling(self, id, afdeling):
-        '''
+        """
         Get a `sectie`.
 
         :param id: An id of a sectie. eg. "A"
         :param afdeling: The :class:`Afdeling` for in which the `sectie` can \
             be found. Can also be the id of and `afdeling`.
         :rtype: A :class:`Sectie`.
-        '''
+        """
         try:
             aid = afdeling.id
         except AttributeError:
             aid = afdeling
             afdeling = self.get_kadastrale_afdeling_by_id(aid)
         afdeling.clear_gateway()
 
         def creator():
-            url = self.base_url + '/municipality/%s/department/%s/section/%s' % (afdeling.gemeente.id, afdeling.id, id)
+            url = (
+                self.base_url
+                + f"/municipality/{afdeling.gemeente.id}/department/{afdeling.id}/section/{id}"
+            )
             h = self.base_headers
-            p = {
-                'geometry': 'bbox',
-                'srs': '31370'
-            }
+            p = {"geometry": "full", "srs": "31370"}
             res = capakey_rest_gateway_request(url, h, p).json()
             return Sectie(
-                res['sectionCode'],
+                res["sectionCode"],
                 afdeling,
-                self._parse_centroid(res['geometry']['center']),
-                self._parse_bounding_box(res['geometry']['boundingBox'])
+                self._parse_centroid(res["geometry"]["center"]),
+                self._parse_bounding_box(res["geometry"]["boundingBox"]),
+                res["geometry"]["shape"],
             )
-        if self.caches['long'].is_configured:
-            key = 'get_sectie_by_id_and_afdeling_rest#%s#%s' % (id, aid)
-            sectie = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["long"].is_configured:
+            key = f"get_sectie_by_id_and_afdeling_rest#{id}#{aid}"
+            sectie = self.caches["long"].get_or_create(key, creator)
         else:
             sectie = creator()
         sectie.set_gateway(self)
         return sectie
 
     def parse_percid(self, capakey):
         import re
+
         match = re.match(
-            r"^([0-9]{5})([A-Z]{1})([0-9]{4})\/([0-9]{2})([A-Z\_]{1})([0-9]{3})$",
-            capakey
+            r"^([0-9]{5})([A-Z]{1})([0-9]{4})\/([0-9]{2})([A-Z\_]{1})([0-9]{3})$", capakey
         )
         if match:
-            percid = match.group(1) + '_' + match.group(2) +\
-                '_' + match.group(3) + '_' + match.group(5) + '_' +\
-                match.group(6) + '_' + match.group(4)
+            percid = (
+                match.group(1)
+                + "_"
+                + match.group(2)
+                + "_"
+                + match.group(3)
+                + "_"
+                + match.group(5)
+                + "_"
+                + match.group(6)
+                + "_"
+                + match.group(4)
+            )
             return percid
         else:
-            raise ValueError(
-                "Invalid Capakey %s can't be parsed" % capakey
-            )
+            raise ValueError("Invalid Capakey %s can't be parsed" % capakey)
 
     def parse_capakey(self, percid):
         import re
+
         match = re.match(
             r"^([0-9]{5})_([A-Z]{1})_([0-9]{4})_([A-Z\_]{1})_([0-9]{3})_([0-9]{2})$",
-            percid
+            percid,
         )
         if match:
-            capakey = match.group(1) + match.group(2) +\
-                match.group(3) + '/' + match.group(5) + '_' +\
-                match.group(6) + '_' + match.group(4)
+            capakey = (
+                match.group(1)
+                + match.group(2)
+                + match.group(3)
+                + "/"
+                + match.group(5)
+                + "_"
+                + match.group(6)
+                + "_"
+                + match.group(4)
+            )
             return capakey
         else:
-            raise ValueError(
-                "Invalid percid %s can't be parsed" % percid
-            )
+            raise ValueError("Invalid percid %s can't be parsed" % percid)
 
     def list_percelen_by_sectie(self, sectie):
-        '''
+        """
         List all percelen in a `sectie`.
 
         :param sectie: The :class:`Sectie` for which the percelen are wanted.
         :param integer sort: Field to sort on.
         :rtype: A :class:`list` of :class:`Perceel`.
-        '''
+        """
         sid = sectie.id
         aid = sectie.afdeling.id
         gid = sectie.afdeling.gemeente.id
         sectie.clear_gateway()
+
         def creator():
-            url = self.base_url + '/municipality/%s/department/%s/section/%s/parcel' % (gid, aid, sid)
+            url = (
+                self.base_url
+                + f"/municipality/{gid}/department/{aid}/section/{sid}/parcel"
+            )
             h = self.base_headers
-            p = {
-                'data': 'cadmap'
-            }
+            p = {"data": "adp", "status": "actual"}
             res = capakey_rest_gateway_request(url, h, p).json()
             return [
                 Perceel(
-                    r['perceelnummer'],
+                    r["perceelnummer"],
                     sectie,
-                    r['capakey'],
-                    self.parse_percid(r['capakey']),
-                ) for r in res['parcels']
+                    r["capakey"],
+                    self.parse_percid(r["capakey"]),
+                )
+                for r in res["parcels"]
             ]
-        if self.caches['short'].is_configured:
-            key = 'list_percelen_by_sectie_rest#%s#%s#%s' % (gid, aid, sid)
-            percelen = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"list_percelen_by_sectie_rest#{gid}#{aid}#{sid}"
+            percelen = self.caches["short"].get_or_create(key, creator)
         else:
             percelen = creator()
         for p in percelen:
             p.set_gateway(self)
         return percelen
 
     def get_perceel_by_id_and_sectie(self, id, sectie):
-        '''
+        """
         Get a `perceel`.
 
         :param id: An id for a `perceel`.
         :param sectie: The :class:`Sectie` that contains the perceel.
         :rtype: :class:`Perceel`
-        '''
+        """
         sid = sectie.id
         aid = sectie.afdeling.id
         gid = sectie.afdeling.gemeente.id
         sectie.clear_gateway()
+
         def creator():
-            url = self.base_url + '/municipality/%s/department/%s/section/%s/parcel/%s' % (gid, aid, sid, id)
+            url = (
+                self.base_url
+                + "/municipality/{}/department/{}/section/{}/parcel/{}".format(
+                    gid, aid, sid, id
+                )
+            )
             h = self.base_headers
-            p = {
-                'geometry': 'bbox',
-                'srs': '31370',
-                'data': 'cadmap'
-            }
-            res = capakey_rest_gateway_request(url, p, h).json()
+            p = {"geometry": "full", "srs": "31370", "data": "adp", "status": "actual"}
+            res = capakey_rest_gateway_request(url, h, p).json()
             return Perceel(
-                res['perceelnummer'],
+                res["perceelnummer"],
                 sectie,
-                res['capakey'],
-                Perceel.get_percid_from_capakey(res['capakey']),
+                res["capakey"],
+                Perceel.get_percid_from_capakey(res["capakey"]),
+                res["adres"],
                 None,
                 None,
-                self._parse_centroid(res['geometry']['center']),
-                self._parse_bounding_box(res['geometry']['boundingBox'])
+                self._parse_centroid(res["geometry"]["center"]),
+                self._parse_bounding_box(res["geometry"]["boundingBox"]),
+                res["geometry"]["shape"],
+            )
+
+        if self.caches["short"].is_configured:
+            key = (
+                f"get_perceel_by_id_and_sectie_rest#{id}#{sectie.id}#{sectie.afdeling.id}"
             )
-        if self.caches['short'].is_configured:
-            key = 'get_perceel_by_id_and_sectie_rest#%s#%s#%s' % (id, sectie.id, sectie.afdeling.id)
-            perceel = self.caches['short'].get_or_create(key, creator)
+            perceel = self.caches["short"].get_or_create(key, creator)
         else:
             perceel = creator()
         perceel.set_gateway(self)
         return perceel
 
-    def get_perceel_by_capakey(self, capakey):
-        '''
-        Get a `perceel`.
-
-        :param capakey: An capakey for a `perceel`.
-        :rtype: :class:`Perceel`
-        '''
+    def _get_perceel_by(self, url, cache_key):
         def creator():
-            url = self.base_url + '/parcel/%s' % capakey
             h = self.base_headers
-            p = {
-                'geometry': 'bbox',
-                'srs': '31370',
-                'data': 'cadmap'
-            }
-            res = capakey_rest_gateway_request(url, p, h).json()
+            p = {"geometry": "full", "srs": "31370", "data": "adp", "status": "actual"}
+            res = capakey_rest_gateway_request(url, h, p).json()
             return Perceel(
-                res['perceelnummer'],
+                res["perceelnummer"],
                 Sectie(
-                    res['sectionCode'],
+                    res["sectionCode"],
                     Afdeling(
-                        res['departmentCode'],
-                        res['departmentName'],
-                        Gemeente(res['municipalityCode'], res['municipalityName'])
-                    )
+                        res["departmentCode"],
+                        res["departmentName"],
+                        Gemeente(res["municipalityCode"], res["municipalityName"]),
+                    ),
                 ),
-                res['capakey'],
-                Perceel.get_percid_from_capakey(res['capakey']),
+                res["capakey"],
+                Perceel.get_percid_from_capakey(res["capakey"]),
+                res["adres"],
                 None,
                 None,
-                self._parse_centroid(res['geometry']['center']),
-                self._parse_bounding_box(res['geometry']['boundingBox'])
+                self._parse_centroid(res["geometry"]["center"]),
+                self._parse_bounding_box(res["geometry"]["boundingBox"]),
+                res["geometry"]["shape"],
             )
-        if self.caches['short'].is_configured:
-            key = 'get_perceel_by_capakey_rest#%s' % capakey
-            perceel = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = cache_key
+            perceel = self.caches["short"].get_or_create(key, creator)
         else:
             perceel = creator()
         perceel.set_gateway(self)
         return perceel
 
+    def get_perceel_by_capakey(self, capakey):
+        """
+        Get a `perceel`.
+
+        :param capakey: An capakey for a `perceel`.
+        :rtype: :class:`Perceel`
+        """
+
+        url = self.base_url + "/parcel/%s" % capakey
+        cache_key = "get_perceel_by_capakey_rest#%s" % capakey
+        return self._get_perceel_by(url, cache_key)
+
+    def get_perceel_by_coordinates(self, x, y):
+        """
+        Get a `perceel`.
+
+        :param capakey: An capakey for a `perceel`.
+        :rtype: :class:`Perceel`
+        """
+
+        url = self.base_url + f"/parcel?x={x}&y={y}"
+        cache_key = f"get_perceel_by_coordinates_rest#{x}{y}"
+        return self._get_perceel_by(url, cache_key)
+
     def get_perceel_by_percid(self, percid):
-        '''
+        """
         Get a `perceel`.
 
         :param percid: A percid for a `perceel`.
         :rtype: :class:`Perceel`
-        '''
-        return self.get_perceel_by_capakey(
-            Perceel.get_capakey_from_percid(percid)
-        )
+        """
+        return self.get_perceel_by_capakey(Perceel.get_capakey_from_percid(percid))
 
 
-class GatewayObject(object):
-    '''
+class GatewayObject:
+    """
     Abstract class for all objects being returned from the Gateway.
-    '''
+    """
 
     gateway = None
-    '''
+    """
     The :class:`crabpy.gateway.capakey.CapakeyGateway` to use when making
     further calls to the Capakey service.
-    '''
+    """
 
     def __init__(self, **kwargs):
-        if 'gateway' in kwargs:
-            self.set_gateway(kwargs['gateway'])
+        if "gateway" in kwargs:
+            self.set_gateway(kwargs["gateway"])
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.capakey.CapakeyGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CapakeyGateway.
-        '''
+        """
         self.gateway = None
 
     def check_gateway(self):
-        '''
+        """
         Check to see if a gateway was set on this object.
-        '''
+        """
         if not self.gateway:
             raise RuntimeError("There's no Gateway I can use")
 
-    if six.PY2:
-        def __str__(self):
-            return self.__unicode__().encode('utf-8')
-    else:
-        def __str__(self):
-            return self.__unicode__()
+    def __str__(self):
+        return self.__unicode__()
 
 
 def check_lazy_load_gemeente(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Gemeente`.
-    '''
+    """
+
     def wrapper(self):
         gemeente = self
-        if (getattr(gemeente, '_%s' % f.__name__, None) is None):
-            log.debug('Lazy loading Gemeente %d', gemeente.id)
+        if getattr(gemeente, "_%s" % f.__name__, None) is None:
+            log.debug("Lazy loading Gemeente %d", gemeente.id)
             gemeente.check_gateway()
             g = gemeente.gateway.get_gemeente_by_id(gemeente.id)
             gemeente._naam = g._naam
             gemeente._centroid = g._centroid
             gemeente._bounding_box = g._bounding_box
         return f(self)
+
     return wrapper
 
 
 class Gemeente(GatewayObject):
-    '''
+    """
     The smallest administrative unit in Belgium.
-    '''
+    """
 
     def __init__(
-            self, id, naam=None,
-            centroid=None, bounding_box=None,
-            **kwargs
+        self, id, naam=None, centroid=None, bounding_box=None, shape=None, **kwargs
     ):
         self.id = int(id)
         self._naam = naam
         self._centroid = centroid
         self._bounding_box = bounding_box
-        super(Gemeente, self).__init__(**kwargs)
+        self.shape = shape
+        super().__init__(**kwargs)
 
     @property
     @check_lazy_load_gemeente
     def naam(self):
         return self._naam
 
     @property
@@ -571,69 +595,77 @@
 
     @property
     def afdelingen(self):
         self.check_gateway()
         return self.gateway.list_kadastrale_afdelingen_by_gemeente(self)
 
     def __unicode__(self):
-        return '%s (%s)' % (self.naam, self.id)
+        return f"{self.naam} ({self.id})"
 
     def __repr__(self):
-        return "Gemeente(%s, '%s')" % (self.id, self.naam)
+        return f"Gemeente({self.id}, '{self.naam}')"
 
 
 def check_lazy_load_afdeling(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Afdeling`.
-    '''
+    """
+
     def wrapper(self):
         afdeling = self
-        if (getattr(afdeling, '_%s' % f.__name__, None) is None):
-            log.debug('Lazy loading Afdeling %d', afdeling.id)
+        if getattr(afdeling, "_%s" % f.__name__, None) is None:
+            log.debug("Lazy loading Afdeling %d", afdeling.id)
             afdeling.check_gateway()
             a = afdeling.gateway.get_kadastrale_afdeling_by_id(afdeling.id)
             afdeling._naam = a._naam
             afdeling._gemeente = a._gemeente
             afdeling._centroid = a._centroid
             afdeling._bounding_box = a._bounding_box
         return f(self)
+
     return wrapper
 
 
 class Afdeling(GatewayObject):
-    '''
+    """
     A Cadastral Division of a :class:`Gemeente`.
-    '''
+    """
 
     def __init__(
-        self, id, naam=None, gemeente=None,
-        centroid=None, bounding_box=None,
-        **kwargs
+        self,
+        id,
+        naam=None,
+        gemeente=None,
+        centroid=None,
+        bounding_box=None,
+        shape=None,
+        **kwargs,
     ):
         self.id = int(id)
         self._naam = naam
         self._gemeente = gemeente
         self._centroid = centroid
         self._bounding_box = bounding_box
-        super(Afdeling, self).__init__(**kwargs)
+        self.shape = shape
+        super().__init__(**kwargs)
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.capakey.CapakeyGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
-        if (self._gemeente is not None):
+        if self._gemeente is not None:
             self._gemeente.set_gateway(gateway)
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CapakeyGateway.
-        '''
+        """
         self.gateway = None
-        if (self._gemeente is not None):
+        if self._gemeente is not None:
             self._gemeente.clear_gateway()
 
     @property
     @check_lazy_load_afdeling
     def naam(self):
         return self._naam
 
@@ -655,70 +687,73 @@
     @property
     def secties(self):
         self.check_gateway()
         return self.gateway.list_secties_by_afdeling(self)
 
     def __unicode__(self):
         if self._naam is not None:
-            return '%s (%s)' % (self._naam, self.id)
+            return f"{self._naam} ({self.id})"
         else:
-            return 'Afdeling %s' % (self.id)
+            return "Afdeling %s" % (self.id)
 
     def __repr__(self):
         if self._naam is not None:
-            return "Afdeling(%s, '%s')" % (self.id, self._naam)
+            return f"Afdeling({self.id}, '{self._naam}')"
         else:
-            return 'Afdeling(%s)' % (self.id)
+            return "Afdeling(%s)" % (self.id)
 
 
 def check_lazy_load_sectie(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Sectie`.
-    '''
+    """
+
     def wrapper(self):
         sectie = self
-        if (getattr(sectie, '_%s' % f.__name__, None) is None):
-            log.debug('Lazy loading Sectie %s in Afdeling %d', sectie.id, sectie.afdeling.id)
+        if getattr(sectie, "_%s" % f.__name__, None) is None:
+            log.debug(
+                "Lazy loading Sectie %s in Afdeling %d", sectie.id, sectie.afdeling.id
+            )
             sectie.check_gateway()
             s = sectie.gateway.get_sectie_by_id_and_afdeling(
                 sectie.id, sectie.afdeling.id
             )
             sectie._centroid = s._centroid
             sectie._bounding_box = s._bounding_box
         return f(self)
+
     return wrapper
 
 
 class Sectie(GatewayObject):
-    '''
+    """
     A subdivision of a :class:`Afdeling`.
-    '''
+    """
 
     def __init__(
-        self, id, afdeling,
-        centroid=None, bounding_box=None,
-        **kwargs
+        self, id, afdeling, centroid=None, bounding_box=None, shape=None, **kwargs
     ):
         self.id = id
         self.afdeling = afdeling
         self._centroid = centroid
         self._bounding_box = bounding_box
-        super(Sectie, self).__init__(**kwargs)
+        self.shape = shape
+        super().__init__(**kwargs)
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.capakey.CapakeyGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
         self.afdeling.set_gateway(gateway)
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CapakeyGateway.
-        '''
+        """
         self.gateway = None
         self.afdeling.clear_gateway()
 
     @property
     @check_lazy_load_sectie
     def centroid(self):
         return self._centroid
@@ -730,136 +765,157 @@
 
     @property
     def percelen(self):
         self.check_gateway()
         return self.gateway.list_percelen_by_sectie(self)
 
     def __unicode__(self):
-        return '%s, Sectie %s' % (self.afdeling, self.id)
+        return f"{self.afdeling}, Sectie {self.id}"
 
     def __repr__(self):
-        return "Sectie('%s', %s)" % (self.id, repr(self.afdeling))
+        return f"Sectie('{self.id}', {repr(self.afdeling)})"
 
 
 def check_lazy_load_perceel(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Perceel`.
-    '''
+    """
+
     def wrapper(self):
         perceel = self
-        if (getattr(perceel, '_%s' % f.__name__, None) is None):
+        if getattr(perceel, "_%s" % f.__name__, None) is None:
             log.debug(
-                'Lazy loading Perceel %s in Sectie %s in Afdeling %d',
+                "Lazy loading Perceel %s in Sectie %s in Afdeling %d",
                 perceel.id,
                 perceel.sectie.id,
-                perceel.sectie.afdeling.id
+                perceel.sectie.afdeling.id,
             )
             perceel.check_gateway()
-            p = perceel.gateway.get_perceel_by_id_and_sectie(
-                perceel.id,
-                perceel.sectie
-            )
+            p = perceel.gateway.get_perceel_by_id_and_sectie(perceel.id, perceel.sectie)
             perceel._centroid = p._centroid
             perceel._bounding_box = p._bounding_box
             perceel._capatype = p._capatype
             perceel._cashkey = p._cashkey
         return f(self)
+
     return wrapper
 
 
 class Perceel(GatewayObject):
-    '''
+    """
     A Cadastral Parcel.
-    '''
+    """
 
     def __init__(
-        self, id, sectie, capakey, percid,
-        capatype=None, cashkey=None,
-        centroid=None, bounding_box=None,
-        **kwargs
+        self,
+        id,
+        sectie,
+        capakey,
+        percid,
+        adres=None,
+        capatype=None,
+        cashkey=None,
+        centroid=None,
+        bounding_box=None,
+        shape=None,
+        **kwargs,
     ):
         self.id = id
         self.sectie = sectie
         self.capakey = capakey
         self.percid = percid
+        self.adres = adres
         self._capatype = capatype
         self._cashkey = cashkey
         self._centroid = centroid
         self._bounding_box = bounding_box
-        super(Perceel, self).__init__(**kwargs)
+        self.shape = shape
+        super().__init__(**kwargs)
         self._split_capakey()
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.capakey.CapakeyGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
         self.sectie.set_gateway(gateway)
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CapakeyGateway.
-        '''
+        """
         self.gateway = None
         self.sectie.clear_gateway()
 
     @staticmethod
     def get_percid_from_capakey(capakey):
         import re
+
         match = re.match(
-            r"^([0-9]{5})([A-Z]{1})([0-9]{4})\/([0-9]{2})([A-Z\_]{1})([0-9]{3})$",
-            capakey
+            r"^([0-9]{5})([A-Z]{1})([0-9]{4})\/([0-9]{2})([A-Z\_]{1})([0-9]{3})$", capakey
         )
         if match:
-            percid = match.group(1) + '_' + match.group(2) +\
-                '_' + match.group(3) + '_' + match.group(5) + '_' +\
-                match.group(6) + '_' + match.group(4)
+            percid = (
+                match.group(1)
+                + "_"
+                + match.group(2)
+                + "_"
+                + match.group(3)
+                + "_"
+                + match.group(5)
+                + "_"
+                + match.group(6)
+                + "_"
+                + match.group(4)
+            )
             return percid
         else:
-            raise ValueError(
-                "Invalid Capakey %s can't be parsed" % capakey
-            )
+            raise ValueError("Invalid Capakey %s can't be parsed" % capakey)
 
     @staticmethod
     def get_capakey_from_percid(percid):
         import re
+
         match = re.match(
             r"^([0-9]{5})_([A-Z]{1})_([0-9]{4})_([A-Z\_]{1})_([0-9]{3})_([0-9]{2})$",
-            percid
+            percid,
         )
         if match:
-            capakey = match.group(1) + match.group(2) +\
-                match.group(3) + '/' + match.group(6) +\
-                match.group(4) + match.group(5)
+            capakey = (
+                match.group(1)
+                + match.group(2)
+                + match.group(3)
+                + "/"
+                + match.group(6)
+                + match.group(4)
+                + match.group(5)
+            )
             return capakey
         else:
-            raise ValueError(
-                "Invalid percid %s can't be parsed" % percid
-            )
+            raise ValueError("Invalid percid %s can't be parsed" % percid)
 
     def _split_capakey(self):
-        '''
+        """
         Split a capakey into more readable elements.
 
         Splits a capakey into it's grondnummer, bisnummer, exponent and macht.
-        '''
+        """
         import re
+
         match = re.match(
             r"^[0-9]{5}[A-Z]{1}([0-9]{4})\/([0-9]{2})([A-Z\_]{1})([0-9]{3})$",
-            self.capakey
+            self.capakey,
         )
         if match:
             self.grondnummer = match.group(1)
             self.bisnummer = match.group(2)
             self.exponent = match.group(3)
             self.macht = match.group(4)
         else:
-            raise ValueError(
-                "Invalid Capakey %s can't be parsed" % self.capakey
-            )
+            raise ValueError("Invalid Capakey %s can't be parsed" % self.capakey)
 
     @property
     @check_lazy_load_perceel
     def centroid(self):
         return self._centroid
 
     @property
@@ -877,10 +933,10 @@
     def cashkey(self):
         return self._cashkey
 
     def __unicode__(self):
         return self.capakey
 
     def __repr__(self):
-        return "Perceel('%s', %s, '%s', '%s')" % (
+        return "Perceel('{}', {}, '{}', '{}')".format(
             self.id, repr(self.sectie), self.capakey, self.percid
         )
```

### Comparing `crabpy-0.9.0/crabpy/gateway/crab.py` & `crabpy-1.0.0/crabpy/gateway/crab.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1246 +1,1195 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 This module contains an opionated gateway for the crab webservice.
 
 .. versionadded:: 0.3.0
-'''
+"""
 
-from __future__ import unicode_literals
-import six
-import math
 import json
-import os
-
-from io import open
-
 import logging
-log = logging.getLogger(__name__)
-
-from crabpy.client import crab_request
+import math
+import os
 
+from dogpile.cache import make_region
 from suds import WebFault
 
-from crabpy.gateway.exception import (
-    GatewayRuntimeException,
-    GatewayResourceNotFoundException
-)
-
-from dogpile.cache import make_region
+from crabpy.client import crab_request
+from crabpy.gateway.exception import GatewayResourceNotFoundException
+from crabpy.gateway.exception import GatewayRuntimeException
 
-parent_dir = os.path.dirname(__file__)
-data_dir = os.path.join(os.path.dirname(__file__), '..', 'data')
-deelgemeenten_json = json.load(
-    open(os.path.join(data_dir, "deelgemeenten.json"),
-    encoding='utf-8')
-)
+log = logging.getLogger(__name__)
 
 
 def crab_gateway_request(client, method, *args):
-    '''
+    """
     Utility function that helps making requests to the CRAB service.
 
     This is a specialised version of :func:`crabpy.client.crab_request` that
     allows adding extra functionality for the calls made by the gateway.
 
     :param client: A :class:`suds.client.Client` for the CRAB service.
     :param string action: Which method to call, eg. `ListGewesten`
     :returns: Result of the SOAP call.
-    '''
+    """
     try:
         return crab_request(client, method, *args)
     except WebFault as wf:
         err = GatewayRuntimeException(
-            'Could not execute request. Message from server:\n%s' % wf.fault['faultstring'],
-            wf
+            "Could not execute request. Message from server:\n%s"
+            % wf.fault["faultstring"],
+            wf,
         )
         raise err
 
 
-class CrabGateway(object):
-    '''
+class CrabGateway:
+    """
     A gateway to the CRAB webservice.
-    '''
+    """
+
     caches = {}
 
     provincies = [
-        (10000, 'Antwerpen', 2),
-        (20001, 'Vlaams-Brabant', 2),
-        (30000, 'West-Vlaanderen', 2),
-        (40000, 'Oost-Vlaanderen', 2),
-        (70000, 'Limburg', 2),
-        (20002, 'Waals-Brabant', 3),
-        (50000, 'Henegouwen', 3),
-        (60000, 'Luik', 3),
-        (80000, 'Luxemburg', 3),
-        (90000, 'Namen', 3)
+        (10000, "Antwerpen", 2),
+        (20001, "Vlaams-Brabant", 2),
+        (30000, "West-Vlaanderen", 2),
+        (40000, "Oost-Vlaanderen", 2),
+        (70000, "Limburg", 2),
+        (20002, "Waals-Brabant", 3),
+        (50000, "Henegouwen", 3),
+        (60000, "Luik", 3),
+        (80000, "Luxemburg", 3),
+        (90000, "Namen", 3),
     ]
 
     def __init__(self, client, **kwargs):
         self.client = client
-        cache_regions = ['permanent', 'long', 'short']
+        cache_regions = ["permanent", "long", "short"]
         for cr in cache_regions:
             self.caches[cr] = make_region(key_mangler=str)
-        if 'cache_config' in kwargs:
+        if "cache_config" in kwargs:
             for cr in cache_regions:
-                if ('%s.backend' % cr) in kwargs['cache_config']:
-                    log.debug('Configuring %s region on CrabGateway', cr)
+                if ("%s.backend" % cr) in kwargs["cache_config"]:
+                    log.debug("Configuring %s region on CrabGateway", cr)
                     self.caches[cr].configure_from_config(
-                        kwargs['cache_config'],
-                        '%s.' % cr
+                        kwargs["cache_config"], "%s." % cr
                     )
+        data_dir = os.path.join(os.path.dirname(__file__), "..", "data")
+        with open(os.path.join(data_dir, "deelgemeenten.json"), encoding="utf-8") as f:
+            deelgemeenten_json = json.load(f)
+
         self.deelgemeenten = {
-            dg['deelgemeente_id']: {
-                'id': dg['deelgemeente_id'],
-                'naam': dg['deelgemeente_naam'],
-                'gemeente_niscode': int(dg['gemeente_id'])
-            } for dg in deelgemeenten_json
+            dg["id"]: {
+                "id": dg["id"],
+                "naam": dg["naam"],
+                "gemeente_niscode": int(dg["gemeente_niscode"]),
+            }
+            for dg in deelgemeenten_json
         }
 
     def list_gewesten(self, sort=1):
-        '''
+        """
         List all `gewesten` in Belgium.
 
         :param integer sort: What field to sort on.
         :rtype: A :class`list` of class: `Gewest`.
-        '''
+        """
+
         def creator():
-            res = crab_gateway_request(self.client, 'ListGewesten', sort)
+            res = crab_gateway_request(self.client, "ListGewesten", sort)
             tmp = {}
             for r in res.GewestItem:
                 if r.GewestId not in tmp:
                     tmp[r.GewestId] = {}
                 tmp[r.GewestId][r.TaalCodeGewestNaam] = r.GewestNaam
-            return[
-                Gewest(
-                    k,
-                    v
-                )for k, v in tmp.items()
-            ]
-        if self.caches['permanent'].is_configured:
-            key = 'ListGewesten#%s' % sort
-            gewesten = self.caches['permanent'].get_or_create(key, creator)
+            return [Gewest(k, v) for k, v in tmp.items()]
+
+        if self.caches["permanent"].is_configured:
+            key = "ListGewesten#%s" % sort
+            gewesten = self.caches["permanent"].get_or_create(key, creator)
         else:
             gewesten = creator()
         for g in gewesten:
             g.set_gateway(self)
         return gewesten
 
     def get_gewest_by_id(self, id):
-        '''
+        """
         Get a `gewest` by id.
 
         :param integer id: The id of a `gewest`.
         :rtype: A :class:`Gewest`.
-        '''
+        """
+
         def creator():
             nl = crab_gateway_request(
-                self.client, 'GetGewestByGewestIdAndTaalCode', id, 'nl'
+                self.client, "GetGewestByGewestIdAndTaalCode", id, "nl"
             )
             fr = crab_gateway_request(
-                self.client, 'GetGewestByGewestIdAndTaalCode', id, 'fr'
+                self.client, "GetGewestByGewestIdAndTaalCode", id, "fr"
             )
             de = crab_gateway_request(
-                self.client, 'GetGewestByGewestIdAndTaalCode', id, 'de'
+                self.client, "GetGewestByGewestIdAndTaalCode", id, "de"
             )
-            if nl == None:
+            if nl is None:
                 raise GatewayResourceNotFoundException()
             return Gewest(
                 nl.GewestId,
-                {
-                    'nl': nl.GewestNaam,
-                    'fr': fr.GewestNaam,
-                    'de': de.GewestNaam
-                },
+                {"nl": nl.GewestNaam, "fr": fr.GewestNaam, "de": de.GewestNaam},
                 (nl.CenterX, nl.CenterY),
                 (nl.MinimumX, nl.MinimumY, nl.MaximumX, nl.MaximumY),
             )
-        if self.caches['permanent'].is_configured:
-            key = 'GetGewestByGewestId#%s' % id
-            gewest = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["permanent"].is_configured:
+            key = "GetGewestByGewestId#%s" % id
+            gewest = self.caches["long"].get_or_create(key, creator)
         else:
             gewest = creator()
         gewest.set_gateway(self)
         return gewest
 
     def list_provincies(self, gewest=2):
-        '''
+        """
         List all `provincies` in a `gewest`.
 
         :param gewest: The :class:`Gewest` for which the \
             `provincies` are wanted.
         :param integer sort: What field to sort on.
         :rtype: A :class:`list` of :class:`Provincie`.
-        '''
+        """
         try:
             gewest_id = gewest.id
         except AttributeError:
             gewest_id = gewest
 
         def creator():
-            return [Provincie(p[0], p[1], Gewest(p[2])) for p in self.provincies if p[2] == gewest_id]
+            return [
+                Provincie(p[0], p[1], Gewest(p[2]))
+                for p in self.provincies
+                if p[2] == gewest_id
+            ]
 
-        if self.caches['permanent'].is_configured:
-            key = 'ListProvinciesByGewestId#%s' % gewest_id
-            provincies = self.caches['permanent'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "ListProvinciesByGewestId#%s" % gewest_id
+            provincies = self.caches["permanent"].get_or_create(key, creator)
         else:
             provincies = creator()
         for p in provincies:
             p.set_gateway(self)
         return provincies
 
     def get_provincie_by_id(self, niscode):
-        '''
+        """
         Retrieve a `provincie` by the niscode.
 
         :param integer niscode: The niscode of the provincie.
         :rtype: :class:`Provincie`
-        '''
+        """
+
         def creator():
             for p in self.provincies:
                 if p[0] == niscode:
                     return Provincie(p[0], p[1], Gewest(p[2]))
 
-        if self.caches['permanent'].is_configured:
-            key = 'GetProvincieByProvincieNiscode#%s' % niscode
-            provincie = self.caches['permanent'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "GetProvincieByProvincieNiscode#%s" % niscode
+            provincie = self.caches["permanent"].get_or_create(key, creator)
         else:
             provincie = creator()
-        if provincie == None:
+        if provincie is None:
             raise GatewayResourceNotFoundException()
         provincie.set_gateway(self)
         return provincie
 
     def list_gemeenten_by_provincie(self, provincie):
-        '''
+        """
         List all `gemeenten` in a `provincie`.
 
         :param provincie: The :class:`Provincie` for which the \
             `gemeenten` are wanted.
         :rtype: A :class:`list` of :class:`Gemeente`.
-        '''
+        """
         try:
             gewest = provincie.gewest
             prov = provincie
         except AttributeError:
             prov = self.get_provincie_by_id(provincie)
             gewest = prov.gewest
         gewest.clear_gateway()
 
         def creator():
             gewest_gemeenten = self.list_gemeenten(gewest.id)
-            return[
-                Gemeente(
-                    r.id,
-                    r.naam,
-                    r.niscode,
-                    gewest
-                )for r in gewest_gemeenten if str(r.niscode)[0] == str(prov.niscode)[0]
+            return [
+                Gemeente(r.id, r.naam, r.niscode, gewest)
+                for r in gewest_gemeenten
+                if str(r.niscode)[0] == str(prov.niscode)[0]
             ]
 
-        if self.caches['permanent'].is_configured:
-            key = 'ListGemeentenByProvincieId#%s' % prov.id
-            gemeente = self.caches['long'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "ListGemeentenByProvincieId#%s" % prov.id
+            gemeente = self.caches["long"].get_or_create(key, creator)
         else:
             gemeente = creator()
         for g in gemeente:
             g.set_gateway(self)
         return gemeente
 
     def list_gemeenten(self, gewest=2, sort=1):
-        '''
+        """
         List all `gemeenten` in a `gewest`.
 
         :param gewest: The :class:`Gewest` for which the \
             `gemeenten` are wanted.
         :param integer sort: What field to sort on.
         :rtype: A :class:`list` of :class:`Gemeente`.
-        '''
+        """
         try:
             gewest_id = gewest.id
         except AttributeError:
             gewest_id = gewest
             gewest = self.get_gewest_by_id(gewest_id)
         gewest.clear_gateway()
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListGemeentenByGewestId', gewest_id, sort
+                self.client, "ListGemeentenByGewestId", gewest_id, sort
             )
-            return[
-                Gemeente(
-                    r.GemeenteId,
-                    r.GemeenteNaam,
-                    r.NISGemeenteCode,
-                    gewest
-                )for r in res.GemeenteItem if r.TaalCode == r.TaalCodeGemeenteNaam
+            return [
+                Gemeente(r.GemeenteId, r.GemeenteNaam, r.NISGemeenteCode, gewest)
+                for r in res.GemeenteItem
+                if r.TaalCode == r.TaalCodeGemeenteNaam
             ]
-        if self.caches['permanent'].is_configured:
-            key = 'ListGemeentenByGewestId#%s#%s' % (gewest_id, sort)
-            gemeenten = self.caches['permanent'].get_or_create(key, creator)
+
+        if self.caches["permanent"].is_configured:
+            key = f"ListGemeentenByGewestId#{gewest_id}#{sort}"
+            gemeenten = self.caches["permanent"].get_or_create(key, creator)
         else:
             gemeenten = creator()
         for g in gemeenten:
             g.set_gateway(self)
         return gemeenten
 
     def get_gemeente_by_id(self, id):
-        '''
+        """
         Retrieve a `gemeente` by the crab id.
 
         :param integer id: The CRAB id of the gemeente.
         :rtype: :class:`Gemeente`
-        '''
+        """
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetGemeenteByGemeenteId', id
-            )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            res = crab_gateway_request(self.client, "GetGemeenteByGemeenteId", id)
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return Gemeente(
                 res.GemeenteId,
                 res.GemeenteNaam,
                 res.NisGemeenteCode,
                 Gewest(res.GewestId),
                 res.TaalCode,
                 (res.CenterX, res.CenterY),
                 (res.MinimumX, res.MinimumY, res.MaximumX, res.MaximumY),
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['long'].is_configured:
-            key = 'GetGemeenteByGemeenteId#%s' % id
-            gemeente = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["long"].is_configured:
+            key = "GetGemeenteByGemeenteId#%s" % id
+            gemeente = self.caches["long"].get_or_create(key, creator)
         else:
             gemeente = creator()
         gemeente.set_gateway(self)
         return gemeente
 
     def get_gemeente_by_niscode(self, niscode):
-        '''
+        """
         Retrieve a `gemeente` by the NIScode.
 
         :param integer niscode: The NIScode of the gemeente.
         :rtype: :class:`Gemeente`
-        '''
+        """
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetGemeenteByNISGemeenteCode', niscode
+                self.client, "GetGemeenteByNISGemeenteCode", niscode
             )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return Gemeente(
                 res.GemeenteId,
                 res.GemeenteNaam,
                 res.NisGemeenteCode,
                 Gewest(res.GewestId),
                 res.TaalCode,
                 (res.CenterX, res.CenterY),
                 (res.MinimumX, res.MinimumY, res.MaximumX, res.MaximumY),
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['long'].is_configured:
-            key = 'GetGemeenteByNISGemeenteCode#%s' % niscode
-            gemeente = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["long"].is_configured:
+            key = "GetGemeenteByNISGemeenteCode#%s" % niscode
+            gemeente = self.caches["long"].get_or_create(key, creator)
         else:
             gemeente = creator()
         gemeente.set_gateway(self)
         return gemeente
 
     def list_deelgemeenten(self, gewest=2):
-        '''
+        """
         List all `deelgemeenten` in a `gewest`.
 
         :param gewest: The :class:`Gewest` for which the \
             `deelgemeenten` are wanted. Currently only Flanders is supported.
         :rtype: A :class:`list` of :class:`Deelgemeente`.
-        '''
+        """
         try:
             gewest_id = gewest.id
         except AttributeError:
             gewest_id = gewest
 
         if gewest_id != 2:
-            raise ValueError('Currently only deelgemeenten in Flanders are known.')
+            raise ValueError("Currently only deelgemeenten in Flanders are known.")
 
         def creator():
-            return [Deelgemeente(dg['id'], dg['naam'], dg['gemeente_niscode']) for dg in self.deelgemeenten.values()]
+            return [
+                Deelgemeente(dg["id"], dg["naam"], dg["gemeente_niscode"])
+                for dg in self.deelgemeenten.values()
+            ]
 
-        if self.caches['permanent'].is_configured:
-            key = 'ListDeelgemeentenByGewestId#%s' % gewest_id
-            deelgemeenten = self.caches['permanent'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "ListDeelgemeentenByGewestId#%s" % gewest_id
+            deelgemeenten = self.caches["permanent"].get_or_create(key, creator)
         else:
             deelgemeenten = creator()
         for dg in deelgemeenten:
             dg.set_gateway(self)
         return deelgemeenten
 
     def list_deelgemeenten_by_gemeente(self, gemeente):
-        '''
+        """
         List all `deelgemeenten` in a `gemeente`.
 
         :param gemeente: The :class:`Gemeente` for which the \
             `deelgemeenten` are wanted. Currently only Flanders is supported.
         :rtype: A :class:`list` of :class:`Deelgemeente`.
-        '''
+        """
         try:
             niscode = gemeente.niscode
         except AttributeError:
             niscode = gemeente
 
         def creator():
             return [
-                Deelgemeente(dg['id'], dg['naam'], dg['gemeente_niscode'])
-                for dg in self.deelgemeenten.values() if dg['gemeente_niscode'] == niscode
+                Deelgemeente(dg["id"], dg["naam"], dg["gemeente_niscode"])
+                for dg in self.deelgemeenten.values()
+                if dg["gemeente_niscode"] == niscode
             ]
 
-        if self.caches['permanent'].is_configured:
-            key = 'ListDeelgemeentenByGemeenteId#%s' % niscode
-            deelgemeenten = self.caches['permanent'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "ListDeelgemeentenByGemeenteId#%s" % niscode
+            deelgemeenten = self.caches["permanent"].get_or_create(key, creator)
         else:
             deelgemeenten = creator()
         for dg in deelgemeenten:
             dg.set_gateway(self)
         return deelgemeenten
 
     def get_deelgemeente_by_id(self, id):
-        '''
+        """
         Retrieve a `deelgemeente` by the id.
 
         :param string id: The id of the deelgemeente.
         :rtype: :class:`Deelgemeente`
-        '''
+        """
+
         def creator():
             if id in self.deelgemeenten:
                 dg = self.deelgemeenten[id]
-                return Deelgemeente(dg['id'], dg['naam'], dg['gemeente_niscode'])
+                return Deelgemeente(dg["id"], dg["naam"], dg["gemeente_niscode"])
             else:
                 return None
 
-        if self.caches['permanent'].is_configured:
-            key = 'GetDeelgemeenteByDeelgemeenteId#%s' % id
-            deelgemeente = self.caches['permanent'].get_or_create(key, creator)
+        if self.caches["permanent"].is_configured:
+            key = "GetDeelgemeenteByDeelgemeenteId#%s" % id
+            deelgemeente = self.caches["permanent"].get_or_create(key, creator)
         else:
             deelgemeente = creator()
-        if deelgemeente == None:
+        if deelgemeente is None:
             raise GatewayResourceNotFoundException()
         deelgemeente.set_gateway(self)
         return deelgemeente
 
     def _list_codeobject(self, function, sort, returnclass):
         def creator():
             res = crab_gateway_request(self.client, function, sort)
-            return[
-                globals()[returnclass](
-                    r.Code,
-                    r.Naam,
-                    r.Definitie
-                )for r in res.CodeItem
+            return [
+                globals()[returnclass](r.Code, r.Naam, r.Definitie) for r in res.CodeItem
             ]
-        if self.caches['permanent'].is_configured:
-            key = function + '#%s' % (sort)
-            return self.caches['permanent'].get_or_create(key, creator)
+
+        if self.caches["permanent"].is_configured:
+            key = function + "#%s" % (sort)
+            return self.caches["permanent"].get_or_create(key, creator)
         else:
             return creator()
 
     def list_talen(self, sort=1):
-        '''
+        """
         List all `talen`.
 
         :rtype: A :class:`list` of :class:`Taal`
-        '''
-        return self._list_codeobject('ListTalen', sort, 'Taal')
+        """
+        return self._list_codeobject("ListTalen", sort, "Taal")
 
     def list_bewerkingen(self, sort=1):
-        '''
+        """
         List all `bewerkingen`.
 
         :rtype: A :class:`list` of :class:`Bewerking`
-        '''
-        return self._list_codeobject(
-            'ListBewerkingen', sort, 'Bewerking'
-        )
+        """
+        return self._list_codeobject("ListBewerkingen", sort, "Bewerking")
 
     def list_organisaties(self, sort=1):
-        '''
+        """
         List all `organisaties`.
 
         :rtype: A :class:`list` of :class:`Organisatie`
-        '''
-        return self._list_codeobject(
-            'ListOrganisaties', sort, 'Organisatie'
-        )
+        """
+        return self._list_codeobject("ListOrganisaties", sort, "Organisatie")
 
     def list_aardsubadressen(self, sort=1):
-        '''
+        """
         List all `aardsubadressen`.
 
         :rtype: A :class:`list` of :class:`Aardsubadres`
-        '''
-        return self._list_codeobject(
-            'ListAardSubadressen', sort, 'Aardsubadres'
-        )
+        """
+        return self._list_codeobject("ListAardSubadressen", sort, "Aardsubadres")
 
     def list_aardadressen(self, sort=1):
-        '''
+        """
         List all `aardadressen`.
 
         :rtype: A :class:`list` of :class:`Aardadres`
-        '''
-        return self._list_codeobject(
-            'ListAardAdressen', sort, 'Aardadres'
-        )
+        """
+        return self._list_codeobject("ListAardAdressen", sort, "Aardadres")
 
     def list_aardgebouwen(self, sort=1):
-        '''
+        """
         List all `aardgebouwen`.
 
         :rtype: A :class:`list` of :class:`Aardgebouw`
-        '''
-        return self._list_codeobject(
-            'ListAardGebouwen', sort, 'Aardgebouw'
-        )
+        """
+        return self._list_codeobject("ListAardGebouwen", sort, "Aardgebouw")
 
     def list_aardwegobjecten(self, sort=1):
-        '''
+        """
         List all `aardwegobjecten`.
 
         :rtype: A :class:`list` of :class:`Aardwegobject`
-        '''
-        return self._list_codeobject(
-            'ListAardWegobjecten', sort, 'Aardwegobject'
-        )
+        """
+        return self._list_codeobject("ListAardWegobjecten", sort, "Aardwegobject")
 
     def list_aardterreinobjecten(self, sort=1):
-        '''
+        """
         List all `aardterreinobjecten`.
 
         :rtype: A :class:`list` of :class:`Aardterreinobject`
-        '''
-        return self._list_codeobject(
-            'ListAardTerreinobjecten', sort, 'Aardterreinobject'
-        )
+        """
+        return self._list_codeobject("ListAardTerreinobjecten", sort, "Aardterreinobject")
 
     def list_statushuisnummers(self, sort=1):
-        '''
+        """
         List all `statushuisnummers`.
 
         :rtype: A :class:`list` of :class:`Statushuisnummer`
-        '''
-        return self._list_codeobject(
-            'ListStatusHuisnummers', sort, 'Statushuisnummer'
-        )
+        """
+        return self._list_codeobject("ListStatusHuisnummers", sort, "Statushuisnummer")
 
     def list_statussubadressen(self, sort=1):
-        '''
+        """
         List all `statussubadressen`.
 
         :rtype: A :class:`list` of :class:`Statussubadres`
-        '''
-        return self._list_codeobject(
-            'ListStatusSubadressen', sort, 'Statussubadres'
-        )
+        """
+        return self._list_codeobject("ListStatusSubadressen", sort, "Statussubadres")
 
     def list_statusstraatnamen(self, sort=1):
-        '''
+        """
         List all `statusstraatnamen`.
 
         :rtype: A :class:`list` of :class:`Statusstraatnaam`
-        '''
-        return self._list_codeobject(
-            'ListStatusStraatnamen', sort, 'Statusstraatnaam'
-        )
+        """
+        return self._list_codeobject("ListStatusStraatnamen", sort, "Statusstraatnaam")
 
     def list_statuswegsegmenten(self, sort=1):
-        '''
+        """
         List all `statuswegsegmenten`.
 
         :rtype: A :class:`list` of :class:`Statuswegsegment`
-        '''
-        return self._list_codeobject(
-            'ListStatusWegsegmenten', sort, 'Statuswegsegment'
-        )
+        """
+        return self._list_codeobject("ListStatusWegsegmenten", sort, "Statuswegsegment")
 
     def list_geometriemethodewegsegmenten(self, sort=1):
-        '''
+        """
         List all `geometriemethodewegsegmenten`.
 
         :rtype: A :class:`list` of :class:`Geometriemethodewegsegment`
-        '''
+        """
         return self._list_codeobject(
-            'ListGeometriemethodeWegsegmenten', sort,
-            'Geometriemethodewegsegment'
+            "ListGeometriemethodeWegsegmenten", sort, "Geometriemethodewegsegment"
         )
 
     def list_statusgebouwen(self, sort=1):
-        '''
+        """
         List all `statusgebouwen`.
 
         :rtype: A :class:`list` of :class:`Statusgebouwen`
-        '''
-        return self._list_codeobject(
-            'ListStatusGebouwen', sort, 'Statusgebouw'
-        )
+        """
+        return self._list_codeobject("ListStatusGebouwen", sort, "Statusgebouw")
 
     def list_geometriemethodegebouwen(self, sort=1):
-        '''
+        """
         List all `geometriegebouwen`.
 
         :rtype: A :class:`list` of :class:`Geometriegebouw`
-        '''
+        """
         return self._list_codeobject(
-            'ListGeometriemethodeGebouwen', sort, 'Geometriemethodegebouw'
+            "ListGeometriemethodeGebouwen", sort, "Geometriemethodegebouw"
         )
 
     def list_herkomstadresposities(self, sort=1):
-        '''
+        """
         List all `herkomstadresposities`.
 
         :rtype: A :class:`list` of :class:`Herkomstadrespositie`
-        '''
+        """
         return self._list_codeobject(
-            'ListHerkomstAdresposities', sort, 'Herkomstadrespositie'
+            "ListHerkomstAdresposities", sort, "Herkomstadrespositie"
         )
 
     def list_straten(self, gemeente, sort=1):
-        '''
+        """
         List all `straten` in a `Gemeente`.
 
         :param gemeente: The :class:`Gemeente` for which the \
             `straten` are wanted.
         :rtype: A :class:`list` of :class:`Straat`
-        '''
+        """
         try:
             id = gemeente.id
         except AttributeError:
             id = gemeente
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListStraatnamenWithStatusByGemeenteId',
-                id, sort
+                self.client, "ListStraatnamenWithStatusByGemeenteId", id, sort
             )
             try:
-                return[
+                return [
                     Straat(
                         r.StraatnaamId,
                         r.StraatnaamLabel,
                         id,
-                        r.StatusStraatnaam
-                    )for r in res.StraatnaamWithStatusItem
+                        r.StatusStraatnaam,
+                        r.Straatnaam,
+                        r.TaalCode,
+                        r.StraatnaamTweedeTaal,
+                        r.TaalCodeTweedeTaal,
+                    )
+                    for r in res.StraatnaamWithStatusItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['long'].is_configured:
-            key = 'ListStraatnamenWithStatusByGemeenteId#%s%s' % (id, sort)
-            straten = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["long"].is_configured:
+            key = f"ListStraatnamenWithStatusByGemeenteId#{id}{sort}"
+            straten = self.caches["long"].get_or_create(key, creator)
         else:
             straten = creator()
         for s in straten:
             s.set_gateway(self)
         return straten
 
     def get_straat_by_id(self, id):
-        '''
+        """
         Retrieve a `straat` by the Id.
 
         :param integer id: The id of the `straat`.
         :rtype: :class:`Straat`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetStraatnaamWithStatusByStraatnaamId', id
+                self.client, "GetStraatnaamWithStatusByStraatnaamId", id
             )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return Straat(
                 res.StraatnaamId,
                 res.StraatnaamLabel,
                 res.GemeenteId,
                 res.StatusStraatnaam,
                 res.Straatnaam,
                 res.TaalCode,
                 res.StraatnaamTweedeTaal,
                 res.TaalCodeTweedeTaal,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
 
-        if self.caches['long'].is_configured:
-            key = 'GetStraatnaamWithStatusByStraatnaamId#%s' % (id)
-            straat = self.caches['long'].get_or_create(key, creator)
+        if self.caches["long"].is_configured:
+            key = "GetStraatnaamWithStatusByStraatnaamId#%s" % (id)
+            straat = self.caches["long"].get_or_create(key, creator)
         else:
             straat = creator()
         straat.set_gateway(self)
         return straat
 
     def list_huisnummers_by_straat(self, straat, sort=1):
-        '''
+        """
         List all `huisnummers` in a `Straat`.
 
         :param straat: The :class:`Straat` for which the \
             `huisnummers` are wanted.
         :rtype: A :class: `list` of :class:`Huisnummer`
-        '''
+        """
         try:
             id = straat.id
         except AttributeError:
             id = straat
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListHuisnummersWithStatusByStraatnaamId',
-                id, sort
+                self.client, "ListHuisnummersWithStatusByStraatnaamId", id, sort
             )
             try:
-                return[
-                    Huisnummer(
-                        r.HuisnummerId,
-                        r.StatusHuisnummer,
-                        r.Huisnummer,
-                        id
-                    ) for r in res.HuisnummerWithStatusItem
+                return [
+                    Huisnummer(r.HuisnummerId, r.StatusHuisnummer, r.Huisnummer, id)
+                    for r in res.HuisnummerWithStatusItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListHuisnummersWithStatusByStraatnaamId#%s%s' % (id, sort)
-            huisnummers = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"ListHuisnummersWithStatusByStraatnaamId#{id}{sort}"
+            huisnummers = self.caches["short"].get_or_create(key, creator)
         else:
             huisnummers = creator()
         for h in huisnummers:
             h.set_gateway(self)
         return huisnummers
 
     def list_huisnummers_by_perceel(self, perceel, sort=1):
-        '''
+        """
         List all `huisnummers` on a `Pereel`.
 
         Generally there will only be one, but multiples are possible.
 
         :param perceel: The :class:`Perceel` for which the \
             `huisnummers` are wanted.
         :rtype: A :class: `list` of :class:`Huisnummer`
-        '''
+        """
         try:
             id = perceel.id
         except AttributeError:
             id = perceel
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListHuisnummersWithStatusByIdentificatorPerceel',
-                id, sort
+                self.client, "ListHuisnummersWithStatusByIdentificatorPerceel", id, sort
             )
             try:
-                huisnummers= []
+                huisnummers = []
                 for r in res.HuisnummerWithStatusItem:
                     h = self.get_huisnummer_by_id(r.HuisnummerId)
                     h.clear_gateway()
                     huisnummers.append(h)
                 return huisnummers
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListHuisnummersWithStatusByIdentificatorPerceel#%s%s' % (id, sort)
-            huisnummers = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"ListHuisnummersWithStatusByIdentificatorPerceel#{id}{sort}"
+            huisnummers = self.caches["short"].get_or_create(key, creator)
         else:
             huisnummers = creator()
         for h in huisnummers:
             h.set_gateway(self)
         return huisnummers
 
     def get_huisnummer_by_id(self, id):
-        '''
+        """
         Retrieve a `huisnummer` by the Id.
 
         :param integer id: the Id of the `huisnummer`
         :rtype: :class:`Huisnummer`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetHuisnummerWithStatusByHuisnummerId', id
+                self.client, "GetHuisnummerWithStatusByHuisnummerId", id
             )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return Huisnummer(
                 res.HuisnummerId,
                 res.StatusHuisnummer,
                 res.Huisnummer,
                 res.StraatnaamId,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetHuisnummerWithStatusByHuisnummerId#%s' % (id)
-            huisnummer = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetHuisnummerWithStatusByHuisnummerId#%s" % (id)
+            huisnummer = self.caches["short"].get_or_create(key, creator)
         else:
             huisnummer = creator()
         huisnummer.set_gateway(self)
         return huisnummer
 
     def get_huisnummer_by_nummer_and_straat(self, nummer, straat):
-        '''
+        """
         Retrieve a `huisnummer` by the `nummer` and `straat`
 
         :param integer nummer: The huisnummer of the 'huisnummer`
         :param straat: The :class:`Straat` in which the `huisnummer` \
             is situated.
         :rtype: A :class:`Huisnummer`
-        '''
+        """
         try:
             straat_id = straat.id
         except AttributeError:
             straat_id = straat
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetHuisnummerWithStatusByHuisnummer',
-                nummer, straat_id
+                self.client, "GetHuisnummerWithStatusByHuisnummer", nummer, straat_id
             )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return Huisnummer(
                 res.HuisnummerId,
                 res.StatusHuisnummer,
                 res.Huisnummer,
                 res.StraatnaamId,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetHuisnummerWithStatusByHuisnummer#%s%s' % (nummer, straat_id)
-            huisnummer = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"GetHuisnummerWithStatusByHuisnummer#{nummer}{straat_id}"
+            huisnummer = self.caches["short"].get_or_create(key, creator)
         else:
             huisnummer = creator()
         huisnummer.set_gateway(self)
         return huisnummer
 
     def list_postkantons_by_gemeente(self, gemeente):
-        '''
+        """
         List all `postkantons` in a :class:`Gemeente`
 
         :param gemeente: The :class:`Gemeente` for which the \
             `potkantons` are wanted.
         :rtype: A :class:`list` of :class:`Postkanton`
-        '''
+        """
         try:
             id = gemeente.id
         except AttributeError:
             id = gemeente
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListPostkantonsByGemeenteId', id
-            )
+            res = crab_gateway_request(self.client, "ListPostkantonsByGemeenteId", id)
             try:
-                return[
-                    Postkanton(
-                        r.PostkantonCode
-                    )for r in res.PostkantonItem
-                ]
+                return [Postkanton(r.PostkantonCode) for r in res.PostkantonItem]
             except AttributeError:
                 return []
-        if self.caches['long'].is_configured:
-            key = 'ListPostkantonsByGemeenteId#%s' % (id)
-            postkantons = self.caches['long'].get_or_create(key, creator)
+
+        if self.caches["long"].is_configured:
+            key = "ListPostkantonsByGemeenteId#%s" % (id)
+            postkantons = self.caches["long"].get_or_create(key, creator)
         else:
             postkantons = creator()
         for r in postkantons:
             r.set_gateway(self)
         return postkantons
 
     def get_postkanton_by_huisnummer(self, huisnummer):
-        '''
+        """
         Retrieve a `postkanton` by the Huisnummer.
 
         :param huisnummer: The :class:`Huisnummer` for which the `postkanton` \
                 is wanted.
         :rtype: :class:`Postkanton`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetPostkantonByHuisnummerId', id
-            )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
-            return Postkanton(
-                res.PostkantonCode
-            )
-        if self.caches['short'].is_configured:
-            key = 'GetPostkantonByHuisnummerId#%s' % (id)
-            postkanton = self.caches['short'].get_or_create(key, creator)
+            res = crab_gateway_request(self.client, "GetPostkantonByHuisnummerId", id)
+            if res is None:
+                raise GatewayResourceNotFoundException()
+            return Postkanton(res.PostkantonCode)
+
+        if self.caches["short"].is_configured:
+            key = "GetPostkantonByHuisnummerId#%s" % (id)
+            postkanton = self.caches["short"].get_or_create(key, creator)
         else:
             postkanton = creator()
         postkanton.set_gateway(self)
         return postkanton
 
     def get_wegobject_by_id(self, id):
-        '''
+        """
         Retrieve a `Wegobject` by the Id.
 
         :param integer id: the Id of the `Wegobject`
         :rtype: :class:`Wegobject`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetWegobjectByIdentificatorWegobject', id
+                self.client, "GetWegobjectByIdentificatorWegobject", id
             )
-            if res == None:
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Wegobject(
                 res.IdentificatorWegobject,
                 res.AardWegobject,
                 (res.CenterX, res.CenterY),
                 (res.MinimumX, res.MinimumY, res.MaximumX, res.MaximumY),
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetWegobjectByIdentificatorWegobject#%s' % (id)
-            wegobject = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetWegobjectByIdentificatorWegobject#%s" % (id)
+            wegobject = self.caches["short"].get_or_create(key, creator)
         else:
             wegobject = creator()
         wegobject.set_gateway(self)
         return wegobject
 
     def list_wegobjecten_by_straat(self, straat):
-        '''
+        """
         List all `wegobjecten` in a :class:`Straat`
 
         :param straat: The :class:`Straat` for which the `wegobjecten` \
                 are wanted.
         :rtype: A :class:`list` of :class:`Wegobject`
-        '''
+        """
         try:
             id = straat.id
         except AttributeError:
             id = straat
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListWegobjectenByStraatnaamId', id
-            )
+            res = crab_gateway_request(self.client, "ListWegobjectenByStraatnaamId", id)
             try:
                 return [
-                    Wegobject(
-                        r.IdentificatorWegobject,
-                        r.AardWegobject
-                    )for r in res.WegobjectItem
+                    Wegobject(r.IdentificatorWegobject, r.AardWegobject)
+                    for r in res.WegobjectItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListWegobjectenByStraatnaamId#%s' % (id)
-            wegobjecten = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListWegobjectenByStraatnaamId#%s" % (id)
+            wegobjecten = self.caches["short"].get_or_create(key, creator)
         else:
             wegobjecten = creator()
         for r in wegobjecten:
             r.set_gateway(self)
         return wegobjecten
 
     def get_wegsegment_by_id(self, id):
-        '''
+        """
         Retrieve a `wegsegment` by the Id.
 
         :param integer id: the Id of the `wegsegment`
         :rtype: :class:`Wegsegment`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client,
-                'GetWegsegmentByIdentificatorWegsegment', id
+                self.client, "GetWegsegmentByIdentificatorWegsegment", id
             )
-            if res == None:
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Wegsegment(
                 res.IdentificatorWegsegment,
                 res.StatusWegsegment,
                 res.GeometriemethodeWegsegment,
                 res.Geometrie,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetWegsegmentByIdentificatorWegsegment#%s' % (id)
-            wegsegment = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetWegsegmentByIdentificatorWegsegment#%s" % (id)
+            wegsegment = self.caches["short"].get_or_create(key, creator)
         else:
             wegsegment = creator()
         wegsegment.set_gateway(self)
         return wegsegment
 
     def list_wegsegmenten_by_straat(self, straat):
-        '''
+        """
         List all `wegsegmenten` in a :class:`Straat`
 
         :param straat: The :class:`Straat` for which the `wegsegmenten` \
                 are wanted.
         :rtype: A :class:`list` of :class:`Wegsegment`
-        '''
+        """
         try:
             id = straat.id
         except AttributeError:
             id = straat
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListWegsegmentenByStraatnaamId', id
-            )
+            res = crab_gateway_request(self.client, "ListWegsegmentenByStraatnaamId", id)
             try:
-                return[
-                    Wegsegment(
-                        r.IdentificatorWegsegment,
-                        r.StatusWegsegment
-                    )for r in res.WegsegmentItem
+                return [
+                    Wegsegment(r.IdentificatorWegsegment, r.StatusWegsegment)
+                    for r in res.WegsegmentItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListWegsegmentenByStraatnaamId#%s' % (id)
-            wegsegmenten = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListWegsegmentenByStraatnaamId#%s" % (id)
+            wegsegmenten = self.caches["short"].get_or_create(key, creator)
         else:
             wegsegmenten = creator()
         for r in wegsegmenten:
             r.set_gateway(self)
         return wegsegmenten
 
     def list_terreinobjecten_by_huisnummer(self, huisnummer):
-        '''
+        """
         List all `terreinobjecten` for a :class:`Huisnummer`
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `terreinobjecten` are wanted.
         :rtype: A :class:`list` of :class:`Terreinobject`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListTerreinobjectenByHuisnummerId', id
+                self.client, "ListTerreinobjectenByHuisnummerId", id
             )
             try:
-                return[
-                    Terreinobject(
-                        r.IdentificatorTerreinobject,
-                        r.AardTerreinobject
-                    )for r in res.TerreinobjectItem
+                return [
+                    Terreinobject(r.IdentificatorTerreinobject, r.AardTerreinobject)
+                    for r in res.TerreinobjectItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListTerreinobjectenByHuisnummerId#%s' % (id)
-            terreinobjecten = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListTerreinobjectenByHuisnummerId#%s" % (id)
+            terreinobjecten = self.caches["short"].get_or_create(key, creator)
         else:
             terreinobjecten = creator()
         for r in terreinobjecten:
             r.set_gateway(self)
         return terreinobjecten
 
     def get_terreinobject_by_id(self, id):
-        '''
+        """
         Retrieve a `Terreinobject` by the Id.
 
         :param integer id: the Id of the `Terreinobject`
         :rtype: :class:`Terreinobject`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client,
-                'GetTerreinobjectByIdentificatorTerreinobject', id
+                self.client, "GetTerreinobjectByIdentificatorTerreinobject", id
             )
-            if res == None:
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Terreinobject(
                 res.IdentificatorTerreinobject,
                 res.AardTerreinobject,
                 (res.CenterX, res.CenterY),
                 (res.MinimumX, res.MinimumY, res.MaximumX, res.MaximumY),
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetTerreinobjectByIdentificatorTerreinobject#%s' % (id)
-            terreinobject = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetTerreinobjectByIdentificatorTerreinobject#%s" % (id)
+            terreinobject = self.caches["short"].get_or_create(key, creator)
         else:
             terreinobject = creator()
         terreinobject.set_gateway(self)
         return terreinobject
 
     def list_percelen_by_huisnummer(self, huisnummer):
-        '''
+        """
         List all `percelen` for a :class:`Huisnummer`
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `percelen` are wanted.
         :rtype: A :class:`list` of :class:`Perceel`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListPercelenByHuisnummerId', id
-            )
+            res = crab_gateway_request(self.client, "ListPercelenByHuisnummerId", id)
             try:
-                return [
-                    Perceel(
-                        r.IdentificatorPerceel
-                    )for r in res.PerceelItem
-                ]
+                return [Perceel(r.IdentificatorPerceel) for r in res.PerceelItem]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListPercelenByHuisnummerId#%s' % (id)
-            percelen = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListPercelenByHuisnummerId#%s" % (id)
+            percelen = self.caches["short"].get_or_create(key, creator)
         else:
             percelen = creator()
         for r in percelen:
             r.set_gateway(self)
         return percelen
 
     def get_perceel_by_id(self, id):
-        '''
+        """
         Retrieve a `Perceel` by the Id.
 
         :param string id: the Id of the `Perceel`
         :rtype: :class:`Perceel`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetPerceelByIdentificatorPerceel', id
+                self.client, "GetPerceelByIdentificatorPerceel", id
             )
-            if res == None:
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Perceel(
                 res.IdentificatorPerceel,
                 (res.CenterX, res.CenterY),
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetPerceelByIdentificatorPerceel#%s' % (id)
-            perceel = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetPerceelByIdentificatorPerceel#%s" % (id)
+            perceel = self.caches["short"].get_or_create(key, creator)
         else:
             perceel = creator()
         perceel.set_gateway(self)
         return perceel
 
     def list_gebouwen_by_huisnummer(self, huisnummer):
-        '''
+        """
         List all `gebouwen` for a :class:`Huisnummer`.
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `gebouwen` are wanted.
         :rtype: A :class:`list` of :class:`Gebouw`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
 
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListGebouwenByHuisnummerId', id
-            )
+            res = crab_gateway_request(self.client, "ListGebouwenByHuisnummerId", id)
             try:
                 return [
-                    Gebouw(
-                        r.IdentificatorGebouw,
-                        r.AardGebouw,
-                        r.StatusGebouw
-                    )for r in res.GebouwItem
+                    Gebouw(r.IdentificatorGebouw, r.AardGebouw, r.StatusGebouw)
+                    for r in res.GebouwItem
                 ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListGebouwenByHuisnummerId#%s' % (id)
-            gebouwen = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListGebouwenByHuisnummerId#%s" % (id)
+            gebouwen = self.caches["short"].get_or_create(key, creator)
         else:
             gebouwen = creator()
         for r in gebouwen:
             r.set_gateway(self)
         return gebouwen
 
     def get_gebouw_by_id(self, id):
-        '''
+        """
         Retrieve a `Gebouw` by the Id.
 
         :param integer id: the Id of the `Gebouw`
         :rtype: :class:`Gebouw`
-        '''
+        """
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetGebouwByIdentificatorGebouw', id
-            )
-            if res == None:
+            res = crab_gateway_request(self.client, "GetGebouwByIdentificatorGebouw", id)
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Gebouw(
                 res.IdentificatorGebouw,
                 res.AardGebouw,
                 res.StatusGebouw,
                 res.GeometriemethodeGebouw,
                 res.Geometrie,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetGebouwByIdentificatorGebouw#%s' % (id)
-            gebouw = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetGebouwByIdentificatorGebouw#%s" % (id)
+            gebouw = self.caches["short"].get_or_create(key, creator)
         else:
             gebouw = creator()
         gebouw.set_gateway(self)
         return gebouw
 
     def get_bewerking(self, res):
         r = self.list_bewerkingen()
@@ -1251,383 +1200,381 @@
     def get_organisatie(self, res):
         r = self.list_organisaties()
         for item in r:
             if int(item.id) == int(res):
                 return item
 
     def list_subadressen_by_huisnummer(self, huisnummer):
-        '''
+        """
         List all `subadressen` for a :class:`Huisnummer`.
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `subadressen` are wanted. OR A huisnummer id.
         :rtype: A :class:`list` of :class:`Gebouw`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
 
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListSubadressenWithStatusByHuisnummerId', id
+                self.client, "ListSubadressenWithStatusByHuisnummerId", id
             )
             try:
-                return [ Subadres(
-                    r.SubadresId,
-                    r.Subadres,
-                    r.StatusSubadres
-                )for r in res.SubadresWithStatusItem ]
+                return [
+                    Subadres(r.SubadresId, r.Subadres, r.StatusSubadres)
+                    for r in res.SubadresWithStatusItem
+                ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListSubadressenWithStatusByHuisnummerId#%s' % (id)
-            subadressen = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListSubadressenWithStatusByHuisnummerId#%s" % (id)
+            subadressen = self.caches["short"].get_or_create(key, creator)
         else:
             subadressen = creator()
         for s in subadressen:
             s.set_gateway(self)
         return subadressen
 
     def get_subadres_by_id(self, id):
-        '''
+        """
         Retrieve a `Subadres` by the Id.
 
         :param integer id: the Id of the `Subadres`
         :rtype: :class:`Subadres`
-        '''
+        """
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'GetSubadresWithStatusBySubadresId', id
+                self.client, "GetSubadresWithStatusBySubadresId", id
             )
-            if res == None:
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Subadres(
                 res.SubadresId,
                 res.Subadres,
                 res.StatusSubadres,
                 res.HuisnummerId,
                 res.AardSubadres,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetSubadresWithStatusBySubadresId#%s' % (id)
-            subadres = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetSubadresWithStatusBySubadresId#%s" % (id)
+            subadres = self.caches["short"].get_or_create(key, creator)
         else:
             subadres = creator()
         subadres.set_gateway(self)
         return subadres
 
     def list_adresposities_by_huisnummer(self, huisnummer):
-        '''
+        """
         List all `adresposities` for a :class:`Huisnummer`.
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `adresposities` are wanted. OR A huisnummer id.
         :rtype: A :class:`list` of :class:`Adrespositie`
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListAdrespositiesByHuisnummerId', id
-            )
+            res = crab_gateway_request(self.client, "ListAdrespositiesByHuisnummerId", id)
             try:
-                return [Adrespositie(
-                    r.AdrespositieId,
-                    r.HerkomstAdrespositie
-                ) for r in res.AdrespositieItem]
+                return [
+                    Adrespositie(r.AdrespositieId, r.HerkomstAdrespositie)
+                    for r in res.AdrespositieItem
+                ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListAdrespositiesByHuisnummerId#%s' % (id)
-            adresposities = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListAdrespositiesByHuisnummerId#%s" % (id)
+            adresposities = self.caches["short"].get_or_create(key, creator)
         else:
             adresposities = creator()
         for a in adresposities:
             a.set_gateway(self)
         return adresposities
 
     def list_adresposities_by_nummer_and_straat(self, nummer, straat):
-        '''
+        """
         List all `adresposities` for a huisnummer and a :class:`Straat`.
 
         :param nummer: A string representing a certain huisnummer.
         :param straat: The :class:`Straat` for which the \
             `adresposities` are wanted. OR A straat id.
         :rtype: A :class:`list` of :class:`Adrespositie`
-        '''
+        """
         try:
             sid = straat.id
         except AttributeError:
             sid = straat
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListAdrespositiesByHuisnummer', nummer, sid
+                self.client, "ListAdrespositiesByHuisnummer", nummer, sid
             )
             try:
-                return [Adrespositie(
-                    r.AdrespositieId,
-                    r.HerkomstAdrespositie
-                )for r in res.AdrespositieItem]
+                return [
+                    Adrespositie(r.AdrespositieId, r.HerkomstAdrespositie)
+                    for r in res.AdrespositieItem
+                ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListAdrespositiesByHuisnummer#%s%s' % (nummer, sid)
-            adresposities = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"ListAdrespositiesByHuisnummer#{nummer}{sid}"
+            adresposities = self.caches["short"].get_or_create(key, creator)
         else:
             adresposities = creator()
         for a in adresposities:
             a.set_gateway(self)
         return adresposities
 
     def list_adresposities_by_subadres(self, subadres):
-        '''
+        """
         List all `adresposities` for a :class:`Subadres`.
 
         :param subadres: The :class:`Subadres` for which the \
             `adresposities` are wanted. OR A subadres id.
         :rtype: A :class:`list` of :class:`Adrespositie`
-        '''
+        """
         try:
             id = subadres.id
         except AttributeError:
             id = subadres
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'ListAdrespositiesBySubadresId', id
-            )
+            res = crab_gateway_request(self.client, "ListAdrespositiesBySubadresId", id)
             try:
-                return [Adrespositie(
-                    r.AdrespositieId,
-                    r.HerkomstAdrespositie
-                )for r in res.AdrespositieItem]
+                return [
+                    Adrespositie(r.AdrespositieId, r.HerkomstAdrespositie)
+                    for r in res.AdrespositieItem
+                ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListAdrespositiesBySubadresId#%s' % (id)
-            adresposities = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "ListAdrespositiesBySubadresId#%s" % (id)
+            adresposities = self.caches["short"].get_or_create(key, creator)
         else:
             adresposities = creator()
         for a in adresposities:
             a.set_gateway(self)
         return adresposities
 
     def list_adresposities_by_subadres_and_huisnummer(self, subadres, huisnummer):
-        '''
+        """
         List all `adresposities` for a subadres and a :class:`Huisnummer`.
 
         :param subadres: A string representing a certain subadres.
         :param huisnummer: The :class:`Huisnummer` for which the \
             `adresposities` are wanted. OR A huisnummer id.
         :rtype: A :class:`list` of :class:`Adrespositie`
-        '''
+        """
         try:
             hid = huisnummer.id
         except AttributeError:
             hid = huisnummer
+
         def creator():
             res = crab_gateway_request(
-                self.client, 'ListAdrespositiesBySubadres', subadres, hid
+                self.client, "ListAdrespositiesBySubadres", subadres, hid
             )
             try:
-                return [Adrespositie(
-                    r.AdrespositieId,
-                    r.HerkomstAdrespositie
-                )for r in res.AdrespositieItem]
+                return [
+                    Adrespositie(r.AdrespositieId, r.HerkomstAdrespositie)
+                    for r in res.AdrespositieItem
+                ]
             except AttributeError:
                 return []
-        if self.caches['short'].is_configured:
-            key = 'ListAdrespositiesBySubadres#%s%s' % (subadres, hid)
-            adresposities = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = f"ListAdrespositiesBySubadres#{subadres}{hid}"
+            adresposities = self.caches["short"].get_or_create(key, creator)
         else:
             adresposities = creator()
         for a in adresposities:
             a.set_gateway(self)
         return adresposities
 
     def get_adrespositie_by_id(self, id):
-        '''
+        """
         Retrieve a `Adrespositie` by the Id.
 
         :param integer id: the Id of the `Adrespositie`
         :rtype: :class:`Adrespositie`
-        '''
+        """
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetAdrespositieByAdrespositieId', id
-            )
-            if res == None:
+            res = crab_gateway_request(self.client, "GetAdrespositieByAdrespositieId", id)
+            if res is None:
                 raise GatewayResourceNotFoundException()
             return Adrespositie(
                 res.AdrespositieId,
                 res.HerkomstAdrespositie,
                 res.Geometrie,
                 res.AardAdres,
                 Metadata(
                     res.BeginDatum,
                     res.BeginTijd,
                     self.get_bewerking(res.BeginBewerking),
-                    self.get_organisatie(res.BeginOrganisatie)
-                )
+                    self.get_organisatie(res.BeginOrganisatie),
+                ),
             )
-        if self.caches['short'].is_configured:
-            key = 'GetAdrespositieByAdrespositieId#%s' % (id)
-            adrespositie = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetAdrespositieByAdrespositieId#%s" % (id)
+            adrespositie = self.caches["short"].get_or_create(key, creator)
         else:
             adrespositie = creator()
         adrespositie.set_gateway(self)
         return adrespositie
 
     def get_postadres_by_huisnummer(self, huisnummer):
-        '''
+        """
         Get the `postadres` for a :class:`Huisnummer`.
 
         :param huisnummer: The :class:`Huisnummer` for which the \
             `postadres` is wanted. OR A huisnummer id.
         :rtype: A :class:`str`.
-        '''
+        """
         try:
             id = huisnummer.id
         except AttributeError:
             id = huisnummer
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetPostadresByHuisnummerId', id
-            )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            res = crab_gateway_request(self.client, "GetPostadresByHuisnummerId", id)
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return res.Postadres
-        if self.caches['short'].is_configured:
-            key = 'GetPostadresByHuisnummerId#%s' % (id)
-            postadres = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetPostadresByHuisnummerId#%s" % (id)
+            postadres = self.caches["short"].get_or_create(key, creator)
         else:
             postadres = creator()
         return postadres
 
     def get_postadres_by_subadres(self, subadres):
-        '''
+        """
         Get the `postadres` for a :class:`Subadres`.
 
         :param subadres: The :class:`Subadres` for which the \
             `postadres` is wanted. OR A subadres id.
         :rtype: A :class:`str`.
-        '''
+        """
         try:
             id = subadres.id
         except AttributeError:
             id = subadres
+
         def creator():
-            res = crab_gateway_request(
-                self.client, 'GetPostadresBySubadresId', id
-            )
-            if res == None:
-                 raise GatewayResourceNotFoundException()
+            res = crab_gateway_request(self.client, "GetPostadresBySubadresId", id)
+            if res is None:
+                raise GatewayResourceNotFoundException()
             return res.Postadres
-        if self.caches['short'].is_configured:
-            key = 'GetPostadresBySubadresId#%s' % (id)
-            postadres = self.caches['short'].get_or_create(key, creator)
+
+        if self.caches["short"].is_configured:
+            key = "GetPostadresBySubadresId#%s" % (id)
+            postadres = self.caches["short"].get_or_create(key, creator)
         else:
             postadres = creator()
         return postadres
 
 
-class GatewayObject(object):
-    '''
+class GatewayObject:
+    """
     Abstract class for objects that are able to use a
     :class:`crabpy.Gateway.CrabGateway` to find further information.
-    '''
+    """
 
     gateway = None
-    '''
+    """
     The :class:`crabpy.gateway.crab.CrabGateway` to use when making
     further calls to the CRAB service.
-    '''
+    """
 
     def __init__(self, **kwargs):
-        if 'gateway' in kwargs:
-            self.set_gateway(kwargs['gateway'])
+        if "gateway" in kwargs:
+            self.set_gateway(kwargs["gateway"])
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.crab.CrabGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CrabGateway.
-        '''
+        """
         self.gateway = None
 
     def check_gateway(self):
-        '''
+        """
         Check to see if a gateway was set on this object.
-        '''
+        """
         if not self.gateway:
             raise RuntimeError("There's no Gateway I can use")
 
-    if six.PY2:
-        def __str__(self):
-            return self.__unicode__().encode('utf-8')
-    else:
-        def __str__(self):
-            return self.__unicode__()
+    def __str__(self):
+        return self.__unicode__()
 
 
 def check_lazy_load_gewest(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Gewest`.
-    '''
+    """
+
     def wrapper(self):
         gewest = self
-        attribute = 'namen' if f.__name__ == 'naam' else f.__name__
-        if (getattr(gewest, '_%s' % attribute, None) is None):
-            log.debug('Lazy loading Gewest %d', gewest.id)
+        attribute = "namen" if f.__name__ == "naam" else f.__name__
+        if getattr(gewest, "_%s" % attribute, None) is None:
+            log.debug("Lazy loading Gewest %d", gewest.id)
             gewest.check_gateway()
             g = gewest.gateway.get_gewest_by_id(gewest.id)
             gewest._namen = g._namen
             gewest._centroid = g._centroid
             gewest._bounding_box = g._bounding_box
         return f(self)
+
     return wrapper
 
 
 class Gewest(GatewayObject):
-    '''
+    """
     A large administrative unit in Belgium.
 
     Belgium consists of 3 `gewesten`. Together they form the entire territory
     of the country.
-    '''
-    def __init__(
-        self,
-        id,
-        namen=None,
-        centroid=None,
-        bounding_box=None,
-        **kwargs
-    ):
+    """
+
+    def __init__(self, id, namen=None, centroid=None, bounding_box=None, **kwargs):
         self.id = int(id)
         self._namen = namen
         self._centroid = centroid
         self._bounding_box = bounding_box
-        super(Gewest, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     @check_lazy_load_gewest
     def naam(self):
-        return self._namen['nl']
+        return self._namen["nl"]
 
     @property
     @check_lazy_load_gewest
     def centroid(self):
         return self._centroid
 
     @property
@@ -1641,117 +1588,128 @@
 
     @property
     def gemeenten(self):
         return self.gateway.list_gemeenten(self.id)
 
     def __unicode__(self):
         if self._namen is not None:
-            return "%s (%s)" % (self.naam, self.id)
+            return f"{self.naam} ({self.id})"
         else:
             return "Gewest %s" % (self.id)
 
     def __repr__(self):
         return "Gewest(%s)" % (self.id)
 
 
 class Provincie(GatewayObject):
-    '''
+    """
     The largest administrative unit within a :class:`Gewest`.
 
     .. versionadded:: 0.4.0
-    '''
-    def __init__(
-        self, niscode, naam, gewest, **kwargs
-    ):
+    """
+
+    def __init__(self, niscode, naam, gewest, **kwargs):
         self.id = self.niscode = int(niscode)
         self.naam = naam
         self.gewest = gewest
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.crab.CrabGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
         self.gewest.gateway = gateway
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CrabGateway.
-        '''
+        """
         self.gateway = None
         self.gewest.clear_gateway()
 
     @property
     def gemeenten(self):
         self.check_gateway()
         return self.gateway.list_gemeenten_by_provincie(self.niscode)
 
     def __unicode__(self):
-        return "%s (%s)" % (self.naam, self.niscode)
+        return f"{self.naam} ({self.niscode})"
 
     def __repr__(self):
-        return "Provincie(%s, '%s', Gewest(%s))" % (self.niscode, self.naam, self.gewest.id)
+        return f"Provincie({self.niscode}, '{self.naam}', Gewest({self.gewest.id}))"
 
 
 def check_lazy_load_gemeente(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Gemeente`.
-    '''
+    """
+
     def wrapper(*args):
         gemeente = args[0]
         if (
-            gemeente._centroid is None or gemeente._bounding_box is None
-            or gemeente._taal_id is None or gemeente._metadata is None
+            gemeente._centroid is None
+            or gemeente._bounding_box is None
+            or gemeente._taal_id is None
+            or gemeente._metadata is None
         ):
-            log.debug('Lazy loading Gemeente %d', gemeente.id)
+            log.debug("Lazy loading Gemeente %d", gemeente.id)
             gemeente.check_gateway()
             g = gemeente.gateway.get_gemeente_by_id(gemeente.id)
             gemeente._taal_id = g._taal_id
             gemeente._centroid = g._centroid
             gemeente._bounding_box = g._bounding_box
             gemeente._metadata = g._metadata
         return f(*args)
+
     return wrapper
 
 
 class Gemeente(GatewayObject):
-    '''
+    """
     The smallest administrative unit in Belgium.
-    '''
+    """
+
     def __init__(
-            self, id, naam, niscode, gewest,
-            taal=None, centroid=None,
-            bounding_box=None, metadata=None, **kwargs
+        self,
+        id,
+        naam,
+        niscode,
+        gewest,
+        taal=None,
+        centroid=None,
+        bounding_box=None,
+        metadata=None,
+        **kwargs,
     ):
         self.id = int(id)
         self.naam = naam
         self.niscode = niscode
         self.gewest = gewest
         try:
             self._taal_id = taal.id
             self._taal = taal
         except AttributeError:
             self._taal_id = taal
             self._taal = None
         self._centroid = centroid
         self._bounding_box = bounding_box
         self._metadata = metadata
-        super(Gemeente, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.crab.CrabGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
         self.gewest.set_gateway(gateway)
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CrabGateway.
-        '''
+        """
         self.gateway = None
         self.gewest.clear_gateway()
 
     @property
     @check_lazy_load_gemeente
     def taal(self):
         if self._taal is None:
@@ -1791,242 +1749,261 @@
         self.check_gateway()
         provincies = self.gateway.list_provincies(self.gewest)
         for p in provincies:
             if math.floor(self.niscode / 10000) == math.floor(p.niscode / 10000):
                 return p
 
     def __unicode__(self):
-        return "%s (%s)" % (self.naam, self.id)
+        return f"{self.naam} ({self.id})"
 
     def __repr__(self):
-        return "Gemeente(%s, '%s', %s)" % (self.id, self.naam, self.niscode)
+        return f"Gemeente({self.id}, '{self.naam}', {self.niscode})"
 
 
 class Deelgemeente(GatewayObject):
-    '''
+    """
     A subdivision of a :class:`Gemeente`.
 
     .. versionadded:: 0.7.0
-    '''
-    def __init__(
-        self, id, naam, gemeente_niscode, **kwargs
-    ):
+    """
+
+    def __init__(self, id, naam, gemeente_niscode, **kwargs):
         self.id = id
         self.naam = naam
         self.gemeente_niscode = gemeente_niscode
 
     def set_gateway(self, gateway):
-        '''
+        """
         :param crabpy.gateway.crab.CrabGateway gateway: Gateway to use.
-        '''
+        """
         self.gateway = gateway
 
     def clear_gateway(self):
-        '''
+        """
         Clear the currently set CrabGateway.
-        '''
+        """
         self.gateway = None
 
     @property
     def gemeente(self):
         return self.gateway.get_gemeente_by_niscode(self.gemeente_niscode)
 
     def __unicode__(self):
-        return "%s (%s)" % (self.naam, self.id)
+        return f"{self.naam} ({self.id})"
 
     def __repr__(self):
-        return "Deelgemeente('%s', '%s', %s)" % (self.id, self.naam, self.gemeente_niscode)
+        return f"Deelgemeente('{self.id}', '{self.naam}', {self.gemeente_niscode})"
 
 
 class Codelijst(GatewayObject):
-    def __init__(
-            self, id, naam, definitie, **kwargs
-    ):
+    def __init__(self, id, naam, definitie, **kwargs):
         self.id = id
         self.naam = naam
         self.definitie = definitie
-        super(Codelijst, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __unicode__(self):
         return self.naam
 
 
 class Taal(Codelijst):
-    '''
+    """
     A language.
-    '''
+    """
+
     def __repr__(self):
-        return "Taal('%s', '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Taal('{self.id}', '{self.naam}', '{self.definitie}')"
 
 
 class Bewerking(Codelijst):
-    '''
+    """
     An edit.
-    '''
+    """
+
     def __repr__(self):
-        return "Bewerking(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Bewerking({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Organisatie(Codelijst):
-    '''
+    """
     An organisation that played a role in the genessis of an object.
-    '''
+    """
+
     def __repr__(self):
-        return "Organisatie(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Organisatie({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Aardsubadres(Codelijst):
-    '''
+    """
     The nature of a subaddress.
-    '''
+    """
+
     def __repr__(self):
-        return "Aardsubadres(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Aardsubadres({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Aardadres(Codelijst):
-    '''
+    """
     The nature of an address.
-    '''
+    """
+
     def __repr__(self):
-        return "Aardadres(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Aardadres({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Aardgebouw(Codelijst):
-    '''
+    """
     The nature of a building.
-    '''
+    """
+
     def __repr__(self):
-        return "Aardgebouw(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Aardgebouw({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Aardwegobject(Codelijst):
-    '''
+    """
     The nature of a `wegobject`.
-    '''
+    """
+
     def __repr__(self):
-        return "Aardwegobject(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Aardwegobject({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Aardterreinobject(Codelijst):
-    '''
+    """
     The nature of a `terreinobject`.
-    '''
+    """
+
     def __repr__(self):
-        return "Aardterreinobject(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Aardterreinobject({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Statushuisnummer(Codelijst):
-    '''
+    """
     The current state of a `huisnummer`.
-    '''
+    """
+
     def __repr__(self):
-        return "Statushuisnummer(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Statushuisnummer({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Statussubadres(Codelijst):
-    '''
+    """
     The current state of a `subadres`.
-    '''
+    """
+
     def __repr__(self):
-        return "Statussubadres(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Statussubadres({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Statusstraatnaam(Codelijst):
-    '''
+    """
     The current state of a `straatnaam`.
-    '''
+    """
+
     def __repr__(self):
-        return "Statusstraatnaam(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Statusstraatnaam({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Statuswegsegment(Codelijst):
-    '''
+    """
     The current state of a `wegsegment`.
-    '''
+    """
+
     def __repr__(self):
-        return "Statuswegsegment(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Statuswegsegment({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Geometriemethodewegsegment(Codelijst):
-    '''
+    """
     The geometry method of a :class:`Wegsegment`.
-    '''
+    """
+
     def __repr__(self):
-        return "Geometriemethodewegsegment(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Geometriemethodewegsegment({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Statusgebouw(Codelijst):
-    '''
+    """
     The current state of a :class:`Gebouw`.
-    '''
+    """
+
     def __repr__(self):
-        return "Statusgebouw(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Statusgebouw({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Geometriemethodegebouw(Codelijst):
-    '''
+    """
     The geometry method of a :class:`Gebouw`.
-    '''
+    """
+
     def __repr__(self):
-        return "Geometriemethodegebouw(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Geometriemethodegebouw({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 class Herkomstadrespositie(Codelijst):
-    '''
+    """
     The origin of an Adressposition.
-    '''
+    """
+
     def __repr__(self):
-        return "Herkomstadrespositie(%s, '%s', '%s')" % (self.id, self.naam, self.definitie)
+        return f"Herkomstadrespositie({self.id}, '{self.naam}', '{self.definitie}')"
 
 
 def check_lazy_load_straat(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Straat`.
-    '''
+    """
+
     def wrapper(*args):
         straat = args[0]
-        if (
-            straat._namen is None or straat._metadata is None
-        ):
-            log.debug('Lazy loading Straat %d', straat.id)
+        if straat._metadata is None:
+            log.debug("Lazy loading Straat %d", straat.id)
             straat.check_gateway()
             s = straat.gateway.get_straat_by_id(straat.id)
-            straat._namen = s._namen
             straat._metadata = s._metadata
         return f(*args)
+
     return wrapper
 
 
 class Straat(GatewayObject):
-    '''
+    """
     A street.
 
     A street object is always located in one and exactly one :class:`Gemeente`.
-    '''
+    """
+
     def __init__(
-            self, id, label, gemeente_id, status,
-            straatnaam=None, taalcode=None,
-            straatnaam2=None, taalcode2=None,
-            metadata=None, **kwargs
+        self,
+        id,
+        label,
+        gemeente_id,
+        status,
+        straatnaam,
+        taalcode,
+        straatnaam2,
+        taalcode2,
+        metadata=None,
+        **kwargs,
     ):
         self.id = id
         self.label = label
         try:
             self.status_id = status.id
             self._status = status
-        except:
+        except Exception:
             self.status_id = status
             self._status = None
         self._namen = ((straatnaam, taalcode), (straatnaam2, taalcode2))
         self.gemeente_id = gemeente_id
         self._metadata = metadata
-        super(Straat, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
-    @check_lazy_load_straat
     def namen(self):
         return self._namen
 
     @property
     def gemeente(self):
         return self.gateway.get_gemeente_by_id(self.gemeente_id)
 
@@ -2069,66 +2046,64 @@
         weg = [x.geometrie for x in self.wegsegmenten]
         if weg == []:
             return None
         x = []
         y = []
         for a in weg:
             a = a.replace("LINESTRING (", "").replace(")", "")
-            list = a.split(',')
+            list = a.split(",")
             for z in list:
                 temp = z.split()
-                x.append(temp[0])
-                y.append(temp[1])
+                x.append(float(temp[0]))
+                y.append(float(temp[1]))
         return [min(x), min(y), max(x), max(y)]
 
     def __unicode__(self):
-        return "%s (%s)" % (self.label, self.id)
+        return f"{self.label} ({self.id})"
 
     def __repr__(self):
-        return "Straat(%s, '%s', %s, %s)" % (self.id, self.label, self.gemeente_id, self.status_id)
+        return f"Straat({self.id}, '{self.label}', {self.gemeente_id}, {self.status_id})"
 
 
 def check_lazy_load_huisnummer(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Huisnummer`.
-    '''
+    """
+
     def wrapper(*args):
         huisnummer = args[0]
-        if (
-            huisnummer._metadata is None
-        ):
-            log.debug('Lazy loading Huisnummer %d', huisnummer.id)
+        if huisnummer._metadata is None:
+            log.debug("Lazy loading Huisnummer %d", huisnummer.id)
             huisnummer.check_gateway()
             h = huisnummer.gateway.get_huisnummer_by_id(huisnummer.id)
             huisnummer._metadata = h._metadata
         return f(*args)
+
     return wrapper
 
 
 class Huisnummer(GatewayObject):
-    '''
+    """
     A house number.
 
     This is mainly a combination of a street and a house number.
-    '''
-    def __init__(
-            self, id, status, huisnummer, straat_id,
-            metadata=None, **kwargs
-    ):
+    """
+
+    def __init__(self, id, status, huisnummer, straat_id, metadata=None, **kwargs):
         self.id = int(id)
         try:
             self.status_id = status.id
             self._status = status
         except AttributeError:
             self.status_id = status
             self._status = None
         self.huisnummer = huisnummer
         self.straat_id = straat_id
         self._metadata = metadata
-        super(Huisnummer, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def straat(self):
         self.check_gateway()
         return self.gateway.get_straat_by_id(self.straat_id)
 
     @property
@@ -2184,74 +2159,76 @@
 
     @property
     def adresposities(self):
         self.check_gateway()
         return self.gateway.list_adresposities_by_huisnummer(self.id)
 
     def __unicode__(self):
-        return "%s (%s)" % (self.huisnummer, self.id)
+        return f"{self.huisnummer} ({self.id})"
 
     def __repr__(self):
-        return "Huisnummer(%s, %s, '%s', %s)" % (self.id, self.status_id, self.huisnummer, self.straat_id)
+        return f"Huisnummer({self.id}, {self.status_id}, '{self.huisnummer}', {self.straat_id})"
 
 
 class Postkanton(GatewayObject):
-    '''
+    """
     A postal code.
 
     Eg. postal code `9000` for the city of Ghent.
-    '''
+    """
+
     def __init__(self, id, **kwargs):
         self.id = int(id)
-        super(Postkanton, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __unicode__(self):
         return "Postkanton %s" % (self.id)
 
     def __repr__(self):
         return "Postkanton(%s)" % (self.id)
 
 
 def check_lazy_load_wegobject(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Wegobject`.
-    '''
+    """
+
     def wrapper(*args):
         wegobject = args[0]
         if (
-            wegobject._centroid is None or
-            wegobject._bounding_box is None or
-            wegobject._metadata is None
+            wegobject._centroid is None
+            or wegobject._bounding_box is None
+            or wegobject._metadata is None
         ):
-            log.debug('Lazy loading Wegobject %d', wegobject.id)
+            log.debug("Lazy loading Wegobject %d", wegobject.id)
             wegobject.check_gateway()
             w = wegobject.gateway.get_wegobject_by_id(wegobject.id)
             wegobject._centroid = w._centroid
             wegobject._bounding_box = w._bounding_box
             wegobject._metadata = w._metadata
         return f(*args)
+
     return wrapper
 
 
 class Wegobject(GatewayObject):
     def __init__(
-        self, id, aard, centroid=None,
-        bounding_box=None, metadata=None, **kwargs
+        self, id, aard, centroid=None, bounding_box=None, metadata=None, **kwargs
     ):
         self.id = id
         try:
             self.aard_id = aard.id
             self._aard = aard
         except AttributeError:
             self.aard_id = aard
             self._aard = None
         self._centroid = centroid
         self._bounding_box = bounding_box
         self._metadata = metadata
-        super(Wegobject, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def aard(self):
         if self._aard is None:
             res = self.gateway.list_aardwegobjecten()
             for aard in res:
                 if int(aard.id) == int(self.aard_id):
@@ -2277,55 +2254,54 @@
         return "Wegobject %s" % (self.id)
 
     def __repr__(self):
         return "Wegobject(%s)" % (self.id)
 
 
 def check_lazy_load_wegsegment(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Wegsegment`.
-    '''
+    """
+
     def wrapper(*args):
         wegsegment = args[0]
         if (
-            wegsegment._methode_id is None or
-            wegsegment._geometrie is None or
-            wegsegment._metadata is None
+            wegsegment._methode_id is None
+            or wegsegment._geometrie is None
+            or wegsegment._metadata is None
         ):
-            log.debug('Lazy loading Wegsegment %d', wegsegment.id)
+            log.debug("Lazy loading Wegsegment %d", wegsegment.id)
             wegsegment.check_gateway()
             w = wegsegment.gateway.get_wegsegment_by_id(wegsegment.id)
             wegsegment._methode_id = w._methode_id
             wegsegment._geometrie = w._geometrie
             wegsegment._metadata = w._metadata
         return f(*args)
+
     return wrapper
 
 
 class Wegsegment(GatewayObject):
-    def __init__(
-        self, id, status, methode=None,
-        geometrie=None, metadata=None, **kwargs
-    ):
+    def __init__(self, id, status, methode=None, geometrie=None, metadata=None, **kwargs):
         self.id = id
         try:
             self.status_id = status.id
             self._status = status
-        except:
+        except Exception:
             self.status_id = status
             self._status = None
         try:
             self._methode_id = methode.id
             self._methode = methode
-        except:
+        except Exception:
             self._methode_id = methode
             self._methode = None
         self._geometrie = geometrie
         self._metadata = metadata
-        super(Wegsegment, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def status(self):
         if self._status is None:
             res = self.gateway.list_statuswegsegmenten()
             for status in res:
                 if int(status.id) == int(self.status_id):
@@ -2356,58 +2332,60 @@
         return "Wegsegment %s" % (self.id)
 
     def __repr__(self):
         return "Wegsegment(%s)" % (self.id)
 
 
 def check_lazy_load_terreinobject(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Terreinobject`.
-    '''
+    """
+
     def wrapper(*args):
         terreinobject = args[0]
         if (
-            terreinobject._centroid is None or
-            terreinobject._bounding_box is None or
-            terreinobject._metadata is None
+            terreinobject._centroid is None
+            or terreinobject._bounding_box is None
+            or terreinobject._metadata is None
         ):
-            log.debug('Lazy loading Terreinobject %s', terreinobject.id)
+            log.debug("Lazy loading Terreinobject %s", terreinobject.id)
             terreinobject.check_gateway()
             t = terreinobject.gateway.get_terreinobject_by_id(terreinobject.id)
             terreinobject._centroid = t._centroid
             terreinobject._bounding_box = t._bounding_box
             terreinobject._metadata = t._metadata
         return f(*args)
+
     return wrapper
 
 
 class Terreinobject(GatewayObject):
-    '''
+    """
     A cadastral parcel.
 
     A :class:`Terreinobject` is somewhat different from a :class:`Perceel`
     in the source of the data and the information provided. eg. A
     `terreinobject` has a `centroid` and a `bounding box`, while a `perceel`
     also has the centroid, but not the `bounding box`.
-    '''
+    """
+
     def __init__(
-        self, id, aard, centroid=None,
-        bounding_box=None, metadata=None, **kwargs
+        self, id, aard, centroid=None, bounding_box=None, metadata=None, **kwargs
     ):
         self.id = id
         try:
             self.aard_id = aard.id
             self._aard = aard
         except AttributeError:
             self.aard_id = aard
             self._aard = None
         self._centroid = centroid
         self._metadata = metadata
         self._bounding_box = bounding_box
-        super(Terreinobject, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def aard(self):
         if self._aard is None:
             res = self.gateway.list_aardterreinobjecten()
             for aard in res:
                 if int(aard.id) == int(self.aard_id):
@@ -2433,136 +2411,140 @@
         return "Terreinobject %s" % (self.id)
 
     def __repr__(self):
         return "Terreinobject(%s)" % (self.id)
 
 
 def check_lazy_load_perceel(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Perceel`.
-    '''
+    """
+
     def wrapper(*args):
         perceel = args[0]
         if perceel._centroid is None or perceel._metadata is None:
-            log.debug('Lazy loading Perceel %s', perceel.id)
+            log.debug("Lazy loading Perceel %s", perceel.id)
             perceel.check_gateway()
             p = perceel.gateway.get_perceel_by_id(perceel.id)
             perceel._centroid = p._centroid
             perceel._metadata = p._metadata
         return f(*args)
+
     return wrapper
 
 
 class Perceel(GatewayObject):
-    '''
+    """
     A cadastral Parcel.
 
     A :class:`Terreinobject` is somewhat different from a :class:`Perceel`
     in the source of the data and the information provided. eg. A
     `terreinobject` has a `centroid` and a `bounding box`, while a `perceel`
     also has the centroid, but not the `bounding box`.
-    '''
-    def __init__(
-        self, id, centroid=None, metadata=None, **kwargs
-    ):
+    """
+
+    def __init__(self, id, centroid=None, metadata=None, **kwargs):
         self.id = id
         self._centroid = centroid
         self._metadata = metadata
-        super(Perceel, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     @check_lazy_load_perceel
     def centroid(self):
         return self._centroid
 
     @property
     @check_lazy_load_perceel
     def metadata(self):
         return self._metadata
 
     @property
     def huisnummers(self):
-        '''
+        """
         Returns the huisnummers on this Perceel.
 
         Some of the huisnummers might no longer be active.
 
         :rtype: list
-        '''
+        """
         self.check_gateway()
         return self.gateway.list_huisnummers_by_perceel(self.id)
 
     @property
     def postadressen(self):
-        '''
+        """
         Returns the postadressen for this Perceel.
 
         Will only take the huisnummers with status `inGebruik` into account.
 
-        :rtype: list 
-        '''
-        return [h.postadres for h in self.huisnummers if h.status.id == '3']
+        :rtype: list
+        """
+        return [h.postadres for h in self.huisnummers if h.status.id == "3"]
 
     def __unicode__(self):
         return "Perceel %s" % (self.id)
 
     def __repr__(self):
         return "Perceel(%s)" % (self.id)
 
 
 def check_lazy_load_gebouw(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Gebouw`.
-    '''
+    """
+
     def wrapper(*args):
         gebouw = args[0]
         if (
-            gebouw._methode_id is None or gebouw._geometrie is None or
-            gebouw._metadata is None
+            gebouw._methode_id is None
+            or gebouw._geometrie is None
+            or gebouw._metadata is None
         ):
-            log.debug('Lazy loading Gebouw %d', gebouw.id)
+            log.debug("Lazy loading Gebouw %d", gebouw.id)
             gebouw.check_gateway()
             g = gebouw.gateway.get_gebouw_by_id(gebouw.id)
             gebouw._methode_id = g._methode_id
             gebouw._geometrie = g._geometrie
             gebouw._metadata = g._metadata
         return f(*args)
+
     return wrapper
 
 
 class Gebouw(GatewayObject):
-    '''
+    """
     A building.
-    '''
+    """
+
     def __init__(
-        self, id, aard, status,
-        methode=None, geometrie=None, metadata=None, **kwargs
+        self, id, aard, status, methode=None, geometrie=None, metadata=None, **kwargs
     ):
         self.id = int(id)
         try:
             self.aard_id = aard.id
             self._aard = aard
-        except:
+        except Exception:
             self.aard_id = aard
             self._aard = None
         try:
             self.status_id = status.id
             self._status = status
-        except:
+        except Exception:
             self.status_id = status
             self._status = None
         try:
             self._methode_id = methode.id
             self._methode = methode
-        except:
+        except Exception:
             self._methode_id = methode
             self._methode = None
         self._geometrie = geometrie
         self._metadata = metadata
-        super(Gebouw, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def aard(self):
         if self._aard is None:
             self.check_gateway()
             res = self.gateway.list_aardgebouwen()
             for aard in res:
@@ -2604,43 +2586,45 @@
         return "Gebouw %s" % (self.id)
 
     def __repr__(self):
         return "Gebouw(%s)" % (self.id)
 
 
 def check_lazy_load_subadres(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Subadres`.
-    '''
+    """
+
     def wrapper(*args):
         subadres = args[0]
         if (
-            subadres._metadata is None or
-            subadres.aard_id is None or
-            subadres.huisnummer_id is None
+            subadres._metadata is None
+            or subadres.aard_id is None
+            or subadres.huisnummer_id is None
         ):
-            log.debug('Lazy loading Subadres %d', subadres.id)
+            log.debug("Lazy loading Subadres %d", subadres.id)
             subadres.check_gateway()
             s = subadres.gateway.get_subadres_by_id(subadres.id)
             subadres._metadata = s._metadata
             subadres.aard_id = s.aard_id
             subadres.huisnummer_id = s.huisnummer_id
         return f(*args)
+
     return wrapper
 
 
 class Subadres(GatewayObject):
-    '''
+    """
     An address within a certain :class:`Huisnummer`.
 
     These can eg. be postboxes within an appartment complex.
-    '''
+    """
+
     def __init__(
-            self, id, subadres, status, huisnummer_id=None, aard=None,
-            metadata=None, **kwargs
+        self, id, subadres, status, huisnummer_id=None, aard=None, metadata=None, **kwargs
     ):
         self.id = int(id)
         self.subadres = subadres
         try:
             self.status_id = status.id
             self._status = status
         except AttributeError:
@@ -2650,15 +2634,15 @@
         try:
             self.aard_id = aard.id
             self._aard = aard
         except AttributeError:
             self.aard_id = aard
             self._aard = None
         self._metadata = metadata
-        super(Subadres, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def huisnummer(self):
         self.check_gateway()
         return self.gateway.get_huisnummer_by_id(self.huisnummer_id)
 
     @property
@@ -2692,56 +2676,56 @@
 
     @property
     def adresposities(self):
         self.check_gateway()
         return self.gateway.list_adresposities_by_subadres(self.id)
 
     def __unicode__(self):
-        return "%s (%s)" % (self.subadres, self.id)
+        return f"{self.subadres} ({self.id})"
 
     def __repr__(self):
-        return "Subadres(%s, %s, '%s', %s)" % (self.id, self.status_id, self.subadres, self.huisnummer_id)
+        return f"Subadres({self.id}, {self.status_id}, '{self.subadres}', {self.huisnummer_id})"
 
 
 def check_lazy_load_adrespositie(f):
-    '''
+    """
     Decorator function to lazy load a :class:`Adrespositie`.
-    '''
+    """
+
     def wrapper(*args):
         adrespositie = args[0]
         if (
-            adrespositie._geometrie is None or
-            adrespositie._aard is None or
-            adrespositie._metadata is None
+            adrespositie._geometrie is None
+            or adrespositie._aard is None
+            or adrespositie._metadata is None
         ):
-            log.debug('Lazy loading Adrespositie %d', adrespositie.id)
+            log.debug("Lazy loading Adrespositie %d", adrespositie.id)
             adrespositie.check_gateway()
             a = adrespositie.gateway.get_adrespositie_by_id(adrespositie.id)
             adrespositie._geometrie = a._geometrie
             adrespositie.aard_id = a.aard_id
             adrespositie._metadata = a._metadata
         return f(*args)
+
     return wrapper
 
 
 class Adrespositie(GatewayObject):
-    '''
+    """
     The position of an `Adres`.
 
     This can be used for the position of both :class:`Huisnummer` and
     :class:`Subadres`.
 
     A `Huisnummer` or `Subadres`, can have more than one `Adrespositie`, each
     offering a different interpretation of the position of the `Adres`. See
     the `herkomst` and `aard` of each `Adrespositie` to know which one to pick.
-    '''
-    def __init__(
-        self, id, herkomst, geometrie=None, aard=None,
-        metadata=None, **kwargs
-    ):
+    """
+
+    def __init__(self, id, herkomst, geometrie=None, aard=None, metadata=None, **kwargs):
         self.id = id
         try:
             self.herkomst_id = herkomst.id
             self._herkomst = herkomst
         except AttributeError:
             self.herkomst_id = herkomst
             self._herkomst = None
@@ -2749,15 +2733,15 @@
         try:
             self.aard_id = aard.id
             self._aard = aard
         except AttributeError:
             self.aard_id = aard
             self._aard = None
         self._metadata = metadata
-        super(Adrespositie, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def herkomst(self):
         if self._herkomst is None:
             self.check_gateway()
             res = self.gateway.list_herkomstadresposities()
             for herkomst in res:
@@ -2785,28 +2769,27 @@
                     self._aard = aard
         return self._aard
 
     def __unicode__(self):
         return "Adrespositie %s" % (self.id)
 
     def __repr__(self):
-        return "Adrespositie(%s, %s)" % (self.id, self.herkomst_id)
+        return f"Adrespositie({self.id}, {self.herkomst_id})"
 
 
 class Metadata(GatewayObject):
-    '''
+    """
     Metadata about a `straat`, `huisnummer`, ...
 
     Some of the metadata available is the datum the object was created, the
     organisation that created it and the type of creation.
-    '''
+    """
+
     def __init__(
-        self, begin_datum, begin_tijd,
-        begin_bewerking, begin_organisatie,
-        **kwargs
+        self, begin_datum, begin_tijd, begin_bewerking, begin_organisatie, **kwargs
     ):
         self.begin_datum = str(begin_datum)
         self.begin_tijd = str(begin_tijd)
         try:
             self._begin_bewerking_id = begin_bewerking.id
             self._begin_bewerking = begin_bewerking
         except AttributeError:
@@ -2814,15 +2797,15 @@
             self._begin_bewerking = None
         try:
             self._begin_organisatie_id = begin_organisatie.id
             self._begin_organisatie = begin_organisatie
         except AttributeError:
             self._begin_organisatie_id = begin_organisatie
             self._begin_organisatie = None
-        super(Metadata, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def begin_bewerking(self):
         if self._begin_bewerking is None:
             self.check_gateway()
             bewerkingen = self.gateway.list_bewerkingen()
             for bewerking in bewerkingen:
```

