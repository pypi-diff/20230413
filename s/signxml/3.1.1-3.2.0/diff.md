# Comparing `tmp/signxml-3.1.1.tar.gz` & `tmp/signxml-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signxml-3.1.1.tar", last modified: Sat Apr  8 17:05:58 2023, max compression
+gzip compressed data, was "signxml-3.2.0.tar", last modified: Thu Apr 13 06:22:34 2023, max compression
```

## Comparing `signxml-3.1.1.tar` & `signxml-3.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.903171 signxml-3.1.1/
--rw-r--r--   0 kislyuk    (501) staff       (20)    11324 2016-06-14 14:22:58.000000 signxml-3.1.1/LICENSE
--rw-r--r--   0 kislyuk    (501) staff       (20)       66 2022-11-14 00:33:49.000000 signxml-3.1.1/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      589 2022-11-13 06:37:55.000000 signxml-3.1.1/NOTICE
--rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-04-08 17:05:58.903255 signxml-3.1.1/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    15648 2023-04-08 16:53:45.000000 signxml-3.1.1/README.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)      288 2023-04-08 16:53:45.000000 signxml-3.1.1/pyproject.toml
--rw-r--r--   0 kislyuk    (501) staff       (20)      177 2023-04-08 17:05:58.903514 signxml-3.1.1/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1809 2023-04-08 17:04:57.000000 signxml-3.1.1/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.897920 signxml-3.1.1/signxml/
--rw-r--r--   0 kislyuk    (501) staff       (20)      612 2022-11-27 19:29:34.000000 signxml-3.1.1/signxml/__init__.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.899371 signxml-3.1.1/signxml/__pyinstaller/
--rw-r--r--   0 kislyuk    (501) staff       (20)      224 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/__pyinstaller/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      231 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/__pyinstaller/hook-signxml.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     9569 2023-04-08 16:53:45.000000 signxml-3.1.1/signxml/algorithms.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      614 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6770 2022-11-30 03:47:11.000000 signxml-3.1.1/signxml/processor.py
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/py.typed
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900077 signxml-3.1.1/signxml/schemas/
--rw-r--r--   0 kislyuk    (501) staff       (20)    10293 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig-core-schema.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)      900 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig1-schema.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)     4664 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig11-schema.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)    24308 2023-01-09 03:45:25.000000 signxml-3.1.1/signxml/signer.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900311 signxml-3.1.1/signxml/util/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8963 2023-04-08 16:53:42.000000 signxml-3.1.1/signxml/util/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    31486 2023-04-08 16:53:42.000000 signxml-3.1.1/signxml/verifier.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900676 signxml-3.1.1/signxml/xades/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1938 2022-11-27 20:16:00.000000 signxml-3.1.1/signxml/xades/__init__.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.902513 signxml-3.1.1/signxml/xades/schemas/
--rw-r--r--   0 kislyuk    (501) staff       (20)    21737 2022-10-29 20:33:16.000000 signxml-3.1.1/signxml/xades/schemas/XAdES.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)    24227 2022-10-29 20:33:33.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201506.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)    24056 2022-10-29 20:34:00.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201601.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)     2664 2022-10-29 20:34:18.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201506.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)     3184 2022-10-29 20:32:55.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201601.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)      910 2022-10-29 20:31:58.000000 signxml-3.1.1/signxml/xades/schemas/XAdESv141.xsd
--rw-r--r--   0 kislyuk    (501) staff       (20)    20109 2023-04-08 16:53:45.000000 signxml-3.1.1/signxml/xades/xades.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.899024 signxml-3.1.1/signxml.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)      931 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       64 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/entry_points.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      123 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/top_level.txt
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.902760 signxml-3.1.1/test/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    38122 2023-04-08 17:03:48.000000 signxml-3.1.1/test/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983986 signxml-3.2.0/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11324 2021-10-07 21:38:03.000000 signxml-3.2.0/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       66 2022-12-16 21:17:49.000000 signxml-3.2.0/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      589 2022-12-16 21:17:49.000000 signxml-3.2.0/NOTICE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16566 2023-04-13 06:22:34.984188 signxml-3.2.0/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15648 2023-03-04 20:01:48.000000 signxml-3.2.0/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      288 2023-03-29 02:44:36.000000 signxml-3.2.0/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      177 2023-04-13 06:22:34.984801 signxml-3.2.0/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1809 2023-04-13 06:21:28.000000 signxml-3.2.0/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.975156 signxml-3.2.0/signxml/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      612 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.978272 signxml-3.2.0/signxml/__pyinstaller/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2022-08-21 15:15:01.000000 signxml-3.2.0/signxml/__pyinstaller/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      231 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/__pyinstaller/hook-signxml.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9569 2023-03-29 03:01:39.000000 signxml-3.2.0/signxml/algorithms.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      614 2022-08-24 04:57:56.000000 signxml-3.2.0/signxml/exceptions.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6722 2023-04-13 05:53:23.000000 signxml-3.2.0/signxml/processor.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2022-08-24 04:57:56.000000 signxml-3.2.0/signxml/py.typed
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.979439 signxml-3.2.0/signxml/schemas/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10293 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig-core-schema.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      900 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig1-schema.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4664 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig11-schema.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24308 2022-12-27 03:50:38.000000 signxml-3.2.0/signxml/signer.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.979817 signxml-3.2.0/signxml/util/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8963 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/util/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    31899 2023-04-13 05:53:23.000000 signxml-3.2.0/signxml/verifier.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.980562 signxml-3.2.0/signxml/xades/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1938 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/xades/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983204 signxml-3.2.0/signxml/xades/schemas/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    21737 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24227 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201506.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24056 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201601.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2664 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201506.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3184 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201601.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      910 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdESv141.xsd
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    20109 2023-04-13 04:51:59.000000 signxml-3.2.0/signxml/xades/xades.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.977434 signxml-3.2.0/signxml.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16566 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      931 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       64 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      123 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/top_level.txt
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983594 signxml-3.2.0/test/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    38559 2023-04-13 05:53:18.000000 signxml-3.2.0/test/test.py
```

### Comparing `signxml-3.1.1/LICENSE` & `signxml-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/NOTICE` & `signxml-3.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/PKG-INFO` & `signxml-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `signxml-3.1.1/README.rst` & `signxml-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/setup.py` & `signxml-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="signxml",
-    version="3.1.1",
+    version="3.2.0",
     url="https://github.com/kislyuk/signxml",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Python XML Signature and XAdES library",
     long_description=open("README.rst").read(),
     python_requires=">=3.7",
```

