# Comparing `tmp/awc-1.0.1-py2.py3-none-any.whl.zip` & `tmp/awc-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21237 bytes, number of entries: 16
--rw-r--r--  2.0 unx     4516 b- defN 23-Apr-12 20:31 awc/__init__.py
+Zip file size: 23385 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6403 b- defN 23-Apr-12 22:27 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
--rw-r--r--  2.0 unx     3357 b- defN 23-Apr-12 19:44 awc/api.py
--rw-r--r--  2.0 unx      292 b- defN 23-Apr-12 17:10 awc/const.py
--rw-r--r--  2.0 unx     1600 b- defN 23-Apr-12 18:57 awc/exc.py
+-rw-r--r--  2.0 unx     5278 b- defN 23-Apr-12 22:27 awc/api.py
+-rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
+-rw-r--r--  2.0 unx     1600 b- defN 23-Apr-12 22:27 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
--rw-r--r--  2.0 unx      845 b- defN 23-Apr-12 18:55 awc/util.py
--rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 18:58 awc/wrn.py
--rw-r--r--  2.0 unx     2785 b- defN 23-Apr-12 19:58 awc/sql/__init__.py
--rw-r--r--  2.0 unx     2062 b- defN 23-Apr-12 19:27 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1790 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1144 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/RECORD
-16 files, 54905 bytes uncompressed, 19401 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     1194 b- defN 23-Apr-12 22:27 awc/util.py
+-rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
+-rw-r--r--  2.0 unx     3566 b- defN 23-Apr-12 22:28 awc/sql/__init__.py
+-rw-r--r--  2.0 unx     2955 b- defN 23-Apr-12 22:28 awc/sql/helpers.py
+-rw-------  2.0 unx    35107 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3780 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.1.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-12 22:31 awc-1.1.0.dist-info/RECORD
+16 files, 62740 bytes uncompressed, 21549 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.0.1.dist-info/LICENSE
+Filename: awc-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.0.1.dist-info/METADATA
+Filename: awc-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.0.1.dist-info/WHEEL
+Filename: awc-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.0.1.dist-info/top_level.txt
+Filename: awc-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.0.1.dist-info/zip-safe
+Filename: awc-1.1.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.0.1.dist-info/RECORD
+Filename: awc-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -1,101 +1,153 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""AWC -- ari-web comments"""
+"""awc -- ari-web comments"""
 
 import time
 import typing
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "1.0.1"
+__version__: typing.Final[str] = "1.1.0"
 
 
 class Awc:
-    """ari-web comments interface"""
+    """ari-web comments interface
+
+    this is where all API requests begin, you must
+    pass an instance of this object to every api wrapper
+    as a first argument"""
 
     __slots__: typing.Tuple[str, ...] = (
         "__instance",
-        "api_key",
+        "__api_key",
         "__rate_limit_wait",
         "__session",
     )
 
     __instance: furl
-    api_key: typing.Optional[str]
+    __api_key: typing.Optional[str]
     __rate_limit_wait: typing.Union[int, float]
     __session: requests.Session
 
     @property
     def instance(self) -> furl:
-        """return API instance url COPY ( parsed )"""
+        """return API instance url COPY ( parsed )
+
+        return furl.furl -- the parsed url copy"""
         return self.__instance.copy()
 
     @property
+    def api_key(self) -> typing.Optional[str]:
+        """api_key getter -- returns the optionally set API key
+
+        return str | None -- optionally set API key"""
+        return self.__api_key
+
+    @api_key.setter
+    def api_key(self, value: typing.Optional[str]) -> None:
+        """api_key setter -- sets the optionally set API key
+
+        raise
+            awc.exc.InvalidAPIKeyError -- on invalid API key"""
+
+        if value is not None and self.get(api="amiadmin").text != "1":
+            raise exc.InvalidAPIKeyError(
+                f"{value[:5]}{'*' * (len(value) - 5)}"[:50]
+                + (" ..." if len(value) > 50 else "")
+            )
+
+        self.__api_key = value
+
+    @property
     def rate_limit_wait(self) -> typing.Union[int, float]:
-        """rate limit getter -- get the rate limit wait in seconds"""
+        """rate limit wait time getter -- get the rate limit wait in seconds
+
+        return int | float -- sleep time in seconds"""
         return self.__rate_limit_wait
 
     @rate_limit_wait.setter
     def rate_limit_wait(self, value: float) -> None:
-        """rate limit setter -- set the rate limit wait in seconds"""
+        """rate limit wait time setter -- set the rate limit wait in seconds
+
+        raise
+            ValueError -- on incorrect supplied value ( typewise or valuewise )"""
 
         if type(value) not in (int, float) or value < 0:
             raise ValueError(f"rate limit wait time cannot be {value!r}")
 
         self.__rate_limit_wait = value
 
     @property
     def session(self) -> requests.Session:
-        """requests.Session instance"""
+        """requests.Session instance
+
+        return requests.Session -- the requests session"""
         return self.__session
 
     def __init__(
         self,
         instance: str,
         api_key: typing.Optional[str] = None,
         rate_limit_wait: typing.Union[int, float] = 5,
     ) -> None:
+        """initialise the awc instance
+
+        instance: str -- the instance URL
+        api_key: str | None = None -- the API key used for requests ( optional )
+        rate_limit_wait: int | float -- the sleep time in seconds for how much to
+                                        sleep when we get rate limited
+
+        raise
+            awc.exc.InvalidInstanceURLError -- on invalid instance
+            awc.exc.InvalidAPIKeyError(api_key.setter) -- on invalid API key"""
+
         ins: furl = furl(instance)
 
         if (
             not ins.host  # type: ignore
             or ins.scheme not in const.INSTANCE_PROTOCOLS  # type: ignore
             or not util.is_up(ins.host, ins.port)  # type: ignore
         ):
             raise exc.InvalidInstanceURLError(instance)
 
         self.__instance = ins
-        self.api_key = api_key
-        self.rate_limit_wait = rate_limit_wait
         self.__session = requests.Session()
 
-        if self.api_key is not None and self.get(api="amiadmin").text != "1":
-            raise exc.InvalidAPIKeyError(
-                f"{self.api_key[:5]}{'*' * (len(self.api_key) - 5)}"[:50]
-                + (" ..." if len(self.api_key) > 50 else "")
-            )
+        self.rate_limit_wait = rate_limit_wait
+        self.api_key = api_key
 
     def __getitem__(self, path: str) -> str:
-        """return API URL"""
+        """return an API URL of requested `path`
+
+        return str -- the URL"""
         return self.instance.join(path).url  # type: ignore
 
     def request(
         self,
         method: typing.Callable[..., requests.Response],
         *args: typing.Any,
         api: str = ".",
         admin: bool = True,
         **kwargs: typing.Any,
     ) -> requests.Response:
-        """general requests API, `method` is a member of `self.session` object"""
+        """general requests API
+
+        method: typing.Callable[..., requests.Response] -- member of Awc.session, used
+                                                           to call to the API endpoints
+        *args: typing.Any -- arguments passed to `method`
+        api: str = "." -- the API endpoint to call to
+        admin: bool = True -- should we add the `api-key` header to this request
+        **kwargs: typing.Any -- keyword arguments passed to `method`
+
+        return requests.Response -- the API response"""
 
         if not (
             hasattr(self.session, method.__name__)
             and callable(getattr(self.session, method.__name__))
         ):
             raise ValueError(f"invalid request method : {method}")
 
@@ -109,39 +161,41 @@
         while True:
             try:
                 r = method(self[api], *args, **kwargs)
             except (
                 requests.exceptions.ConnectionError,
                 requests.exceptions.HTTPError,
             ) as e:
-                raise exc.APIRequestFailedError(api, e.response)
+                raise exc.APIRequestFailedError(api, e.response) from e
 
             if self.rate_limit_wait and r.status_code == 429:
                 time.sleep(self.rate_limit_wait)
             else:
                 break
 
         if not r.ok:
             raise exc.APIRequestFailedError(api, r)
 
         return r
 
     def get(self, *args: typing.Any, **kwargs: typing.Any) -> requests.Response:
-        """similar to Awc.request() but for GET requests"""
+        """similar to `Awc.request` but for GET requests,
+
+        return requests.Response"""
         return self.request(self.session.get, *args, **kwargs)
 
     def post(self, *args: typing.Any, **kwargs: typing.Any) -> requests.Response:
-        """similar to Awc.request() but for POST requests"""
+        """similar to `Awc.request` but for POST requests"""
         return self.request(self.session.post, *args, **kwargs)
 
     @staticmethod
     def require_key(
         f: typing.Callable[..., typing.Any]
     ) -> typing.Callable[..., typing.Any]:
-        """decorator to require an api key"""
+        """decorator to require an api key to run a function"""
 
         @wraps(f)
         def wrap(awc: "Awc", *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
             if awc.api_key is None:
                 raise exc.NoAPIKeyError(f.__name__)
 
             return f(awc, *args, **kwargs)
```

## awc/api.py

```diff
@@ -1,35 +1,51 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""ari-web api wrappers"""
+"""ari-web comments api wrappers"""
 
 import typing
 
 import requests
 
 from . import Awc, const, exc, util
 
 
 def post_comment(awc: Awc, content: str) -> typing.List[typing.Union[int, bool]]:
-    """post a comment"""
+    """post a comment
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+    content: str(const.MAX_CONTENT_LEN) -- the comment content
+
+    return typing.List[typing.Union[int, bool]] -- [comment id, is admin]"""
 
     try:
         return awc.post(
             data={"content": util.truncate(content, const.MAX_CONTENT_LEN)}
         ).json()
     except requests.exceptions.InvalidJSONError as e:
         raise exc.UnexpectedResponseError(
             e.response.text, typing.List[typing.Union[int, bool]]
-        )
+        ) from e
 
 
 def get_comments(
     awc: Awc, from_id: int, to_id: int
 ) -> typing.Dict[str, typing.List[typing.Union[str, bool, None]]]:
-    """get comments in range from-to"""
+    """get comments in range from-to, range is to_id >= cid >= from_id
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+    from_id: int -- the comment ID to begin the range from
+    to_id: int -- the comment ID to end the range with
+
+    raise
+        ValueError -- on from_id > to_id
+        ValueError -- on abs(to_id - from_id) > awc.const.MAX_FETCH_COUNT
+        awc.exc.UnexpectedResponseError -- on invalid returned JSON
+
+    return typing.Dict[str, typing.List[typing.Union[str, bool, None]]] -- comments"""
 
     if from_id > to_id:
         raise ValueError(
             f"from_id ( {from_id} ) most not be larger than to_id ( {to_id} )"
         )
 
     if (diff := abs(to_id - from_id)) > const.MAX_FETCH_COUNT:
