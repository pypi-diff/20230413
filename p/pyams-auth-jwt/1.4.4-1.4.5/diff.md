# Comparing `tmp/pyams_auth_jwt-1.4.4.tar.gz` & `tmp/pyams_auth_jwt-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_auth_jwt-1.4.4.tar", last modified: Tue Dec 27 01:21:58 2022, max compression
+gzip compressed data, was "dist/pyams_auth_jwt-1.4.5.tar", last modified: Thu Apr 13 10:27:19 2023, max compression
```

## Comparing `pyams_auth_jwt-1.4.4.tar` & `pyams_auth_jwt-1.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2875 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1269 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2552 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/
--rw-rw-rw-   0 root         (0) root         (0)      900 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/api/
--rw-rw-rw-   0 root         (0) root         (0)    11978 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    23102 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2783 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/include.py
--rw-rw-rw-   0 root         (0) root         (0)    10397 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8274 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo
--rw-rw-rw-   0 root         (0) root         (0)    10829 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po
--rw-rw-rw-   0 root         (0) root         (0)     6737 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot
--rw-rw-rw-   0 root         (0) root         (0)    11495 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6942 2022-12-27 01:21:38.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/zmi/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2875 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      950 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      236 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-12-27 01:21:58.000000 pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1348 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2552 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/
+-rw-rw-rw-   0 root         (0) root         (0)    12397 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    22983 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    10397 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10797 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11495 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6942 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/top_level.txt
```

### Comparing `pyams_auth_jwt-1.4.4/LICENSE` & `pyams_auth_jwt-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/PKG-INFO` & `pyams_auth_jwt-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_auth_jwt
-Version: 1.4.4
+Version: 1.4.5
 Summary: PyAMS security plug-in for JWT authentication
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,18 @@
 
 You have to include this package in your Pyramid configuration to active this plug-in.
 
 
 Changelog
 =========
 
+1.4.5
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
  - added support for Python 3.11
 
 1.4.3
 -----
```

### Comparing `pyams_auth_jwt-1.4.4/docs/HISTORY.rst` & `pyams_auth_jwt-1.4.5/docs/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.4.5
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
  - added support for Python 3.11
 
 1.4.3
 -----
