# Comparing `tmp/icecube-skyreader-0.0.1.tar.gz` & `tmp/icecube-skyreader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-0.0.1.tar", last modified: Thu Apr 13 20:07:05 2023, max compression
+gzip compressed data, was "icecube-skyreader-0.0.2.tar", last modified: Thu Apr 13 20:09:30 2023, max compression
```

## Comparing `icecube-skyreader-0.0.1.tar` & `icecube-skyreader-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1954 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1954 2023-04-13 20:07:05.000000 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-13 20:07:05.000000 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 20:07:05.000000 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-13 20:07:05.000000 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 20:07:05.000000 icecube-skyreader-0.0.1/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1671 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/skyreader/
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 20:07:02.000000 icecube-skyreader-0.0.1/skyreader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:07:05.990691 icecube-skyreader-0.0.1/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-13 20:07:01.000000 icecube-skyreader-0.0.1/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:09:30.152757 icecube-skyreader-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-13 20:09:30.152757 icecube-skyreader-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:09:30.148757 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-13 20:09:30.000000 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-13 20:09:30.000000 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 20:09:30.000000 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-13 20:09:30.000000 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 20:09:30.000000 icecube-skyreader-0.0.2/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 20:09:30.152757 icecube-skyreader-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:09:30.148757 icecube-skyreader-0.0.2/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 20:09:28.000000 icecube-skyreader-0.0.2/skyreader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 20:09:30.152757 icecube-skyreader-0.0.2/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-13 20:09:27.000000 icecube-skyreader-0.0.2/skyreader/result.py
```

### Comparing `icecube-skyreader-0.0.1/LICENSE` & `icecube-skyreader-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.0.1/PKG-INFO` & `icecube-skyreader-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.0.1
+Version: 0.0.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
 Project-URL: Source, https://github.com/icecube/skyreader
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skyreader-0.0.1/README.md` & `icecube-skyreader-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.0.1/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-0.0.2/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.0.1
+Version: 0.0.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
 Project-URL: Source, https://github.com/icecube/skyreader
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skyreader-0.0.1/setup.cfg` & `icecube-skyreader-0.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	skymap
 	HEALPix
 	neutrino
 	reconstruction
 	IceCube
 license = MIT
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 download_url = https://pypi.org/project/icecube-skyreader/
 project_urls =
```

### Comparing `icecube-skyreader-0.0.1/skyreader/__init__.py` & `icecube-skyreader-0.0.2/skyreader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

