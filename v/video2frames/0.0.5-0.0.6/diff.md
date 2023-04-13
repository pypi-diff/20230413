# Comparing `tmp/video2frames-0.0.5.tar.gz` & `tmp/video2frames-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2frames-0.0.5.tar", last modified: Thu Apr 13 18:33:35 2023, max compression
+gzip compressed data, was "video2frames-0.0.6.tar", last modified: Thu Apr 13 18:37:50 2023, max compression
```

## Comparing `video2frames-0.0.5.tar` & `video2frames-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:33:35.042656 video2frames-0.0.5/
--rw-rw-rw-   0        0        0      531 2023-04-13 18:33:35.042656 video2frames-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-13 18:33:35.042656 video2frames-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-04-13 18:33:11.000000 video2frames-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:33:35.005946 video2frames-0.0.5/video2frames/
--rw-rw-rw-   0        0        0       40 2023-04-13 18:27:38.000000 video2frames-0.0.5/video2frames/__init__.py
--rw-rw-rw-   0        0        0     1044 2023-04-13 18:27:37.000000 video2frames-0.0.5/video2frames/frame_split.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:33:35.038657 video2frames-0.0.5/video2frames.egg-info/
--rw-rw-rw-   0        0        0      531 2023-04-13 18:33:34.000000 video2frames-0.0.5/video2frames.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-13 18:33:34.000000 video2frames-0.0.5/video2frames.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:33:34.000000 video2frames-0.0.5/video2frames.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 18:33:34.000000 video2frames-0.0.5/video2frames.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 18:33:34.000000 video2frames-0.0.5/video2frames.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:37:50.110448 video2frames-0.0.6/
+-rw-rw-rw-   0        0        0      531 2023-04-13 18:37:50.106448 video2frames-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:37:50.110448 video2frames-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-04-13 18:36:46.000000 video2frames-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:37:49.988968 video2frames-0.0.6/video2frames/
+-rw-rw-rw-   0        0        0       40 2023-04-13 18:27:38.000000 video2frames-0.0.6/video2frames/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-04-13 18:36:56.000000 video2frames-0.0.6/video2frames/frame_split.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:37:50.102454 video2frames-0.0.6/video2frames.egg-info/
+-rw-rw-rw-   0        0        0      531 2023-04-13 18:37:49.000000 video2frames-0.0.6/video2frames.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-13 18:37:49.000000 video2frames-0.0.6/video2frames.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:37:49.000000 video2frames-0.0.6/video2frames.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 18:37:49.000000 video2frames-0.0.6/video2frames.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 18:37:49.000000 video2frames-0.0.6/video2frames.egg-info/top_level.txt
```

### Comparing `video2frames-0.0.5/PKG-INFO` & `video2frames-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2frames
-Version: 0.0.5
+Version: 0.0.6
 Summary: video2frames package test
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `video2frames-0.0.5/setup.py` & `video2frames-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'video2frames package test'
 LONG_DESCRIPTION = 'Testing video2frames in a package format'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="video2frames",
```

### Comparing `video2frames-0.0.5/video2frames/frame_split.py` & `video2frames-0.0.6/video2frames/frame_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # parser.add_argument('-vid', '--videoPath', required = False, type = str, help = "Path of video")
 # args = parser.parse_args()
 # frameRate = args.frameRate
 # videoPath = args.videoPath
 
 sec = 0
 count = 1
-frameRate = 2.75
+frameRate = 5
 videoPath = ('videos/video2.mp4')
 
 vidcap = cv2.VideoCapture(videoPath)
 
 directory = 'capture'
 if not os.path.exists(directory):
     os.makedirs(directory)
```

### Comparing `video2frames-0.0.5/video2frames.egg-info/PKG-INFO` & `video2frames-0.0.6/video2frames.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2frames
-Version: 0.0.5
+Version: 0.0.6
 Summary: video2frames package test
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

