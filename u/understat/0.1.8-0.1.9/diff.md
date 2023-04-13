# Comparing `tmp/understat-0.1.8.tar.gz` & `tmp/understat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/amosbastian/Development/understat/dist/.tmp-k37lqgn5/understat-0.1.8.tar", last modified: Wed Jan  4 17:14:35 2023, max compression
+gzip compressed data, was "/Users/amosbastian/Development/understat/dist/.tmp-yk_5djoa/understat-0.1.9.tar", last modified: Sun Jan  8 13:14:44 2023, max compression
```

## Comparing `understat-0.1.8.tar` & `understat-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-04 17:14:35.191329 understat-0.1.8/
--rw-r--r--   0 amosbastian   (501) staff       (20)      315 2022-07-26 11:00:32.000000 understat-0.1.8/AUTHORS.rst
--rw-r--r--   0 amosbastian   (501) staff       (20)     1069 2020-10-19 12:57:52.000000 understat-0.1.8/LICENSE
--rw-r--r--   0 amosbastian   (501) staff       (20)     3633 2023-01-04 17:14:35.190821 understat-0.1.8/PKG-INFO
--rw-r--r--   0 amosbastian   (501) staff       (20)     2802 2022-09-27 10:33:45.000000 understat-0.1.8/README.md
--rw-r--r--   0 amosbastian   (501) staff       (20)       38 2023-01-04 17:14:35.191414 understat-0.1.8/setup.cfg
--rw-r--r--   0 amosbastian   (501) staff       (20)     1282 2023-01-04 17:14:25.000000 understat-0.1.8/setup.py
-drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-04 17:14:35.185790 understat-0.1.8/tests/
--rw-r--r--   0 amosbastian   (501) staff       (20)        0 2022-07-26 10:54:38.000000 understat-0.1.8/tests/__init__.py
--rw-r--r--   0 amosbastian   (501) staff       (20)      212 2020-10-19 13:03:27.000000 understat-0.1.8/tests/conftest.py
--rw-r--r--   0 amosbastian   (501) staff       (20)     8840 2023-01-04 17:14:25.000000 understat-0.1.8/tests/test_understat.py
--rw-r--r--   0 amosbastian   (501) staff       (20)     2663 2022-07-26 11:00:32.000000 understat-0.1.8/tests/test_utils.py
-drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-04 17:14:35.188794 understat-0.1.8/understat/
--rw-r--r--   0 amosbastian   (501) staff       (20)       33 2020-10-19 12:57:52.000000 understat-0.1.8/understat/__init__.py
--rw-r--r--   0 amosbastian   (501) staff       (20)      271 2020-10-19 12:57:52.000000 understat-0.1.8/understat/constants.py
--rw-r--r--   0 amosbastian   (501) staff       (20)    14462 2022-09-27 10:33:45.000000 understat-0.1.8/understat/understat.py
--rw-r--r--   0 amosbastian   (501) staff       (20)     2681 2022-09-27 10:34:32.000000 understat-0.1.8/understat/utils.py
-drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-04 17:14:35.190446 understat-0.1.8/understat.egg-info/
--rw-r--r--   0 amosbastian   (501) staff       (20)     3633 2023-01-04 17:14:35.000000 understat-0.1.8/understat.egg-info/PKG-INFO
--rw-r--r--   0 amosbastian   (501) staff       (20)      369 2023-01-04 17:14:35.000000 understat-0.1.8/understat.egg-info/SOURCES.txt
--rw-r--r--   0 amosbastian   (501) staff       (20)        1 2023-01-04 17:14:35.000000 understat-0.1.8/understat.egg-info/dependency_links.txt
--rw-r--r--   0 amosbastian   (501) staff       (20)      127 2023-01-04 17:14:35.000000 understat-0.1.8/understat.egg-info/requires.txt
--rw-r--r--   0 amosbastian   (501) staff       (20)       16 2023-01-04 17:14:35.000000 understat-0.1.8/understat.egg-info/top_level.txt
+drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-08 13:14:44.066985 understat-0.1.9/
+-rw-r--r--   0 amosbastian   (501) staff       (20)      315 2022-07-26 11:00:32.000000 understat-0.1.9/AUTHORS.rst
+-rw-r--r--   0 amosbastian   (501) staff       (20)     1069 2020-10-19 12:57:52.000000 understat-0.1.9/LICENSE
+-rw-r--r--   0 amosbastian   (501) staff       (20)     3633 2023-01-08 13:14:44.066711 understat-0.1.9/PKG-INFO
+-rw-r--r--   0 amosbastian   (501) staff       (20)     2802 2022-09-27 10:33:45.000000 understat-0.1.9/README.md
+-rw-r--r--   0 amosbastian   (501) staff       (20)       38 2023-01-08 13:14:44.067104 understat-0.1.9/setup.cfg
+-rw-r--r--   0 amosbastian   (501) staff       (20)     1282 2023-01-08 13:13:54.000000 understat-0.1.9/setup.py
+drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-08 13:14:44.062301 understat-0.1.9/tests/
+-rw-r--r--   0 amosbastian   (501) staff       (20)        0 2022-07-26 10:54:38.000000 understat-0.1.9/tests/__init__.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)      212 2020-10-19 13:03:27.000000 understat-0.1.9/tests/conftest.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)     8840 2023-01-04 17:14:25.000000 understat-0.1.9/tests/test_understat.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)     2663 2022-07-26 11:00:32.000000 understat-0.1.9/tests/test_utils.py
+drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-08 13:14:44.064373 understat-0.1.9/understat/
+-rw-r--r--   0 amosbastian   (501) staff       (20)       33 2020-10-19 12:57:52.000000 understat-0.1.9/understat/__init__.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)      271 2020-10-19 12:57:52.000000 understat-0.1.9/understat/constants.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)    14462 2022-09-27 10:33:45.000000 understat-0.1.9/understat/understat.py
+-rw-r--r--   0 amosbastian   (501) staff       (20)     2711 2023-01-08 13:13:28.000000 understat-0.1.9/understat/utils.py
+drwxr-xr-x   0 amosbastian   (501) staff       (20)        0 2023-01-08 13:14:44.066176 understat-0.1.9/understat.egg-info/
+-rw-r--r--   0 amosbastian   (501) staff       (20)     3633 2023-01-08 13:14:44.000000 understat-0.1.9/understat.egg-info/PKG-INFO
+-rw-r--r--   0 amosbastian   (501) staff       (20)      369 2023-01-08 13:14:44.000000 understat-0.1.9/understat.egg-info/SOURCES.txt
+-rw-r--r--   0 amosbastian   (501) staff       (20)        1 2023-01-08 13:14:44.000000 understat-0.1.9/understat.egg-info/dependency_links.txt
+-rw-r--r--   0 amosbastian   (501) staff       (20)      127 2023-01-08 13:14:44.000000 understat-0.1.9/understat.egg-info/requires.txt
+-rw-r--r--   0 amosbastian   (501) staff       (20)       16 2023-01-08 13:14:44.000000 understat-0.1.9/understat.egg-info/top_level.txt
```

### Comparing `understat-0.1.8/LICENSE` & `understat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `understat-0.1.8/PKG-INFO` & `understat-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understat
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python wrapper for https://understat.com/
 Home-page: https://github.com/amosbastian/understat
 Author: amosbastian
 Author-email: amosbastian@gmail.com
 License: MIT
 Project-URL: Documentation, http://fpl.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/amosbastian/fpl
```

