# Comparing `tmp/kittenai-0.1.4.tar.gz` & `tmp/kittenai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kittenai-0.1.4.tar", last modified: Thu Mar 18 08:23:05 2021, max compression
+gzip compressed data, was "dist\kittenai-0.1.5.tar", last modified: Thu Apr 13 01:17:21 2023, max compression
```

## Comparing `kittenai-0.1.4.tar` & `kittenai-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-03-18 08:23:05.221946 kittenai-0.1.4/
--rw-rw-rw-   0        0        0      274 2021-03-18 08:23:05.221946 kittenai-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      145 2020-12-09 04:50:19.000000 kittenai-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2021-03-18 08:23:05.211951 kittenai-0.1.4/kittenai/
--rw-rw-rw-   0        0        0       28 2020-12-09 05:17:33.000000 kittenai-0.1.4/kittenai/__init__.py
--rw-rw-rw-   0        0        0     8588 2021-03-18 08:22:30.000000 kittenai-0.1.4/kittenai/baiduai.py
-drwxrwxrwx   0        0        0        0 2021-03-18 08:23:05.219948 kittenai-0.1.4/kittenai.egg-info/
--rw-rw-rw-   0        0        0      274 2021-03-18 08:23:04.000000 kittenai-0.1.4/kittenai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2021-03-18 08:23:04.000000 kittenai-0.1.4/kittenai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-18 08:23:04.000000 kittenai-0.1.4/kittenai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-03-18 08:23:04.000000 kittenai-0.1.4/kittenai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-03-18 08:23:04.000000 kittenai-0.1.4/kittenai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-18 08:23:05.222945 kittenai-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      400 2021-03-18 08:22:52.000000 kittenai-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:17:21.000000 kittenai-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:01:41.000000 kittenai-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      256 2023-04-13 01:17:21.000000 kittenai-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2023-04-13 01:01:41.000000 kittenai-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 01:17:21.000000 kittenai-0.1.5/kittenai/
+-rw-rw-rw-   0        0        0       28 2023-04-13 01:01:41.000000 kittenai-0.1.5/kittenai/__init__.py
+-rw-rw-rw-   0        0        0     8609 2023-04-13 01:01:41.000000 kittenai-0.1.5/kittenai/baiduai.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:17:21.000000 kittenai-0.1.5/kittenai.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-04-13 01:17:20.000000 kittenai-0.1.5/kittenai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-13 01:17:20.000000 kittenai-0.1.5/kittenai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 01:17:20.000000 kittenai-0.1.5/kittenai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 01:17:20.000000 kittenai-0.1.5/kittenai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 01:17:20.000000 kittenai-0.1.5/kittenai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 01:17:21.000000 kittenai-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      400 2023-04-13 01:01:41.000000 kittenai-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `kittenai-0.1.4/kittenai/baiduai.py` & `kittenai-0.1.5/kittenai/baiduai.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,60 +55,60 @@
       'version': '2.0',
       'session_id': '',
       'user_id': randrange(0, 99999),
       'log_id': "ROBOT_{}".format(randrange(0, 99999)),
       'rememberskill': 0
     }
 
-  def text2speech(self, text, lang='zh', per=0, format='wav'):
-    
+  def text2speech(self, text, lang='zh', per=0, format='wav', **kwargs):
     data ={
       'tex': text,
       'lan': lang,
       'ctp':1,
       'cuid':'kittenai',
       'tok': self.tokens['voice'],
       'per': per,
-      'aue': getattr(format2aue, format, 6)
+      'aue': format2aue.get(format, 6)
     }
+    data = dict(data, **kwargs)
     headers = {
       'Content-Type' : 'application/json; charset=UTF-8'
     }
     resp = requests.post('http://tsn.baidu.com/text2audio', headers=headers, data=data)
     if resp.headers['content-type'] == 'application/json':
       obj = resp.json()
       if obj['err_no'] != 0:
-        raise RuntimeError(obj['err_detail'])
-    else:
+        raise RuntimeError(obj['error_no'])
+    else:   
       return resp.content
 
-  def speech2text(self, speech, format='wav', lang="zh", options={}):
+  def speech2text(self, speech, format='wav', lang='zh'):
     data = {
       "format": format,
       "token": self.tokens['voice'],
       "cuid": "kittenai",
-      "dev_pid": getattr(lang2devpid, lang, 1537),
+      "dev_pid": lang2devpid.get(lang, 1537),
       "speech": base64.b64encode(speech).decode(),
       "len": len(speech)
     }
     if format == 'wav':
       wav = wave.open(BytesIO(speech))
       data['channel'] = wav.getnchannels()
       data['rate'] = wav.getframerate()
       wav.close()
 
-    data = dict(data, **(options))
     url = "http://vop.baidu.com/server_api"
     headers = {
         'Content-Type' : 'application/json; charset=UTF-8'
     }
     resp = requests.post(url,headers=headers,data=json.dumps(data))
     obj = resp.json()
     if obj['err_no'] != 0:
-      raise RuntimeError(obj['err_msg'])
+      raise RuntimeError(obj['err_no'])
+    # raise RuntimeError(obj['err_msg'])
     return obj['result'][0]
 
   def _processImage(self, image):
     data = {}
     if type(image) == str:
       data['image_type'] = 'FACE_TOKEN'
       data['image'] = image
```

