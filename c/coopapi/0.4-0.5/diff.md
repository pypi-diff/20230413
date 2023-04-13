# Comparing `tmp/coopapi-0.4.tar.gz` & `tmp/coopapi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopapi-0.4.tar", last modified: Tue Feb 28 17:58:03 2023, max compression
+gzip compressed data, was "coopapi-0.5.tar", last modified: Thu Apr 13 17:37:33 2023, max compression
```

## Comparing `coopapi-0.4.tar` & `coopapi-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 17:58:03.019937 coopapi-0.4/
--rw-rw-rw-   0        0        0     2838 2023-02-28 17:58:03.018965 coopapi-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 17:58:02.991937 coopapi-0.4/coopapi/
--rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.4/coopapi/__init__.py
--rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.4/coopapi/apiShell.py
--rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.4/coopapi/enums.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.4/coopapi/errors.py
--rw-rw-rw-   0        0        0     4536 2023-02-28 17:55:46.000000 coopapi-0.4/coopapi/http_request.py
--rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.4/coopapi/http_request_handlers.py
-drwxrwxrwx   0        0        0        0 2023-02-28 17:58:03.017937 coopapi-0.4/coopapi.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-02-28 17:58:02.000000 coopapi-0.4/coopapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-02-28 17:58:02.000000 coopapi-0.4/coopapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 17:58:02.000000 coopapi-0.4/coopapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.4/coopapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      279 2023-02-28 17:58:02.000000 coopapi-0.4/coopapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-28 17:58:02.000000 coopapi-0.4/coopapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-28 17:58:03.019937 coopapi-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-02-28 17:57:59.000000 coopapi-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.080935 coopapi-0.5/
+-rw-rw-rw-   0        0        0     2838 2023-04-13 17:37:33.079902 coopapi-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.051928 coopapi-0.5/coopapi/
+-rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.5/coopapi/__init__.py
+-rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.5/coopapi/apiShell.py
+-rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.5/coopapi/enums.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.5/coopapi/errors.py
+-rw-rw-rw-   0        0        0     4536 2023-02-28 17:55:46.000000 coopapi-0.5/coopapi/http_request.py
+-rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.5/coopapi/http_request_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.077926 coopapi-0.5/coopapi.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-04-13 17:37:33.000000 coopapi-0.5/coopapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.5/coopapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      279 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:37:33.080935 coopapi-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-04-13 17:37:25.000000 coopapi-0.5/setup.py
```

### Comparing `coopapi-0.4/PKG-INFO` & `coopapi-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.4
+Version: 0.5
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.4/README.md` & `coopapi-0.5/README.md`

 * *Files identical despite different names*

### Comparing `coopapi-0.4/coopapi/apiShell.py` & `coopapi-0.5/coopapi/apiShell.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.4/coopapi/http_request.py` & `coopapi-0.5/coopapi/http_request.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.4/coopapi/http_request_handlers.py` & `coopapi-0.5/coopapi/http_request_handlers.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.4/coopapi.egg-info/PKG-INFO` & `coopapi-0.5/coopapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.4
+Version: 0.5
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.4/setup.py` & `coopapi-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopapi',
-      version='0.04',
+      version='0.05',
       description='Tools for setting up an API. Built on the FastAPI framework',
       url='https://github.com/tylertjburns/coopapi',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