### Comparing `signxml-3.1.1/signxml/__init__.py` & `signxml-3.2.0/signxml/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/algorithms.py` & `signxml-3.2.0/signxml/algorithms.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/exceptions.py` & `signxml-3.2.0/signxml/exceptions.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/processor.py` & `signxml-3.2.0/signxml/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import warnings
 from typing import Any, List, Tuple
 from xml.etree import ElementTree as stdlibElementTree
 
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.hashes import Hash
 from lxml import etree
 
@@ -49,18 +48,18 @@
     def get_root(self, data):
         if isinstance(data, (str, bytes)):
             return self._fromstring(data)
         elif isinstance(data, stdlibElementTree.Element):
             # TODO: add debug level logging statement re: performance impact here
             return self._fromstring(stdlibElementTree.tostring(data, encoding="utf-8"))
         else:
-            # HACK: deep copy won't keep root's namespaces resulting in an invalid digest
-            # We use a copy so we can modify the tree
-            # TODO: turn this off for xmlenc
-            return self._fromstring(etree.tostring(data))
+            # Create a separate copy of the node so we can modify the tree and avoid any c14n inconsistencies from
+            # namespaces propagating from parent nodes. The lxml docs recommend using copy.deepcopy for this, but it
+            # doesn't seem to preserve namespaces. It would be nice to find a less heavy-handed way of doing this.
+            return self._fromstring(self._tostring(data))
 
 
 class XMLSignatureProcessor(XMLProcessor):
     schema_files = ["xmldsig1-schema.xsd"]
 
     # See https://tools.ietf.org/html/rfc5656
     known_ecdsa_curves = {
@@ -122,18 +121,14 @@
                 node,
                 method="c14n",
                 exclusive=exclusive,
                 with_comments=with_comments,
                 inclusive_ns_prefixes=inclusive_ns_prefixes,
             )
         if exclusive is False and self.excise_empty_xmlns_declarations is True:
