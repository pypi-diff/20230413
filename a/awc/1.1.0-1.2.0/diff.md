# Comparing `tmp/awc-1.1.0-py2.py3-none-any.whl.zip` & `tmp/awc-1.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23385 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6403 b- defN 23-Apr-12 22:27 awc/__init__.py
+Zip file size: 23683 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6692 b- defN 23-Apr-13 15:09 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
--rw-r--r--  2.0 unx     5278 b- defN 23-Apr-12 22:27 awc/api.py
+-rw-r--r--  2.0 unx     5416 b- defN 23-Apr-13 15:09 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
--rw-r--r--  2.0 unx     1600 b- defN 23-Apr-12 22:27 awc/exc.py
+-rw-r--r--  2.0 unx     1600 b- defN 23-Apr-13 14:32 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
--rw-r--r--  2.0 unx     1194 b- defN 23-Apr-12 22:27 awc/util.py
+-rw-r--r--  2.0 unx     1383 b- defN 23-Apr-13 14:54 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
--rw-r--r--  2.0 unx     3566 b- defN 23-Apr-12 22:28 awc/sql/__init__.py
--rw-r--r--  2.0 unx     2955 b- defN 23-Apr-12 22:28 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3780 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.1.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/RECORD
-16 files, 62740 bytes uncompressed, 21549 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     4429 b- defN 23-Apr-13 15:08 awc/sql/__init__.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Apr-13 15:11 awc/sql/helpers.py
+-rw-------  2.0 unx    35107 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3780 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/RECORD
+16 files, 64131 bytes uncompressed, 21847 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.1.0.dist-info/LICENSE
+Filename: awc-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.1.0.dist-info/METADATA
+Filename: awc-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.1.0.dist-info/WHEEL
+Filename: awc-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.1.0.dist-info/top_level.txt
+Filename: awc-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.1.0.dist-info/zip-safe
+Filename: awc-1.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.1.0.dist-info/RECORD
+Filename: awc-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "1.1.0"
+__version__: typing.Final[str] = "1.2.0"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
@@ -50,22 +50,24 @@
     @api_key.setter
     def api_key(self, value: typing.Optional[str]) -> None:
         """api_key setter -- sets the optionally set API key
 
         raise
             awc.exc.InvalidAPIKeyError -- on invalid API key"""
 
+        self.__api_key = value
+
         if value is not None and self.get(api="amiadmin").text != "1":
+            self.__api_key = None
+
             raise exc.InvalidAPIKeyError(
                 f"{value[:5]}{'*' * (len(value) - 5)}"[:50]
                 + (" ..." if len(value) > 50 else "")
             )
 
-        self.__api_key = value
-
     @property
     def rate_limit_wait(self) -> typing.Union[int, float]:
         """rate limit wait time getter -- get the rate limit wait in seconds
 
         return int | float -- sleep time in seconds"""
         return self.__rate_limit_wait
 
@@ -122,14 +124,20 @@
 
     def __getitem__(self, path: str) -> str:
         """return an API URL of requested `path`
 
         return str -- the URL"""
         return self.instance.join(path).url  # type: ignore
 
