# Comparing `tmp/pyams_sequence-1.2.2.tar.gz` & `tmp/pyams_sequence-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_sequence-1.2.2.tar", last modified: Tue May 17 08:31:16 2022, max compression
+gzip compressed data, was "dist/pyams_sequence-1.2.3.tar", last modified: Thu Apr 13 12:32:47 2023, max compression
```

## Comparing `pyams_sequence-1.2.2.tar` & `pyams_sequence-1.2.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3186 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)      652 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1385 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2648 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/api/
--rw-rw-rw-   0 root         (0) root         (0)     1475 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4049 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10254 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1988 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4882 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3742 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
--rw-rw-rw-   0 root         (0) root         (0)     5074 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
--rw-rw-rw-   0 root         (0) root         (0)     3353 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/locales/pyams_sequence.pot
--rw-rw-rw-   0 root         (0) root         (0)     4616 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/sequence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     6172 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/widget/
--rw-rw-rw-   0 root         (0) root         (0)     3604 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2134 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2022-05-17 08:30:52.000000 pyams_sequence-1.2.2/src/pyams_sequence/zmi/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3186 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1193 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      288 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-05-17 08:31:16.000000 pyams_sequence-1.2.2/src/pyams_sequence.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      773 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2648 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10379 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/pyams_sequence.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4616 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/sequence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     3604 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      288 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/top_level.txt
```

### Comparing `pyams_sequence-1.2.2/docs/README.txt` & `pyams_sequence-1.2.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/setup.py` & `pyams_sequence-1.2.3/setup.py`

 * *Files 3% similar despite different names*

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
 
-version = '1.2.2'
+version = '1.2.3'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/api/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/api/rest.py` & `pyams_sequence-1.2.3/src/pyams_sequence/api/rest.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,101 +15,102 @@
 This modules defines REST API used to search internal references.
 """
 
 import sys
 
 from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
-from cornice.validators import colander_querystring_validator
+from cornice.validators import colander_validator
 from pyramid.httpexceptions import HTTPOk
 
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_sequence.interfaces import ISequentialIntIds, REST_REFERENCES_SEARCH_ROUTE
 from pyams_sequence.sequence import get_sequence_dict
 from pyams_utils.registry import query_utility
+from pyams_utils.rest import BaseResponseSchema, STATUS, rest_responses
 
 
 __docformat__ = 'restructuredtext'
 
-from pyams_sequence import _  # pylint: disable=ungrouped-imports
-
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
-class ReferencesSearchQuerySchema(MappingSchema):
+class ReferencesSearchQuery(MappingSchema):
     """Internal references search schema"""
     term = SchemaNode(String(),
-                      title=_("References search string"),
-                      description=_("Query can be an internal reference OID, eventually "
-                                    "prefixed with a \"+\", or a text query which should "
-                                    "match contents title"))
+                      description="Terms search query; can be an internal reference OID, eventually "
+                                  "prefixed with a \"+\", or a text query which should "
+                                  "match contents title")
     content_type = SchemaNode(String(),
-                              title=_("Content type"),
-                              description=_("References search can be restricted to a given "
-                                            "content type"),
+                              description="Set content type to restrict references search",
                               missing=drop)
 
 
-class ReferenceResultSchema(MappingSchema):
+class Reference(MappingSchema):
     """Reference result schema"""
     id = SchemaNode(String(),
-                    description=_("Reference ID"))
+                    description="Reference ID")
     text = SchemaNode(String(),
-                      description=_("Reference title"))
+                      description="Reference title")
 
 
-class ReferencesSearchResults(SequenceSchema):
+class ReferencesList(SequenceSchema):
     """References search results"""
-    result = ReferenceResultSchema()
+    result = Reference()
 
 
-class ReferencesSearchResultsSchema(MappingSchema):
+class ReferencesSearchResults(BaseResponseSchema):
     """References search results schema"""
-    results = ReferencesSearchResults(description=_("Results list"))
-
+    results = ReferencesList(description="References search results list")
 
-search_responses = {
-    HTTPOk.code: ReferencesSearchResultsSchema(description=_("Search results")),
-}
-if TEST_MODE:
-    service_params = {}
-else:
-    service_params = {
-        'response_schemas': search_responses
-    }
 
-service = Service(name=REST_REFERENCES_SEARCH_ROUTE,
-                  pyramid_route=REST_REFERENCES_SEARCH_ROUTE,
-                  description="Internal references management")
+references_service = Service(name=REST_REFERENCES_SEARCH_ROUTE,
+                             pyramid_route=REST_REFERENCES_SEARCH_ROUTE,
+                             description="Internal references management")
 
 
-@service.options(validators=(check_cors_origin, set_cors_headers),
-                 **service_params)
+@references_service.options(validators=(check_cors_origin, set_cors_headers))
 def references_options(request):  # pylint: disable=unused-argument
     """References service OPTIONS handler"""
     return ''
 
 
-@service.get(permission=VIEW_SYSTEM_PERMISSION,
-             schema=ReferencesSearchQuerySchema(),
-             validators=(check_cors_origin, colander_querystring_validator,
-                         set_cors_headers),
-             **service_params)
+class ReferencesGetRequest(MappingSchema):
+    """References getter request"""
+    querystring = ReferencesSearchQuery()
+
+
+class ReferencesGetResponse(MappingSchema):
+    """References getter response"""
+    body = ReferencesSearchResults()
+
+
+references_get_responses = rest_responses.copy()
+references_get_responses[HTTPOk.code] = ReferencesGetResponse(
+    description="References search results")
+
+
+@references_service.get(permission=VIEW_SYSTEM_PERMISSION,
+                        schema=ReferencesGetRequest(),
+                        validators=(check_cors_origin, colander_validator, set_cors_headers),
+                        response_schemas=references_get_responses)
 def find_references(request):
     """Returns list of references matching given query"""
-    if TEST_MODE:
-        query = request.params.get('term')
-        content_type = request.params.get('content_type')
-    else:
-        query = request.validated.get('term')
-        content_type = request.validated.get('content_type')
+    params = request.params if TEST_MODE else request.validated
+    query = params.get('term')
     if not query:
-        return []
+        return {
+            'status': STATUS.ERROR.value,
+            'message': 'Missing arguments',
+            'results': []
+        }
+    content_type = params.get('content_type')
     sequence = query_utility(ISequentialIntIds)
     return {
+        'status': STATUS.SUCCESS.value,
         'results': sorted([
             get_sequence_dict(result)
             for result in sequence.find_references(query, content_type, request)
         ], key=lambda x: x['text'])
     }
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/doctests/README.rst` & `pyams_sequence-1.2.3/src/pyams_sequence/doctests/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     >>> config = setUp(hook_zca=True)
     >>> config.registry.settings['zodbconn.uri'] = 'memory://'
 
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
     >>> from pyams_i18n import includeme as include_i18n
     >>> include_i18n(config)
     >>> from pyams_catalog import includeme as include_catalog
@@ -151,15 +153,16 @@
 
 A REST API is also available to look for internal references:
 
     >>> from pyams_sequence.api.rest import find_references
     >>> request = DummyRequest(params={'term': '+b'})
     >>> handle_site_before_traverse(BeforeTraverseEvent(app, request))
     >>> pprint(find_references(request))
-    {'results': [{'id': 'AMS:000000000b', 'text': 'Content title (AMS: b)'}]}
+    {'results': [{'id': 'AMS:000000000b', 'text': 'Content title (AMS: b)'}],
+     'status': 'success'}
 
 
 Sequences schema
 ----------------
 
 Internal references fields are available, to easily search and reference other internal
 objects using their internal ID:
@@ -229,15 +232,15 @@
             data-ajax--url="/api/sequence/references"
             data-minimum-input-length="2">
             <option></option>
             <option id="form-widgets-reference-0"
                     value="AMS:000000000b"
                     selected="selected">Content title (AMS: b)</option>
     </select>
-    <input name="form.widgets.reference-empty-marker" type="hidden" value="1"/>
+    <input name="form.widgets.reference-empty-marker" type="hidden" value="1" />
 
 You can filter internal references using a "content_type" field attribute; this should then
 match a catalog keyword index with this name:
 
     >>> from zope.interface import Interface
     >>> from zope.schema.fieldproperty import FieldProperty
     >>> from pyams_sequence.schema import InternalReferenceField
@@ -265,15 +268,15 @@
             size="1"
             data-placeholder="No selected reference"
             data-ajax--url="/api/sequence/references"
             data-ajax--params='{"content_type": "MyContent"}'
             data-minimum-input-length="2">
             <option></option>
     </select>
-    <input name="form.widgets.reference-empty-marker" type="hidden" value="1"/>
+    <input name="form.widgets.reference-empty-marker" type="hidden" value="1" />
 
 Select options list is actually empty in this test because we don't have a testing catalog
 with "content_type" name!
 
 
 Workflow related functions
 --------------------------
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/generations/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/include.py` & `pyams_sequence-1.2.3/src/pyams_sequence/include.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/interfaces.py` & `pyams_sequence-1.2.3/src/pyams_sequence/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo` & `pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -11,17 +11,14 @@
 "Generated-By: Lingua 4.14\n"
 
 msgid "Can't set last OID to value lower than current one!"
 msgstr ""
 "Vous ne pouvez pas redéfinir la valeur du dernier OID à une valeur "
 "inférieure à sa valeur actuelle"
 
-msgid "Content type"
-msgstr "Type de contenu"
-
 msgid "Full length of hexadecimal ID, not including prefix"
 msgstr "Longueur complète de l'ID hexadécimal, non compris le préfixe"
 
 msgid "Hexadecimal ID length"
 msgstr "Longueur de l'ID hexadécimal"
 
 msgid "Hexadecimal prefix"
@@ -75,41 +72,14 @@
 "Préfixe hexadécimal spécifique ajouté après le préfixe de la séquence ; "
 "généralement paramétré au niveau de la classe, pour concerner tous les "
 "contenus d'un même type..."
 
 msgid "Properties"
 msgstr "Propriétés"
 
-msgid ""
-"Query can be an internal reference OID, eventually prefixed with a \"+\", or "
-"a text query which should match contents title"
-msgstr ""
-"La recherche peut s'effectuer via une référence interne, éventuellement "
-"préfixée par un \"+\", ou via un texte contenu dans le titre des contenus"
-
-msgid "Reference ID"
-msgstr "ID de la référence"
-
-msgid "Reference title"
-msgstr "Titre"
-
-msgid "References search can be restricted to a given content type"
-msgstr ""
-"À indiquer lorsque la recherche doit être contrainte à un type de contenu "
-"spécifique"
-
-msgid "References search string"
-msgstr "Critères de recherche"
-
-msgid "Results list"
-msgstr "Liste de résultats"
-
-msgid "Search results"
-msgstr "Résultats de la recherche"
-
 msgid "Sequence name"
 msgstr "Nom de séquence"
 
 msgid "Sequences generator"
 msgstr "Générateur de séquences"
 
 msgid "Sequences manager"
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po` & `pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2021-07-22 20:11+0200\n"
+"POT-Creation-Date: 2023-04-12 16:01+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -96,58 +96,52 @@
 msgid "List of internal references"
 msgstr ""
 "Vous pouvez définir une liste de références internes en les sélectionnant "
 "une par une ; vous pouvez créer une référence en indiquant un \"+\" "
 "directement suivi de l'identifiant du contenu que vous souhaitez associer, "
 "ou en entrant du texte correspondant au titre du contenu recherché..."
 
-#: src/pyams_sequence/api/rest.py:42
-msgid "References search string"
-msgstr "Critères de recherche"
-
-#: src/pyams_sequence/api/rest.py:43
-msgid ""
-"Query can be an internal reference OID, eventually prefixed with a \"+\", or "
-"a text query which should match contents title"
-msgstr ""
-"La recherche peut s'effectuer via une référence interne, éventuellement préfixée "
-"par un \"+\", ou via un texte contenu dans le titre des contenus"
-
-#: src/pyams_sequence/api/rest.py:47
-msgid "Content type"
-msgstr "Type de contenu"
-
-#: src/pyams_sequence/api/rest.py:48
-msgid "References search can be restricted to a given content type"
-msgstr "À indiquer lorsque la recherche doit être contrainte à un type de contenu spécifique"
-
-#: src/pyams_sequence/api/rest.py:56
-msgid "Reference ID"
-msgstr "ID de la référence"
-
-#: src/pyams_sequence/api/rest.py:58
-msgid "Reference title"
-msgstr "Titre"
-
-#: src/pyams_sequence/api/rest.py:68
-msgid "Results list"
-msgstr "Liste de résultats"
-
-#: src/pyams_sequence/api/rest.py:72
-msgid "Search results"
-msgstr "Résultats de la recherche"
+#: src/pyams_sequence/widget/__init__.py:72
+msgid "No selected reference"
+msgstr "Aucune référence sélectionnée"
 
 #: src/pyams_sequence/zmi/__init__.py:42
 msgid "Sequences manager"
 msgstr "Gestionnaire de séquences"
 
 #: src/pyams_sequence/zmi/__init__.py:55
 msgid "Sequences generator"
 msgstr "Générateur de séquences"
 
 #: src/pyams_sequence/zmi/__init__.py:56
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_sequence/widget/__init__.py:72
-msgid "No selected reference"
-msgstr "Aucune référence sélectionnée"
+#~ msgid "References search string"
+#~ msgstr "Critères de recherche"
+
+#~ msgid ""
+#~ "Query can be an internal reference OID, eventually prefixed with a \"+\", "
+#~ "or a text query which should match contents title"
+#~ msgstr ""
+#~ "La recherche peut s'effectuer via une référence interne, éventuellement "
+#~ "préfixée par un \"+\", ou via un texte contenu dans le titre des contenus"
+
+#~ msgid "Content type"
+#~ msgstr "Type de contenu"
+
+#~ msgid "References search can be restricted to a given content type"
+#~ msgstr ""
+#~ "À indiquer lorsque la recherche doit être contrainte à un type de contenu "
+#~ "spécifique"
+
+#~ msgid "Reference ID"
+#~ msgstr "ID de la référence"
+
+#~ msgid "Reference title"
+#~ msgstr "Titre"
+
+#~ msgid "Results list"
+#~ msgstr "Liste de résultats"
+
+#~ msgid "Search results"
+#~ msgstr "Résultats de la recherche"
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/locales/pyams_sequence.pot` & `pyams_sequence-1.2.3/src/pyams_sequence/locales/pyams_sequence.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2021-07-22 20:11+0200\n"
+"POT-Creation-Date: 2023-04-12 16:01+0200\n"
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
 
 #: ./src/pyams_sequence/utility.py:59
 msgid "Can't set last OID to value lower than current one!"
 msgstr ""
 
 #: ./src/pyams_sequence/interfaces.py:36 ./src/pyams_sequence/interfaces.py:105
 msgid "Hexadecimal prefix"
@@ -82,56 +82,22 @@
 msgid "Internal references"
 msgstr ""
 
 #: ./src/pyams_sequence/interfaces.py:132
 msgid "List of internal references"
 msgstr ""
 
-#: ./src/pyams_sequence/api/rest.py:42
-msgid "References search string"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:43
-msgid ""
-"Query can be an internal reference OID, eventually prefixed with a \"+\", or "
-"a text query which should match contents title"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:47
-msgid "Content type"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:48
-msgid "References search can be restricted to a given content type"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:56
-msgid "Reference ID"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:58
-msgid "Reference title"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:68
-msgid "Results list"
-msgstr ""
-
-#: ./src/pyams_sequence/api/rest.py:72
-msgid "Search results"
+#: ./src/pyams_sequence/widget/__init__.py:72
+msgid "No selected reference"
 msgstr ""
 
 #: ./src/pyams_sequence/zmi/__init__.py:42
 msgid "Sequences manager"
 msgstr ""
 
 #: ./src/pyams_sequence/zmi/__init__.py:55
 msgid "Sequences generator"
 msgstr ""
 
 #: ./src/pyams_sequence/zmi/__init__.py:56
 msgid "Properties"
 msgstr ""
-
-#: ./src/pyams_sequence/widget/__init__.py:72
-msgid "No selected reference"
-msgstr ""
```

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/reference.py` & `pyams_sequence-1.2.3/src/pyams_sequence/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/schema.py` & `pyams_sequence-1.2.3/src/pyams_sequence/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/sequence.py` & `pyams_sequence-1.2.3/src/pyams_sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/tests/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/tests/test_utilsdocs.py` & `pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/tests/test_utilsdocstrings.py` & `pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/utility.py` & `pyams_sequence-1.2.3/src/pyams_sequence/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/widget/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/widget/interfaces.py` & `pyams_sequence-1.2.3/src/pyams_sequence/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/workflow.py` & `pyams_sequence-1.2.3/src/pyams_sequence/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/zmi/__init__.py` & `pyams_sequence-1.2.3/src/pyams_sequence/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence/zmi/reference.py` & `pyams_sequence-1.2.3/src/pyams_sequence/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.2/src/pyams_sequence.egg-info/SOURCES.txt` & `pyams_sequence-1.2.3/src/pyams_sequence.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 setup.py
-docs/HISTORY.txt
-docs/README.txt
+docs/HISTORY.rst
+docs/README.rst
 src/pyams_sequence/__init__.py
 src/pyams_sequence/include.py
 src/pyams_sequence/interfaces.py
 src/pyams_sequence/reference.py
 src/pyams_sequence/schema.py
 src/pyams_sequence/sequence.py
 src/pyams_sequence/utility.py
```

