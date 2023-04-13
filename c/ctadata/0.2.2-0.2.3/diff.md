# Comparing `tmp/ctadata-0.2.2.tar.gz` & `tmp/ctadata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.2.tar", max compression
+gzip compressed data, was "ctadata-0.2.3.tar", max compression
```

## Comparing `ctadata-0.2.2.tar` & `ctadata-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.2/README.md
--rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.2/ctadata/__init__.py
--rw-r--r--   0        0        0     3281 2023-04-13 12:57:13.282724 ctadata-0.2.2/ctadata/api.py
--rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.2/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.2/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-04-13 13:02:26.559246 ctadata-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.3/README.md
+-rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.3/ctadata/__init__.py
+-rw-r--r--   0        0        0     3579 2023-04-13 13:11:58.651143 ctadata-0.2.3/ctadata/api.py
+-rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.3/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.3/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-04-13 13:15:22.160977 ctadata-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.3/PKG-INFO
```

### Comparing `ctadata-0.2.2/README.md` & `ctadata-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.2/ctadata/__init__.py` & `ctadata-0.2.3/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.2/ctadata/api.py` & `ctadata-0.2.3/ctadata/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,15 +89,23 @@
     
 
     def upload_file(self, local_fn, path):
         url = self.construct_endpoint_url('upload', path)
         logger.info("uploading %s to %s", local_fn, url)
 
         with open(local_fn, "rb") as f:
-            r = requests.post(url, data=f, params={'token': self.token, 'ctadata_version': __version__}, stream=True)
+            stats = {'total_size': 0}
+
+            def generate(stats):
+                while r := f.read(self.chunk_size):
+                    stats['total_size'] += len(r)
+                    logger.info("uploaded %s Mb", stats['total_size']/1024/1024)
+                    yield r
+
+            r = requests.post(url, data=generate(stats), params={'token': self.token, 'ctadata_version': __version__}, stream=True)
             logger.info("upload result: %s %s", r, r.json())
 
         if r.status_code != 200:
             logger.error("error: %s", r.text)
             raise StorageException(r.text)
 
         return r.json()
```

### Comparing `ctadata-0.2.2/ctadata/cli.py` & `ctadata-0.2.3/ctadata/cli.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.2/PKG-INFO` & `ctadata-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctadata
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Volodymyr Savchenko
 Author-email: contact@volodymyrsavchenko.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

