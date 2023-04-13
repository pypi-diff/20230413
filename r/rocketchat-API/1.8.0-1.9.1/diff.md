# Comparing `tmp/rocketchat_API-1.8.0-py3-none-any.whl.zip` & `tmp/rocketchat_API-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9787 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        0 b- defN 20-Aug-29 10:00 rocketchat_API/__init__.py
--rw-rw-r--  2.0 unx    37443 b- defN 20-Aug-29 10:00 rocketchat_API/rocketchat.py
--rw-rw-r--  2.0 unx      215 b- defN 20-Aug-29 10:00 rocketchat_API/APIExceptions/RocketExceptions.py
--rw-rw-r--  2.0 unx        0 b- defN 20-Aug-29 10:00 rocketchat_API/APIExceptions/__init__.py
--rw-rw-r--  2.0 unx     1115 b- defN 20-Aug-29 10:02 rocketchat_API-1.8.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3818 b- defN 20-Aug-29 10:02 rocketchat_API-1.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Aug-29 10:02 rocketchat_API-1.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 20-Aug-29 10:02 rocketchat_API-1.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      789 b- defN 20-Aug-29 10:02 rocketchat_API-1.8.0.dist-info/RECORD
-9 files, 43487 bytes uncompressed, 8401 bytes compressed:  80.7%
+Zip file size: 9829 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        0 b- defN 20-Sep-12 11:12 rocketchat_API/__init__.py
+-rw-rw-r--  2.0 unx    37709 b- defN 20-Sep-12 11:12 rocketchat_API/rocketchat.py
+-rw-rw-r--  2.0 unx      215 b- defN 20-Sep-12 11:12 rocketchat_API/APIExceptions/RocketExceptions.py
+-rw-rw-r--  2.0 unx        0 b- defN 20-Sep-12 11:12 rocketchat_API/APIExceptions/__init__.py
+-rw-rw-r--  2.0 unx     1115 b- defN 20-Sep-12 11:14 rocketchat_API-1.9.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     3818 b- defN 20-Sep-12 11:14 rocketchat_API-1.9.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 20-Sep-12 11:14 rocketchat_API-1.9.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 20-Sep-12 11:14 rocketchat_API-1.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      789 b- defN 20-Sep-12 11:14 rocketchat_API-1.9.1.dist-info/RECORD
+9 files, 43753 bytes uncompressed, 8443 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: rocketchat_API/APIExceptions/RocketExceptions.py
 Comment: 
 
 Filename: rocketchat_API/APIExceptions/__init__.py
 Comment: 
 
-Filename: rocketchat_API-1.8.0.dist-info/LICENSE.txt
+Filename: rocketchat_API-1.9.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rocketchat_API-1.8.0.dist-info/METADATA
+Filename: rocketchat_API-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: rocketchat_API-1.8.0.dist-info/WHEEL
+Filename: rocketchat_API-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: rocketchat_API-1.8.0.dist-info/top_level.txt
+Filename: rocketchat_API-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rocketchat_API-1.8.0.dist-info/RECORD
+Filename: rocketchat_API-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rocketchat_API/rocketchat.py

```diff
@@ -10,20 +10,21 @@
 
 
 class RocketChat:
     API_path = '/api/v1/'
 
     def __init__(self, user=None, password=None, auth_token=None, user_id=None,
                  server_url='http://127.0.0.1:3000', ssl_verify=True, proxies=None,
-                 timeout=30, session=None):
+                 timeout=30, session=None, client_certs=None):
         """Creates a RocketChat object and does login on the specified server"""
         self.headers = {}
         self.server_url = server_url
         self.proxies = proxies
         self.ssl_verify = ssl_verify
+        self.cert = client_certs
         self.timeout = timeout
         self.req = session or requests
         if user and password:
             self.login(user, password)  # skipcq: PTC-W1006
         if auth_token and user_id:
             self.headers['X-Auth-Token'] = auth_token
             self.headers['X-User-Id'] = user_id
@@ -47,14 +48,15 @@
             else i + '=' + str(args[i])
             for i in args
         )
         return self.req.get(
             '%s?%s' % (url, params),
             headers=self.headers,
             verify=self.ssl_verify,
+            cert=self.cert,
             proxies=self.proxies,
             timeout=self.timeout
         )
 
     def __call_api_post(self, method, files=None, use_json=True, **kwargs):
         reduced_args = self.__reduce_kwargs(kwargs)
         # Since pass is a reserved word in Python it has to be injected on the request dict
@@ -63,23 +65,25 @@
             reduced_args['pass'] = reduced_args['password']
         if use_json:
             return self.req.post(self.server_url + self.API_path + method,
                                  json=reduced_args,
                                  files=files,
                                  headers=self.headers,
                                  verify=self.ssl_verify,
+                                 cert=self.cert,
                                  proxies=self.proxies,
                                  timeout=self.timeout
                                  )
         else:
             return self.req.post(self.server_url + self.API_path + method,
                                  data=reduced_args,
                                  files=files,
                                  headers=self.headers,
                                  verify=self.ssl_verify,
+                                 cert=self.cert,
                                  proxies=self.proxies,
                                  timeout=self.timeout
                                  )
 
     # Authentication
 
     def login(self, user, password):
@@ -89,15 +93,16 @@
         if re.match(r'^[_a-z0-9-]+(\.[_a-z0-9-]+)*@[a-z0-9-]+(\.[a-z0-9-]+)*(\.[a-z]{2,4})$', user):
             request_data['user'] = user
         else:
             request_data['username'] = user
         login_request = requests.post(self.server_url + self.API_path + 'login',
                                       data=request_data,
                                       verify=self.ssl_verify,
-                                      proxies=self.proxies)
+                                      proxies=self.proxies,
+                                      cert=self.cert)
         if login_request.status_code == 401:
             raise RocketAuthenticationException()
 
         if login_request.status_code == 200:
             if login_request.json().get('status') == "success":
                 self.headers['X-Auth-Token'] = login_request.json().get('data').get('authToken')
                 self.headers['X-User-Id'] = login_request.json().get('data').get('userId')
@@ -185,16 +190,17 @@
         elif username:
             response = self.__call_api_get('users.getAvatar', username=username, kwargs=kwargs)
         else:
             raise RocketMissingParamException('userID or username required')
 
         # If Accounts_AvatarBlockUnauthorizedAccess is set, we need to provide the Token as cookies
         if response.status_code == 403:
-            return self.req.get(response.url, cookies={'rc_uid': self.headers.get('X-User-Id'),
-                                                       'rc_token': self.headers.get('X-Auth-Token')})
+            return self.req.get(response.url, cert=self.cert,
+                                cookies={'rc_uid': self.headers.get('X-User-Id'),
+                                         'rc_token': self.headers.get('X-Auth-Token')})
         return response
 
     def users_set_avatar(self, avatar_url, **kwargs):
         """Set a user’s avatar"""
         if avatar_url.startswith('http://') or avatar_url.startswith('https://'):
             return self.__call_api_post('users.setAvatar', avatarUrl=avatar_url, kwargs=kwargs)
         else:
```

## Comparing `rocketchat_API-1.8.0.dist-info/LICENSE.txt` & `rocketchat_API-1.9.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rocketchat_API-1.8.0.dist-info/METADATA` & `rocketchat_API-1.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketchat-API
-Version: 1.8.0
+Version: 1.9.1
 Summary: Python API wrapper for Rocket.Chat
 Home-page: https://github.com/jadolg/rocketchat_API
 Author: Jorge Alberto Díaz Orozco
 Author-email: diazorozcoj@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