+    def __enter__(self) -> "Awc":
+        return self
+
+    def __exit__(self, *_: typing.Any) -> None:
+        self.end()
+
     def request(
         self,
         method: typing.Callable[..., requests.Response],
         *args: typing.Any,
         api: str = ".",
         admin: bool = True,
         **kwargs: typing.Any,
@@ -183,14 +191,20 @@
         return requests.Response"""
         return self.request(self.session.get, *args, **kwargs)
 
     def post(self, *args: typing.Any, **kwargs: typing.Any) -> requests.Response:
         """similar to `Awc.request` but for POST requests"""
         return self.request(self.session.post, *args, **kwargs)
 
+    def end(self) -> None:
+        """end an instance ( close it )"""
+
+        self.__api_key = None
+        self.session.close()
+
     @staticmethod
     def require_key(
         f: typing.Callable[..., typing.Any]
     ) -> typing.Callable[..., typing.Any]:
         """decorator to require an api key to run a function"""
 
         @wraps(f)
```

## awc/api.py

```diff
@@ -107,15 +107,17 @@
     awc: awc.Awc -- the awc.Awc instance to work on
     queries: typing.Iterable[str] -- the queries to run
     backup: str | None = None -- optionally set backup database name
 
     raise
         awc.exc.UnexpectedResponseError from requests.exceptions.InvalidJSONError --
             on invalid JSON
-    """
+        ValueError -- on invalid queries
+
+    return typing.List[typing.List[typing.Any]] -- query results"""
 
     data: typing.Dict[str, typing.Union[typing.Iterable[str], str]] = {"sql": queries}
 
     if backup is not None:
         data["backup"] = backup
 
     try:
@@ -151,23 +153,23 @@
     return awc.get(api="whoami").text
 
 
 def get_comment_lock(awc: Awc) -> bool:
     """gets comments lock status
 
     awc: awc.Awc -- the awc.Awc instance to work on"""
-    return awc.get(api="lock").text == "1"
+    return util.resp_to_bool(awc.get(api="lock").text)
 
 
 @Awc.require_key
 def toggle_comment_lock(awc: Awc) -> bool:
     """toggles comments lock status
 
     awc: awc.Awc -- the awc.Awc instance to work on"""
-    return awc.post(api="lock").text == "1"
+    return util.resp_to_bool(awc.post(api="lock").text)
 
 
 def amiadmin(awc: Awc) -> bool:
     """returns your admin status ( `True` if API key is correct ( you are admin ) )
 
     awc: awc.Awc -- the awc.Awc instance to work on"""
-    return awc.get(api="amiadmin").text == "1"
+    return util.resp_to_bool(awc.get(api="amiadmin").text)
```

## awc/util.py

```diff
@@ -41,7 +41,17 @@
 
     return str -- the truncated content"""
 
     if do_warn and len(content) > length:
         warn(ContentTruncatedWarning(content, length))
 
     return content[:length]
+
+
+def resp_to_bool(resp: str) -> bool:
+    """convets a response like 0 and 1 to boolean
+
+    resp: str -- the response
+
+    return bool -- the converted boolean"""
+
+    return resp == "1"
```

## awc/sql/__init__.py

```diff
@@ -63,14 +63,41 @@
     @classmethod
     def all(cls) -> pypika.queries.QueryBuilder:
         """select the whole table
 
         return pypika.queries.QueryBuilder -- `SELECT * FROM self.t` query"""
         return pypika.Query.from_(cls.t).select("*")  # type: ignore
 
+    @classmethod
+    def set(
+        cls,
+        where: pypika.queries.QueryBuilder,
+        what: typing.Dict[pypika.Column, typing.Any],
+    ) -> pypika.queries.QueryBuilder:
+        """SET statement
+
+        where: pypika.queries.QueryBuilder -- the condition on which to set
+        what: dict[pypika.Column, typing.Any] -- the columns and values to set
+
+        return pypika.queries.QueryBuilder -- the query"""
+        q: pypika.queries.QueryBuilder = cls.t.update()
+
+        for k, v in what.items():
+            q = q.set(k, v)  # type: ignore
+
+        return q.where(where)  # type: ignore
+
+    @classmethod
+    def purge(cls) -> pypika.queries.QueryBuilder:
+        """purge the table ( delete everything ) **BE CAREFUL**
+
+        return pypika.queries.QueryBuilder -- the query"""
+
+        return pypika.Query.from_(cls.t).delete()  # type: ignore
+
 
 class Comment(SQLTable):
     """comment / post table"""
 
     tname: str = "comments"
     t: pypika.Table = pypika.Table(tname)
```

## awc/sql/helpers.py

```diff
@@ -44,32 +44,42 @@
                     const.MAX_AUTHOR_LEN,
                 )
             )
         ),
     ]
 
 
+def ban_ip(ip: pypika.queries.QueryBuilder) -> typing.List[pypika.queries.QueryBuilder]:
+    """ban an ip
+
+    ip: pypika.queries.QueryBuilder -- the query to get the user ip
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
+
+    return [Ban.add(ip)]  # type: ignore
+
+
 def ban(author: str) -> typing.List[pypika.queries.QueryBuilder]:
     """ban and unwhitelist a user
 
     author: str -- the author to ip ban ( needs to be whitelisted )
 
     return typing.List[pypika.queries.QueryBuilder] -- the queries"""
 
     author = util.truncate(author, const.MAX_AUTHOR_LEN)
 
     return [
-        Ban.add(IpWhitelist.select(IpWhitelist.author == author, "ip"))  # type: ignore
+        *ban_ip(IpWhitelist.select(IpWhitelist.author == author, "ip"))  # type: ignore
     ] + unwhitelist(author)
 
 
 def unban(ip: str) -> typing.List[pypika.queries.QueryBuilder]:
     """unban an IP
 
-    ip: str -- the SHA256 hash of the IP bein unbannned
+    ip: str -- the SHA256 hash of the IP being unbannned
 
     return typing.List[pypika.queries.QueryBuilder] -- the queries"""
     return [delete(Ban.query(Ban.ip == ip).limit(1))]  # type: ignore
 
 
 def censor_comments(
     where: pypika.queries.QueryBuilder,
@@ -78,23 +88,15 @@
     """censor comments
 
     where: pypika.queries.QueryBuilder -- the condition on which to censor
     censoring: str = "[censored]" -- the string to use for censoring
 
     return typing.List[pypika.queries.QueryBuilder] -- the queries"""
     return [
-        Comment.t.update()  # type: ignore
-        .set(Comment.author, censoring)
-        .set(Comment.content, censoring)
-        .where(where)
+        Comment.set(
+            where,
+            {
+                Comment.author: censoring,
+                Comment.content: censoring,
+            },
+        )
     ]
-
-
-def set_comments_admin(
-    where: pypika.queries.QueryBuilder,
-    value: bool = True,
-) -> typing.List[pypika.queries.QueryBuilder]:
-    """set admin status on comments
-
-    where: pypika.queries.QueryBuilder -- the condition on which to set
-    value: bool = True -- the value to set the admin status to"""
-    return [Comment.t.update().set(Comment.admin, value).where(where)]  # type: ignore
```

## Comparing `awc-1.1.0.dist-info/LICENSE` & `awc-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-1.1.0.dist-info/METADATA` & `awc-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 1.1.0
+Version: 1.2.0
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

