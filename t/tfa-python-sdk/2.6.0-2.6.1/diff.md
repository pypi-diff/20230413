# Comparing `tmp/tfa-python-sdk-2.6.0.tar.gz` & `tmp/tfa-python-sdk-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfa-python-sdk-2.6.0.tar", last modified: Tue Apr 11 21:57:04 2023, max compression
+gzip compressed data, was "tfa-python-sdk-2.6.1.tar", last modified: Thu Apr 13 09:27:14 2023, max compression
```

## Comparing `tfa-python-sdk-2.6.0.tar` & `tfa-python-sdk-2.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.233758 tfa-python-sdk-2.6.0/
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     1111 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/LICENSE
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-11 21:57:04.233869 tfa-python-sdk-2.6.0/PKG-INFO
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2525 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/README.md
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       79 2023-04-11 21:57:04.234123 tfa-python-sdk-2.6.0/setup.cfg
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      568 2023-04-11 21:54:32.000000 tfa-python-sdk-2.6.0/setup.py
-drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.232539 tfa-python-sdk-2.6.0/tfa_python_sdk/
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       31 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/tfa_python_sdk/__init__.py
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      563 2023-04-11 21:50:36.000000 tfa-python-sdk-2.6.0/tfa_python_sdk/tfa_python_sdk.py
-drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.233622 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      285 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)        1 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/requires.txt
--rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-13 09:27:14.975154 tfa-python-sdk-2.6.1/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     1111 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.1/LICENSE
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-13 09:27:14.975203 tfa-python-sdk-2.6.1/PKG-INFO
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2525 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.1/README.md
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       79 2023-04-13 09:27:14.975369 tfa-python-sdk-2.6.1/setup.cfg
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      568 2023-04-13 09:26:54.000000 tfa-python-sdk-2.6.1/setup.py
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-13 09:27:14.974543 tfa-python-sdk-2.6.1/tfa_python_sdk/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       31 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.1/tfa_python_sdk/__init__.py
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      509 2023-04-13 09:26:30.000000 tfa-python-sdk-2.6.1/tfa_python_sdk/tfa_python_sdk.py
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-13 09:27:14.975054 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-13 09:27:14.000000 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      285 2023-04-13 09:27:14.000000 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)        1 2023-04-13 09:27:14.000000 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-13 09:27:14.000000 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-13 09:27:14.000000 tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/top_level.txt
```

### Comparing `tfa-python-sdk-2.6.0/LICENSE` & `tfa-python-sdk-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tfa-python-sdk-2.6.0/PKG-INFO` & `tfa-python-sdk-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfa-python-sdk
-Version: 2.6.0
+Version: 2.6.1
 Summary: Telegram Factor Authentication python library
 Home-page: https://github.com/tfasoft/sdk-python
 Author: Amirhossein Mohammadi
 Author-email: amirhosseinmohammadi1380@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tfa-python-sdk-2.6.0/README.md` & `tfa-python-sdk-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tfa-python-sdk-2.6.0/setup.py` & `tfa-python-sdk-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='tfa-python-sdk',
-    version='2.6.0',
+    version='2.6.1',
     author='Amirhossein Mohammadi',
     license='MIT',
     author_email="amirhosseinmohammadi1380@yahoo.com",
     description="Telegram Factor Authentication python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tfasoft/sdk-python",
```

### Comparing `tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/PKG-INFO` & `tfa-python-sdk-2.6.1/tfa_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfa-python-sdk
-Version: 2.6.0
+Version: 2.6.1
 Summary: Telegram Factor Authentication python library
 Home-page: https://github.com/tfasoft/sdk-python
 Author: Amirhossein Mohammadi
 Author-email: amirhosseinmohammadi1380@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

