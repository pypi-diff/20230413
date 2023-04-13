# Comparing `tmp/nonebot_plugin_shindan-0.3.1.tar.gz` & `tmp/nonebot_plugin_shindan-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_shindan-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_shindan-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_shindan-0.3.1.tar` & `nonebot_plugin_shindan-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/LICENSE
--rw-r--r--   0        0        0     1626 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/README.md
--rw-r--r--   0        0        0     8442 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/__init__.py
--rw-r--r--   0        0        0      119 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/config.py
--rw-r--r--   0        0        0     2374 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/manager.py
--rw-r--r--   0        0        0     3393 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
--rw-r--r--   0        0        0      530 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/model.py
--rw-r--r--   0        0        0     4479 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/shindanmaker.py
--rw-r--r--   0        0        0   180778 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/app.css
--rw-r--r--   0        0        0   247324 2023-03-10 12:29:33.120308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/app.js
--rw-r--r--   0        0        0   477118 2023-03-10 12:29:33.124308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/chart.js
--rw-r--r--   0        0        0      339 2023-03-10 12:29:33.124308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/shindan.html
--rw-r--r--   0        0        0     1965 2023-03-10 12:29:33.124308 nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/shindan_list.html
--rw-r--r--   0        0        0      843 2023-03-10 12:29:33.124308 nonebot_plugin_shindan-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1626 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/README.md
+-rw-r--r--   0        0        0     8442 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/config.py
+-rw-r--r--   0        0        0     2374 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/manager.py
+-rw-r--r--   0        0        0     3393 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
+-rw-r--r--   0        0        0      530 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/model.py
+-rw-r--r--   0        0        0     4518 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/shindanmaker.py
+-rw-r--r--   0        0        0   180778 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.css
+-rw-r--r--   0        0        0   247324 2023-04-13 02:47:47.091901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.js
+-rw-r--r--   0        0        0   477118 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/chart.js
+-rw-r--r--   0        0        0      339 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan.html
+-rw-r--r--   0        0        0     1965 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan_list.html
+-rw-r--r--   0        0        0      843 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_shindan-0.3.1/LICENSE` & `nonebot_plugin_shindan-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/README.md` & `nonebot_plugin_shindan-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/__init__.py` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     description="使用ShindanMaker网站的趣味占卜",
     usage="发送“占卜列表”查看可用占卜\n发送“{占卜名} {名字}”使用占卜",
     config=Config,
     extra={
         "unique_name": "shindan",
         "example": "人设生成 小Q",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.1",
+        "version": "0.3.2",
     },
 )
 
 add_usage = """Usage:
 添加占卜 {id} {指令}
 如：添加占卜 917962 人设生成"""
```

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/manager.py` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/model.py` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/shindanmaker.py` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/shindanmaker.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,50 +36,59 @@
 
 if shindan_config.shindanmaker_cookie:
     headers["cookie"] = shindan_config.shindanmaker_cookie
 
 
 @retry
 async def get(client: httpx.AsyncClient, url: str, **kwargs):
-    return await client.get(url, headers=headers, timeout=20, **kwargs)
+    resp = await client.get(
+        url, headers=headers, timeout=20, follow_redirects=True, **kwargs
+    )
+    resp.raise_for_status()
+    return resp
 
 
 @retry
 async def post(client: httpx.AsyncClient, url: str, **kwargs):
-    return await client.post(url, headers=headers, timeout=20, **kwargs)
+    resp = await client.post(
+        url, headers=headers, timeout=20, follow_redirects=True, **kwargs
+    )
+    resp.raise_for_status()
+    return resp
 
 
 async def download_image(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         resp = await get(client, url)
         return resp.read()
 
 
 async def get_shindan_title(id: str) -> str:
     url = f"https://shindanmaker.com/{id}"
     async with httpx.AsyncClient() as client:
         resp = await get(client, url)
-        if resp.status_code == 302:
-            resp = await get(client, resp.headers["location"])
         dom = BeautifulSoup(resp.text, "lxml")
         title = dom.find("h1", {"id": "shindanTitle"})
         assert title
         return title.text
 
 
 async def make_shindan(id: str, name: str, mode="image") -> Union[str, bytes]:
     url = f"https://shindanmaker.com/{id}"
     seed = time.strftime("%y%m%d", time.localtime())
     async with httpx.AsyncClient() as client:
         resp = await get(client, url)
-        if resp.status_code == 302:
-            resp = await get(client, resp.headers["location"])
         dom = BeautifulSoup(resp.text, "lxml")
         token = dom.find("form", {"id": "shindanForm"}).find("input")["value"]  # type: ignore
-        payload = {"_token": token, "shindanName": name + seed, "hiddenName": "名無しのR"}
+        payload = {
+            "_token": token,
+            "shindanName": name + seed,
+            "hiddenName": "名無しのR",
+            "type": "name",
+        }
         resp = await post(client, url, json=payload)
 
     content = resp.text
     if mode == "image":
         html, has_chart = await render_html(content)
         html = html.replace(seed, "")
         return await html_to_pic(
```

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/app.css` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/app.js` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/chart.js` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/chart.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/nonebot_plugin_shindan/templates/shindan_list.html` & `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan_list.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.1/pyproject.toml` & `nonebot_plugin_shindan-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_shindan"
-version = "0.3.1"
+version = "0.3.2"
 description = "Nonebot2 plugin for using ShindanMaker"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-shindan"
 repository = "https://github.com/noneplugin/nonebot-plugin-shindan"
```

### Comparing `nonebot_plugin_shindan-0.3.1/PKG-INFO` & `nonebot_plugin_shindan-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-shindan
-Version: 0.3.1
+Version: 0.3.2
 Summary: Nonebot2 plugin for using ShindanMaker
 Home-page: https://github.com/noneplugin/nonebot-plugin-shindan
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

