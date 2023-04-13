# Comparing `tmp/vnpy-okex-pro-2023.4.14.1.tar.gz` & `tmp/vnpy-okex-pro-2023.4.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy-okex-pro-2023.4.14.1.tar", last modified: Thu Apr 13 06:46:52 2023, max compression
+gzip compressed data, was "vnpy-okex-pro-2023.4.14.2.tar", last modified: Thu Apr 13 06:53:03 2023, max compression
```

## Comparing `vnpy-okex-pro-2023.4.14.1.tar` & `vnpy-okex-pro-2023.4.14.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:46:52.692797 vnpy-okex-pro-2023.4.14.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2548 2023-04-13 06:46:52.692902 vnpy-okex-pro-2023.4.14.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      987 2023-04-13 06:46:52.693404 vnpy-okex-pro-2023.4.14.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:46:52.688950 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    32912 2023-04-13 05:51:53.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro/okex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:46:52.692564 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2548 2023-04-13 06:46:52.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-13 06:46:52.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:52.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-13 06:46:52.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-13 06:46:52.000000 vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.944679 vnpy-okex-pro-2023.4.14.2/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.2/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 06:53:03.944799 vnpy-okex-pro-2023.4.14.2/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.2/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1014 2023-04-13 06:53:03.945327 vnpy-okex-pro-2023.4.14.2/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.2/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.941103 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    32912 2023-04-13 05:51:53.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/okex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 06:53:03.944448 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-13 06:53:03.000000 vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/top_level.txt
```

### Comparing `vnpy-okex-pro-2023.4.14.1/LICENSE` & `vnpy-okex-pro-2023.4.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.1/PKG-INFO` & `vnpy-okex-pro-2023.4.14.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.1
+Version: 2023.4.14.2
 Summary: OKEX gateway for vn.py quant trading framework.
-Home-page: https://www.vnpy.com
+Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vnpy-okex-pro-2023.4.14.1/README.md` & `vnpy-okex-pro-2023.4.14.2/README.md`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.1/setup.cfg` & `vnpy-okex-pro-2023.4.14.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = vnpy-okex-pro
-version = 2023.4.14.1
-url = https://www.vnpy.com
+version = 2023.4.14.2
+url = https://github.com/monk-after-90s/vnpy-okex-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = OKEX gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords =
```

### Comparing `vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro/__init__.py` & `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro/okex_gateway.py` & `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro/okex_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.1/vnpy_okex_pro.egg-info/PKG-INFO` & `vnpy-okex-pro-2023.4.14.2/vnpy_okex_pro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.1
+Version: 2023.4.14.2
 Summary: OKEX gateway for vn.py quant trading framework.
-Home-page: https://www.vnpy.com
+Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

