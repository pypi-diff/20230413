# Comparing `tmp/vnpy-okex-pro-2023.4.14.2.tar.gz` & `tmp/vnpy-okex-pro-2023.4.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy-okex-pro-2023.4.14.2.tar", last modified: Thu Apr 13 06:53:03 2023, max compression
+gzip compressed data, was "vnpy-okex-pro-2023.4.14.3.tar", last modified: Thu Apr 13 09:32:43 2023, max compression
```

## Comparing `vnpy-okex-pro-2023.4.14.2.tar` & `vnpy-okex-pro-2023.4.14.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.944679 vnpy-okex-pro-2023.4.14.2/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.2/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 06:53:03.944799 vnpy-okex-pro-2023.4.14.2/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.2/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1014 2023-04-13 06:53:03.945327 vnpy-okex-pro-2023.4.14.2/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.2/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.941103 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    32912 2023-04-13 05:51:53.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/okex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.944448 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.834563 vnpy-okex-pro-2023.4.14.3/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.3/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 09:32:43.834656 vnpy-okex-pro-2023.4.14.3/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.3/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1014 2023-04-13 09:32:43.835108 vnpy-okex-pro-2023.4.14.3/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.3/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.831550 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    33594 2023-04-13 09:07:29.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/okex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.834373 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/top_level.txt
```

### Comparing `vnpy-okex-pro-2023.4.14.2/LICENSE` & `vnpy-okex-pro-2023.4.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.2/PKG-INFO` & `vnpy-okex-pro-2023.4.14.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.2
+Version: 2023.4.14.3
 Summary: OKEX gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy-okex-pro-2023.4.14.2/README.md` & `vnpy-okex-pro-2023.4.14.3/README.md`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.2/setup.cfg` & `vnpy-okex-pro-2023.4.14.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy-okex-pro
-version = 2023.4.14.2
+version = 2023.4.14.3
 url = https://github.com/monk-after-90s/vnpy-okex-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = OKEX gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/__init__.py` & `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/okex_gateway.py` & `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/okex_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,38 +394,53 @@
 
         """
         # todo 改为并发版本
         buf: Dict[datetime, BarData] = {}
         end_time = str(int((datetime.now().timestamp() + 1) * 1000))  # 现在的毫秒时间戳
         path: str = "/api/v5/market/history-candles"
 
+        last_req_ts = None  # 上次请求时间戳
         while True:
             # 创建查询参数
             params: dict = {
                 "instId": req.symbol,
                 "bar": INTERVAL_VT2OKEX[req.interval],
                 "after": end_time,  # 虽然叫after，但"请求此时间戳之前（更旧的数据）的分页内容，传的值为对应接口的ts"，不包含参数中的时间
                 "before": str(int((req.start.timestamp() - 1) * 1000))
                 # 虽然叫before，但"请求此时间戳之后（更新的数据）的分页内容，传的值为对应接口的ts"，不包含参数中的时间
             }
 
             if params['after'] <= params['before']:
                 break
+
+            # 限速：20次/2s(okex)，粗略处理为请求间隔不低于0.1s
+            if last_req_ts is not None:
+                interval = time.time() - last_req_ts
+                if interval < 0.1:  # 间隔太短
+                    sleep_seconds = 0.1 - interval
+                    self.gateway.write_log(f"{sleep_seconds=}")
+                    time.sleep(sleep_seconds)
             # 从服务器获取响应
+            last_req_ts = time.time()
             resp: Response = self.request(
                 "GET",
                 path,
                 params=params
             )
-
             # 如果请求失败则终止循环
             if resp.status_code // 100 != 2:
                 msg = f"获取历史数据失败，状态码：{resp.status_code}，信息：{resp.text}"
                 self.gateway.write_log(msg)
-                break
+
+                if json.loads(resp.text)['code'] == '50011':
+                    time.sleep(0.5)
+                    self.gateway.write_log("重试")
+                    continue
+                else:
+                    break
             else:
                 data: dict = resp.json()
 
                 if not data["data"]:
                     # m = data["msg"]
                     msg = f"获取历史数据结束"
                     self.gateway.write_log(msg)
```

### Comparing `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/PKG-INFO` & `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.2
+Version: 2023.4.14.3
 Summary: OKEX gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
```

