# Comparing `tmp/hcf-backend-0.5.1.tar.gz` & `tmp/hcf-backend-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcf-backend-0.5.1.tar", last modified: Tue Apr 11 21:21:50 2023, max compression
+gzip compressed data, was "hcf-backend-0.5.2.tar", last modified: Thu Apr 13 17:20:10 2023, max compression
```

## Comparing `hcf-backend-0.5.1.tar` & `hcf-backend-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       46 2023-04-11 21:21:16.000000 hcf-backend-0.5.1/hcf_backend/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-11 20:57:08.000000 hcf-backend-0.5.1/hcf_backend/backend.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4286 2021-07-13 20:41:18.000000 hcf-backend-0.5.1/hcf_backend/manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.1/hcf_backend/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3896 2023-04-11 21:07:29.000000 hcf-backend-0.5.1/hcf_backend/utils/crawlmanager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13407 2023-04-11 21:12:01.000000 hcf-backend-0.5.1/hcf_backend/utils/hcfpal.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/top_level.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1012 2023-04-11 21:21:23.000000 hcf-backend-0.5.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       46 2023-04-13 16:15:44.000000 hcf-backend-0.5.2/hcf_backend/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2/hcf_backend/backend.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2/hcf_backend/manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2/hcf_backend/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3896 2023-04-11 21:07:29.000000 hcf-backend-0.5.2/hcf_backend/utils/crawlmanager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13380 2023-04-13 16:12:38.000000 hcf-backend-0.5.2/hcf_backend/utils/hcfpal.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/top_level.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1012 2023-04-13 16:15:32.000000 hcf-backend-0.5.2/setup.py
```

### Comparing `hcf-backend-0.5.1/LICENSE` & `hcf-backend-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.1/PKG-INFO` & `hcf-backend-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.1
+Version: 0.5.2
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.1/README.md` & `hcf-backend-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.1/hcf_backend/backend.py` & `hcf-backend-0.5.2/hcf_backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,23 +320,23 @@
             return False
         return self.n_consumed_requests >= self.hcf_consumer_max_requests
 
     def _init_roles(self):
 
         if self.hcf_producer_frontier:
             self.producer = HCFManager(
-                project_id=self.hcf_project_id,
                 frontier=self.hcf_producer_frontier,
+                project_id=self.hcf_project_id,
                 auth=self.hcf_auth,
                 batch_size=self.hcf_producer_batch_size,
             )
 
         if self.hcf_consumer_frontier and self.hcf_consumer_slot:
             self.consumer = HCFManager(
-                project_id=self.hcf_project_id, frontier=self.hcf_consumer_frontier, auth=self.hcf_auth
+                frontier=self.hcf_consumer_frontier, project_id=self.hcf_project_id, auth=self.hcf_auth
             )
 
     def hcf_get_producer_slot(self, request):
         """Determine to which slot should be saved the request.
 
         Depending on the urls, this distribution might or not be evenly among
         the slots.
```

### Comparing `hcf-backend-0.5.1/hcf_backend/manager.py` & `hcf-backend-0.5.2/hcf_backend/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import logging
 import time
 from collections import defaultdict
+from typing import Optional, Dict
 
 import requests as requests_lib
 from scrapinghub import ScrapinghubClient
+from shub_workflow.utils import resolve_project_id
 
 from hcf_backend.utils import get_apikey
 
 
 LOG = logging.getLogger(__name__)
 
 
 class HCFManager(object):
-    def __init__(self, project_id, frontier, auth=None, batch_size=0):
+    def __init__(
+        self, frontier: str, project_id: Optional[int] = None, auth: Optional[str] = None, batch_size: int = 0
+    ):
         if auth is None:
             auth = get_apikey()
         self._client = ScrapinghubClient(auth=auth)
+        project_id = project_id or resolve_project_id()
         self._hcf = self._client.get_project(project_id).frontiers
         self._frontier = self._hcf.get(frontier)
-        self._links_count = defaultdict(int)
-        self._links_to_flush_count = defaultdict(int)
+        self._links_count: Dict[str, int] = defaultdict(int)
+        self._links_to_flush_count: Dict[str, int] = defaultdict(int)
         self._batch_size = batch_size
         self._hcf_retries = 10
 
-    def add_request(self, slot, request):
+    def add_request(self, slot: str, request):
         self._frontier.get(slot).q.add([request])
         self._links_count[slot] += 1
         self._links_to_flush_count[slot] += 1
         if self._batch_size and self._links_to_flush_count[slot] >= self._batch_size:
             return self.flush(slot)
         return 0
```

### Comparing `hcf-backend-0.5.1/hcf_backend/utils/__init__.py` & `hcf-backend-0.5.2/hcf_backend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.1/hcf_backend/utils/crawlmanager.py` & `hcf-backend-0.5.2/hcf_backend/utils/crawlmanager.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.1/hcf_backend/utils/hcfpal.py` & `hcf-backend-0.5.2/hcf_backend/utils/hcfpal.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from itertools import cycle, groupby
 from operator import itemgetter
 from typing import Optional
 
 import humanize
 import requests
 from requests.auth import HTTPBasicAuth
-from retrying import retry
 from shub_workflow.script import BaseScript, SCProjectClass
 from shub_workflow.utils import dash_retry_decorator
 
 from hcf_backend.utils import assign_slotno
 
 
 class HCFPal(SCProjectClass):
```

### Comparing `hcf-backend-0.5.1/hcf_backend.egg-info/PKG-INFO` & `hcf-backend-0.5.2/hcf_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.1
+Version: 0.5.2
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.1/setup.py` & `hcf-backend-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="hcf-backend",
-    version="0.5.1",
+    version="0.5.2",
     description="ScrapyCloud HubStorage frontier backend for Frontera",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/hcf-backend",
     maintainer="Scrapinghub",
     packages=find_packages(),
```

