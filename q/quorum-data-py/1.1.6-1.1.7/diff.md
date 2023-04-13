# Comparing `tmp/quorum_data_py-1.1.6.tar.gz` & `tmp/quorum_data_py-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.1.6.tar", last modified: Thu Apr 13 09:21:50 2023, max compression
+gzip compressed data, was "quorum_data_py-1.1.7.tar", last modified: Thu Apr 13 15:25:13 2023, max compression
```

## Comparing `quorum_data_py-1.1.6.tar` & `quorum_data_py-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.094824 quorum_data_py-1.1.6/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-13 09:21:50.094321 quorum_data_py-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.6/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.080669 quorum_data_py-1.1.6/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-12 12:28:26.000000 quorum_data_py-1.1.6/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     6008 2023-04-13 09:20:07.000000 quorum_data_py-1.1.6/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.6/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.6/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.6/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:21:50.092170 quorum_data_py-1.1.6/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 09:21:49.000000 quorum_data_py-1.1.6/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 09:21:50.095824 quorum_data_py-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1314 2023-04-12 12:28:26.000000 quorum_data_py-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.254452 quorum_data_py-1.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-13 15:25:13.253485 quorum_data_py-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.7/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.237881 quorum_data_py-1.1.7/quorum_data_py/
+-rw-rw-rw-   0        0        0      349 2023-04-13 15:24:47.000000 quorum_data_py-1.1.7/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-13 15:24:01.000000 quorum_data_py-1.1.7/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.7/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.7/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.7/quorum_data_py/trx_type.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.251453 quorum_data_py-1.1.7/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:25:13.255447 quorum_data_py-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1314 2023-04-13 15:24:47.000000 quorum_data_py-1.1.7/setup.py
```

### Comparing `quorum_data_py-1.1.6/LICENSE` & `quorum_data_py-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.6/PKG-INFO` & `quorum_data_py-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.6/README.md` & `quorum_data_py-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.6/quorum_data_py/_utils.py` & `quorum_data_py-1.1.7/quorum_data_py/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,16 @@
             }
         )
     return imgs
 
 
 def pack_obj(content: str, images: list, name: str, post_id: str):
     content = content or ""
-    images = images[:IMAGE_NUM_LIMIT] or []
+    images = images or []
+    images = images[:IMAGE_NUM_LIMIT]
     if not (content or images):
         raise ValueError("content and images are empty")
     if not isinstance(images, list):
         raise TypeError("images must be list")
 
     obj = {"type": "Note"}
     if content:
```

### Comparing `quorum_data_py-1.1.6/quorum_data_py/converter.py` & `quorum_data_py-1.1.7/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.6/quorum_data_py/feed.py` & `quorum_data_py-1.1.7/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.6/quorum_data_py/trx_type.py` & `quorum_data_py-1.1.7/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.6/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.1.7/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.6/setup.py` & `quorum_data_py-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.1.6",
+    version="1.1.7",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

