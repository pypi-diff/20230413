# Comparing `tmp/HTTP_PyServer-0.0.1-py3-none-any.whl.zip` & `tmp/HTTP_PyServer-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 7555 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      129 b- defN 23-Apr-12 01:27 server/__init__.py
--rw-rw-rw-  2.0 fat     4101 b- defN 23-Apr-12 05:07 server/render.py
+Zip file size: 9321 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Apr-13 02:01 server/__init__.py
+-rw-rw-rw-  2.0 fat     5028 b- defN 23-Apr-13 02:02 server/render.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-Apr-12 04:52 server/request.py
--rw-rw-rw-  2.0 fat     3181 b- defN 23-Apr-12 19:08 server/routes.py
+-rw-rw-rw-  2.0 fat     3930 b- defN 23-Apr-13 01:37 server/responses.py
+-rw-rw-rw-  2.0 fat     3592 b- defN 23-Apr-13 02:00 server/routes.py
 -rw-rw-rw-  2.0 fat     4229 b- defN 23-Apr-12 19:38 server/server.py
--rw-rw-rw-  2.0 fat     1067 b- defN 23-Apr-12 20:29 HTTP_PyServer-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2047 b- defN 23-Apr-12 20:29 HTTP_PyServer-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 20:29 HTTP_PyServer-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-12 20:29 HTTP_PyServer-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      782 b- defN 23-Apr-12 20:29 HTTP_PyServer-0.0.1.dist-info/RECORD
-10 files, 17785 bytes uncompressed, 6229 bytes compressed:  65.0%
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Apr-13 02:06 HTTP_PyServer-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2024 b- defN 23-Apr-13 02:06 HTTP_PyServer-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 02:06 HTTP_PyServer-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-13 02:06 HTTP_PyServer-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      858 b- defN 23-Apr-13 02:06 HTTP_PyServer-0.0.2.dist-info/RECORD
+11 files, 23168 bytes uncompressed, 7881 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: server/render.py
 Comment: 
 
 Filename: server/request.py
 Comment: 
 
+Filename: server/responses.py
+Comment: 
+
 Filename: server/routes.py
 Comment: 
 
 Filename: server/server.py
 Comment: 
 
-Filename: HTTP_PyServer-0.0.1.dist-info/LICENSE
+Filename: HTTP_PyServer-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: HTTP_PyServer-0.0.1.dist-info/METADATA
+Filename: HTTP_PyServer-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: HTTP_PyServer-0.0.1.dist-info/WHEEL
+Filename: HTTP_PyServer-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: HTTP_PyServer-0.0.1.dist-info/top_level.txt
+Filename: HTTP_PyServer-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: HTTP_PyServer-0.0.1.dist-info/RECORD
+Filename: HTTP_PyServer-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## server/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .request import Request
 from .routes import Routes
-from .render import file, redirect, attachment
-from .server import run
+from .render import file, text, redirect, attachment
+from .server import run
+from .responses import ResponseMessages, ResponseCodes
```

## server/render.py

```diff
@@ -1,64 +1,87 @@
 import mimetypes
 import os
-import urllib
 
+from . import responses
 from . import request
 from . import routes
 
 def _get_template(*args,
                   data: bytes = '',
                   **template_vars) -> str:
-    '''Replaces all template variables in a data with their values. Template variables are defined as {{var_name}}, and are replaced with the value of var_name in template_vars.'''
-    
-    if not data:
-        
-        return ''
+    '''Replaces all template variables in a data with their values.
+    Template variables are defined as {{var_name}},
+    and are replaced with the value of var_name in template_vars.'''
     
     for var_name, var_value in template_vars.items():
 
-        data = data.replace(f'{{{{{var_name}}}}}', str(var_value))
+        data = data.replace(f'{{{{{var_name}}}}}'.encode(encoding = 'utf-8',
+                                                         errors = 'ignore'),
+                            var_value.encode(encoding = 'utf-8',
+                                             errors = 'ignore'))
 
     return data
 
