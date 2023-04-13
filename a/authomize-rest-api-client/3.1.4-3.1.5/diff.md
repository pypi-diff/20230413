# Comparing `tmp/authomize-rest-api-client-3.1.4.tar.gz` & `tmp/authomize-rest-api-client-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.1.4.tar", last modified: Wed Mar 22 13:57:12 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.1.5.tar", last modified: Thu Apr 13 14:25:11 2023, max compression
```

## Comparing `authomize-rest-api-client-3.1.4.tar` & `authomize-rest-api-client-3.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69821 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22617 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183922 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63846 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-22 13:56:45.000000 authomize-rest-api-client-3.1.4/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-03-22 13:57:12.000000 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-03-22 13:57:12.000000 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 13:57:12.000000 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-03-22 13:57:12.000000 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-22 13:57:12.000000 authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-03-22 13:57:12.521533 authomize-rest-api-client-3.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-03-22 13:56:49.000000 authomize-rest-api-client-3.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69815 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22617 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   183916 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63846 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 14:24:51.000000 authomize-rest-api-client-3.1.5/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 14:25:11.000000 authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-13 14:25:11.966683 authomize-rest-api-client-3.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-04-13 14:24:55.000000 authomize-rest-api-client-3.1.5/setup.py
```

### Comparing `authomize-rest-api-client-3.1.4/LICENSE.txt` & `authomize-rest-api-client-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/README.md` & `authomize-rest-api-client-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-03-22T13:34:19+00:00
+#   timestamp: 2023-04-13T14:20:13+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -291,15 +291,15 @@
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         'Other',
-        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`Git Repository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`Virtual Machine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
+        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
         None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
@@ -844,15 +844,15 @@
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         'Other',
-        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`Git Repository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`Virtual Machine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
+        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
         None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
@@ -999,15 +999,15 @@
     name: constr(min_length=1) = Field(
         ...,
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         'Other',
-        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`Git Repository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`Virtual Machine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
+        description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
     originType: Optional[str] = Field(
         None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
```

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874966128410732%*

 * *Differences: {"'components'": "{'schemas': {'AssetSchema': {'properties': {'type': {'description': 'The asset "*

 * *                 'types that are supported by Authomize **Mandatory**\\n\\nPermitted '*

 * *                 'values:\\n\\n   •\\t`Application` (federation) \\n   •\\t`Database`\\n   '*

 * *                 '•\\t`Drive`\\n   •\\t`File`\\n   •\\t`Folder`\\n   •\\t`GitRepository`\\n   '*

 * *                 '•\\t`Integration`\\n   •\\t`Project`\\n   •\\t`Site`\\n   •\\t`Table`\\n   '*

 * *                 '•\\t`Ticket`\\n   •\\t`V […]*

```diff
@@ -231,15 +231,15 @@
                     "type": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AssetType"
                             }
                         ],
                         "default": "Other",
-                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`Git Repository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`Virtual Machine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
+                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`GitRepository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`VirtualMachine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
                     },
                     "uniqueId": {
                         "description": "Asset ID. **Mandatory, must be unique.**\n",
                         "minLength": 1,
                         "title": "Uniqueid",
                         "type": "string"
                     }
@@ -1206,15 +1206,15 @@
                     "type": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AssetType"
                             }
                         ],
                         "default": "Other",
-                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`Git Repository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`Virtual Machine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
+                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`GitRepository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`VirtualMachine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
                     },
                     "uniqueId": {
                         "description": "Asset ID. **Mandatory, must be unique.**\n",
                         "minLength": 1,
                         "title": "Uniqueid",
                         "type": "string"
                     }
@@ -3121,15 +3121,15 @@
                     "type": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AssetType"
                             }
                         ],
                         "default": "Other",
-                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`Git Repository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`Virtual Machine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
+                        "description": "The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   \u2022\t`Application` (federation) \n   \u2022\t`Database`\n   \u2022\t`Drive`\n   \u2022\t`File`\n   \u2022\t`Folder`\n   \u2022\t`GitRepository`\n   \u2022\t`Integration`\n   \u2022\t`Project`\n   \u2022\t`Site`\n   \u2022\t`Table`\n   \u2022\t`Ticket`\n   \u2022\t`VirtualMachine`\n   \u2022\t`Other`\n\nIf the asset type does not exist use `Other`.\n"
                     },
                     "uniqueId": {
                         "description": "Asset ID. **Mandatory, must be unique.**\n",
                         "minLength": 1,
                         "title": "Uniqueid",
                         "type": "string"
                     }
@@ -3669,15 +3669,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.3",
+        "version": "3.1.4",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5418,15 +5418,15 @@
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-03-22T13:14:19.738299+00:00",
+                        "example": "2023-04-11T05:48:47.081171+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-3.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.1.5/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.4/setup.py` & `authomize-rest-api-client-3.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.1.4',
+        version='3.1.5',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

