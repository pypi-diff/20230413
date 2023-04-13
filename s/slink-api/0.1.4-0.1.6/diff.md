# Comparing `tmp/slink_api-0.1.4.tar.gz` & `tmp/slink_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slink_api-0.1.4.tar", max compression
+gzip compressed data, was "slink_api-0.1.6.tar", max compression
```

## Comparing `slink_api-0.1.4.tar` & `slink_api-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3699 2023-03-16 12:55:53.427982 slink_api-0.1.4/README.md
--rw-r--r--   0        0        0      638 2023-03-16 12:55:53.431982 slink_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       45 2023-03-16 12:55:53.431982 slink_api-0.1.4/slink/__init__.py
--rw-r--r--   0        0        0     2037 2023-03-16 12:55:53.431982 slink_api-0.1.4/slink/api.py
--rw-r--r--   0        0        0     3389 2023-03-16 12:55:53.431982 slink_api-0.1.4/slink/decorators.py
--rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 slink_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3679 2023-04-13 06:52:25.996761 slink_api-0.1.6/README.md
+-rw-r--r--   0        0        0      640 2023-04-13 06:52:42.953208 slink_api-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/__init__.py
+-rw-r--r--   0        0        0     2159 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/api.py
+-rw-r--r--   0        0        0     4043 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/decorators.py
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 slink_api-0.1.6/PKG-INFO
```

### Comparing `slink_api-0.1.4/README.md` & `slink_api-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -56,58 +56,53 @@
 
 Slink allows you to elegantly iterate most style of paged APIs. As example, we can implement one of the most common
 pagination patterns, an an offseted pagination API. With such an API, you request an offset of the dataset with some
 limit on the size of the data returned:
 
 ```python
 class OffsettedPager:
-    def __init__(self, results_per_page=5) -> None:
-        self.results_per_page = results_per_page
-        self.startAt = 0
-        self.total = None  # needs to be determined
-
-    def pages(self, url):
-        while self.total is None or self.startAt < self.total:
-            # yield a tuple of the next url and any parameters to be added to the original request
-            yield url, {"startAt": self.startAt, "results_per_page": self.maxCount}
-            self.startAt += self.results_per_page
-
-    def process(self, response):
-        # update the Pager with any response variables; usually either info about the next page or the total number of pages
-        self.total = response.json()["total"]
+    def __init__(self, max_count=5) -> None:
+        self.max_count = max_count
+
+    def pages(self, url: str) -> Generator[Tuple[str, dict], requests.Response, None]:
+        start_at = 0
+        total = None
+        while total is None or start_at < total:
+            # yield a tuple of the next url and any parameters to be added to the original request, get back the response to update the iteration
+            response = yield url, {
+                "startAt": start_at,
+                "maxCount": self.max_count,
+            }
+            total = response.json()["total"]
+            start_at += self.max_count
 ```
 
 You can then use the pager with the `@get_pages` decorator to iterate through the pages:
 
 ```python
 class PagedApi(Api):
     @get_pages("rest/api/3/pages", pager=OffsetedPager())
     def get_paginated(self)
         # our data field in the json result just contains a list of ints, but they could be a much more complicated object
         for value in self.response.json()["data"]:
             yield int(value)
 
 api = PagedApi(base_url=base_url)
-all_results = [e for e in api.get_paginated()]
+all_results = list(api.get_paginated())  # note the list construction because pages are returned as generators
 ```
 
 Another example would be a pagination API where there is a next link:
 
 ```python
 class LinkedPager:
-    def __init__(self) -> None:
-        self.next_url = None
-
-    def pages(self, url):
-        yield url, {}  # first page is just the raw url
-        while self.next_url:
-            yield self.next_url, {}
-
-    def process(self, response):
-        self.next_url = response.json()["links"].get("next")
+    def pages(self, url) -> Generator[Tuple[str, dict], requests.Response, None]:
+        response = yield url, {}  # first page is just the raw url
+        # use assignment operator since python 3.8
+        while next_url := response.json()["links"].get("next"):
+            response = yield next_url, {}
 ```
 
 Note in both cases, iteration can be stopped early by simply stopping calling the endpoint, ie the following will make
 any more requests once it finds the required value:
 
 ```python
 for e in api.get_paginated():
```

