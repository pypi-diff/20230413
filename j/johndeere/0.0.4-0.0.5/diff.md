# Comparing `tmp/johndeere-0.0.4.tar.gz` & `tmp/johndeere-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johndeere-0.0.4.tar", last modified: Sun Mar 12 18:37:31 2023, max compression
+gzip compressed data, was "johndeere-0.0.5.tar", last modified: Thu Apr 13 19:44:20 2023, max compression
```

## Comparing `johndeere-0.0.4.tar` & `johndeere-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-03-12 18:37:31.434281 johndeere-0.0.4/
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1825 2023-03-12 18:36:28.000000 johndeere-0.0.4/.gitignore
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      634 2023-03-12 18:37:31.434145 johndeere-0.0.4/PKG-INFO
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       34 2023-03-08 18:34:37.000000 johndeere-0.0.4/README.md
-drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-03-12 18:37:31.432369 johndeere-0.0.4/johndeere/
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      126 2023-03-08 10:45:38.000000 johndeere-0.0.4/johndeere/__init__.py
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1415 2023-03-10 19:48:08.000000 johndeere-0.0.4/johndeere/client.py
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1593 2023-03-08 10:43:07.000000 johndeere-0.0.4/johndeere/enum.py
-drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-03-12 18:37:31.433926 johndeere-0.0.4/johndeere/mixins/
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     5997 2023-03-12 10:45:44.000000 johndeere-0.0.4/johndeere/mixins/fields.py
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     2450 2023-03-10 19:48:35.000000 johndeere-0.0.4/johndeere/mixins/org.py
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     2851 2023-03-12 10:48:26.000000 johndeere-0.0.4/johndeere/mixins/private.py
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      245 2023-03-10 19:46:25.000000 johndeere-0.0.4/johndeere/typing.py
-drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-03-12 18:37:31.433331 johndeere-0.0.4/johndeere.egg-info/
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      634 2023-03-12 18:37:31.000000 johndeere-0.0.4/johndeere.egg-info/PKG-INFO
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      352 2023-03-12 18:37:31.000000 johndeere-0.0.4/johndeere.egg-info/SOURCES.txt
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)        1 2023-03-12 18:37:31.000000 johndeere-0.0.4/johndeere.egg-info/dependency_links.txt
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       58 2023-03-12 18:37:31.000000 johndeere-0.0.4/johndeere.egg-info/requires.txt
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       10 2023-03-12 18:37:31.000000 johndeere-0.0.4/johndeere.egg-info/top_level.txt
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       38 2023-03-12 18:37:31.434327 johndeere-0.0.4/setup.cfg
--rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1130 2023-03-12 18:37:26.000000 johndeere-0.0.4/setup.py
+drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-04-13 19:44:20.209731 johndeere-0.0.5/
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1825 2023-03-12 18:36:28.000000 johndeere-0.0.5/.gitignore
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      634 2023-04-13 19:44:20.209581 johndeere-0.0.5/PKG-INFO
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       34 2023-03-08 18:34:37.000000 johndeere-0.0.5/README.md
+drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-04-13 19:44:20.206514 johndeere-0.0.5/johndeere/
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      126 2023-03-08 10:45:38.000000 johndeere-0.0.5/johndeere/__init__.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1483 2023-04-13 19:43:29.000000 johndeere-0.0.5/johndeere/client.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1593 2023-03-08 10:43:07.000000 johndeere-0.0.5/johndeere/enum.py
+drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-04-13 19:44:20.209315 johndeere-0.0.5/johndeere/mixins/
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1763 2023-04-13 19:43:11.000000 johndeere-0.0.5/johndeere/mixins/clients.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      269 2023-04-13 19:37:07.000000 johndeere-0.0.5/johndeere/mixins/commons.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     5859 2023-04-13 19:42:17.000000 johndeere-0.0.5/johndeere/mixins/fields.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     2450 2023-03-10 19:48:35.000000 johndeere-0.0.5/johndeere/mixins/org.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     2851 2023-03-12 10:48:26.000000 johndeere-0.0.5/johndeere/mixins/private.py
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      245 2023-03-10 19:46:25.000000 johndeere-0.0.5/johndeere/typing.py
+drwxr-xr-x   0 arbyn.argabioso   (501) staff       (20)        0 2023-04-13 19:44:20.207801 johndeere-0.0.5/johndeere.egg-info/
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      634 2023-04-13 19:44:20.000000 johndeere-0.0.5/johndeere.egg-info/PKG-INFO
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)      408 2023-04-13 19:44:20.000000 johndeere-0.0.5/johndeere.egg-info/SOURCES.txt
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)        1 2023-04-13 19:44:20.000000 johndeere-0.0.5/johndeere.egg-info/dependency_links.txt
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       58 2023-04-13 19:44:20.000000 johndeere-0.0.5/johndeere.egg-info/requires.txt
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       10 2023-04-13 19:44:20.000000 johndeere-0.0.5/johndeere.egg-info/top_level.txt
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)       38 2023-04-13 19:44:20.209775 johndeere-0.0.5/setup.cfg
+-rw-r--r--   0 arbyn.argabioso   (501) staff       (20)     1130 2023-04-13 19:44:08.000000 johndeere-0.0.5/setup.py
```

### Comparing `johndeere-0.0.4/.gitignore` & `johndeere-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `johndeere-0.0.4/PKG-INFO` & `johndeere-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johndeere
-Version: 0.0.4
+Version: 0.0.5
 Summary: John Deere API wrapper.
 Author: Arbyn Acosta
 Author-email: arbyn.acosta@gmail.com
 Keywords: john deere,john-deere,john deere api,john-deere-api,john deere client,john-deere-client
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `johndeere-0.0.4/johndeere/client.py` & `johndeere-0.0.5/johndeere/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import logging
 import os
 
 from yarl import URL
 
