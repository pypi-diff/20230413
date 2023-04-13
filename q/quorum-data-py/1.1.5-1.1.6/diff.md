# Comparing `tmp/quorum_data_py-1.1.5.tar.gz` & `tmp/quorum_data_py-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.1.5.tar", last modified: Thu Apr  6 13:07:05 2023, max compression
+gzip compressed data, was "quorum_data_py-1.1.6.tar", last modified: Thu Apr 13 09:21:50 2023, max compression
```

## Comparing `quorum_data_py-1.1.5.tar` & `quorum_data_py-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:05.858582 quorum_data_py-1.1.5/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-06 13:07:05.857630 quorum_data_py-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.5/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:05.842979 quorum_data_py-1.1.5/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-06 13:04:34.000000 quorum_data_py-1.1.5/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     5500 2023-03-28 06:45:29.000000 quorum_data_py-1.1.5/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.5/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.5/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.5/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:07:05.855592 quorum_data_py-1.1.5/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-06 13:07:05.000000 quorum_data_py-1.1.5/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-06 13:07:05.000000 quorum_data_py-1.1.5/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:07:05.000000 quorum_data_py-1.1.5/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-06 13:07:05.000000 quorum_data_py-1.1.5/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-06 13:07:05.000000 quorum_data_py-1.1.5/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 13:07:05.858582 quorum_data_py-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1314 2023-04-06 13:04:34.000000 quorum_data_py-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.094824 quorum_data_py-1.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-13 09:21:50.094321 quorum_data_py-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.6/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.080669 quorum_data_py-1.1.6/quorum_data_py/
+-rw-rw-rw-   0        0        0      349 2023-04-12 12:28:26.000000 quorum_data_py-1.1.6/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     6008 2023-04-13 09:20:07.000000 quorum_data_py-1.1.6/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.6/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.6/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.6/quorum_data_py/trx_type.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.092170 quorum_data_py-1.1.6/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:21:50.095824 quorum_data_py-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1314 2023-04-12 12:28:26.000000 quorum_data_py-1.1.6/setup.py
```

### Comparing `quorum_data_py-1.1.5/LICENSE` & `quorum_data_py-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.5/PKG-INFO` & `quorum_data_py-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.5/README.md` & `quorum_data_py-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.5/quorum_data_py/_utils.py` & `quorum_data_py-1.1.6/quorum_data_py/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import base64
 import datetime
 import io
+import json
 import logging
 import os
 import uuid
 import zipfile
 
 import filetype
 from PIL import Image
 from pygifsicle import gifsicle
 
 logger = logging.getLogger(__name__)
 
 
-# 每条 trx 有大小限制，否则会导致链异常；此为链端限定
-IMAGE_MAX_SIZE_KB = 300  # kb, 每条trx中所包含的图片总大小限制
-# 单条 trx 最多4 张图片；此为 rum app 客户端限定：第三方 app 调整该限定
-IMAGE_MAX_NUM = 4
-CHUNK_SIZE = 200 * 1024  # b, 文件切割为多条trxs时，每条 trx 所包含的文件字节流上限
+TRX_SIZE_LIMIT = 300  # kb, 每条trx的总大小上限，超出会被限制出块
+IMAGE_NUM_LIMIT = 4  # 单条 trx 最多4 张图片；此为 rum app 限定：第三方 app 可调整该限定
+CHUNK_SIZE = 280 * 1024  # bytes, 文件切割为多条trxs时，每条 trx 所包含的文件字节流上限
 
 
 def _filename_init(img):
     file_bytes, is_file = _get_filebytes(img)
     if is_file:
         file_name = os.path.basename(img).encode().decode("utf-8")
     else:
         extension = filetype.guess(file_bytes).extension
         name = f"{uuid.uuid4()}-{datetime.date.today()}"
         file_name = ".".join([name, extension])
     return file_name
 
 
-def _zip_image_bytes(img_bytes, kb=IMAGE_MAX_SIZE_KB):
+def _zip_image_bytes(img_bytes, kb=TRX_SIZE_LIMIT):
     """zip image bytes and return bytes; default changed to .jpeg"""
 
-    kb = kb or IMAGE_MAX_SIZE_KB
     guess_extension = filetype.guess(img_bytes).extension
 
     with io.BytesIO(img_bytes) as im:
         size = len(im.getvalue()) // 1024
         if size < kb:
             return img_bytes
         while size >= kb:
@@ -46,15 +44,15 @@
             x, y = img.size
             out = img.resize((int(x * 0.95), int(y * 0.95)), Image.ANTIALIAS)
             im.close()
             im = io.BytesIO()
             try:
                 out.save(im, "jpeg")
             except Exception as err:
-                logger.debug(err)
+                logger.info(err)
                 out.save(im, guess_extension)
             size = len(im.getvalue()) // 1024
         return im.getvalue()
 
 
 def check_file(file_path):
     if not os.path.exists(file_path):
