# Comparing `tmp/krrsnkapi-0.1.tar.gz` & `tmp/krrsnkapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.1.tar", last modified: Thu Apr 13 13:14:58 2023, max compression
+gzip compressed data, was "krrsnkapi-0.1.1.tar", last modified: Thu Apr 13 13:20:59 2023, max compression
```

## Comparing `krrsnkapi-0.1.tar` & `krrsnkapi-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:14:58.774901 krrsnkapi-0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      601 2023-04-13 13:14:58.775901 krrsnkapi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:14:58.709897 krrsnkapi-0.1/krrsnkapi/
--rw-rw-rw-   0        0        0       34 2023-04-13 13:11:31.000000 krrsnkapi-0.1/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-12 17:26:21.000000 krrsnkapi-0.1/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:14:58.772901 krrsnkapi-0.1/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      601 2023-04-13 13:14:56.000000 krrsnkapi-0.1/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-13 13:14:57.000000 krrsnkapi-0.1/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:14:56.000000 krrsnkapi-0.1/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 13:14:56.000000 krrsnkapi-0.1/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 13:14:56.000000 krrsnkapi-0.1/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 13:14:58.778901 krrsnkapi-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1441 2023-04-13 13:07:18.000000 krrsnkapi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.152514 krrsnkapi-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      603 2023-04-13 13:20:59.152514 krrsnkapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.132512 krrsnkapi-0.1.1/krrsnkapi/
+-rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.1.1/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-12 17:26:21.000000 krrsnkapi-0.1.1/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.149513 krrsnkapi-0.1.1/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 13:20:59.155514 krrsnkapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1443 2023-04-13 13:19:59.000000 krrsnkapi-0.1.1/setup.py
```

### Comparing `krrsnkapi-0.1/LICENSE.txt` & `krrsnkapi-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.1/PKG-INFO` & `krrsnkapi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.1
+Version: 0.1.1
 Summary: Module for easy use of my api
 Home-page: https://github.com/kararasenok_gd/krrsnkapi
 Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.1.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
```

### Comparing `krrsnkapi-0.1/README.md` & `krrsnkapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.1/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.1.1/krrsnkapi/krrsnkapi.py`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.1/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.1.1/krrsnkapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.1
+Version: 0.1.1
 Summary: Module for easy use of my api
 Home-page: https://github.com/kararasenok_gd/krrsnkapi
 Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.1.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
```

### Comparing `krrsnkapi-0.1/setup.py` & `krrsnkapi-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Module for easy use of my api',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok_gd/krrsnkapi',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.1.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
```

