# Comparing `tmp/video2frames-0.0.2.tar.gz` & `tmp/video2frames-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2frames-0.0.2.tar", last modified: Thu Apr 13 16:39:22 2023, max compression
+gzip compressed data, was "video2frames-0.0.3.tar", last modified: Thu Apr 13 18:11:47 2023, max compression
```

## Comparing `video2frames-0.0.2.tar` & `video2frames-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:22.558308 video2frames-0.0.2/
--rw-rw-rw-   0        0        0      531 2023-04-13 16:39:22.554301 video2frames-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-13 16:39:22.558308 video2frames-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-04-13 16:38:23.000000 video2frames-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:22.518298 video2frames-0.0.2/video2frames/
--rw-rw-rw-   0        0        0       44 2023-04-13 16:27:35.000000 video2frames-0.0.2/video2frames/__init__.py
--rw-rw-rw-   0        0        0      977 2023-04-13 15:38:02.000000 video2frames-0.0.2/video2frames/frame_split.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:22.550306 video2frames-0.0.2/video2frames.egg-info/
--rw-rw-rw-   0        0        0      531 2023-04-13 16:39:22.000000 video2frames-0.0.2/video2frames.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-13 16:39:22.000000 video2frames-0.0.2/video2frames.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:39:22.000000 video2frames-0.0.2/video2frames.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 16:39:22.000000 video2frames-0.0.2/video2frames.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 16:39:22.000000 video2frames-0.0.2/video2frames.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:11:47.223964 video2frames-0.0.3/
+-rw-rw-rw-   0        0        0      531 2023-04-13 18:11:47.222963 video2frames-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:11:47.224963 video2frames-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-04-13 18:10:52.000000 video2frames-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:11:47.164573 video2frames-0.0.3/video2frames/
+-rw-rw-rw-   0        0        0       32 2023-04-13 16:45:53.000000 video2frames-0.0.3/video2frames/__init__.py
+-rw-rw-rw-   0        0        0      979 2023-04-13 18:08:17.000000 video2frames-0.0.3/video2frames/frame_split.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:11:47.220962 video2frames-0.0.3/video2frames.egg-info/
+-rw-rw-rw-   0        0        0      531 2023-04-13 18:11:46.000000 video2frames-0.0.3/video2frames.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-13 18:11:47.000000 video2frames-0.0.3/video2frames.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:11:46.000000 video2frames-0.0.3/video2frames.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 18:11:46.000000 video2frames-0.0.3/video2frames.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 18:11:46.000000 video2frames-0.0.3/video2frames.egg-info/top_level.txt
```

### Comparing `video2frames-0.0.2/PKG-INFO` & `video2frames-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2frames
-Version: 0.0.2
+Version: 0.0.3
 Summary: video2frames package test
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `video2frames-0.0.2/setup.py` & `video2frames-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'video2frames package test'
 LONG_DESCRIPTION = 'Testing video2frames in a package format'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="video2frames",
```

### Comparing `video2frames-0.0.2/video2frames/frame_split.py` & `video2frames-0.0.3/video2frames/frame_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cv2
 import os
 import argparse
 
 parser = argparse.ArgumentParser()
-parser.add_argument('-fps', '--frameRate', required = True, type = int, help = "Number of frames inbetween image capture")
-parser.add_argument('-vid', '--videoPath', required = True, type = str, help = "Path of video")
+parser.add_argument('-fps', '--frameRate', required = False, type = int, help = "Number of frames inbetween image capture")
+parser.add_argument('-vid', '--videoPath', required = False, type = str, help = "Path of video")
 args = parser.parse_args()
 frameRate = args.frameRate
 videoPath = args.videoPath
 
 sec = 0
 count = 1
```

### Comparing `video2frames-0.0.2/video2frames.egg-info/PKG-INFO` & `video2frames-0.0.3/video2frames.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2frames
-Version: 0.0.2
+Version: 0.0.3
 Summary: video2frames package test
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

