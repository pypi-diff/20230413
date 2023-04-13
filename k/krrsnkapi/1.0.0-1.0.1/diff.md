# Comparing `tmp/krrsnkapi-1.0.0.tar.gz` & `tmp/krrsnkapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-1.0.0.tar", last modified: Thu Apr 13 11:33:48 2023, max compression
+gzip compressed data, was "krrsnkapi-1.0.1.tar", last modified: Thu Apr 13 11:57:19 2023, max compression
```

## Comparing `krrsnkapi-1.0.0.tar` & `krrsnkapi-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:33:48.907725 krrsnkapi-1.0.0/
--rw-rw-rw-   0        0        0     1082 2023-04-13 10:47:17.000000 krrsnkapi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2067 2023-04-13 11:33:48.908725 krrsnkapi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1572 2023-04-13 11:13:16.000000 krrsnkapi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:33:48.905725 krrsnkapi-1.0.0/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0     2067 2023-04-13 11:33:48.000000 krrsnkapi-1.0.0/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-13 11:33:48.000000 krrsnkapi-1.0.0/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:33:48.000000 krrsnkapi-1.0.0/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 11:33:48.000000 krrsnkapi-1.0.0/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:33:48.000000 krrsnkapi-1.0.0/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 11:33:48.911725 krrsnkapi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-04-13 11:33:09.000000 krrsnkapi-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:57:18.973376 krrsnkapi-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-13 10:47:17.000000 krrsnkapi-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2067 2023-04-13 11:57:18.975376 krrsnkapi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1572 2023-04-13 11:13:16.000000 krrsnkapi-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:57:18.924373 krrsnkapi-1.0.1/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0     2067 2023-04-13 11:57:17.000000 krrsnkapi-1.0.1/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-13 11:57:18.000000 krrsnkapi-1.0.1/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:57:17.000000 krrsnkapi-1.0.1/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 11:57:17.000000 krrsnkapi-1.0.1/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 11:57:17.000000 krrsnkapi-1.0.1/krrsnkapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 11:57:18.969375 krrsnkapi-1.0.1/package/
+-rw-rw-rw-   0        0        0       20 2023-04-13 11:56:50.000000 krrsnkapi-1.0.1/package/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-12 17:26:21.000000 krrsnkapi-1.0.1/package/krrsnkapi.py
+-rw-rw-rw-   0        0        0       86 2023-04-13 11:57:18.979376 krrsnkapi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-04-13 11:57:09.000000 krrsnkapi-1.0.1/setup.py
```

### Comparing `krrsnkapi-1.0.0/LICENSE` & `krrsnkapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krrsnkapi-1.0.0/PKG-INFO` & `krrsnkapi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for easy use of my api
 Home-page: https://github.com/kararasenok-gd/krrsnk-api
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 Project-URL: Documentation, https://github.com/kararasenok-gd/krrsnk-api
 Keywords: api
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `krrsnkapi-1.0.0/README.md` & `krrsnkapi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-1.0.0/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-1.0.1/krrsnkapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for easy use of my api
 Home-page: https://github.com/kararasenok-gd/krrsnk-api
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 Project-URL: Documentation, https://github.com/kararasenok-gd/krrsnk-api
 Keywords: api
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `krrsnkapi-1.0.0/setup.py` & `krrsnkapi-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='krrsnkapi',
-  version='1.0.0',
+  version='1.0.1',
   author='kararasenok_gd',
   author_email='murzikkurzikpro@gmail.com',
   description='Module for easy use of my api',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/kararasenok-gd/krrsnk-api',
   packages=find_packages(),
```