-            warnings.warn(
-                "excise_empty_xmlns_declarations is deprecated and will be removed in a future SignXML release",
-                DeprecationWarning,
-            )
             # Incorrect legacy behavior. See also:
             # - https://github.com/XML-Security/signxml/issues/193
             # - http://www.w3.org/TR/xml-c14n, "namespace axis"
             # - http://www.w3.org/TR/xml-c14n2/#sec-Namespace-Processing
             c14n = c14n.replace(b' xmlns=""', b"")
         logger.debug("Canonicalized string (exclusive=%s, with_comments=%s): %s", exclusive, with_comments, c14n)
         return c14n
```

### Comparing `signxml-3.1.1/signxml/schemas/xmldsig-core-schema.xsd` & `signxml-3.2.0/signxml/schemas/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/schemas/xmldsig1-schema.xsd` & `signxml-3.2.0/signxml/schemas/xmldsig1-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/schemas/xmldsig11-schema.xsd` & `signxml-3.2.0/signxml/schemas/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/signer.py` & `signxml-3.2.0/signxml/signer.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/util/__init__.py` & `signxml-3.2.0/signxml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/verifier.py` & `signxml-3.2.0/signxml/verifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,20 @@
         for transform in transforms:
             algorithm = transform.get("Algorithm")
             try:
                 c14n_algorithm_from_transform = CanonicalizationMethod(algorithm)
             except ValueError:
                 continue
             inclusive_ns_prefixes = self._get_inclusive_ns_prefixes(transform)
+
+            # Create a separate copy of the node so we can modify the tree and avoid any c14n inconsistencies from
+            # namespaces propagating from parent nodes. The lxml docs recommend using copy.deepcopy for this, but it
+            # doesn't seem to preserve namespaces. It would be nice to find a less heavy-handed way of doing this.
+            payload = self._fromstring(self._tostring(payload))
+
             payload = self._c14n(
                 payload, algorithm=c14n_algorithm_from_transform, inclusive_ns_prefixes=inclusive_ns_prefixes
             )
             c14n_applied = True
 
         if not c14n_applied and not isinstance(payload, (str, bytes)):
             payload = self._c14n(payload, algorithm=self._default_reference_c14n_method)
```

### Comparing `signxml-3.1.1/signxml/xades/__init__.py` & `signxml-3.2.0/signxml/xades/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdES.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdES.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201506.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201601.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201506.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201601.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/schemas/XAdESv141.xsd` & `signxml-3.2.0/signxml/xades/schemas/XAdESv141.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml/xades/xades.py` & `signxml-3.2.0/signxml/xades/xades.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/signxml.egg-info/PKG-INFO` & `signxml-3.2.0/signxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `signxml-3.1.1/signxml.egg-info/SOURCES.txt` & `signxml-3.2.0/signxml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signxml-3.1.1/test/test.py` & `signxml-3.2.0/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,14 +636,24 @@
     def test_payload_c14n(self):
         doc = etree.fromstring('<abc xmlns="http://example.com"><foo xmlns="">bar</foo></abc>')
         self.assertEqual(
             XMLSignatureProcessor()._c14n(doc, algorithm=CanonicalizationMethod.CANONICAL_XML_1_1),
             b'<abc xmlns="http://example.com"><foo xmlns="">bar</foo></abc>',
         )
 
+    def test_xmlns_insulation_of_reference_c14n(self):
+        cert, key = self.load_example_keys()
+        doc = etree.fromstring(
+            '<rDE xmlns="http://example.com/ns1">'
+            '<DE Id="target"><dDVId>9</dDVId><gOpeDE><iTipEmi>1</iTipEmi></gOpeDE></DE>'
+            "</rDE>"
+        )
+        root = XMLSigner().sign(doc, cert=cert, key=key, reference_uri="#target")
+        XMLVerifier().verify(root, x509_cert=cert)
+
     def test_verify_config(self):
         data = etree.parse(self.example_xml_files[0]).getroot()
         cert, key = self.load_example_keys()
         signer = XMLSigner()
         signed = signer.sign(data, cert=cert, key=key)
         verifier = XMLVerifier()
         verifier.verify(signed, x509_cert=cert)
```