### Comparing `slink_api-0.1.4/pyproject.toml` & `slink_api-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slink-api"
-version = "0.1.4"
+version = "v0.1.6"
 description = "Simple and expressive REST clients without the fuss"
 authors = ["James Lloyd <james.allan.lloyd@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/james-allan-lloyd/slink"
 packages = [{include = "slink"}]
 
 [tool.poetry.dependencies]
@@ -21,8 +21,8 @@
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.7"
 mypy = "^1.1.1"
 types-requests = "^2.28.11.15"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `slink_api-0.1.4/slink/api.py` & `slink_api-0.1.6/slink/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,47 +20,50 @@
             return self._response
         else:
             raise Exception("No current response!")
 
     def check_signature(self, signature: inspect.Signature, args, kwargs):
         signature.bind(self, *args, **kwargs)
 
+    def check_response(self):
+        pass
+
     def construct_url(self, url_template: str, kwargs: dict):
         try:
             formatted_url = url_template.format_map(kwargs)
         except KeyError as e:
             raise Exception(f"Cannot match '{e.args[0]}' in url to function parameters")
         return urljoin(
             self.base_url,
             formatted_url,
         )
 
 
 class Query:
-    pass
+    def __init__(self, alias: str = ""):
+        self.alias = alias
 
 
 class Body:
     pass
 
 
 class DecoratorParser:
     def __init__(self, kwargs) -> None:
-        self.queryParams = [k for k, v in kwargs.items() if type(v) == Query]
+        self.queryParams = {k: v.alias if len(v.alias) else k for k, v in kwargs.items() if type(v) == Query}
         self.bodyParams = [k for k, v in kwargs.items() if type(v) == Body]
 
     def parse(self, args, kwargs) -> Tuple[Dict[str, str], List[str]]:
         if len(args):
             raise Exception("Must use keyword arguments in api calls")
 
-        params = {k: v for k, v in kwargs.items() if k in self.queryParams}
+        params = {
+            self.queryParams[k]: v for k, v in kwargs.items() if k in self.queryParams
+        }
         body = [v for k, v in kwargs.items() if k in self.bodyParams]
 
         return params, body
 
 
 class Pager(Protocol):
-    def pages(self, url: str) -> Generator[Tuple[str, dict], None, None]:  # type: ignore
-        pass
-
-    def process(self, response: requests.Response):
+    def pages(self, url: str) -> Generator[Tuple[str, dict], requests.Response, None]:  # type: ignore
         pass
```

### Comparing `slink_api-0.1.4/PKG-INFO` & `slink_api-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slink-api
-Version: 0.1.4
+Version: 0.1.6
 Summary: Simple and expressive REST clients without the fuss
 Home-page: https://github.com/james-allan-lloyd/slink
 Author: James Lloyd
 Author-email: james.allan.lloyd@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -74,58 +74,53 @@
 
 Slink allows you to elegantly iterate most style of paged APIs. As example, we can implement one of the most common
 pagination patterns, an an offseted pagination API. With such an API, you request an offset of the dataset with some
 limit on the size of the data returned:
 
 ```python
 class OffsettedPager:
-    def __init__(self, results_per_page=5) -> None:
-        self.results_per_page = results_per_page
-        self.startAt = 0
-        self.total = None  # needs to be determined
-
-    def pages(self, url):
-        while self.total is None or self.startAt < self.total:
-            # yield a tuple of the next url and any parameters to be added to the original request
-            yield url, {"startAt": self.startAt, "results_per_page": self.maxCount}
-            self.startAt += self.results_per_page
-
-    def process(self, response):
-        # update the Pager with any response variables; usually either info about the next page or the total number of pages
-        self.total = response.json()["total"]
+    def __init__(self, max_count=5) -> None:
+        self.max_count = max_count
+
+    def pages(self, url: str) -> Generator[Tuple[str, dict], requests.Response, None]:
+        start_at = 0
+        total = None
+        while total is None or start_at < total:
+            # yield a tuple of the next url and any parameters to be added to the original request, get back the response to update the iteration
+            response = yield url, {
+                "startAt": start_at,
+                "maxCount": self.max_count,
+            }
+            total = response.json()["total"]
+            start_at += self.max_count
 ```
 
 You can then use the pager with the `@get_pages` decorator to iterate through the pages:
 
 ```python
 class PagedApi(Api):
     @get_pages("rest/api/3/pages", pager=OffsetedPager())
     def get_paginated(self)
         # our data field in the json result just contains a list of ints, but they could be a much more complicated object
         for value in self.response.json()["data"]:
             yield int(value)
 
 api = PagedApi(base_url=base_url)
-all_results = [e for e in api.get_paginated()]
+all_results = list(api.get_paginated())  # note the list construction because pages are returned as generators
 ```
 
 Another example would be a pagination API where there is a next link:
 
 ```python
 class LinkedPager:
-    def __init__(self) -> None:
-        self.next_url = None
-
-    def pages(self, url):
-        yield url, {}  # first page is just the raw url
-        while self.next_url:
-            yield self.next_url, {}
-
-    def process(self, response):
-        self.next_url = response.json()["links"].get("next")
+    def pages(self, url) -> Generator[Tuple[str, dict], requests.Response, None]:
+        response = yield url, {}  # first page is just the raw url
+        # use assignment operator since python 3.8
+        while next_url := response.json()["links"].get("next"):
+            response = yield next_url, {}
 ```
 
 Note in both cases, iteration can be stopped early by simply stopping calling the endpoint, ie the following will make
 any more requests once it finds the required value:
 
 ```python
 for e in api.get_paginated():
```

