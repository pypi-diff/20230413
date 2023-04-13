# Comparing `tmp/glass-camb-2023.2.tar.gz` & `tmp/glass.camb-2023.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glass-camb-2023.2.tar", last modified: Wed Mar  1 11:56:21 2023, max compression
+gzip compressed data, was "glass.camb-2023.2.dev1.tar", last modified: Thu Apr 13 21:01:39 2023, max compression
```

## Comparing `glass-camb-2023.2.tar` & `glass.camb-2023.2.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:56:21.783410 glass-camb-2023.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-01 11:56:11.000000 glass-camb-2023.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-01 11:56:21.783410 glass-camb-2023.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-01 11:56:11.000000 glass-camb-2023.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:56:21.779410 glass-camb-2023.2/glass/
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-01 11:56:11.000000 glass-camb-2023.2/glass/camb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:56:21.783410 glass-camb-2023.2/glass_camb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-01 11:56:21.000000 glass-camb-2023.2/glass_camb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-01 11:56:21.000000 glass-camb-2023.2/glass_camb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:56:21.000000 glass-camb-2023.2/glass_camb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 11:56:21.000000 glass-camb-2023.2/glass_camb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 11:56:21.000000 glass-camb-2023.2/glass_camb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-01 11:56:21.783410 glass-camb-2023.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 11:56:11.000000 glass-camb-2023.2/setup.py
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-13 21:01:39.962987 glass.camb-2023.2.dev1/
+-rw-r--r--   0 ntessore   (501) staff       (20)     1072 2022-03-21 22:38:33.000000 glass.camb-2023.2.dev1/LICENSE
+-rw-r--r--   0 ntessore   (501) staff       (20)      716 2023-04-13 21:01:39.963096 glass.camb-2023.2.dev1/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)      157 2023-02-05 01:16:20.000000 glass.camb-2023.2.dev1/README.md
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-13 21:01:39.960775 glass.camb-2023.2.dev1/glass/
+-rw-r--r--   0 ntessore   (501) staff       (20)     1902 2023-04-13 21:01:21.000000 glass.camb-2023.2.dev1/glass/camb.py
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-13 21:01:39.962782 glass.camb-2023.2.dev1/glass.camb.egg-info/
+-rw-r--r--   0 ntessore   (501) staff       (20)      716 2023-04-13 21:01:39.000000 glass.camb-2023.2.dev1/glass.camb.egg-info/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)      219 2023-04-13 21:01:39.000000 glass.camb-2023.2.dev1/glass.camb.egg-info/SOURCES.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-13 21:01:39.000000 glass.camb-2023.2.dev1/glass.camb.egg-info/dependency_links.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)       40 2023-04-13 21:01:39.000000 glass.camb-2023.2.dev1/glass.camb.egg-info/requires.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)        6 2023-04-13 21:01:39.000000 glass.camb-2023.2.dev1/glass.camb.egg-info/top_level.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)      812 2023-04-13 21:01:39.964003 glass.camb-2023.2.dev1/setup.cfg
+-rw-r--r--   0 ntessore   (501) staff       (20)       38 2022-03-11 21:52:33.000000 glass.camb-2023.2.dev1/setup.py
```

### Comparing `glass-camb-2023.2/LICENSE` & `glass.camb-2023.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `glass-camb-2023.2/PKG-INFO` & `glass.camb-2023.2.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: glass-camb
-Version: 2023.2
+Name: glass.camb
+Version: 2023.2.dev1
 Summary: GLASS module for CAMB interoperability
 Home-page: https://github.com/glass-dev/glass-camb
 Maintainer: Nicolas Tessore
 Maintainer-email: n.tessore@ucl.ac.uk
 License: MIT
 Project-URL: Issues, https://github.com/glass-dev/glass-camb/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glass-camb-2023.2/glass/camb.py` & `glass.camb-2023.2.dev1/glass/camb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # author: Nicolas Tessore <n.tessore@ucl.ac.uk>
 # license: MIT
 '''GLASS module for CAMB interoperability'''
 
-__version__ = '2023.2'
+__version__ = '2023.2.dev1'
 
 import warnings
 import numpy as np
 import camb
 
 
 def camb_tophat_weight(z):
```

### Comparing `glass-camb-2023.2/glass_camb.egg-info/PKG-INFO` & `glass.camb-2023.2.dev1/glass.camb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: glass-camb
-Version: 2023.2
+Name: glass.camb
+Version: 2023.2.dev1
 Summary: GLASS module for CAMB interoperability
 Home-page: https://github.com/glass-dev/glass-camb
 Maintainer: Nicolas Tessore
 Maintainer-email: n.tessore@ucl.ac.uk
 License: MIT
 Project-URL: Issues, https://github.com/glass-dev/glass-camb/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glass-camb-2023.2/setup.cfg` & `glass.camb-2023.2.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = glass-camb
+name = glass.camb
 version = attr: glass.camb.__version__
 maintainer = Nicolas Tessore
 maintainer_email = n.tessore@ucl.ac.uk
 description = GLASS module for CAMB interoperability
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