+from johndeere.mixins.clients import ClientsMixin
 from johndeere.mixins.fields import FieldsMixin
 from johndeere.mixins.org import OrganizationsMixin
 from johndeere.mixins.private import PrivateMixin
 
 
 __all__ = [
     # Class exports
@@ -19,14 +20,15 @@
 
 DEFAULT_LOGGER = logging.getLogger("johndeere")
 
 
 class Client(
     PrivateMixin,
     OrganizationsMixin,
+    ClientsMixin,
     FieldsMixin,
 ):
 
     BASE_URL = URL("https://sandboxapi.deere.com/platform/")
 
     def __init__(self, *args, **kwargs):
         self._logger = kwargs.get("logger", DEFAULT_LOGGER)
```

### Comparing `johndeere-0.0.4/johndeere/enum.py` & `johndeere-0.0.5/johndeere/enum.py`

 * *Files identical despite different names*

### Comparing `johndeere-0.0.4/johndeere/mixins/fields.py` & `johndeere-0.0.5/johndeere/mixins/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 """Module containing class mixins for field endpoints."""
 
 from __future__ import annotations
 
 from johndeere.enum import ExtendableStrEnum
+from johndeere.mixins.commons import RecordStatuses
 from johndeere.typing import JSONLike
 
 
 __all__ = [
     # Class exports
     "FieldsMixin",
-    "RecordStatuses",
 ]
 
 
-class RecordStatuses(ExtendableStrEnum):
-    ALL: str = "ALL"
-    ACTIVE: str = "ACTIVE"
-    ARCHIVED: str = "ARCHIVED"
-
-
 class FieldOperationTypes(ExtendableStrEnum):
     APPLICATION: str = "APPLICATION"
     HARVEST: str = "HARVEST"
     SEEDING: str = "SEEDING"
     TILLAGE: str = "TILLAGE"
 
 
@@ -38,15 +32,14 @@
         self,
         org_id: int | str,
         *,
         field_name: str | None = None,
         farm_name: str | None = None,
         client_name: str | None = None,
         record_filter: str = RecordStatuses.ACTIVE.value,
-        embed: str | list[str] | None = None,
     ) -> JSONLike:
         """Get the list of fields within a specified organization.
 
         Arguments:
             org_id: A String or integer ID of the organization.
             field_name: Optional string argument to filter fields by name.
             farm_name: Optional string argument to filter fields by farm.
```

### Comparing `johndeere-0.0.4/johndeere/mixins/org.py` & `johndeere-0.0.5/johndeere/mixins/org.py`

 * *Files identical despite different names*

### Comparing `johndeere-0.0.4/johndeere/mixins/private.py` & `johndeere-0.0.5/johndeere/mixins/private.py`

 * *Files identical despite different names*

### Comparing `johndeere-0.0.4/johndeere.egg-info/PKG-INFO` & `johndeere-0.0.5/johndeere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johndeere
-Version: 0.0.4
+Version: 0.0.5
 Summary: John Deere API wrapper.
 Author: Arbyn Acosta
 Author-email: arbyn.acosta@gmail.com
 Keywords: john deere,john-deere,john deere api,john-deere-api,john deere client,john-deere-client
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `johndeere-0.0.4/setup.py` & `johndeere-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "aenum<4.0,>=3.1.11",
     "yarl<2.0,>=1.8.2",
 ]
 
 
 setuptools.setup(
     name="johndeere",
-    version="0.0.4",
+    version="0.0.5",
     author="Arbyn Acosta",
     author_email="arbyn.acosta@gmail.com",
     # url="https://github.com/adw0rd/instagrapi",
     install_requires=REQUIREMENTS,
     keywords=[
         "john deere",
         "john-deere",
```

