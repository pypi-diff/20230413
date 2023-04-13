# Comparing `tmp/libs3tl-0.1.8.tar.gz` & `tmp/libs3tl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libs3tl-0.1.8.tar", last modified: Thu Oct 27 05:48:00 2022, max compression
+gzip compressed data, was "libs3tl-0.1.9.tar", last modified: Thu Oct 27 05:50:47 2022, max compression
```

## Comparing `libs3tl-0.1.8.tar` & `libs3tl-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-27 05:48:00.214622 libs3tl-0.1.8/
--rw-rw-rw-   0        0        0     1073 2022-10-20 06:03:17.000000 libs3tl-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1743 2022-10-27 05:48:00.213619 libs3tl-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2022-10-26 03:34:15.000000 libs3tl-0.1.8/README.txt
-drwxrwxrwx   0        0        0        0 2022-10-27 05:48:00.182373 libs3tl-0.1.8/libs3tl/
--rw-rw-rw-   0        0        0     1276 2022-10-27 05:44:27.000000 libs3tl-0.1.8/libs3tl/Extract.py
--rw-rw-rw-   0        0        0      629 2022-10-25 11:32:11.000000 libs3tl-0.1.8/libs3tl/Load.py
--rw-rw-rw-   0        0        0     1810 2022-10-25 11:40:53.000000 libs3tl-0.1.8/libs3tl/Ml.py
--rw-rw-rw-   0        0        0     8206 2022-10-21 09:56:33.000000 libs3tl-0.1.8/libs3tl/Step.py
--rw-rw-rw-   0        0        0     3086 2022-10-25 11:34:32.000000 libs3tl-0.1.8/libs3tl/Transform.py
--rw-rw-rw-   0        0        0        0 2022-10-20 06:03:17.000000 libs3tl-0.1.8/libs3tl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-27 05:48:00.212633 libs3tl-0.1.8/libs3tl.egg-info/
--rw-rw-rw-   0        0        0     1743 2022-10-27 05:48:00.000000 libs3tl-0.1.8/libs3tl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2022-10-27 05:48:00.000000 libs3tl-0.1.8/libs3tl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-27 05:48:00.000000 libs3tl-0.1.8/libs3tl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2022-10-27 05:48:00.000000 libs3tl-0.1.8/libs3tl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-27 05:48:00.000000 libs3tl-0.1.8/libs3tl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-27 05:48:00.214622 libs3tl-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1194 2022-10-27 05:47:18.000000 libs3tl-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-27 05:50:47.631007 libs3tl-0.1.9/
+-rw-rw-rw-   0        0        0     1073 2022-10-20 06:03:17.000000 libs3tl-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1743 2022-10-27 05:50:47.629006 libs3tl-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2022-10-26 03:34:15.000000 libs3tl-0.1.9/README.txt
+drwxrwxrwx   0        0        0        0 2022-10-27 05:50:47.603843 libs3tl-0.1.9/libs3tl/
+-rw-rw-rw-   0        0        0     1274 2022-10-27 05:50:01.000000 libs3tl-0.1.9/libs3tl/Extract.py
+-rw-rw-rw-   0        0        0      629 2022-10-25 11:32:11.000000 libs3tl-0.1.9/libs3tl/Load.py
+-rw-rw-rw-   0        0        0     1810 2022-10-25 11:40:53.000000 libs3tl-0.1.9/libs3tl/Ml.py
+-rw-rw-rw-   0        0        0     8206 2022-10-21 09:56:33.000000 libs3tl-0.1.9/libs3tl/Step.py
+-rw-rw-rw-   0        0        0     3086 2022-10-25 11:34:32.000000 libs3tl-0.1.9/libs3tl/Transform.py
+-rw-rw-rw-   0        0        0        0 2022-10-20 06:03:17.000000 libs3tl-0.1.9/libs3tl/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-27 05:50:47.627007 libs3tl-0.1.9/libs3tl.egg-info/
+-rw-rw-rw-   0        0        0     1743 2022-10-27 05:50:47.000000 libs3tl-0.1.9/libs3tl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2022-10-27 05:50:47.000000 libs3tl-0.1.9/libs3tl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-27 05:50:47.000000 libs3tl-0.1.9/libs3tl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2022-10-27 05:50:47.000000 libs3tl-0.1.9/libs3tl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-10-27 05:50:47.000000 libs3tl-0.1.9/libs3tl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-27 05:50:47.632007 libs3tl-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2022-10-27 05:50:16.000000 libs3tl-0.1.9/setup.py
```

### Comparing `libs3tl-0.1.8/LICENSE.txt` & `libs3tl-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/PKG-INFO` & `libs3tl-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libs3tl
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a 3TL module for pipeline creation
 Home-page: https://3tl.dev
 Author: Thinkartha
 Author-email: navin.naik@thinkartha.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libs3tl-0.1.8/README.txt` & `libs3tl-0.1.9/README.txt`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/libs3tl/Extract.py` & `libs3tl-0.1.9/libs3tl/Extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from requests import Request, Session
-from ..libs3tl import Step
+from libs3tl import Step
 import websocket
 
 
 class Extract(Step):
     def __init__(self):
         self.setStartTime()
         self.step = "Ex"
```

### Comparing `libs3tl-0.1.8/libs3tl/Load.py` & `libs3tl-0.1.9/libs3tl/Load.py`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/libs3tl/Ml.py` & `libs3tl-0.1.9/libs3tl/Ml.py`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/libs3tl/Step.py` & `libs3tl-0.1.9/libs3tl/Step.py`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/libs3tl/Transform.py` & `libs3tl-0.1.9/libs3tl/Transform.py`

 * *Files identical despite different names*

### Comparing `libs3tl-0.1.8/libs3tl.egg-info/PKG-INFO` & `libs3tl-0.1.9/libs3tl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libs3tl
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a 3TL module for pipeline creation
 Home-page: https://3tl.dev
 Author: Thinkartha
 Author-email: navin.naik@thinkartha.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libs3tl-0.1.8/setup.py` & `libs3tl-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='libs3tl',
-    version='0.1.8',    
+    version='0.1.9',    
     description='This is a 3TL module for pipeline creation',
     long_description_content_type=open('README.txt').read(),
     url='https://3tl.dev',
     author='Thinkartha',
     author_email='navin.naik@thinkartha.com',
     license='BSD 2-clause',
     packages=['libs3tl'],
```

