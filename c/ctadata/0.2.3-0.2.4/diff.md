# Comparing `tmp/ctadata-0.2.3.tar.gz` & `tmp/ctadata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.3.tar", max compression
+gzip compressed data, was "ctadata-0.2.4.tar", max compression
```

## Comparing `ctadata-0.2.3.tar` & `ctadata-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.3/README.md
--rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.3/ctadata/__init__.py
--rw-r--r--   0        0        0     3579 2023-04-13 13:11:58.651143 ctadata-0.2.3/ctadata/api.py
--rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.3/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.3/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-04-13 13:15:22.160977 ctadata-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.4/README.md
+-rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.4/ctadata/__init__.py
+-rw-r--r--   0        0        0     4125 2023-04-13 14:55:57.598706 ctadata-0.2.4/ctadata/api.py
+-rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.4/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.4/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-04-13 14:56:39.307201 ctadata-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.4/PKG-INFO
```

### Comparing `ctadata-0.2.3/README.md` & `ctadata-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.3/ctadata/__init__.py` & `ctadata-0.2.4/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.3/ctadata/api.py` & `ctadata-0.2.4/ctadata/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 from urllib.parse import urljoin
 import requests
 import logging
 from .util import urljoin_multipart
 from . import __version__
 
 
@@ -62,30 +63,46 @@
             return r.json()                        
         except Exception as e:
             logger.error("error: %s", e)
             raise
 
 
     def fetch_and_save_file(self, path, save_to_fn=None):
+        fileinfo = self.get_endpoint('list', path)
+        if fileinfo.status_code not in [200, 207]:
+            logger.error("error: %s", fileinfo.text)
+            raise StorageException(fileinfo.text)
+        
+        fileinfo = fileinfo.json()[0]
+        filesize = int(fileinfo['size'])
+
         total_wrote = 0
 
         if save_to_fn is None:
             save_to_fn = path.split("/")[-1]
 
+        last_pc = 0
+
+        t0 = time.time()
+
         with open(save_to_fn, "wb") as out_file:
             # with get(url, token, downloadservice, stream=True) as f:          
             f = self.get_endpoint('fetch', path, stream=True, chunk_size=self.chunk_size)
 
             logger.info("got response %s", f)
             f.raise_for_status()
             i_chunk = 0
             
             for r in f.iter_content(chunk_size=self.chunk_size):
-                logger.info("wrote %s Mb in %s chunks", total_wrote/1024/1024, i_chunk)
-                out_file.write(r)                
+                pc = int(total_wrote / filesize * 100)
+                if pc > last_pc:
+                    logger.info("wrote %.2f / %.2f Mb in %d chunks in %.2f seconds", total_wrote/1024/1024, filesize/1024/1024, i_chunk, time.time() - t0)
+                    last_pc = pc
+                    
+                out_file.write(r)
                 total_wrote += len(r)
                 i_chunk += 1
 
         return total_wrote
     
 
     def upload_file(self, local_fn, path):
```

### Comparing `ctadata-0.2.3/ctadata/cli.py` & `ctadata-0.2.4/ctadata/cli.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.3/PKG-INFO` & `ctadata-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctadata
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Volodymyr Savchenko
 Author-email: contact@volodymyrsavchenko.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