### Comparing `understat-0.1.8/README.md` & `understat-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `understat-0.1.8/setup.py` & `understat-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="understat",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     description="A Python wrapper for https://understat.com/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/amosbastian/understat",
     author="amosbastian",
     author_email="amosbastian@gmail.com",
```

### Comparing `understat-0.1.8/tests/test_understat.py` & `understat-0.1.9/tests/test_understat.py`

 * *Files identical despite different names*

### Comparing `understat-0.1.8/tests/test_utils.py` & `understat-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `understat-0.1.8/understat/understat.py` & `understat-0.1.9/understat/understat.py`

 * *Files identical despite different names*

### Comparing `understat-0.1.8/understat/utils.py` & `understat-0.1.9/understat/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     try:
         return league_mapper[league_name]
     except KeyError:
         return league_name
 
 
 async def fetch(session, url):
-    async with session.get(url) as response:
+    async with session.get(url, cookies={"beget": "begetok"}) as response:
         return await response.text()
 
 
 def find_match(scripts, pattern):
     """Returns the first match found in the given scripts."""
 
     for script in scripts:
```

### Comparing `understat-0.1.8/understat.egg-info/PKG-INFO` & `understat-0.1.9/understat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understat
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python wrapper for https://understat.com/
 Home-page: https://github.com/amosbastian/understat
 Author: amosbastian
 Author-email: amosbastian@gmail.com
 License: MIT
 Project-URL: Documentation, http://fpl.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/amosbastian/fpl
```

