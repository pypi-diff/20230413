# Comparing `tmp/pyams_auth_apikey-1.0.0.tar.gz` & `tmp/pyams_auth_apikey-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_auth_apikey-1.0.0.tar", last modified: Sun Feb 19 15:09:02 2023, max compression
+gzip compressed data, was "dist/pyams_auth_apikey-1.0.1.tar", last modified: Thu Apr 13 10:11:10 2023, max compression
```

## Comparing `pyams_auth_apikey-1.0.0.tar` & `pyams_auth_apikey-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2064 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/PKG-INFO
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1449 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2494 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/setup.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/__init__.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     8434 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/include.py
--rw-rw-rw-   0 root         (0) root         (0)     5240 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/interfaces.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4220 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.mo
--rw-rw-rw-   0 root         (0) root         (0)     6445 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.po
--rw-rw-rw-   0 root         (0) root         (0)     4697 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/pyams_auth_apikey.pot
--rw-rw-rw-   0 root         (0) root         (0)    14387 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/plugin.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/test_utilsdocstrings.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9236 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6831 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/plugin.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/namespace_packages.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-19 15:00:31.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-02-19 15:09:02.000000 pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)       86 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2494 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     8434 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4220 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.mo
+-rw-rw-rw-   0 root         (0) root         (0)     6445 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.po
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/pyams_auth_apikey.pot
+-rw-rw-rw-   0 root         (0) root         (0)    14387 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9236 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6831 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 10:10:48.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-13 10:11:10.000000 pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/top_level.txt
```

### Comparing `pyams_auth_apikey-1.0.0/LICENSE` & `pyams_auth_apikey-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/PKG-INFO` & `pyams_auth_apikey-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_auth_apikey
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyAMS authentication module using API keys
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -54,12 +54,16 @@
 At first, API keys can only be provided using a specific HTTP header which can be configured
 for all keys; maybe other authentication modes will be provided in future versions.
 
 
 Changelog
 =========
 
+1.0.1
+-----
+ - interface cleanup
+
 1.0.0
 -----
  - initial release
```

### Comparing `pyams_auth_apikey-1.0.0/docs/README.rst` & `pyams_auth_apikey-1.0.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/setup.py` & `pyams_auth_apikey-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.0.0'
+version = '1.0.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_form',
     'pyams_layer',
     'pyams_security_views',
     'pyams_site',
```

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/__init__.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/doctests/README.rst` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/include.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/include.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/interfaces.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
                    default=False)
 
     http_header = TextLine(title=_("HTTP header"),
                            description=_("Name of the HTTP header used to provide the API key"),
                            required=True,
                            default='X-API-Key')
 
-    by_name = Attribute("API keys mapping by key name")
     by_hash = Attribute("API keys mapping by key hash")
     by_principal = Attribute("API keys mapping by principal ID")
 
     def get_apikey(self, request):
         """Extract API key from provided request"""
 
     def find_active_key(self, request):
```

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.mo` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.mo`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.po` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/fr/LC_MESSAGES/pyams_auth_apikey.po`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/locales/pyams_auth_apikey.pot` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/locales/pyams_auth_apikey.pot`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/plugin.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/__init__.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/test_utilsdocs.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/tests/test_utilsdocstrings.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/__init__.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/container.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/interfaces.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey/zmi/plugin.py` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey/zmi/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/PKG-INFO` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-auth-apikey
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyAMS authentication module using API keys
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -54,12 +54,16 @@
 At first, API keys can only be provided using a specific HTTP header which can be configured
 for all keys; maybe other authentication modes will be provided in future versions.
 
 
 Changelog
 =========
 
+1.0.1
+-----
+ - interface cleanup
+
 1.0.0
 -----
  - initial release
```

### Comparing `pyams_auth_apikey-1.0.0/src/pyams_auth_apikey.egg-info/SOURCES.txt` & `pyams_auth_apikey-1.0.1/src/pyams_auth_apikey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