@@ -40,80 +56,118 @@
 
     try:
         return awc.get(api=f"{from_id}/{to_id}").json()
     except requests.exceptions.InvalidJSONError as e:
         raise exc.UnexpectedResponseError(
             e.response.text,
             typing.Dict[int, typing.List[typing.Union[str, bool, None]]],
-        )
+        ) from e
 
 
 def get_comment(awc: Awc, cid: int) -> typing.List[typing.Union[str, bool, None]]:
-    """get coment by ID"""
+    """get coment by ID
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+    cid: int -- same as both from_id and to_id arguments to `get_comments`
+
+    raise
+        awc.exc.ResouceNotFoundError from KeyError -- on a comment not found
+
+    return typing.List[typing.Union[str, bool, None]] -- the comment"""
 
     try:
         return get_comments(awc, cid, cid)[str(cid)]
     except KeyError as e:
         raise exc.ResouceNotFoundError(cid) from e
 
 
 def total(awc: Awc) -> int:
-    """total comments count api"""
+    """total comments count api
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+
+    raise
+        awc.exc.UnexpectedResponseError from ValueError -- when returned response is NaN
+
+    return int -- total comments count"""
 
     r: requests.Response = awc.get(api="total")
 
     try:
         return int(r.text)
     except ValueError as e:
         raise exc.UnexpectedResponseError(r.text, int) from e
 
 
 @Awc.require_key
 def sql(
     awc: Awc, queries: typing.Iterable[str], backup: typing.Optional[str] = None
 ) -> typing.List[typing.List[typing.Any]]:
-    """run SQL queries"""
+    """run SQL queries
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+    queries: typing.Iterable[str] -- the queries to run
+    backup: str | None = None -- optionally set backup database name
+
+    raise
+        awc.exc.UnexpectedResponseError from requests.exceptions.InvalidJSONError --
+            on invalid JSON
+    """
 
     data: typing.Dict[str, typing.Union[typing.Iterable[str], str]] = {"sql": queries}
 
     if backup is not None:
         data["backup"] = backup
 
     try:
         return awc.post(api="sql", data=data).json()  # type: ignore
     except requests.exceptions.InvalidJSONError as e:
         raise exc.UnexpectedResponseError(
             e.response.text, typing.Dict[int, typing.List[typing.List[typing.Any]]]
-        )
+        ) from e
 
 
 def apply(awc: Awc, author: str, content: str) -> requests.Response:
-    """apply to the whitelist"""
+    """apply to the whitelist
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+    author: str -- the author / username you want to have
+    content: str -- the reason why youre applying
+
+    return requests.Response -- the apply API response"""
 
     return awc.post(
         api="apply",
         data={
             "author": util.truncate(author, const.MAX_AUTHOR_LEN),
             "content": util.truncate(content, const.MAX_CONTENT_LEN),
         },
     )
 
 
 def whoami(awc: Awc) -> str:
