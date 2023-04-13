# Comparing `tmp/ctadata-0.2.1.tar.gz` & `tmp/ctadata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.1.tar", max compression
+gzip compressed data, was "ctadata-0.2.2.tar", max compression
```

## Comparing `ctadata-0.2.1.tar` & `ctadata-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1976 2023-04-12 15:32:43.928799 ctadata-0.2.1/README.md
--rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.1/ctadata/__init__.py
--rw-r--r--   0        0        0     3220 2023-04-13 11:56:04.865225 ctadata-0.2.1/ctadata/api.py
--rw-r--r--   0        0        0      850 2023-04-13 12:12:59.548331 ctadata-0.2.1/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.1/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-04-13 12:35:47.719374 ctadata-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 ctadata-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.2/README.md
+-rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.2/ctadata/__init__.py
+-rw-r--r--   0        0        0     3281 2023-04-13 12:57:13.282724 ctadata-0.2.2/ctadata/api.py
+-rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.2/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.2/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-04-13 13:02:26.559246 ctadata-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.2/PKG-INFO
```

### Comparing `ctadata-0.2.1/ctadata/__init__.py` & `ctadata-0.2.2/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.1/ctadata/api.py` & `ctadata-0.2.2/ctadata/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
     def upload_file(self, local_fn, path):
         url = self.construct_endpoint_url('upload', path)
         logger.info("uploading %s to %s", local_fn, url)
 
         with open(local_fn, "rb") as f:
             r = requests.post(url, data=f, params={'token': self.token, 'ctadata_version': __version__}, stream=True)
+            logger.info("upload result: %s %s", r, r.json())
 
         if r.status_code != 200:
             logger.error("error: %s", r.text)
             raise StorageException(r.text)
 
         return r.json()
```

### Comparing `ctadata-0.2.1/ctadata/cli.py` & `ctadata-0.2.2/ctadata/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 import logging
+import os
 import click
 
 from .api import APIClient
 
 
 logger = logging.getLogger(__name__)
 
 @click.group
 @click.pass_context
-def main(ctx):
+def cli(ctx):
     ctx.obj['api'] = APIClient()
+    ctx.obj['api'].token = os.getenv("JUPYTERHUB_API_TOKEN")
+    ctx.obj['api'].downloadservice = os.getenv("CTADS_URL", "http://hub:5000/services/downloadservice/")
     logging.basicConfig(level='INFO')
 
 
-@main.command("list")
+@cli.command("list")
 @click.pass_context
 @click.argument("path", type=str)
 def list_path(ctx, path):
     r = ctx.obj['api'].list_dir(path)
 
     if isinstance(r, list):
         for fn in r:
             click.echo(fn)
     else:
         logger.warning("problem listing files: %s", r)
 
 
-@main.command("get")
+@cli.command("get")
 @click.pass_context
 @click.argument("path", type=str)
 def get_path(ctx, path):
     ctx.obj['api'].fetch_and_save_file(path)
 
 
-@main.command("put")
+@cli.command("put")
 @click.pass_context
 @click.argument("file", type=click.Path(exists=True))
 @click.argument("path", type=str)
 def put_path(ctx, file, path):
-    ctx.obj['api'].upload_file(file, path)
+    ctx.obj['api'].upload_file(file, path)
+
+
+def main():
+    cli(obj={})
```

