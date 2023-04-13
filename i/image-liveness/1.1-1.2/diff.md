# Comparing `tmp/image-liveness-1.1.tar.gz` & `tmp/image-liveness-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-liveness-1.1.tar", last modified: Thu Apr 13 05:40:29 2023, max compression
+gzip compressed data, was "image-liveness-1.2.tar", last modified: Thu Apr 13 05:58:17 2023, max compression
```

## Comparing `image-liveness-1.1.tar` & `image-liveness-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 05:40:29.534982 image-liveness-1.1/
--rw-rw-rw-   0        0        0    11541 2023-04-13 04:10:36.000000 image-liveness-1.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 05:40:29.503999 image-liveness-1.1/Liveness/
--rw-rw-rw-   0        0        0     3359 2023-04-12 12:10:50.000000 image-liveness-1.1/Liveness/anti_spoof_predict.py
--rw-rw-rw-   0        0        0     1856 2023-04-12 10:44:07.000000 image-liveness-1.1/Liveness/generate_patches.py
--rw-rw-rw-   0        0        0     4554 2023-04-13 05:19:55.000000 image-liveness-1.1/Liveness/livecheck.py
--rw-rw-rw-   0        0        0      990 2020-08-05 05:53:18.000000 image-liveness-1.1/Liveness/utility copy.py
--rw-rw-rw-   0        0        0      990 2020-08-05 05:53:18.000000 image-liveness-1.1/Liveness/utility.py
--rw-rw-rw-   0        0        0        0 2023-04-13 04:03:07.000000 image-liveness-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2023-04-13 05:40:29.535982 image-liveness-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-13 04:03:12.000000 image-liveness-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 05:40:29.531983 image-liveness-1.1/image_liveness.egg-info/
--rw-rw-rw-   0        0        0      827 2023-04-13 05:40:28.000000 image-liveness-1.1/image_liveness.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-13 05:40:29.000000 image-liveness-1.1/image_liveness.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 05:40:28.000000 image-liveness-1.1/image_liveness.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 05:40:28.000000 image-liveness-1.1/image_liveness.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 05:40:28.000000 image-liveness-1.1/image_liveness.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-13 04:03:00.000000 image-liveness-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-13 05:40:29.543976 image-liveness-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-04-13 05:40:26.000000 image-liveness-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:58:17.423918 image-liveness-1.2/
+-rw-rw-rw-   0        0        0    11541 2023-04-13 04:10:36.000000 image-liveness-1.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 05:58:17.399920 image-liveness-1.2/Liveness/
+-rw-rw-rw-   0        0        0     3359 2023-04-12 12:10:50.000000 image-liveness-1.2/Liveness/anti_spoof_predict.py
+-rw-rw-rw-   0        0        0     1856 2023-04-12 10:44:07.000000 image-liveness-1.2/Liveness/generate_patches.py
+-rw-rw-rw-   0        0        0     4554 2023-04-13 05:19:55.000000 image-liveness-1.2/Liveness/livecheck.py
+-rw-rw-rw-   0        0        0      990 2020-08-05 05:53:18.000000 image-liveness-1.2/Liveness/utility copy.py
+-rw-rw-rw-   0        0        0      990 2020-08-05 05:53:18.000000 image-liveness-1.2/Liveness/utility.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 04:03:07.000000 image-liveness-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      827 2023-04-13 05:58:17.423918 image-liveness-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-13 04:03:12.000000 image-liveness-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 05:58:17.415919 image-liveness-1.2/image_liveness.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-04-13 05:58:16.000000 image-liveness-1.2/image_liveness.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-13 05:58:16.000000 image-liveness-1.2/image_liveness.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 05:58:16.000000 image-liveness-1.2/image_liveness.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 05:58:16.000000 image-liveness-1.2/image_liveness.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 05:58:16.000000 image-liveness-1.2/image_liveness.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-13 04:03:00.000000 image-liveness-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-13 05:58:17.423918 image-liveness-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-04-13 05:57:39.000000 image-liveness-1.2/setup.py
```

### Comparing `image-liveness-1.1/LICENSE.txt` & `image-liveness-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/Liveness/anti_spoof_predict.py` & `image-liveness-1.2/Liveness/anti_spoof_predict.py`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/Liveness/generate_patches.py` & `image-liveness-1.2/Liveness/generate_patches.py`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/Liveness/livecheck.py` & `image-liveness-1.2/Liveness/livecheck.py`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/Liveness/utility copy.py` & `image-liveness-1.2/Liveness/utility copy.py`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/Liveness/utility.py` & `image-liveness-1.2/Liveness/utility.py`

 * *Files identical despite different names*

### Comparing `image-liveness-1.1/PKG-INFO` & `image-liveness-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-liveness
-Version: 1.1
+Version: 1.2
 Summary: This library offers a liveness detection on static images, which can be used to distinguish if it is a live capture or a spoofed image based on facial features and other indicators of authenticity.
 Home-page: https://github.com/ashishf1soft
 Download-URL: https://github.com/ashishf1soft/liveness-detection/archive/refs/tags/v_01.tar.gz
 Author: Ashish Thapa
 Author-email: ashish.f1soft@gmail.com
 License: Apache License 2.0
 Keywords: LIVENESS,FACE FACE,DETECTION
```

### Comparing `image-liveness-1.1/image_liveness.egg-info/PKG-INFO` & `image-liveness-1.2/image_liveness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-liveness
-Version: 1.1
+Version: 1.2
 Summary: This library offers a liveness detection on static images, which can be used to distinguish if it is a live capture or a spoofed image based on facial features and other indicators of authenticity.
 Home-page: https://github.com/ashishf1soft
 Download-URL: https://github.com/ashishf1soft/liveness-detection/archive/refs/tags/v_01.tar.gz
 Author: Ashish Thapa
 Author-email: ashish.f1soft@gmail.com
 License: Apache License 2.0
 Keywords: LIVENESS,FACE FACE,DETECTION
```

### Comparing `image-liveness-1.1/setup.py` & `image-liveness-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'image-liveness',         
   packages = ['Liveness'],  
-  version = '1.1',      
+  version = '1.2',      
   license='Apache License 2.0',        
   description = 'This library offers a liveness detection on static images, which can be used to distinguish if it is a live capture or a spoofed image based on facial features and other indicators of authenticity.',  
   author = 'Ashish Thapa',                   
   author_email = 'ashish.f1soft@gmail.com',      
   url = 'https://github.com/ashishf1soft',  
   download_url = 'https://github.com/ashishf1soft/liveness-detection/archive/refs/tags/v_01.tar.gz',   
   keywords = ['LIVENESS','FACE FACE','DETECTION'],
```