-    """returns your username ( if youre in the whitelist )"""
+    """returns your username ( if youre in the whitelist )
+
+    awc: awc.Awc -- the awc.Awc instance to work on"""
     return awc.get(api="whoami").text
 
 
 def get_comment_lock(awc: Awc) -> bool:
-    """gets comments lock status"""
+    """gets comments lock status
+
+    awc: awc.Awc -- the awc.Awc instance to work on"""
     return awc.get(api="lock").text == "1"
 
 
 @Awc.require_key
 def toggle_comment_lock(awc: Awc) -> bool:
-    """toggles comments lock status"""
+    """toggles comments lock status
+
+    awc: awc.Awc -- the awc.Awc instance to work on"""
     return awc.post(api="lock").text == "1"
 
 
 def amiadmin(awc: Awc) -> bool:
-    """returns your admin status ( 1 if API key is correct ( you are admin ) )"""
+    """returns your admin status ( `True` if API key is correct ( you are admin ) )
+
+    awc: awc.Awc -- the awc.Awc instance to work on"""
     return awc.get(api="amiadmin").text == "1"
```

## awc/const.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""ari-web constants"""
+"""ari-web comments API constants"""
 
 from typing import Tuple
 
 MAX_CONTENT_LEN: int = 1024
 MAX_AUTHOR_LEN: int = 64
 MAX_APPS_ACOUNT: int = 25
 MAX_FETCH_COUNT: int = 25
```

## awc/exc.py

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""AWC exceptions"""
+"""awc exceptions"""
 
 import typing
 
 import requests
 
 
 class AWCException(Exception):
-    """base AWC exception"""
+    """base awc exception"""
 
 
 class InvalidInstanceURLError(AWCException, requests.exceptions.InvalidURL):
     """raised when an API instance URL isnt valid"""
 
     instance: str
```

## awc/util.py

```diff
@@ -7,30 +7,41 @@
 import warnings
 
 from .wrn import AWCWarning, ContentTruncatedWarning
 
 
 @functools.lru_cache
 def is_up(host: str, port: int) -> bool:
-    """check if host:port is up, this result is cached"""
+    """check if host:port is up, this result is cached
+
+    host: str -- the hostname
+    port: int -- the port you want to check"""
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         try:
             sock.connect((host, port))
             return True
         except socket.error:
             return False
 
 
 def warn(msg: AWCWarning) -> None:
-    """throw a warning message"""
+    """throw a warning message
+
+    msg: awc.wrn.AWCWarning -- the warning"""
 
     warnings.warn(msg, stacklevel=2)
 
 
 def truncate(content: str, length: int, do_warn: bool = True) -> str:
-    """truncate content and warn if appropriate"""
+    """truncate content and warn if appropriate
+
+    content: str -- content you want to truncated
+    length: int -- to what length should the content be truncated to
+    do_warn: bool = True -- do we warn if content is being truncated
+
+    return str -- the truncated content"""
 
     if do_warn and len(content) > length:
         warn(ContentTruncatedWarning(content, length))
 
     return content[:length]
```

## awc/wrn.py

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc warnings"""
 
 
 class AWCWarning(Warning):
-    """base AWC warning"""
+    """base awc warning"""
 
     message: str
 
     def __str__(self) -> str:
         return self.message
```

## awc/sql/__init__.py

```diff
@@ -18,42 +18,57 @@
 
     @classmethod
     def select(
         cls,
         where: pypika.queries.QueryBuilder,
         *select: str,
     ) -> pypika.queries.QueryBuilder:
-        """select statement"""
+        """select statement
+
+        where: pypika.queries.QueryBuilder -- the condition on which to select
+        *select: str -- what fields to select
+
+        return pypika.queries.QueryBuilder -- the query"""
         return (
             pypika.Query.from_(cls.t)  # type: ignore
             .select(
                 *(select or ("*",)),
             )
             .where(where)
         )
 
     @classmethod
     def query(
         cls,
         where: pypika.queries.QueryBuilder,
     ) -> pypika.queries.QueryBuilder:
-        """select table row"""
+        """select table row
+
+        where: pypika.queries.QueryBuilder -- the condition on which to select
+
+        return pypika.queries.QueryBuilder -- the query"""
         return pypika.Query.from_(cls.t).where(where)  # type: ignore
 
     @classmethod
     def add(
         cls,
         *what: typing.Any,
     ) -> pypika.queries.QueryBuilder:
-        """insert statement"""
+        """insert statement
+
+        *what: typing.Any -- VALUES() to insert
+
+        return pypika.queries.QueryBuilder -- the query"""
         return pypika.Query.into(cls.t).insert(what)  # type: ignore
 
     @classmethod
     def all(cls) -> pypika.queries.QueryBuilder:
