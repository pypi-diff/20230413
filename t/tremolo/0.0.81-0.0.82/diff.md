# Comparing `tmp/tremolo-0.0.81.tar.gz` & `tmp/tremolo-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.81.tar", last modified: Wed Apr 12 13:07:53 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.82.tar", last modified: Wed Apr 12 23:55:57 2023, max compression
```

## Comparing `tremolo-0.0.81.tar` & `tremolo-0.0.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 13:07:53.000000 tremolo-0.0.81/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.81/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-12 13:07:53.000000 tremolo-0.0.81/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-12 13:07:35.000000 tremolo-0.0.81/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11735 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13633 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8527 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     5466 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 23:55:57.000000 tremolo-0.0.82/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.82/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-12 23:55:57.000000 tremolo-0.0.82/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-12 23:52:43.000000 tremolo-0.0.82/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11749 2023-04-12 23:50:45.000000 tremolo-0.0.82/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.82/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     8527 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     5466 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.81/PKG-INFO` & `tremolo-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.81
+Version: 0.0.82
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

### Comparing `tremolo-0.0.81/README.md` & `tremolo-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/setup.py` & `tremolo-0.0.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.81',
+    version='0.0.82',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.81/tremolo/http_server.py` & `tremolo-0.0.82/tremolo/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             self._server['context'].set('options', options)
 
         data = await func(**self._server)
 
         if data is None:
             return options
 
-        if not isinstance(data, (bytes, bytearray, str)):
+        if not isinstance(data, (bytes, bytearray, str, tuple)):
             return
 
         if 'status' in options:
             self._server['response'].set_status(*options['status'])
 
         if 'content_type' in options:
             self._server['response'].set_content_type(options['content_type'])
@@ -155,15 +155,15 @@
         except AttributeError:
             data = await agen
 
             if data is None:
                 self._server['response'].close()
                 return
 
-            if not isinstance(data, (bytes, bytearray, str)):
+            if not isinstance(data, (bytes, bytearray, str, tuple)):
                 return
 
             is_agen = False
 
         status = self._server['response'].get_status()
         no_content = status[0] in (204, 304) or 100 <= status[0] < 200
         self._server['response'].http_chunked = options.get(
```

### Comparing `tremolo-0.0.81/tremolo/lib/connection_pool.py` & `tremolo-0.0.82/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/http_exception.py` & `tremolo-0.0.82/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/http_protocol.py` & `tremolo-0.0.82/tremolo/lib/http_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,24 +155,25 @@
         if self.options['debug']:
             data = b'<ul><li>%s</li></ul>' % '</li><li>'.join(
                 traceback.TracebackException.from_exception(exc).format()
             ).encode(encoding=encoding)
         else:
             data = str(exc).encode(encoding=encoding)
 
-        await response.send(
-            b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\n\
-            Date: %s\r\nServer: %s\r\n\r\n%s' % (request.version,
-                                                 exc.code,
-                                                 exc.message.encode(encoding='latin-1'),
-                                                 exc.content_type.encode(encoding='latin-1'),
-                                                 len(data),
-                                                 datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
-                                                 self._options['server_name'],
-                                                 data))
+        await response.send((
+            b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\n' +
+            b'Date: %s\r\nServer: %s\r\n\r\n%s') % (request.version,
+                                                    exc.code,
+                                                    exc.message.encode(encoding='latin-1'),
+                                                    exc.content_type.encode(encoding='latin-1'),
+                                                    len(data),
+                                                    datetime.utcnow().strftime(
+                                                        '%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
+                                                    self._options['server_name'],
+                                                    data))
 
         response.close()
 
     async def _handle_request_header(self, data, header_size):
         self._data = None
 
         if not self._header.parse(data, header_size=header_size, excludes=[b'proxy']).is_request:
```

### Comparing `tremolo-0.0.81/tremolo/lib/http_request.py` & `tremolo-0.0.82/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/http_response.py` & `tremolo-0.0.82/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/parsed/parse.py` & `tremolo-0.0.82/tremolo/lib/parsed/parse.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/request.py` & `tremolo-0.0.82/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/lib/response.py` & `tremolo-0.0.82/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo/tremolo.py` & `tremolo-0.0.82/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.81/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.82/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.81
+Version: 0.0.82
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