@@ -74,24 +72,23 @@
     check_file(file_path)
     to_zipfile = to_zipfile or file_path + "_.zip"
     with zipfile.ZipFile(to_zipfile, mode, zipfile.ZIP_DEFLATED) as zf:
         zf.write(file_path, arcname=os.path.basename(file_path))
     return to_zipfile
 
 
-def zip_gif(gif, kb=IMAGE_MAX_SIZE_KB, cover=False):
+def zip_gif(gif, kb=TRX_SIZE_LIMIT, cover=False):
     """压缩动图(gif)到指定大小(kb)以下
 
     gif: gif 格式动图本地路径
     kb: 指定压缩大小, 默认 200kb
     cover: 是否覆盖原图, 默认不覆盖
 
     返回压缩后图片字节. 该方法需要安装 gifsicle 软件和 pygifsicle 模块
     """
-    kb = kb or IMAGE_MAX_SIZE_KB
     size = os.path.getsize(gif) / 1024
     if size < kb:
         return read_file_to_bytes(gif)
 
     destination = None
     if not cover:
         destination = f"{os.path.splitext(gif)[0]}-zip.gif"
@@ -108,22 +105,21 @@
             gif = destination
         size = os.path.getsize(gif) / 1024
         n -= 0.05
 
     return read_file_to_bytes(gif)
 
 
-def _zip_image(img, kb=IMAGE_MAX_SIZE_KB):
+def _zip_image(img, kb=TRX_SIZE_LIMIT):
     file_bytes, is_file = _get_filebytes(img)
-
     try:
         if filetype.guess(file_bytes).extension == "gif" and is_file:
             img_bytes = zip_gif(img, kb=kb, cover=False)
         else:
-            img_bytes = _zip_image_bytes(file_bytes, kb=kb)
+            img_bytes = _zip_image_bytes(file_bytes, kb)
     except Exception as e:
         logger.warning("zip_image %s", e)
     return img_bytes
 
 
 def pack_icon(icon):
     """icon: one image as file path, or bytes, or bytes-string."""
@@ -154,40 +150,56 @@
     else:
         raise TypeError(
             f"not support for type: {type(img)} and length: {_size}"
         )
     return file_bytes, is_file
 
 
-def pack_imgs(images):
-    kb = int(IMAGE_MAX_SIZE_KB // min(len(images), IMAGE_MAX_NUM))
+def pack_imgs(images: list, kb: int = TRX_SIZE_LIMIT):
+    """
+    打包图片为 feed 所需的数据格式。
+    由于每个 trx 限定了 300kb 的大小，图片的大小需要根据已有 content 计算得出余量。
+    """
+    # check images size
+    if len(images) == 0:
+        raise ValueError("images is empty.")
+    # 从图片字节转换为 base64string 大小会膨胀 1.33 左右
+    bytes_limit = int(1024 * kb / 1.34)
+    sizes = [len(read_file_to_bytes(i)) for i in images]
+    total_size = sum(sizes)
+
+    if total_size < bytes_limit:
+        target_size = sizes
+    else:
+        target_size = [int(i * bytes_limit / total_size) for i in sizes]
+
     imgs = []
-    for img in images[:IMAGE_MAX_NUM]:
-        _bytes = _zip_image(img, kb)
+    for i, _img in enumerate(images):
+        _bytes = _zip_image(_img, target_size[i] // 1024)
         imgs.append(
             {
-                "name": _filename_init(img),
                 "mediaType": filetype.guess(_bytes).mime,
                 "content": base64.b64encode(_bytes).decode("utf-8"),
                 "type": "Image",
             }
         )
     return imgs
 
 
 def pack_obj(content: str, images: list, name: str, post_id: str):
     content = content or ""
-    images = images or []
+    images = images[:IMAGE_NUM_LIMIT] or []
     if not (content or images):
         raise ValueError("content and images are empty")
     if not isinstance(images, list):
         raise TypeError("images must be list")
 
     obj = {"type": "Note"}
     if content:
         obj["content"] = content
     if images:
-        obj["image"] = pack_imgs(images)
+        kb = TRX_SIZE_LIMIT - int(len(json.dumps(obj)) // 1024) - 1
+        obj["image"] = pack_imgs(images, kb)
     if name:
         obj["name"] = name
     obj["id"] = post_id or str(uuid.uuid4())
     return obj
```

### Comparing `quorum_data_py-1.1.5/quorum_data_py/converter.py` & `quorum_data_py-1.1.6/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.5/quorum_data_py/feed.py` & `quorum_data_py-1.1.6/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.5/quorum_data_py/trx_type.py` & `quorum_data_py-1.1.6/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.5/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.1.6/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.5/setup.py` & `quorum_data_py-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.1.5",
+    version="1.1.6",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