-        """select the whole table"""
+        """select the whole table
+
+        return pypika.queries.QueryBuilder -- `SELECT * FROM self.t` query"""
         return pypika.Query.from_(cls.t).select("*")  # type: ignore
 
 
 class Comment(SQLTable):
     """comment / post table"""
 
     tname: str = "comments"
@@ -99,14 +114,23 @@
     """return an sql query"""
     return query.get_sql()
 
 
 def multisql(
     queries: typing.List[pypika.queries.QueryBuilder],
 ) -> typing.Tuple[str, ...]:
-    """convert a list of queries into a list of SQL string queries"""
+    """convert a list of queries into a list of SQL string queries
+
+    queries: typing.List[pypika.queries.QueryBuilder]
+        -- the queries you want to be converted
+
+    return typing.Tuple[str, ...] -- the converted queries"""
     return tuple(map(sql, queries))
 
 
 def delete(what: pypika.queries.QueryBuilder) -> pypika.queries.QueryBuilder:
-    """delete result from your query"""
+    """delete result from your query
+
+    what: what: pypika.queries.QueryBuilder -- what to delete
+
+    return pypika.queries.QueryBuilder -- the query"""
     return what.delete()  # type: ignore
```

## awc/sql/helpers.py

```diff
@@ -7,29 +7,37 @@
 import pypika.queries  # type: ignore
 
 from .. import const, util
 from . import Ban, Comment, IpQueue, IpWhitelist, delete
 
 
 def whitelist(author: str) -> typing.List[pypika.queries.QueryBuilder]:
-    """whitelist a user"""
+    """whitelist a user
+
+    author: str -- the aplicant ( author ) to whitelist from the queue
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
 
     author = util.truncate(author, const.MAX_AUTHOR_LEN)
 
     return [
         IpWhitelist.add(
             IpQueue.select(IpQueue.author == author, "ip"),  # type: ignore
             IpQueue.select(IpQueue.author == author, "author"),  # type: ignore
         ),
         delete(IpQueue.query(IpQueue.author == author).limit(1)),  # type: ignore
     ]
 
 
 def unwhitelist(author: str) -> typing.List[pypika.queries.QueryBuilder]:
-    """unwhitelist a user"""
+    """unwhitelist a user
+
+    author: str -- the aplicant ( author ) to unwhitelist
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
 
     return [
         delete(
             IpWhitelist.query(
                 IpWhitelist.author
                 == util.truncate(  # type: ignore
                     author,
@@ -37,40 +45,56 @@
                 )
             )
         ),
     ]
 
 
 def ban(author: str) -> typing.List[pypika.queries.QueryBuilder]:
-    """ban a user"""
+    """ban and unwhitelist a user
+
+    author: str -- the author to ip ban ( needs to be whitelisted )
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
 
     author = util.truncate(author, const.MAX_AUTHOR_LEN)
 
     return [
         Ban.add(IpWhitelist.select(IpWhitelist.author == author, "ip"))  # type: ignore
     ] + unwhitelist(author)
 
 
 def unban(ip: str) -> typing.List[pypika.queries.QueryBuilder]:
-    """unban a user"""
+    """unban an IP
+
+    ip: str -- the SHA256 hash of the IP bein unbannned
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
     return [delete(Ban.query(Ban.ip == ip).limit(1))]  # type: ignore
 
 
 def censor_comments(
     where: pypika.queries.QueryBuilder,
     censoring: str = "[censored]",
 ) -> typing.List[pypika.queries.QueryBuilder]:
-    """censor comments"""
+    """censor comments
+
+    where: pypika.queries.QueryBuilder -- the condition on which to censor
+    censoring: str = "[censored]" -- the string to use for censoring
+
+    return typing.List[pypika.queries.QueryBuilder] -- the queries"""
     return [
         Comment.t.update()  # type: ignore
         .set(Comment.author, censoring)
         .set(Comment.content, censoring)
         .where(where)
     ]
 
 
 def set_comments_admin(
     where: pypika.queries.QueryBuilder,
     value: bool = True,
 ) -> typing.List[pypika.queries.QueryBuilder]:
-    """set admin status on comments"""
+    """set admin status on comments
+
+    where: pypika.queries.QueryBuilder -- the condition on which to set
+    value: bool = True -- the value to set the admin status to"""
     return [Comment.t.update().set(Comment.admin, value).where(where)]  # type: ignore
```

## Comparing `awc-1.0.1.dist-info/LICENSE` & `awc-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

