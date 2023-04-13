# Comparing `tmp/rdhyee_utils-0.1.7.tar.gz` & `tmp/rdhyee_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rdhyee_utils-0.1.7.tar", last modified: Mon Feb 17 01:09:46 2014, max compression
+gzip compressed data, was "dist/rdhyee_utils-0.1.8.tar", last modified: Fri Mar 31 06:29:42 2017, max compression
```

## Comparing `rdhyee_utils-0.1.7.tar` & `rdhyee_utils-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 raymondyee   (501) raymondyee   (501)        0 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      453 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/PKG-INFO
-drwxr-xr-x   0 raymondyee   (501) raymondyee   (501)        0 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/rdhyee_utils/
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      863 2013-10-15 18:31:21.000000 rdhyee_utils-0.1.7/rdhyee_utils/__init__.py
-drwxr-xr-x   0 raymondyee   (501) raymondyee   (501)        0 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/rdhyee_utils/aws/
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)     6175 2013-10-15 18:47:26.000000 rdhyee_utils-0.1.7/rdhyee_utils/aws/__init__.py
-drwxr-xr-x   0 raymondyee   (501) raymondyee   (501)        0 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)        1 2014-02-17 01:09:45.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/dependency_links.txt
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)       37 2014-02-17 01:09:45.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/entry_points.txt
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)        1 2013-10-15 15:48:57.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/not-zip-safe
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      453 2014-02-17 01:09:45.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/PKG-INFO
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      290 2014-02-17 01:09:45.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/SOURCES.txt
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)       13 2014-02-17 01:09:45.000000 rdhyee_utils-0.1.7/rdhyee_utils.egg-info/top_level.txt
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      100 2014-02-17 01:09:46.000000 rdhyee_utils-0.1.7/setup.cfg
--rw-r--r--   0 raymondyee   (501) raymondyee   (501)      951 2014-02-17 00:25:10.000000 rdhyee_utils-0.1.7/setup.py
+drwxr-xr-x   0 raymondyee   (501) access_bpf   (501)        0 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)      453 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/PKG-INFO
+drwxr-xr-x   0 raymondyee   (501) access_bpf   (501)        0 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils/
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)      870 2017-03-31 05:24:06.000000 rdhyee_utils-0.1.8/rdhyee_utils/__init__.py
+drwxr-xr-x   0 raymondyee   (501) access_bpf   (501)        0 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils/aws/
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)     6175 2013-10-15 18:47:26.000000 rdhyee_utils-0.1.8/rdhyee_utils/aws/__init__.py
+drwxr-xr-x   0 raymondyee   (501) access_bpf   (501)        0 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)        1 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)       37 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/entry_points.txt
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)        1 2013-10-15 15:48:57.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/not-zip-safe
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)       47 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/pbr.json
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)      453 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/PKG-INFO
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)      321 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)       13 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/rdhyee_utils.egg-info/top_level.txt
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)       79 2017-03-31 06:29:42.000000 rdhyee_utils-0.1.8/setup.cfg
+-rw-r--r--   0 raymondyee   (501) access_bpf   (501)      951 2017-03-31 06:28:43.000000 rdhyee_utils-0.1.8/setup.py
```

### Comparing `rdhyee_utils-0.1.7/rdhyee_utils/__init__.py` & `rdhyee_utils-0.1.8/rdhyee_utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     instances = {}
     def getinstance():
         if cls not in instances:
             instances[cls] = cls()
         return instances[cls]
     return getinstance
 
-def nowish_tz():
+def nowish_tz(tzname='US/Pacific'):
     # put in Pacific time
-    tz_PT = pytz.timezone("US/Pacific")
-    return datetime.datetime(*datetime.datetime.utcnow().timetuple()[:6]).replace(tzinfo=pytz.utc).astimezone(tz_PT)
+    tz = pytz.timezone(tzname)
+    return datetime.datetime(*datetime.datetime.utcnow().timetuple()[:6]).replace(tzinfo=pytz.utc).astimezone(tz)
```

### Comparing `rdhyee_utils-0.1.7/rdhyee_utils/aws/__init__.py` & `rdhyee_utils-0.1.8/rdhyee_utils/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `rdhyee_utils-0.1.7/setup.py` & `rdhyee_utils-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.1.7'
+version = '0.1.8'
 
 setup(name='rdhyee_utils',
       version=version,
       description="Some simple methods and classes Raymond Yee developed for his own work.",
       long_description="""\
 Some simple methods and classes Raymond Yee developed for his own work.""",
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
       keywords='utilities',
       author='Raymond Yee',
       author_email='raymond.yee@gmail.com',
       url='https://github.com/rdhyee/rdhyee_utils',
-      download_url="https://github.com/rdhyee/rdhyee_utils/tarball/0.1.7",
+      download_url="https://github.com/rdhyee/rdhyee_utils/tarball/0.1.8",
       license='Apache 2.0',
       packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           # -*- Extra requirements: -*-
       ],
```

