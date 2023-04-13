# Comparing `tmp/pyams_auth_jwt-1.4.5.tar.gz` & `tmp/pyams_auth_jwt-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_auth_jwt-1.4.5.tar", last modified: Thu Apr 13 10:27:19 2023, max compression
+gzip compressed data, was "dist/pyams_auth_jwt-1.4.6.tar", last modified: Thu Apr 13 12:08:56 2023, max compression
```

## Comparing `pyams_auth_jwt-1.4.5.tar` & `pyams_auth_jwt-1.4.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2954 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1348 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2552 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/
--rw-rw-rw-   0 root         (0) root         (0)    12397 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    22983 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2783 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/include.py
--rw-rw-rw-   0 root         (0) root         (0)    10397 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8200 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo
--rw-rw-rw-   0 root         (0) root         (0)    10797 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po
--rw-rw-rw-   0 root         (0) root         (0)     6655 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot
--rw-rw-rw-   0 root         (0) root         (0)    11495 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6942 2023-04-13 10:27:00.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2954 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 10:27:19.000000 pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1383 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2552 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/api/
+-rw-rw-rw-   0 root         (0) root         (0)    12397 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    22983 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    10456 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10797 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11495 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6942 2023-04-13 12:08:31.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/zmi/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 12:08:56.000000 pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/top_level.txt
```

### Comparing `pyams_auth_jwt-1.4.5/LICENSE` & `pyams_auth_jwt-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/PKG-INFO` & `pyams_auth_jwt-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_auth_jwt
-Version: 1.4.5
+Version: 1.4.6
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
 
+1.4.6
+-----
+ - interfaces cleanup
+
 1.4.5
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
```

### Comparing `pyams_auth_jwt-1.4.5/docs/HISTORY.rst` & `pyams_auth_jwt-1.4.6/docs/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.4.6
+-----
+ - interfaces cleanup
+
 1.4.5
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
```

### Comparing `pyams_auth_jwt-1.4.5/docs/README.rst` & `pyams_auth_jwt-1.4.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/setup.py` & `pyams_auth_jwt-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.4.5'
+version = '1.4.6'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_form',
     'pyams_layer',
     'pyams_site',
     'pyams_skin',
```

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/__init__.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/api/__init__.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/doctests/README.rst` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/include.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/include.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """PyAMS JWT authentication package.include module
 
 This module is used for Pyramid integration.
 """
 
 import jwt
 
-from pyams_auth_jwt.interfaces import REST_TOKEN_ROUTE, REST_VERIFY_ROUTE
+from pyams_auth_jwt.interfaces import REST_TOKEN_PATH, REST_TOKEN_ROUTE, REST_VERIFY_PATH, REST_VERIFY_ROUTE
 from pyams_auth_jwt.plugin import JWTTokenObjectPredicate, create_jwt_token, get_jwt_claims
 
 
 __docformat__ = 'restructuredtext'
 
 
 def include_package(config):
@@ -36,18 +36,18 @@
 
     # add route predicate
     config.add_view_predicate('jwt_object', JWTTokenObjectPredicate)
 
     # register new REST API routes
     config.add_route(REST_TOKEN_ROUTE,
                      config.registry.settings.get('pyams.jwt.rest_token_route',
-                                                  '/api/auth/jwt/token'))
+                                                  REST_TOKEN_PATH))
     config.add_route(REST_VERIFY_ROUTE,
                      config.registry.settings.get('pyams.jwt.rest_verify_route',
-                                                  '/api/auth/jwt/verify'))
+                                                  REST_VERIFY_PATH))
 
     # update JWT algorithms
     try:
         import pycrypto  # pylint: disable=import-outside-toplevel,unused-import
     except ImportError:
         pass
     else:
```

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/interfaces.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 
 #
 # API endpoints
 #
 
 REST_TOKEN_ROUTE = 'jwt.rest.token'
+REST_TOKEN_PATH = '/api/auth/jwt/token'
+
 REST_VERIFY_ROUTE = 'jwt.rest.verify'
+REST_VERIFY_PATH = '/api/auth/jwt/verify'
 
 
 #
 # JWT authentication utility interface
 #
 
 JWT_CONFIGURATION_KEY = 'pyams_auth_jwt.configuration'
@@ -137,15 +140,15 @@
                                        "authority to which tokens management requests will be "
                                        "forwarded"),
                          required=False)
 
     get_token_service = HTTPMethodField(title=_("Token getter service"),
                                         description=_("REST HTTP service used to get a new token"),
                                         required=False,
-                                        default=('POST', '/api/auth/jwt/token'))
+                                        default=('POST', REST_TOKEN_PATH))
 
     proxy_access_token_name = TextLine(title=_("Access token attribute"),
                                        description=_("Name of the JSON attribute returned by "
                                                      "REST API containing access tokens"),
                                        required=False,
                                        default=ACCESS_TOKEN_NAME)
 
@@ -155,27 +158,27 @@
                                         required=False,
                                         default=REFRESH_TOKEN_NAME)
 
     get_claims_service = HTTPMethodField(title=_("Token claims getter"),
                                          description=_("REST HTTP service used to extract claims "
                                                        "from provided authorization token"),
                                          required=False,
-                                         default=('GET', '/api/auth/jwt/token'))
+                                         default=('GET', REST_TOKEN_PATH))
 
     refresh_token_service = HTTPMethodField(title=_("Token refresh service"),
                                             description=_("REST HTTP service used to get a new "
                                                           "access token with a refresh token"),
                                             required=False,
-                                            default=('PATCH', '/api/auth/jwt/token'))
+                                            default=('PATCH', REST_TOKEN_PATH))
 
     verify_token_service = HTTPMethodField(title=_("Token verify service"),
                                            description=_("REST HTTP service used to check "
                                                          "validity of an existing token"),
                                            required=False,
-                                           default=('POST', '/api/auth/jwt/verify'))
+                                           default=('POST', REST_VERIFY_PATH))
 
     verify_ssl = Bool(title=_("Verify SSL?"),
                       description=_("If 'no', SSL certificates will not be verified"),
                       required=False,
                       default=True)
 
     use_cache = Bool(title=_("Use verified tokens cache?"),
```

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.mo`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/fr/LC_MESSAGES/pyams_auth_jwt.po`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/locales/pyams_auth_jwt.pot`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/plugin.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/proxy.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/proxy.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/__init__.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocs.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/tests/test_utilsdocstrings.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/__init__.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt/zmi/plugin.py` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt/zmi/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/PKG-INFO` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-auth-jwt
-Version: 1.4.5
+Version: 1.4.6
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
 
+1.4.6
+-----
+ - interfaces cleanup
+
 1.4.5
 -----
  - updated Colander API schemas for better OpenAPI specifications
 
 1.4.4
 -----
  - updated PyJWT package dependency to 2.6.0
```

### Comparing `pyams_auth_jwt-1.4.5/src/pyams_auth_jwt.egg-info/SOURCES.txt` & `pyams_auth_jwt-1.4.6/src/pyams_auth_jwt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

