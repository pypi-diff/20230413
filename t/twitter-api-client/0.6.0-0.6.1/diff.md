# Comparing `tmp/twitter-api-client-0.6.0.tar.gz` & `tmp/twitter-api-client-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.0.tar", last modified: Mon Apr 10 19:12:07 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.1.tar", last modified: Thu Apr 13 01:52:02 2023, max compression
```

## Comparing `twitter-api-client-0.6.0.tar` & `twitter-api-client-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-10 19:12:02.000000 twitter-api-client-0.6.0/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.853313 twitter-api-client-0.6.0/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.6.0/twitter/account.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.853313 twitter-api-client-0.6.0/twitter/config/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/log.py
--rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/operations.py
--rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/config/settings.py
--rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.6.0/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5242 2023-04-10 19:10:29.000000 twitter-api-client-0.6.0/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    12811 2023-04-10 18:38:31.000000 twitter-api-client-0.6.0/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5035 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.6.0/twitter/utils.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-10 19:12:07.854313 twitter-api-client-0.6.0/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-10 19:12:07.000000 twitter-api-client-0.6.0/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-13 01:51:56.000000 twitter-api-client-0.6.1/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.523536 twitter-api-client-0.6.1/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.6.1/twitter/account.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.525536 twitter-api-client-0.6.1/twitter/config/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/log.py
+-rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/operations.py
+-rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/settings.py
+-rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.6.1/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5242 2023-04-10 19:10:29.000000 twitter-api-client-0.6.1/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    12761 2023-04-13 00:22:22.000000 twitter-api-client-0.6.1/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5105 2023-04-12 03:42:43.000000 twitter-api-client-0.6.1/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/utils.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.0/LICENSE` & `twitter-api-client-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/PKG-INFO` & `twitter-api-client-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.6.0/setup.py` & `twitter-api-client-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.6.0",
+    version="0.6.1",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.6.0/twitter/account.py` & `twitter-api-client-0.6.1/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/config/log.py` & `twitter-api-client-0.6.1/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/config/operations.py` & `twitter-api-client-0.6.1/twitter/config/operations.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/config/settings.py` & `twitter-api-client-0.6.1/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/constants.py` & `twitter-api-client-0.6.1/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/login.py` & `twitter-api-client-0.6.1/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter/scraper.py` & `twitter-api-client-0.6.1/twitter/scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -232,15 +232,17 @@
 
     def save_data(self, data: list, name: str = ''):
         try:
             for d in data:
                 path = Path(f'data/raw/{d[ID]}')
                 path.mkdir(parents=True, exist_ok=True)
                 (path / f'{time.time_ns()}_{name}.json').write_text(
-                    orjson.dumps(d, option=orjson.OPT_INDENT_2).decode())
+                    orjson.dumps(d, option=orjson.OPT_INDENT_2).decode(),
+                    encoding='utf-8'
+                )
 
         except KeyError as e:
             logger.debug(f'[{ERROR}error{RESET}] failed to save data: {e}')
 
     def download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
         """
         Download file
@@ -270,22 +272,19 @@
         res = self.tweet_by_rest_id(ids)
         for r in res:
             user_id = find_key(r, 'user_results')[0]['result']['rest_id']
             url = f'https://twitter.com/{user_id}/status/{r[ID]}'  # evaluates to username in browser
             media = [y for x in find_key(r, 'media') for y in x]  # in case of arbitrary schema
             if photos:
                 photos = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
-                # logger.debug(f'{photos = }')
                 if photos:
                     [self.download(url, photo) for photo in photos]
             if videos:
                 videos = [x['variants'] for m in media if (x := m.get('video_info'))]
                 hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in videos}
-                # logger.debug(f'{videos = }')
-                # logger.debug(f'{hq_videos = }')
                 if hq_videos:
                     [self.download(url, video) for video in hq_videos]
 
     def trends(self) -> dict:
         """Get trends for all UTC offsets"""
         url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
         headers = get_headers(self.session)
@@ -300,9 +299,11 @@
         for data in res:
             trends = find_key(data, 'item')
             for t in trends:
                 all_trends |= {t['content']['trend']['name']: t}
         path = Path(f'data/raw/trends')
         path.mkdir(parents=True, exist_ok=True)
         (path / f'{time.time_ns()}.json').write_text(
-            orjson.dumps(all_trends, option=orjson.OPT_INDENT_2).decode())
+            orjson.dumps(all_trends, option=orjson.OPT_INDENT_2).decode(),
+            encoding='utf-8'
+        )
         return all_trends
```

### Comparing `twitter-api-client-0.6.0/twitter/search.py` & `twitter-api-client-0.6.1/twitter/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,18 @@
     all_data = []
     c = colors.pop() if colors else ''
     while next_cursor:
         logger.debug(f'{c}{query}{reset}')
         config['cursor'] = next_cursor
         data, next_cursor = await backoff(lambda: get(session, api, config), query)
         data['query'] = query
-        (out / f'raw/{time.time_ns()}.json').write_text(orjson.dumps(data, option=orjson.OPT_INDENT_2).decode())
+        (out / f'raw/{time.time_ns()}.json').write_text(
+            orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
+            encoding='utf-8'
+        )
         all_data.append(data)
     return all_data
 
 
 async def backoff(fn, info, retries=12):
     for i in range(retries + 1):
         try:
@@ -136,10 +139,10 @@
 @atexit.register
 def combine_results(in_path: Path = IN_PATH, out_path: Path = OUT_PATH):
     try:
         out_path.write_text(orjson.dumps({
             k: v
             for p in in_path.iterdir() if p.suffix == '.json'
             for k, v in orjson.loads(p.read_text())['globalObjects']['tweets'].items()
-        }, option=orjson.OPT_INDENT_2).decode())
+        }, option=orjson.OPT_INDENT_2).decode(), encoding='utf-8')
     except Exception as e:
         logger.debug(f'FAILED to combine search results, {e}')
```

### Comparing `twitter-api-client-0.6.0/twitter/utils.py` & `twitter-api-client-0.6.1/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.0/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.1/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

