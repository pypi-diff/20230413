# Comparing `tmp/crabpy_pyramid-1.1.0.tar.gz` & `tmp/crabpy_pyramid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-1.1.0.tar", last modified: Thu Mar 30 15:41:04 2023, max compression
+gzip compressed data, was "crabpy_pyramid-1.2.0.tar", last modified: Thu Apr 13 13:30:20 2023, max compression
```

## Comparing `crabpy_pyramid-1.1.0.tar` & `crabpy_pyramid-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     4237 2023-03-30 15:30:30.000000 crabpy_pyramid-1.1.0/CHANGES.rst
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     1089 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/LICENSE
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)       39 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/MANIFEST.in
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     6437 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/PKG-INFO
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     1326 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/README.rst
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/crabpy_pyramid/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     8719 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     3726 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/capakey.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)    15765 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/crab.py
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/crabpy_pyramid/routes/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     1901 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     4825 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/routes/crab.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     2735 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/crabpy_pyramid/views/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     5610 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)    13969 2023-03-30 15:21:12.000000 crabpy_pyramid-1.1.0/crabpy_pyramid/views/crab.py
-drwxrwxr-x   0 vandercf  (1001) vandercf  (1001)        0 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     6437 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)      676 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)        1 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)       65 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)        1 2023-03-30 15:22:19.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)       42 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)       15 2023-03-30 15:41:04.000000 crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)      173 2023-03-30 15:41:04.946084 crabpy_pyramid-1.1.0/setup.cfg
--rw-rw-r--   0 vandercf  (1001) vandercf  (1001)     1631 2023-03-30 15:26:03.000000 crabpy_pyramid-1.1.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4343 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6373 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.920411 crabpy_pyramid-1.2.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11550 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6556 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3458 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12175 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6373 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      804 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/setup.py
```

### Comparing `crabpy_pyramid-1.1.0/CHANGES.rst` & `crabpy_pyramid-1.2.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+1.2.0 (13-04-2023)
+------------------
+
+- Drop python < 3.8 support
+- Adressenregister implementeren (#165)
+
 1.1.0 (30-03-2023)
--------------------
+------------------
 
 - Overschakelen naar nieuwe AGIV services (#164)
 
 1.0.0 (13-04-2022)
--------------------
+------------------
 
 - Upgrade naar Pyramid 2.0 (#144)
 
 0.12.0 (15-12-2021)
 -------------------
 
 - crabpy en crabpy_pyramid dependencies nakijken (#155)
```

### Comparing `crabpy_pyramid-1.1.0/LICENSE` & `crabpy_pyramid-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/PKG-INFO` & `crabpy_pyramid-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: crabpy_pyramid
-Version: 1.1.0
+Version: 1.2.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
@@ -52,21 +48,27 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.2.0 (13-04-2023)
+------------------
+
+- Drop python < 3.8 support
+- Adressenregister implementeren (#165)
+
 1.1.0 (30-03-2023)
--------------------
+------------------
 
 - Overschakelen naar nieuwe AGIV services (#164)
 
 1.0.0 (13-04-2022)
--------------------
+------------------
 
 - Upgrade naar Pyramid 2.0 (#144)
 
 0.12.0 (15-12-2021)
 -------------------
 
 - crabpy en crabpy_pyramid dependencies nakijken (#155)
@@ -205,9 +207,7 @@
 - Proxy settings in ini file. (#5)
 - Range headers. (#9)
 
 0.1.0a1 (2014-03-19)
 --------------------
 
 - Initial version
-
-
```

### Comparing `crabpy_pyramid-1.1.0/README.rst` & `crabpy_pyramid-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,100 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 from collections import Sequence
 
+from crabpy.client import AdressenRegisterClient
 from crabpy.client import crab_factory
+from crabpy.gateway.adressenregister import Gateway
 from crabpy.gateway.capakey import CapakeyRestGateway
 from crabpy.gateway.crab import CrabGateway
 from pyramid.config import Configurator
 from pyramid.settings import asbool
 from zope.interface import Interface
 
-from crabpy_pyramid.renderers.capakey import (
-    json_list_renderer as capakey_json_list_renderer,
+from crabpy_pyramid.renderers.adressenregister import \
+    json_item_renderer as adresreg_json_item_renderer
+from crabpy_pyramid.renderers.adressenregister import \
+    json_list_renderer as adresreg_json_list_renderer
+from crabpy_pyramid.renderers.capakey import \
     json_item_renderer as capakey_json_item_renderer
-)
-from crabpy_pyramid.renderers.crab import (
-    json_list_renderer as crab_json_list_renderer,
-    json_item_renderer as crab_json_item_renderer
-)
+from crabpy_pyramid.renderers.capakey import \
+    json_list_renderer as capakey_json_list_renderer
+from crabpy_pyramid.renderers.crab import json_item_renderer as crab_json_item_renderer
+from crabpy_pyramid.renderers.crab import json_list_renderer as crab_json_list_renderer
 
 log = logging.getLogger(__name__)
 GENERATE_ETAG_ROUTE_NAMES = set()
 
 
 class ICapakey(Interface):
     pass
 
 
 class ICrab(Interface):
     pass
 
 
+class IAdressenregister(Interface):
+    pass
+
 def _parse_settings(settings):
     defaults = {
         'capakey.include': False,
         'crab.include': True,
-        'cache.file.root': '/tmp/dogpile_data'
+        'adressenregister.include': True,
+        'adressenregister.base_url': 'https://api.basisregisters.vlaanderen.be',
+        'adressenregister.api_key': None,
+        'cache.file.root': '/tmp/dogpile_data',
     }
     args = defaults.copy()
+    if 'adressenregister.api_key' not in settings:
+        log.warning(
+            "No adressenregister.api_key set in settings. "
+            "The api might stop working after reaching the limit of x requests per day."
+        )
 
     # booelean settings
-    for short_key_name in ('capakey.include', 'crab.include'):
+    for short_key_name in ('capakey.include', 'crab.include', 'adressenregister.include'):
         key_name = "crabpy.%s" % short_key_name
         if key_name in settings:
             args[short_key_name] = asbool(settings.get(
                 key_name, defaults.get(short_key_name)
             ))
 
     # string setting
-    for short_key_name in ('proxy.http', 'proxy.https', 'cache.file.root'):
+    for short_key_name in (
+        'proxy.http',
+        'proxy.https',
+        'cache.file.root',
+        'adressenregister.base_url',
+        'adressenregister.api_key'
+    ):
         key_name = "crabpy.%s" % short_key_name
         if key_name in settings:
             args[short_key_name] = settings.get(key_name)
 
     # cache configuration
-    for short_key_name in ('crab.cache_config', 'capakey.cache_config'):
+    for short_key_name in (
+        'crab.cache_config',
+        'capakey.cache_config',
+        'adressenregister.cache_config'
+    ):
         key_name = "crabpy.%s." % short_key_name
         cache_config = {}
         for skey in settings.keys():
             if skey.startswith(key_name):
                 cache_config[skey[len(key_name):]] = settings.get(skey)
         if cache_config:
             args[short_key_name] = cache_config
 
     # crab wsdl settings
-    for short_key_name in ('crab.wsdl', ):
+    for short_key_name in ('crab.wsdl',):
         key_name = "crabpy.%s" % short_key_name
         if key_name in settings:
             args[short_key_name] = settings.get(key_name)
 
     log.debug(settings)
     log.debug(args)
     return args
@@ -118,14 +143,32 @@
     factory = crab_factory(**settings)
     gateway = CrabGateway(factory, cache_config=cache_config)
 
     registry.registerUtility(gateway, ICrab)
     return registry.queryUtility(ICrab)
 
 
+def _build_adressenregister(registry, settings):
+    adressenregister = registry.queryUtility(IAdressenregister)
+    if adressenregister is not None:
+        return adressenregister
+    if 'cache_config' in settings:
+        cache_config = settings['cache_config']
+        del settings['cache_config']
+    else:
+        cache_config = None
+    gateway = Gateway(
+        client=AdressenRegisterClient(settings["base_url"], settings["api_key"]),
+        cache_settings=cache_config
+    )
+
+    registry.registerUtility(gateway, IAdressenregister)
+    return registry.queryUtility(IAdressenregister)
+
+
 def get_capakey(registry):
     """
     Get the Capakey Gateway
 
     :rtype: :class:`crabpy.gateway.capakey.CapakeyRestGateway`
     """
     # argument might be a config or a request
@@ -147,14 +190,29 @@
     regis = getattr(registry, 'registry', None)
     if regis is None:
         regis = registry
 
     return regis.queryUtility(ICrab)
 
 
+def get_adressenregister(registry):
+    """
+    Get the Adresssenregister Gateway
+
+    :rtype: :class:`crabpy.gateway.adressenregister.Gateway`
+    # argument might be a config or a request
+    """
+    # argument might be a config or a request
+    regis = getattr(registry, 'registry', None)
+    if regis is None:
+        regis = registry
+
+    return regis.queryUtility(IAdressenregister)
+
+
 def _get_proxy_settings(settings):
     base_settings = {}
     http = settings.get('proxy.http', None)
     https = settings.get('proxy.https', None)
     if (http or https):
         base_settings["proxy"] = {}
         if "proxy.http" in settings:
@@ -256,14 +314,31 @@
         config.add_renderer('crab_itemjson', crab_json_item_renderer)
         _build_crab(config.registry, crab_settings)
         config.add_directive('get_crab', get_crab)
         config.add_request_method(get_crab, 'crab_gateway')
         config.include('crabpy_pyramid.routes.crab')
         config.scan('crabpy_pyramid.views.crab')
 
+    # adressenregister wordt afgekort tot adresreg
+    adresreg_settings = dict(
+        _filter_settings(settings, 'adressenregister.'),
+        **base_settings
+    )
+
+    if adresreg_settings['include']:
+        log.info('Adding adressen register Gateway.')
+        del adresreg_settings['include']
+        config.add_renderer('adresreg_listjson', adresreg_json_list_renderer)
+        config.add_renderer('adresreg_itemjson', adresreg_json_item_renderer)
+        _build_adressenregister(config.registry, adresreg_settings)
+        config.add_directive('get_adressenregister', get_adressenregister)
+        config.add_request_method(get_adressenregister, 'adressenregister_gateway')
+        config.include('crabpy_pyramid.routes.adressenregister')
+        config.scan('crabpy_pyramid.views.adressenregister')
+
 
 def main(global_config, **settings):
     """
      This function returns a Pyramid WSGI application.
     """
     config = Configurator(settings=settings)
```

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/renderers/crab.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/routes/crab.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/routes/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid/views/crab.py` & `crabpy_pyramid-1.2.0/crabpy_pyramid/views/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.1.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: crabpy-pyramid
-Version: 1.1.0
+Version: 1.2.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
@@ -52,21 +48,27 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.2.0 (13-04-2023)
+------------------
+
+- Drop python < 3.8 support
+- Adressenregister implementeren (#165)
+
 1.1.0 (30-03-2023)
--------------------
+------------------
 
 - Overschakelen naar nieuwe AGIV services (#164)
 
 1.0.0 (13-04-2022)
--------------------
+------------------
 
 - Upgrade naar Pyramid 2.0 (#144)
 
 0.12.0 (15-12-2021)
 -------------------
 
 - crabpy en crabpy_pyramid dependencies nakijken (#155)
@@ -205,9 +207,7 @@
 - Proxy settings in ini file. (#5)
 - Range headers. (#9)
 
 0.1.0a1 (2014-03-19)
 --------------------
 
 - Initial version
-
-
```

### Comparing `crabpy_pyramid-1.1.0/setup.py` & `crabpy_pyramid-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,20 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='1.1.0',
+      version='1.2.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
         "Topic :: Internet :: WWW/HTTP",
         "Intended Audience :: Developers",
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
```

