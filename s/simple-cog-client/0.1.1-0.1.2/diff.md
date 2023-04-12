# Comparing `tmp/simple_cog_client-0.1.1.tar.gz` & `tmp/simple_cog_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_cog_client-0.1.1.tar", max compression
+gzip compressed data, was "simple_cog_client-0.1.2.tar", max compression
```

## Comparing `simple_cog_client-0.1.1.tar` & `simple_cog_client-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-02-20 03:52:31.044496 simple_cog_client-0.1.1/README.md
--rw-r--r--   0        0        0      363 2023-02-20 17:21:08.103278 simple_cog_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-20 03:56:04.536257 simple_cog_client-0.1.1/simple_cog_client/__init__.py
--rw-r--r--   0        0        0      250 2023-02-20 06:19:16.473488 simple_cog_client-0.1.1/simple_cog_client/client.py
--rw-r--r--   0        0        0      498 2023-02-20 14:13:19.750549 simple_cog_client-0.1.1/simple_cog_client/processors.py
--rw-r--r--   0        0        0     1239 2023-02-20 14:12:16.033909 simple_cog_client-0.1.1/simple_cog_client/use_cases.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 simple_cog_client-0.1.1/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 simple_cog_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-20 03:52:31.044496 simple_cog_client-0.1.2/README.md
+-rw-r--r--   0        0        0      363 2023-04-12 22:18:05.638564 simple_cog_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-02-20 03:56:04.536257 simple_cog_client-0.1.2/simple_cog_client/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-20 06:19:16.473488 simple_cog_client-0.1.2/simple_cog_client/client.py
+-rw-r--r--   0        0        0      717 2023-04-12 19:42:16.597760 simple_cog_client-0.1.2/simple_cog_client/processors.py
+-rw-r--r--   0        0        0     1239 2023-02-20 14:12:16.033909 simple_cog_client-0.1.2/simple_cog_client/use_cases.py
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 simple_cog_client-0.1.2/setup.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 simple_cog_client-0.1.2/PKG-INFO
```

### Comparing `simple_cog_client-0.1.1/simple_cog_client/use_cases.py` & `simple_cog_client-0.1.2/simple_cog_client/use_cases.py`

 * *Files identical despite different names*

### Comparing `simple_cog_client-0.1.1/setup.py` & `simple_cog_client-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pillow>=9.4.0,<10.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'simple-cog-client',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'Carlos Aranda',
     'author_email': 'carlos.aranda@ksms.mx',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `simple_cog_client-0.1.1/PKG-INFO` & `simple_cog_client-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-cog-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Carlos Aranda
 Author-email: carlos.aranda@ksms.mx
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