```

### Comparing `pyams_auth_jwt-1.4.4/docs/README.rst` & `pyams_auth_jwt-1.4.5/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/setup.py` & `pyams_auth_jwt-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.4.4'
+version = '1.4.5'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_form',
     'pyams_layer',
     'pyams_site',
     'pyams_skin',
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/__init__.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/api/__init__.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,300 +16,312 @@
 """
 
 import sys
 
 from colander import Int, MappingSchema, OneOf, SchemaNode, String, drop
 from cornice import Service
 from cornice.validators import colander_body_validator
-from pyramid.httpexceptions import HTTPAccepted, HTTPBadRequest, HTTPForbidden, \
-    HTTPNotFound, HTTPOk, HTTPServiceUnavailable, HTTPUnauthorized
+from pyramid.httpexceptions import HTTPAccepted, HTTPBadRequest, HTTPForbidden, HTTPOk, HTTPServiceUnavailable, \
+    HTTPUnauthorized
 from pyramid.security import Authenticated
 
 from pyams_auth_jwt.interfaces import ACCESS_OBJECT, IJWTProxyHandler, \
     IJWTSecurityConfiguration, REFRESH_OBJECT, REST_TOKEN_ROUTE, REST_VERIFY_ROUTE
 from pyams_auth_jwt.plugin import create_jwt_token, get_jwt_claims as get_request_claims
 from pyams_security.credential import Credentials
 from pyams_security.interfaces import ISecurityManager
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_utils.registry import query_utility
-from pyams_utils.rest import PropertiesMapping
-
+from pyams_utils.rest import BaseStatusSchema, PropertiesMapping, STATUS, http_error, rest_responses
 
 __docformat__ = 'restructuredtext'
 
-from pyams_auth_jwt import _  # pylint: disable=ungrouped-imports
-
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
-class ErrorSchema(MappingSchema):
-    """Base error schema"""
-    status = SchemaNode(String(),
-                        title=_("Response status"))
-    message = SchemaNode(String(),
-                         title=_("Error message"),
-                         missing=drop)
-
-
-class ClaimsSetterSchema(MappingSchema):
+class ClaimsInfo(MappingSchema):
     """Claims setter schema"""
     claims = SchemaNode(PropertiesMapping(),
-                        title=_("Custom claims"),
+                        description="Custom claims",
                         missing=drop)
 
 
-class LoginSchema(ClaimsSetterSchema):
+class LoginInfo(ClaimsInfo):
     """Login schema"""
     login = SchemaNode(String(),
-                       title=_("Login"))
+                       description="User login")
     password = SchemaNode(String(),
-                          title=_("Password"))
-
-
-class StatusSchema(MappingSchema):
-    """Base status response schema"""
-    status = SchemaNode(String(),
-                        title=_("Response status"),
-                        validator=OneOf(('success', 'error')))
+                          description="User password")
 
 
-class TokensSchema(StatusSchema):
-    """Tokens response schema"""
+class TokensResult(BaseStatusSchema):
+    """Tokens result schema"""
     accessToken = SchemaNode(String(),
-                             title=_("Access token"))
+                             description="Access token")
     refreshToken = SchemaNode(String(),
-                              title=_("Refresh token"))
+                              description="Refresh token")
 
 
-class ClaimsObjectSchema(MappingSchema):
-    """Claims getter schema"""
+class ClaimsObjectInfo(MappingSchema):
+    """Claims object info"""
     obj = SchemaNode(String(),
-                     title=_("Token object"),
+                     description="Token object",
                      validator=OneOf((ACCESS_OBJECT, REFRESH_OBJECT)),
                      missing=drop)
 
 
-class ClaimsSchema(ClaimsObjectSchema):
-    """Token claims schema"""
+class ClaimsElements(ClaimsObjectInfo):
+    """Token claims elements schema"""
     sub = SchemaNode(String(),
-                     title=_("Principal ID"))
+                     description="Principal ID")
     iat = SchemaNode(Int(),
-                     title=_("Token issue timestamp, in seconds"))
+                     description="Token issue timestamp, in seconds")
     exp = SchemaNode(Int(),
-                     title=_("Token expiration timestamp, in seconds"))
+                     description="Token expiration timestamp, in seconds")
 
 
-jwt_responses = {
-    HTTPOk.code: TokensSchema(description=_("Tokens properties")),
-    HTTPAccepted.code: StatusSchema(description=_("Token accepted")),
-    HTTPNotFound.code: ErrorSchema(description=_("Page not found")),
-    HTTPUnauthorized.code: ErrorSchema(description=_("Unauthorized")),
-    HTTPForbidden.code: ErrorSchema(description=_("Forbidden access")),
-    HTTPBadRequest.code: ErrorSchema(description=_("Missing arguments")),
-    HTTPServiceUnavailable.code: ErrorSchema(description=_("Service unavailable"))
-}
-
-if TEST_MODE:
-    service_params = {}
-else:
-    service_params = {
-        'response_schemas': jwt_responses
-    }
-
+#
+# JWT token management service
+#
 
 jwt_token = Service(name=REST_TOKEN_ROUTE,
                     pyramid_route=REST_TOKEN_ROUTE,
                     description="JWT tokens management")
 
 
-@jwt_token.options(validators=(check_cors_origin, set_cors_headers),
-                   **service_params)
+@jwt_token.options(validators=(check_cors_origin, set_cors_headers))
 def jwt_token_options(request):  # pylint: disable=unused-argument
     """JWT token OPTIONS handler"""
     return ''
 
 
+class JWTTokenPostResponse(MappingSchema):
+    """Token post response"""
+
+    body = TokensResult()
+
+
+jwt_token_post_responses = rest_responses.copy()
+jwt_token_post_responses[HTTPOk.code] = JWTTokenPostResponse(
+    description="Get new access and refresh tokens matching credentials")
+
+
 @jwt_token.post(require_csrf=False,
                 content_type=('application/json', 'multipart/form-data'),
-                schema=LoginSchema(),
-                validators=(check_cors_origin, colander_body_validator,
-                            set_cors_headers),
-                **service_params)
+                schema=LoginInfo(),
+                validators=(check_cors_origin, colander_body_validator, set_cors_headers),
+                response_schemas=jwt_token_post_responses)
 def get_jwt_token(request):
-    """REST login endpoint for JWT authentication"""
+    """Get new access and refresh tokens matching credentials"""
     # check security manager utility
     sm = query_utility(ISecurityManager)  # pylint: disable=invalid-name
     if sm is None:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     configuration = IJWTSecurityConfiguration(sm)
     if not configuration.enabled:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     # check request params
     params = request.params if TEST_MODE else request.validated
     login = params.get('login')
     if not login:
-        raise HTTPBadRequest()
+        return http_error(request, HTTPBadRequest, 'missing credentials')
     credentials = Credentials('jwt', id=login, **params)
     # use remote authentication authority
     if configuration.proxy_mode:
         handler = IJWTProxyHandler(sm, None)
         if handler is not None:
             status_code, tokens = handler.get_tokens(request, credentials)  # pylint: disable=assignment-from-no-return
             request.response.status_code = status_code
             return tokens
     # authenticate principal in security manager
     principal_id = sm.authenticate(credentials, request)
-    if principal_id is not None:
-        custom_claims = params.get('claims', {})
-        request.response.cache_expires(configuration.refresh_expiration)
-        return {
-            'status': 'success',
-            configuration.access_token_name:
-                create_jwt_token(request,
-                                 principal_id,
-                                 expiration=configuration.access_expiration,
-                                 obj=ACCESS_OBJECT,
-                                 **custom_claims),
-            configuration.refresh_token_name:
-                create_jwt_token(request,
-                                 principal_id,
-                                 expiration=configuration.refresh_expiration,
-                                 obj=REFRESH_OBJECT)
-        }
-    request.response.status_code = HTTPUnauthorized.code
+    if principal_id is None:
+        return http_error(request, HTTPUnauthorized, "invalid credentials")
+    custom_claims = params.get('claims', {})
+    request.response.cache_expires(configuration.refresh_expiration)
     return {
-        'status': 'error',
-        'message': request.localizer.translate(_("Invalid credentials!"))
+        'status': STATUS.SUCCESS.value,
+        configuration.access_token_name:
+            create_jwt_token(request,
+                             principal_id,
+                             expiration=configuration.access_expiration,
+                             obj=ACCESS_OBJECT,
+                             **custom_claims),
+        configuration.refresh_token_name:
+            create_jwt_token(request,
+                             principal_id,
+                             expiration=configuration.refresh_expiration,
+                             obj=REFRESH_OBJECT)
     }
 
 
+class JWTTokenGetResponse(MappingSchema):
+    """Token claims getter response"""
+
+    body = ClaimsElements()
+
+
+jwt_token_get_responses = rest_responses.copy()
+jwt_token_get_responses[HTTPOk.code] = JWTTokenGetResponse(
+    description="Extract claims from provided token")
+
+
 @jwt_token.get(content_type=('multipart/form-data', 'application/json'),
-               schema=ClaimsObjectSchema(),
-               validators=(check_cors_origin, colander_body_validator,
-                           set_cors_headers),
-               **service_params)
+               schema=ClaimsObjectInfo(),
+               validators=(check_cors_origin, colander_body_validator, set_cors_headers),
+               response_schemas=jwt_token_get_responses)
 def get_jwt_claims(request):
-    """Extract claims from provided JWT token"""
+    """Extract claims from provided token"""
     sm = query_utility(ISecurityManager)  # pylint: disable=invalid-name
     if sm is None:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     configuration = IJWTSecurityConfiguration(sm)
     if not configuration.enabled:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     params = request.params if TEST_MODE else request.validated
     obj = params.get('obj')
     if configuration.proxy_mode:
         handler = IJWTProxyHandler(sm, None)
         if handler is not None:
             status_code, claims = handler.get_claims(request, obj)  # pylint: disable=assignment-from-no-return
             request.response.status_code = status_code
             return claims
     return get_request_claims(request, obj)
 
 
+class JWTTokenPatchResponse(MappingSchema):
+    """Token patch response"""
+
+    body = TokensResult()
+
+
+jwt_token_patch_responses = rest_responses.copy()
+jwt_token_patch_responses[HTTPOk.code] = JWTTokenPatchResponse(
+    description="Get new access token from valid refresh token")
+
+
 @jwt_token.patch(require_csrf=False,
                  content_type=('multipart/form-data', 'application/json'),
                  jwt_object=REFRESH_OBJECT,
-                 schema=ClaimsSetterSchema(),
-                 validators=(check_cors_origin, colander_body_validator,
-                             set_cors_headers),
-                 **service_params)
+                 schema=ClaimsInfo(),
+                 validators=(check_cors_origin, colander_body_validator, set_cors_headers),
+                 response_schemas=jwt_token_patch_responses)
 def refresh_jwt_token(request):
     """JWT token refresh service"""
     sm = query_utility(ISecurityManager)  # pylint: disable=invalid-name
     if sm is None:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     configuration = IJWTSecurityConfiguration(sm)
     if not configuration.enabled:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     # user remote authentication authority
     if configuration.proxy_mode:
         handler = IJWTProxyHandler(sm, None)
         if handler is not None:
             status_code, token = handler.refresh_token(request)  # pylint: disable=assignment-from-no-return
             request.response.status_code = status_code
             return token
     # refresh token locally
     claims = get_jwt_claims(request)
     if not claims:
-        raise HTTPForbidden()
+        return http_error(request, HTTPForbidden)
     principal_id = claims.get('sub')
     if not principal_id:
-        raise HTTPUnauthorized()
+        return http_error(request, HTTPUnauthorized)
     params = request.params if TEST_MODE else request.validated
     custom_claims = params.get('claims', {})
     return {
-        'status': 'success',
+        'status': STATUS.SUCCESS.value,
         configuration.access_token_name:
             create_jwt_token(request,
                              principal_id,
                              expiration=configuration.access_expiration,
                              obj=ACCESS_OBJECT,
                              **custom_claims)
     }
 
 
 jwt_verify = Service(name=REST_VERIFY_ROUTE,
                      pyramid_route=REST_VERIFY_ROUTE,
                      description="JWT tokens verification")
 
 
-@jwt_verify.options(validators=(check_cors_origin, set_cors_headers),
-                    **service_params)
+@jwt_verify.options(validators=(check_cors_origin, set_cors_headers))
 def jwt_verify_options(request):  # pylint: disable=unused-argument
     """JWT token verification OPTIONS handler"""
     return ''
 
 
-@jwt_verify.get(schema=ClaimsObjectSchema(),
+class JWTVerifyGetResponse(MappingSchema):
+    """Token verification response"""
+
+    body = TokensResult()
+
+
+jwt_verify_get_responses = rest_responses.copy()
+jwt_verify_get_responses[HTTPOk.code] = JWTVerifyGetResponse(
+    description="Get JWT token for authenticated principal")
+
+
+@jwt_verify.get(schema=ClaimsObjectInfo(),
                 validators=(check_cors_origin, set_cors_headers),
-                **service_params)
+                response_schemas=jwt_verify_get_responses)
 def get_current_jwt_token(request):
-    """Get current JWT token for authenticated principal"""
+    """Get JWT token for authenticated principal"""
     manager = query_utility(ISecurityManager)
     if manager is None:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     configuration = IJWTSecurityConfiguration(manager)
     if not configuration.enabled:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     if Authenticated not in request.effective_principals:
-        raise HTTPForbidden()
+        return http_error(request, HTTPForbidden)
     custom_claims = request.params.get('claims', {})
     request.response.cache_expires(configuration.refresh_expiration)
     return {
-        'status': 'success',
+        'status': STATUS.SUCCESS.value,
         configuration.access_token_name:
             create_jwt_token(request,
                              request.authenticated_userid,
                              expiration=configuration.access_expiration,
                              obj=ACCESS_OBJECT,
                              **custom_claims),
         configuration.refresh_token_name:
             create_jwt_token(request,
                              request.authenticated_userid,
                              expiration=configuration.refresh_expiration,
                              obj=REFRESH_OBJECT)
     }
 
 
+class JWTVerifyPostResponse(MappingSchema):
+    """JWT token verification response"""
+
+    body = BaseStatusSchema()
+
+
+jwt_verify_post_responses = rest_responses.copy()
+jwt_verify_post_responses[HTTPOk.code] = JWTVerifyPostResponse(
+    description="Verify JWT access token")
+
+
 @jwt_verify.post(require_csrf=False,
                  jwt_object=ACCESS_OBJECT,
-                 schema=ClaimsObjectSchema(),
-                 validators=(check_cors_origin, colander_body_validator,
-                             set_cors_headers),
-                 **service_params)
+                 schema=ClaimsObjectInfo(),
+                 validators=(check_cors_origin, colander_body_validator, set_cors_headers),
+                 response_schemas=jwt_verify_post_responses)
 def verify_jwt_token(request):
-    """JWT token verification view"""
+    """Verify JWT access token"""
     manager = query_utility(ISecurityManager)
     if manager is None:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     configuration = IJWTSecurityConfiguration(manager)
     if not configuration.enabled:
-        raise HTTPServiceUnavailable()
+        return http_error(request, HTTPServiceUnavailable)
     claims = get_jwt_claims(request)
     if not claims:
-        raise HTTPForbidden()
+        return http_error(request, HTTPForbidden)
     request.response.status_code = HTTPAccepted.code
     return {
-        'status': 'success'
+        'status': STATUS.SUCCESS.value
     }
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/doctests/README.rst` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     >>> cache_regions.update({'default': {'type': 'memory', 'expire': 60}})
     >>> cache_regions.update({'long': {'type': 'memory', 'expire': 600}})
 
     >>> from pyramid_zodbconn import includeme as include_zodbconn
     >>> include_zodbconn(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
+    >>> from cornice_swagger import includeme as include_swagger
+    >>> include_swagger(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_site import includeme as include_site
     >>> include_site(config)
     >>> from pyams_security import includeme as include_security
     >>> include_security(config)
     >>> from pyams_auth_jwt import includeme as include_auth_jwt
@@ -124,15 +126,15 @@
     True
 
     >>> jwt_request = DummyRequest(method='POST', path='/api/auth/jwt/login',
     ...                            params={'login': 'user1', 'password': 'passwd'})
     >>> jwt_request.create_jwt_token = lambda *args, **kwargs: create_jwt_token(jwt_request, *args, **kwargs)
     >>> jwt_result = get_jwt_token(jwt_request)
     >>> pprint.pprint(jwt_result)
-    {'message': 'Invalid credentials!', 'status': 'error'}
+    {'message': 'Unauthorized: invalid credentials', 'status': 'error'}
 
 This error is normal, because the user doesn't actually exist! So let's create it:
 
     >>> from pyams_security.plugin.userfolder import UsersFolder
     >>> folder = UsersFolder()
     >>> folder.prefix = 'users'
     >>> folder.title = 'Local users folder'
@@ -183,15 +185,15 @@
 We can try the same process using bad credentials or a bad JWT token:
 
     >>> jwt_request = DummyRequest(method='POST', path='/api/auth/jwt/login',
     ...                            params={'login': 'user1', 'password': 'badpasswd'})
     >>> jwt_request.create_jwt_token = lambda *args, **kwargs: create_jwt_token(jwt_request, *args, **kwargs)
     >>> jwt_result = get_jwt_token(jwt_request)
     >>> pprint.pprint(jwt_result)
-    {'message': 'Invalid credentials!', 'status': 'error'}
+    {'message': 'Unauthorized: invalid credentials', 'status': 'error'}
 
     >>> jwt_request = DummyRequest(authorization=('Bearer', 'abc.def.ghi'), remote_addr='127.0.0.1')
     >>> jwt_principal_id = sm.authenticated_userid(jwt_request)
     >>> jwt_principal_id is None
     True
     >>> policy.authenticated_userid(jwt_request) is None
     True
@@ -328,33 +330,33 @@
     >>> pprint.pprint(jwt_request.get_jwt_claims())
     {}
 
     >>> jwt_request = DummyRequest(method='POST', path='/api/auth/jwt/token',
     ...                            params={'login': 'user1', 'password': 'passwd'})
     >>> jwt_request.create_jwt_token = lambda *args, **kwargs: create_jwt_token(jwt_request, *args, **kwargs)
     >>> jwt_result = get_jwt_token(jwt_request)
-    Traceback (most recent call last):
-    ...
-    pyramid.httpexceptions.HTTPServiceUnavailable: The server is currently unavailable. Please try again at a later time.
+    >>> pprint.pprint(jwt_result)
+    {'message': 'Service Unavailable',
+     'status': 'error'}
 
 
 Testing plugin API
 ------------------
 
 We first have to get JWT tokens; let's reactivate our plug-in:
 
     >>> config.registry.settings['pyams.jwt.auth_type'] = 'Bearer'
     >>> jwt_configuration.local_mode = True
 
     >>> jwt_request = DummyRequest(method='PATCH', path='/api/auth/jwt/token')
     >>> jwt_request.create_jwt_token = lambda *args, **kwargs: create_jwt_token(jwt_request, *args, **kwargs)
     >>> jwt_result = get_jwt_token(jwt_request)
-    Traceback (most recent call last):
-    ...
-    pyramid.httpexceptions.HTTPBadRequest: The server could not comply with the request since it is either malformed or otherwise incorrect.
+    >>> pprint.pprint(jwt_result)
+    {'message': 'Bad Request: missing credentials',
+     'status': 'error'}
 
     >>> jwt_request = DummyRequest(method='PATCH', path='/api/auth/jwt/token',
     ...                            params={'login': 'user1', 'password': 'passwd'})
     >>> jwt_result = get_jwt_token(jwt_request)
     >>> pprint.pprint(jwt_result)
     {'accessToken': 'eyJ...',
      'refreshToken': 'eyJ...',
@@ -396,36 +398,32 @@
      'obj': 'refresh',
      'sub': 'users:user1'}
 
 We can always try o refresh a token without providing any access token:
 
     >>> jwt_request = DummyRequest()
     >>> jwt_request.get_jwt_claims = lambda *args, **kwargs: get_jwt_claims(jwt_request, *args, **kwargs)
-    >>> refresh_jwt_token(jwt_request)
-    Traceback (most recent call last):
-    ...
-    pyramid.httpexceptions.HTTPForbidden: Access was denied to this resource.
+    >>> pprint.pprint(refresh_jwt_token(jwt_request))
+    {'message': 'Forbidden', 'status': 'error'}
 
 
 Let's finally try to verify a token; this requires a POST on another access point:
 
     >>> from pyams_auth_jwt.api import verify_jwt_token
 
     >>> jwt_request = DummyRequest(authorization=('Bearer', jwt_result['refreshToken']))
     >>> jwt_request.get_jwt_claims = lambda *args, **kwargs: get_jwt_claims(jwt_request, *args, **kwargs)
     >>> verify_jwt_token(jwt_request)
     {'status': 'success'}
 
     >>> another_token = 'eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJvYmoiOiJhY2Nlc3MiLCJpYXQiOjE2MDg2NDU2NzQsImV4cCI6MTYwODY0OTI3NCwic3ViIjoic3lzdGVtOmFkbWluIn0.HeKZILlFb9qWA0quEwlLTlgWGA3nMx32bsnao1GFNxSR5_7NDlG3XJhzMMWvR7iMwf6u2AdLiVajZSDtpi1UVQ'
     >>> jwt_request = DummyRequest(authorization=('Bearer', another_token))
     >>> jwt_request.get_jwt_claims = lambda *args, **kwargs: get_jwt_claims(jwt_request, *args, **kwargs)
-    >>> verify_jwt_token(jwt_request)
-    Traceback (most recent call last):
-    ...
-    pyramid.httpexceptions.HTTPForbidden: ...
+    >>> pprint.pprint(verify_jwt_token(jwt_request))
+    {'message': 'Forbidden', 'status': 'error'}
 
 
 Custom JWT tokens object predicate
 ----------------------------------
 
 When a view is protected by a JWT token, you can add a custom predicate to specify which token
 type is authorized.
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/include.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/include.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/interfaces.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -57,17 +57,14 @@
 msgid ""
 "If this option is enabled, tokens management requests will be forwarded to "
 "another authentication authority"
 msgstr ""
 "Si cette option est activée, la gestion des jetons JWT est déléguée à une "
 "autre autorité d'authentification"
 
-msgid "Invalid credentials!"
-msgstr "Paramètres de connexion invalides !"
-
 msgid "JWT access token lifetime, in seconds"
 msgstr "Durée de vie des jetons d'accès JWT, en secondes"
 
 msgid "JWT authentication"
 msgstr "Authentification JWT"
 
 msgid ""
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,284 +1,280 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2021-01-01 16:01+0100\n"
+"POT-Creation-Date: 2023-04-12 15:58+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
 
-#: src/pyams_auth_jwt/plugin.py:95
-msgid "JWT authentication"
-msgstr "Authentification JWT"
-
-#: src/pyams_auth_jwt/interfaces.py:73 src/pyams_auth_jwt/interfaces.py:138
+#: src/pyams_auth_jwt/interfaces.py:81 src/pyams_auth_jwt/interfaces.py:146
 msgid "Access token attribute"
 msgstr "Nom du jeton d'accès"
 
-#: src/pyams_auth_jwt/interfaces.py:74
+#: src/pyams_auth_jwt/interfaces.py:82
 msgid ""
 "Name of the JSON attribute containing access token returned by REST APIs"
 msgstr ""
 "Nom de l'attribut JSON retourné par l'API REST contenant le jeton d'accès"
 
-#: src/pyams_auth_jwt/interfaces.py:79 src/pyams_auth_jwt/interfaces.py:144
+#: src/pyams_auth_jwt/interfaces.py:87 src/pyams_auth_jwt/interfaces.py:152
 msgid "Refresh token attribute"
 msgstr "Nom du jeton de rafraîchissement"
 
-#: src/pyams_auth_jwt/interfaces.py:80
+#: src/pyams_auth_jwt/interfaces.py:88
 msgid ""
 "Name of the JSON attribute containing refresh token returned by REST APIs"
 msgstr ""
 "Nom de l'attribut JSON retourné par l'API REST contenant le jeton de "
 "rafraîchissement"
 
-#: src/pyams_auth_jwt/interfaces.py:87
+#: src/pyams_auth_jwt/interfaces.py:95
 msgid "Enable JWT direct authentication?"
 msgstr "Activer le mode \"local\" ?"
 
-#: src/pyams_auth_jwt/interfaces.py:88
+#: src/pyams_auth_jwt/interfaces.py:96
 msgid "Enable direct login via JWT authentication"
 msgstr "Activer la gestion en local des jetons JWT"
 
-#: src/pyams_auth_jwt/interfaces.py:92
+#: src/pyams_auth_jwt/interfaces.py:100
 msgid "JWT encoding algorithm"
 msgstr "Algorithme d'encryptage"
 
-#: src/pyams_auth_jwt/interfaces.py:93
+#: src/pyams_auth_jwt/interfaces.py:101
 msgid ""
 "HS* protocols are using the secret, while RS* protocols are using RSA keys"
 msgstr ""
 "Les protocoles de type HS utilisent le code secret, tandis que les "
 "protocoles de types RS utilisent les clés RSA"
 
-#: src/pyams_auth_jwt/interfaces.py:99
+#: src/pyams_auth_jwt/interfaces.py:107
 msgid "JWT secret"
 msgstr "Code secret"
 
-#: src/pyams_auth_jwt/interfaces.py:100
+#: src/pyams_auth_jwt/interfaces.py:108
 msgid "This secret is required when using HS* encryption"
 msgstr ""
 "Ce code secret est nécessaire si vous utilisez un encryptage de type HS*"
 
-#: src/pyams_auth_jwt/interfaces.py:103
+#: src/pyams_auth_jwt/interfaces.py:111
 msgid "JWT private key"
 msgstr "Clé privée"
 
-#: src/pyams_auth_jwt/interfaces.py:104
+#: src/pyams_auth_jwt/interfaces.py:112
 msgid "The secret key is required when using RS* algorithm"
 msgstr "Une clé privée est nécessaire pour utiliser un encryptage de type RS*"
 
-#: src/pyams_auth_jwt/interfaces.py:107
+#: src/pyams_auth_jwt/interfaces.py:115
 msgid "JWT public key"
 msgstr "Clé publique"
 
-#: src/pyams_auth_jwt/interfaces.py:108
+#: src/pyams_auth_jwt/interfaces.py:116
 msgid "The public key is required when using RS* algorithm"
 msgstr ""
 "Une clé publique est nécessaire pour utiliser un encryptage de type RS*"
 
-#: src/pyams_auth_jwt/interfaces.py:111
+#: src/pyams_auth_jwt/interfaces.py:119
 msgid "Access token lifetime"
 msgstr "Durée de vie des jetons d'accès"
 
-#: src/pyams_auth_jwt/interfaces.py:112
+#: src/pyams_auth_jwt/interfaces.py:120
 msgid "JWT access token lifetime, in seconds"
 msgstr "Durée de vie des jetons d'accès JWT, en secondes"
 
-#: src/pyams_auth_jwt/interfaces.py:116
+#: src/pyams_auth_jwt/interfaces.py:124
 msgid "Refresh token lifetime"
 msgstr "Durée de vie des jetons de refresh"
 
-#: src/pyams_auth_jwt/interfaces.py:117
+#: src/pyams_auth_jwt/interfaces.py:125
 msgid "JWT refresh token lifetime, in seconds"
 msgstr "Durée de vie des jetons de rafraîchissement, en secondes"
 
-#: src/pyams_auth_jwt/interfaces.py:121
+#: src/pyams_auth_jwt/interfaces.py:129
 msgid "Enable JWT proxy authentication?"
 msgstr "Activer le mode \"proxy\" ?"
 
-#: src/pyams_auth_jwt/interfaces.py:122
+#: src/pyams_auth_jwt/interfaces.py:130
 msgid ""
 "If this option is enabled, tokens management requests will be forwarded to "
 "another authentication authority"
 msgstr ""
 "Si cette option est activée, la gestion des jetons JWT est déléguée à une "
 "autre autorité d'authentification"
 
-#: src/pyams_auth_jwt/interfaces.py:127
+#: src/pyams_auth_jwt/interfaces.py:135
 msgid "Authentication authority"
 msgstr "Autorité d'authentification"
 
-#: src/pyams_auth_jwt/interfaces.py:128
+#: src/pyams_auth_jwt/interfaces.py:136
 msgid ""
 "Base URL (protocol and hostname) of the authentication authority to which "
 "tokens management requests will be forwarded"
 msgstr ""
 "URL de base (protocole et nom d'hôte) de l'autorité d'authentification à "
 "laquelle est déléguée la gestion des jetons"
 
-#: src/pyams_auth_jwt/interfaces.py:133
+#: src/pyams_auth_jwt/interfaces.py:141
 msgid "Token getter service"
 msgstr "Service d'obtention"
 
-#: src/pyams_auth_jwt/interfaces.py:134
+#: src/pyams_auth_jwt/interfaces.py:142
 msgid "REST HTTP service used to get a new token"
 msgstr ""
 "URL relative du service REST permettant de récupérer de nouveaux jetons JWT "
 "à partir d'un login et d'un mot de passe"
 
-#: src/pyams_auth_jwt/interfaces.py:139
+#: src/pyams_auth_jwt/interfaces.py:147
 msgid ""
 "Name of the JSON attribute returned by REST API containing access tokens"
 msgstr ""
 "Nom de l'attribut JSON retourné par l'API REST contenant les jetons d'accès"
 
-#: src/pyams_auth_jwt/interfaces.py:145
+#: src/pyams_auth_jwt/interfaces.py:153
 msgid ""
 "Name of the JSON attribute returned by REST API containing refresh tokens"
 msgstr ""
 "Nom de l'attribut JSON retourné par l'API REST contenant les jetons de "
 "rafraîchissement"
 
-#: src/pyams_auth_jwt/interfaces.py:150
+#: src/pyams_auth_jwt/interfaces.py:158
 msgid "Token claims getter"
 msgstr "Service de consultation"
 
-#: src/pyams_auth_jwt/interfaces.py:151
+#: src/pyams_auth_jwt/interfaces.py:159
 msgid ""
 "REST HTTP service used to extract claims from provided authorization token"
 msgstr ""
 "URL relative du service REST permettant d'extraire les \"réclamations"
 "\" (claims) des jetons JWT"
 
-#: src/pyams_auth_jwt/interfaces.py:156
+#: src/pyams_auth_jwt/interfaces.py:164
 msgid "Token refresh service"
 msgstr "Service de rafraîchissement"
 
-#: src/pyams_auth_jwt/interfaces.py:157
+#: src/pyams_auth_jwt/interfaces.py:165
 msgid "REST HTTP service used to get a new access token with a refresh token"
 msgstr ""
 "URL relative du service REST permettant de récupérer un nouveau jeton "
 "d'accès à partir d'un jeton de rafraîchissement"
 
-#: src/pyams_auth_jwt/interfaces.py:162
+#: src/pyams_auth_jwt/interfaces.py:170
 msgid "Token verify service"
 msgstr "Service de vérification"
 
-#: src/pyams_auth_jwt/interfaces.py:163
+#: src/pyams_auth_jwt/interfaces.py:171
 msgid "REST HTTP service used to check validity of an existing token"
 msgstr ""
 "URL relative du service REST permettant de vérifier la validité d'un jeton"
 
-#: src/pyams_auth_jwt/interfaces.py:168
+#: src/pyams_auth_jwt/interfaces.py:176
 msgid "Verify SSL?"
 msgstr "Vérification SSL ?"
 
-#: src/pyams_auth_jwt/interfaces.py:169
+#: src/pyams_auth_jwt/interfaces.py:177
 msgid "If 'no', SSL certificates will not be verified"
 msgstr "Si 'non', les certificats SSL ne seront pas vérifiés"
 
-#: src/pyams_auth_jwt/interfaces.py:173
+#: src/pyams_auth_jwt/interfaces.py:181
 msgid "Use verified tokens cache?"
 msgstr "Mettre les jetons en cache ?"
 
-#: src/pyams_auth_jwt/interfaces.py:174
+#: src/pyams_auth_jwt/interfaces.py:182
 msgid ""
 "If selected, this option allows to store credentials in a local cache from "
 "which they can be reused"
 msgstr ""
 "En sélectionnant cette option, les jetons validés seront mis en cache, de "
 "façon à limiter les requêtes auprès de l'autorité d'authentification"
 
-#: src/pyams_auth_jwt/interfaces.py:179
+#: src/pyams_auth_jwt/interfaces.py:187
 msgid "Selected tokens cache"
 msgstr "Cache de jetons"
 
-#: src/pyams_auth_jwt/interfaces.py:180
+#: src/pyams_auth_jwt/interfaces.py:188
 msgid "Beaker cache selected to store validated tokens"
 msgstr "Cache pré-défini dans lequel seront stockés les jetons"
 
-#: src/pyams_auth_jwt/interfaces.py:189
+#: src/pyams_auth_jwt/interfaces.py:197
 msgid "You can't enable both local and proxy modes"
 msgstr ""
 "Vous ne pouvez pas activer le mode local et le mode proxy en même temps !"
 
-#: src/pyams_auth_jwt/interfaces.py:192
+#: src/pyams_auth_jwt/interfaces.py:200
 msgid "You must choose an algorithm to enable JWT authentication"
 msgstr ""
 "Vous devez sélectionner un algorithme d'encryptage pour activer "
 "l'authentification JWT"
 
-#: src/pyams_auth_jwt/interfaces.py:202
-msgid "You must define authentication authority to use proxy mode"
-msgstr ""
-"Vous devez indiquer l'autorité d'authentification pour utiliser le mode "
-"proxy !"
-
-#: src/pyams_auth_jwt/interfaces.py:204
-msgid "You must choose a cache to enable tokens caching"
-msgstr ""
-"Vous devez sélectionner un cache pour activer la mise en cache des jetons"
-
-#: src/pyams_auth_jwt/interfaces.py:195
+#: src/pyams_auth_jwt/interfaces.py:203
 msgid "You must define JWT secret to use HS256 algorithm"
 msgstr ""
 "Vous devez définir un code secret pour utiliser un encryptage de type HS*"
 
-#: src/pyams_auth_jwt/interfaces.py:198
+#: src/pyams_auth_jwt/interfaces.py:206
 msgid "You must define a private and a public key to use RS256 algorithm"
 msgstr ""
 "Vous devez définir une clé privée et une clé publique pour utiliser un "
 "encryptage de type RS*"
 
-#: src/pyams_auth_jwt/api/__init__.py:81
-msgid "Invalid credentials!"
-msgstr "Paramètres de connexion invalides !"
+#: src/pyams_auth_jwt/interfaces.py:210
+msgid "You must define authentication authority to use proxy mode"
+msgstr ""
+"Vous devez indiquer l'autorité d'authentification pour utiliser le mode "
+"proxy !"
+
+#: src/pyams_auth_jwt/interfaces.py:212
+msgid "You must choose a cache to enable tokens caching"
+msgstr ""
+"Vous devez sélectionner un cache pour activer la mise en cache des jetons"
 
-#: src/pyams_auth_jwt/zmi/plugin.py:54 src/pyams_auth_jwt/zmi/plugin.py:64
+#: src/pyams_auth_jwt/plugin.py:94
+msgid "JWT authentication"
+msgstr "Authentification JWT"
+
+#: src/pyams_auth_jwt/zmi/plugin.py:50 src/pyams_auth_jwt/zmi/plugin.py:61
 msgid "JWT configuration"
 msgstr "Configuration JWT"
 
-#: src/pyams_auth_jwt/zmi/plugin.py:63
+#: src/pyams_auth_jwt/zmi/plugin.py:60
 msgid "Security manager"
 msgstr "Gestionnaire de sécurité"
 
-#: src/pyams_auth_jwt/zmi/plugin.py:113
+#: src/pyams_auth_jwt/zmi/plugin.py:109
 msgid ""
 "JWT authentication module \"local mode\" allows to generate, check and "
 "refresh tokens locally.\n"
 "You can choose to use a simple secret key to encrypt your tokens, or to use "
 "a private and public keys pair (which can to be used to share tokens between "
 "two applications)."
 msgstr ""
 "Le mode \"local\" du module d'authentification JWT permet de générer, "
 "vérifier et rafraîchir les jetons JWT localement.\n"
 "Vous pouvez utiliser un simple secret pour encrypter les jetons, ou utiliser "
 "un couple de clés publique et privée (qui peuvent notamment être utilisées "
 "pour partager des jetons entre plusieurs applications qui peuvent s'appuyer "
 "sur une autorité d'authentification commune)."
 
-#: src/pyams_auth_jwt/zmi/plugin.py:126
+#: src/pyams_auth_jwt/zmi/plugin.py:122
 msgid ""
 "You can use the `openssl` command to generate your keys:\n"
 "\n"
 "    openssl genpkey -algorithm RSA -out private-key.pem\n"
 "    openssl rsa -pubout -in private-key.pem -out public-key.pem\n"
 msgstr ""
 "Vous pouvez utiliser la commande `openssl` pour générer vos clés :\n"
 "\n"
 "         openssl genpkey -algorithm RSA -out private-key.pem\n"
 "         openssl rsa -pubout -in private-key.pem -out public-key.pem\n"
 
-#: src/pyams_auth_jwt/zmi/plugin.py:161
+#: src/pyams_auth_jwt/zmi/plugin.py:156
 msgid ""
 "JWT authentication module \"proxy mode\" relies on another authentication "
 "authority (which can be another application using this JWT package) to "
 "generate, check and refresh tokens. This authority can be used to share "
 "access tokens between different applications.\n"
 "You can cache tokens to reduce the number of requests which will be "
 "forwarded to the authentication authority."
@@ -288,14 +284,17 @@
 "le même package JWT en mode local) pour générer, vérifier et rafraîchir les "
 "jetons JWT, via la même API REST. Cette autorité peut par ailleurs être "
 "utilisée par différentes applications pour partager des jetons.\n"
 "Vous pouvez également choisir d'activer un cache dans lequel seront stockés "
 "les jetons validés, afin de limiter le nombre de requêtes transmises à "
 "l'autorité d'authentification."
 
+#~ msgid "Invalid credentials!"
+#~ msgstr "Paramètres de connexion invalides !"
+
 #~ msgid "Enable JWT login?"
 #~ msgstr "Activer l'authentification JWT ?"
 
 #~ msgid "Send cookie?"
 #~ msgstr "Envoyer un cookie ?"
 
 #~ msgid "If 'yes', a session cookie will be sent on authentication"
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot`

 * *Files 5% similar despite different names*

```diff
@@ -1,241 +1,237 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2021-01-01 16:01+0100\n"
+"POT-Creation-Date: 2023-04-12 15:58+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Lingua 3.10.dev0\n"
+"Generated-By: Lingua 4.15.0\n"
 
-#: ./src/pyams_auth_jwt/plugin.py:95
-msgid "JWT authentication"
-msgstr ""
-
-#: ./src/pyams_auth_jwt/interfaces.py:73 ./src/pyams_auth_jwt/interfaces.py:138
+#: ./src/pyams_auth_jwt/interfaces.py:81 ./src/pyams_auth_jwt/interfaces.py:146
 msgid "Access token attribute"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:74
+#: ./src/pyams_auth_jwt/interfaces.py:82
 msgid ""
 "Name of the JSON attribute containing access token returned by REST APIs"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:79 ./src/pyams_auth_jwt/interfaces.py:144
+#: ./src/pyams_auth_jwt/interfaces.py:87 ./src/pyams_auth_jwt/interfaces.py:152
 msgid "Refresh token attribute"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:80
+#: ./src/pyams_auth_jwt/interfaces.py:88
 msgid ""
 "Name of the JSON attribute containing refresh token returned by REST APIs"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:87
+#: ./src/pyams_auth_jwt/interfaces.py:95
 msgid "Enable JWT direct authentication?"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:88
+#: ./src/pyams_auth_jwt/interfaces.py:96
 msgid "Enable direct login via JWT authentication"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:92
+#: ./src/pyams_auth_jwt/interfaces.py:100
 msgid "JWT encoding algorithm"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:93
+#: ./src/pyams_auth_jwt/interfaces.py:101
 msgid ""
 "HS* protocols are using the secret, while RS* protocols are using RSA keys"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:99
+#: ./src/pyams_auth_jwt/interfaces.py:107
 msgid "JWT secret"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:100
+#: ./src/pyams_auth_jwt/interfaces.py:108
 msgid "This secret is required when using HS* encryption"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:103
+#: ./src/pyams_auth_jwt/interfaces.py:111
 msgid "JWT private key"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:104
+#: ./src/pyams_auth_jwt/interfaces.py:112
 msgid "The secret key is required when using RS* algorithm"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:107
+#: ./src/pyams_auth_jwt/interfaces.py:115
 msgid "JWT public key"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:108
+#: ./src/pyams_auth_jwt/interfaces.py:116
 msgid "The public key is required when using RS* algorithm"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:111
+#: ./src/pyams_auth_jwt/interfaces.py:119
 msgid "Access token lifetime"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:112
+#: ./src/pyams_auth_jwt/interfaces.py:120
 msgid "JWT access token lifetime, in seconds"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:116
+#: ./src/pyams_auth_jwt/interfaces.py:124
 msgid "Refresh token lifetime"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:117
+#: ./src/pyams_auth_jwt/interfaces.py:125
 msgid "JWT refresh token lifetime, in seconds"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:121
+#: ./src/pyams_auth_jwt/interfaces.py:129
 msgid "Enable JWT proxy authentication?"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:122
+#: ./src/pyams_auth_jwt/interfaces.py:130
 msgid ""
 "If this option is enabled, tokens management requests will be forwarded to "
 "another authentication authority"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:127
+#: ./src/pyams_auth_jwt/interfaces.py:135
 msgid "Authentication authority"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:128
+#: ./src/pyams_auth_jwt/interfaces.py:136
 msgid ""
 "Base URL (protocol and hostname) of the authentication authority to which "
 "tokens management requests will be forwarded"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:133
+#: ./src/pyams_auth_jwt/interfaces.py:141
 msgid "Token getter service"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:134
+#: ./src/pyams_auth_jwt/interfaces.py:142
 msgid "REST HTTP service used to get a new token"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:139
+#: ./src/pyams_auth_jwt/interfaces.py:147
 msgid ""
 "Name of the JSON attribute returned by REST API containing access tokens"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:145
+#: ./src/pyams_auth_jwt/interfaces.py:153
 msgid ""
 "Name of the JSON attribute returned by REST API containing refresh tokens"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:150
+#: ./src/pyams_auth_jwt/interfaces.py:158
 msgid "Token claims getter"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:151
+#: ./src/pyams_auth_jwt/interfaces.py:159
 msgid ""
 "REST HTTP service used to extract claims from provided authorization token"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:156
+#: ./src/pyams_auth_jwt/interfaces.py:164
 msgid "Token refresh service"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:157
+#: ./src/pyams_auth_jwt/interfaces.py:165
 msgid "REST HTTP service used to get a new access token with a refresh token"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:162
+#: ./src/pyams_auth_jwt/interfaces.py:170
 msgid "Token verify service"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:163
+#: ./src/pyams_auth_jwt/interfaces.py:171
 msgid "REST HTTP service used to check validity of an existing token"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:168
+#: ./src/pyams_auth_jwt/interfaces.py:176
 msgid "Verify SSL?"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:169
+#: ./src/pyams_auth_jwt/interfaces.py:177
 msgid "If 'no', SSL certificates will not be verified"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:173
+#: ./src/pyams_auth_jwt/interfaces.py:181
 msgid "Use verified tokens cache?"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:174
+#: ./src/pyams_auth_jwt/interfaces.py:182
 msgid ""
 "If selected, this option allows to store credentials in a local cache from "
 "which they can be reused"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:179
+#: ./src/pyams_auth_jwt/interfaces.py:187
 msgid "Selected tokens cache"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:180
+#: ./src/pyams_auth_jwt/interfaces.py:188
 msgid "Beaker cache selected to store validated tokens"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:189
+#: ./src/pyams_auth_jwt/interfaces.py:197
 msgid "You can't enable both local and proxy modes"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:192
+#: ./src/pyams_auth_jwt/interfaces.py:200
 msgid "You must choose an algorithm to enable JWT authentication"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:202
-msgid "You must define authentication authority to use proxy mode"
+#: ./src/pyams_auth_jwt/interfaces.py:203
+msgid "You must define JWT secret to use HS256 algorithm"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:204
-msgid "You must choose a cache to enable tokens caching"
+#: ./src/pyams_auth_jwt/interfaces.py:206
+msgid "You must define a private and a public key to use RS256 algorithm"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:195
-msgid "You must define JWT secret to use HS256 algorithm"
+#: ./src/pyams_auth_jwt/interfaces.py:210
+msgid "You must define authentication authority to use proxy mode"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/interfaces.py:198
-msgid "You must define a private and a public key to use RS256 algorithm"
+#: ./src/pyams_auth_jwt/interfaces.py:212
+msgid "You must choose a cache to enable tokens caching"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/api/__init__.py:81
-msgid "Invalid credentials!"
+#: ./src/pyams_auth_jwt/plugin.py:94
+msgid "JWT authentication"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/zmi/plugin.py:54 ./src/pyams_auth_jwt/zmi/plugin.py:64
+#: ./src/pyams_auth_jwt/zmi/plugin.py:50 ./src/pyams_auth_jwt/zmi/plugin.py:61
 msgid "JWT configuration"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/zmi/plugin.py:63
+#: ./src/pyams_auth_jwt/zmi/plugin.py:60
 msgid "Security manager"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/zmi/plugin.py:113
+#: ./src/pyams_auth_jwt/zmi/plugin.py:109
 msgid ""
 "JWT authentication module \"local mode\" allows to generate, check and refresh tokens locally.\n"
 "You can choose to use a simple secret key to encrypt your tokens, or to use a private and public keys pair (which can to be used to share tokens between two applications)."
 msgstr ""
 
-#: ./src/pyams_auth_jwt/zmi/plugin.py:126
+#: ./src/pyams_auth_jwt/zmi/plugin.py:122
 msgid ""
 "You can use the `openssl` command to generate your keys:\n"
 "\n"
 "    openssl genpkey -algorithm RSA -out private-key.pem\n"
 "    openssl rsa -pubout -in private-key.pem -out public-key.pem\n"
 msgstr ""
 
-#: ./src/pyams_auth_jwt/zmi/plugin.py:161
+#: ./src/pyams_auth_jwt/zmi/plugin.py:156
 msgid ""
 "JWT authentication module \"proxy mode\" relies on another authentication authority (which can be another application using this JWT package) to generate, check and refresh tokens. This authority can be used to share access tokens between different applications.\n"
 "You can cache tokens to reduce the number of requests which will be forwarded to the authentication authority."
 msgstr ""
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/plugin.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/proxy.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/proxy.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/__init__.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/test_utilsdocs.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/tests/test_utilsdocstrings.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/zmi/__init__.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt/zmi/plugin.py` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/PKG-INFO` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-auth-jwt
-Version: 1.4.4
+Version: 1.4.5
 Summary: PyAMS security plug-in for JWT authentication
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,18 @@
 
 You have to include this package in your Pyramid configuration to active this plug-in.
 
 
 Changelog
 =========
 
+1.4.5
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
  - added support for Python 3.11
 
 1.4.3
 -----
```

### Comparing `pyams_auth_jwt-1.4.4/src/pyams_auth_jwt.egg-info/SOURCES.txt` & `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

