# Comparing `tmp/django-mapper-0.1.0.tar.gz` & `tmp/django-mapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-0.1.0.tar", last modified: Thu Apr 13 20:52:33 2023, max compression
+gzip compressed data, was "django-mapper-0.1.1.tar", last modified: Thu Apr 13 21:45:42 2023, max compression
```

## Comparing `django-mapper-0.1.0.tar` & `django-mapper-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 20:52:33.421026 django-mapper-0.1.0/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      668 2023-04-13 20:52:33.421026 django-mapper-0.1.0/PKG-INFO
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 20:52:33.421026 django-mapper-0.1.0/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-0.1.0/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2481 2023-04-13 20:17:57.000000 django-mapper-0.1.0/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 20:52:33.421026 django-mapper-0.1.0/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      668 2023-04-13 20:52:33.000000 django-mapper-0.1.0/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      242 2023-04-13 20:52:33.000000 django-mapper-0.1.0/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-13 20:52:33.000000 django-mapper-0.1.0/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-13 20:52:33.000000 django-mapper-0.1.0/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-13 20:52:33.000000 django-mapper-0.1.0/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-13 20:52:33.421026 django-mapper-0.1.0/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      779 2023-04-13 20:13:18.000000 django-mapper-0.1.0/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-13 21:45:42.964242 django-mapper-0.1.1/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-0.1.1/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-0.1.1/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     2481 2023-04-13 20:17:57.000000 django-mapper-0.1.1/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-13 21:45:42.964242 django-mapper-0.1.1/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-13 21:43:57.000000 django-mapper-0.1.1/setup.py
```

### Comparing `django-mapper-0.1.0/PKG-INFO` & `django-mapper-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility class for mapping data between Django models
-Home-page: https://github.com/yourusername/django-mapper
-Author: Your Name
-Author-email: your@email.com
+Home-page: https://github.com/shubh95/django-mapper
+Author: Shubham Vashisht
+Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-mapper-0.1.0/django_mapper/mapper.py` & `django-mapper-0.1.1/django_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mapper-0.1.0/django_mapper.egg-info/PKG-INFO` & `django-mapper-0.1.1/django_mapper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility class for mapping data between Django models
-Home-page: https://github.com/yourusername/django-mapper
-Author: Your Name
-Author-email: your@email.com
+Home-page: https://github.com/shubh95/django-mapper
+Author: Shubham Vashisht
+Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-mapper-0.1.0/setup.py` & `django-mapper-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='0.1.0',
+    version='0.1.1',
     description='A utility class for mapping data between Django models',
-    author='Your Name',
-    author_email='your@email.com',
-    url='https://github.com/yourusername/django-mapper',
+    author='Shubham Vashisht',
+    author_email='shubhvas95@gmail.com',
+    url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