+def text(*args,
+         text: str = '',
+         filetype: str = 'txt',
+         code: int | responses.ResponseCodes = 200,
+         message: str | responses.ResponseMessages = 'OK',
+         ) -> bytes:
+    '''Returns a text response. Use this to return plain text, JSON, XML, etc.'''
+
+    text = text.encode(encoding = 'utf-8',
+                       errors = 'ignore')
+
+    headers = {
+
+        'Content-Type': mimetypes.guess_type(f'file.{filetype.strip(".")}')[0],
+
+        'Content-Length': str(len(text)),
+
+    }
+
+    return (f'HTTP/1.1 {code} {message}\r\n'\
+            + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
+            .encode(encoding = 'utf-8',
+            errors = 'ignore') \
+            + b'\r\n\r\n' \
+            + text
+
 def file(*args,
-         data: str = '',
          filepath: str = '',
-         extension: str = '',
-         request: request.Request = None,
+         request: request.Request = request.Request(),
          templated_vars: dict = {},
-         code: int = 200,
-         message: str = 'OK'
+         code: int | responses.ResponseCodes = 200,
+         message: str | responses.ResponseMessages = 'OK'
          ) -> bytes:
     '''Returns a file as a response. Use this to return HTML, CSS, JS, images, etc.'''
 
-    if filepath:
-
-        if not os.path.exists(filepath):
+    if not filepath or not os.path.exists(filepath):
 
-            data = routes.Routes.get_route(path = '404',
-                                           request = request)
+        return text(text = routes.Routes.get_route('/404',
+                                                   request = request),
+                    code = responses.ResponseCodes.NOT_FOUND,
+                    message = responses.ResponseMessages.NOT_FOUND)
             
-        else:
+    else:
 
-            with open(filepath, 'r') as file:
+        with open(filepath, 'rb') as file:
 
-                data = file.read()
+            data = file.read()
 
     if templated_vars:
 
         data = _get_template(data = data,
                              **templated_vars)
 
-    data = data.encode(encoding = 'utf-8',
-                        errors = 'ignore')
-
     headers = {
 
-        'Content-Type': mimetypes.guess_type(f'file.{extension.strip(".")}')[0] or mimetypes.guess_type(os.path.basename(filepath))[0] or 'text/plain',
+        'Content-Type': mimetypes.guess_type(os.path.basename(filepath))[0]\
+                        or 'application/octet-stream',
 
         'Content-Length': str(len(data)),
 
     }
 
     return (f'HTTP/1.1 {code} {message}\r\n' \
             + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
@@ -76,62 +99,52 @@
         \r\nContent-Type: text/html\
         \r\n\r\n\
         <html>\
             <head>\
                 <meta http-equiv="refresh" content="0;URL={url}" />\
             </head>\
         </html>'
-    
-    print(len(redirect_request))
-
-    print(len('<html>\
-            <head>\
-                <meta http-equiv="refresh" content="0;URL=" />\
-            </head>\
-        </html>'))
 
     return redirect_request.encode(encoding = 'utf-8',
                                    errors = 'ignore')
 
 def attachment(*args,
                filepath: str = '',
-               filedata: bytes = b'',
-               download: bool = False,
-               text: bool = False,
+               is_download: bool = False,
+               is_text: bool = False,
                filename: str = '',
-               request: request.Request = None) -> bytes:
-    '''Returns a file as an attachment. Can be used to download or view files.'''
+               request: request.Request = request.Request()) -> bytes:
+    '''Returns a file as an attachment.
+    Use this to return files for download or viewing.
+    Sometimes browsers will preview text files, so you can use is_text
+    to force the browser to display the raw text instead of previewing it.'''
+
+    if not filepath or not os.path.exists(filepath):
+
+        return text(text = routes.Routes.get_route('/404',
+                                                   request = request),
+                    code = responses.ResponseCodes.NOT_FOUND,
+                    message = responses.ResponseMessages.NOT_FOUND)
 
-    if not filepath:
+    with open(filepath, 'rb') as f:
 
-        data = filedata
-
-    elif not os.path.exists(filepath): # Filepath entered does not exist
-
-        return file(data = routes.Routes.get_route(path = '404',
-                                            request = request),
-                    code = 404,
-                    message = 'Not Found'
-                    )
-    
-    else:
-
-        with open(filepath, 'rb') as file:
-
-            data = file.read()
+        data = f.read()
 
     headers = {
 
-        'Content-Type': 'text/plain' if text else mimetypes.guess_type(os.path.basename(filepath))[0] or 'application/octet-stream',
+        'Content-Type': 'text/plain' if is_text else\
+                        mimetypes.guess_type(os.path.basename(filepath))[0]\
+                        or 'application/octet-stream',
 
         'Content-Length': str(len(data)),
 
-        'Content-Disposition': ('attachment' if download else 'inline') + f'; filename="{urllib.parse.quote(filename)}"' if filename else ('attachment' if download else 'inline')
+        'Content-Disposition': ('attachment' if is_download else 'inline')\
+                                + f'; filename="{filename}"' if filename else ''
 
     }
 
-    return (f'HTTP/1.1 200 OK\r\n' \
+    return ('HTTP/1.1 200 OK\r\n' \
             + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
             .encode(encoding = 'utf-8',
             errors = 'ignore') \
             + b'\r\n\r\n' \
             + data
```

## server/routes.py

```diff
@@ -1,9 +1,10 @@
 import os
 
+from . import responses
 from . import request
 from . import render
 
 class Routes:
 
     routes: dict[str, callable] = {
 
@@ -37,18 +38,18 @@
         for ressource_file_path, ressource_reference_path in ressources:
 
             ressource_reference_path = '/' + ressource_reference_path.strip('/')
 
             if not os.path.exists(ressource_file_path):
 
                 cls.routes[ressource_reference_path] = \
-                    lambda _: render.file(
-                    data = cls.get_route('404'),
-                    code = 404,
-                    message = 'Not Found')
+                    lambda _: render.text(text = Routes.get_route('/404',
+                                                   request = request),
+                                          code = responses.ResponseCodes.NOT_FOUND,
+                                          message = responses.ResponseMessages.NOT_FOUND)
 
             else:
 
                 ressource = render.attachment(filepath = ressource_file_path)
 
                 cls.routes[ressource_reference_path] = \
                 lambda _, ressource = ressource: ressource
@@ -92,15 +93,18 @@
                     if sub_route.startswith('%') and sub_route.endswith('%'):
 
                         wildcard_values.append(sub_path)
 
                 return cls.routes[route](request,
                                          *wildcard_values)
 
-        return cls.routes['/404'](request)
+        return render.text(text = Routes.get_route('/404',
+                                                   request = request),
+                           code = responses.ResponseCodes.NOT_FOUND,
+                           message = responses.ResponseMessages.NOT_FOUND)
 
     @classmethod
     def get_route(cls,
                   *args,
                   path: str = '',
                   request: request.Request = request.Request()) -> bytes:
         '''Gets a route from the routes dictionary.'''
```

## Comparing `HTTP_PyServer-0.0.1.dist-info/LICENSE` & `HTTP_PyServer-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `HTTP_PyServer-0.0.1.dist-info/METADATA` & `HTTP_PyServer-0.0.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple way to make complex http servers
 Author-email: Alex-Jando <alexjando2007@outlook.com>
-Project-URL: Homepage, https://github.com/Alex-Jando/Simple-Server
-Project-URL: Bug Tracker, https://github.com/Alex-Jando/Simple-Server/issues
+Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
+Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,21 +26,20 @@
 python -m pip install HTTP-PyServer
 ```
 
 # Simple Example
 
 ```
 # Saved as "main.py"
-from server import Routes, file, run
+from server import Routes, text, run
 
 @Routes.route(path = '/')
 def home(request):
 
-    return file(data='Hello, World!',
-                extension='html')
+    return text(text = 'Hello, world!')
 
 if __name__ == '__main__':
 
     run()
 ```
 
 ```
@@ -60,7 +59,8 @@
 - `threading`
 - `socket`
 - `sys`
 - `logging`
 - `os`
 - `urllib`
 - `mimetypes`
+- `enum`
```

