# Comparing `tmp/optim3d-0.2.6.tar.gz` & `tmp/optim3d-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optim3d-0.2.6.tar", last modified: Thu Apr 13 12:11:06 2023, max compression
+gzip compressed data, was "dist\optim3d-0.2.7.tar", last modified: Thu Apr 13 13:11:03 2023, max compression
```

## Comparing `optim3d-0.2.6.tar` & `optim3d-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:06.000000 optim3d-0.2.6/
--rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.6/COPYING
--rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d/config/
--rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.2.6/optim3d/config/reconstruct.json
--rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.2.6/optim3d/config/reconstruct_.json
--rw-rw-rw-   0        0        0    21672 2023-04-12 14:06:45.000000 optim3d-0.2.6/optim3d/main.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.2.6/optim3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    14824 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0      323 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 12:11:06.000000 optim3d-0.2.6/optim3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14824 2023-04-13 12:11:06.000000 optim3d-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 12:11:06.000000 optim3d-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-04-13 12:11:02.000000 optim3d-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:11:03.000000 optim3d-0.2.7/
+-rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.7/COPYING
+-rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-13 13:09:55.000000 optim3d-0.2.7/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d/config/
+-rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.2.7/optim3d/config/reconstruct.json
+-rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.2.7/optim3d/config/reconstruct_.json
+-rw-rw-rw-   0        0        0    21672 2023-04-12 14:06:45.000000 optim3d-0.2.7/optim3d/main.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.2.7/optim3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    14824 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      335 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 13:11:03.000000 optim3d-0.2.7/optim3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14824 2023-04-13 13:11:03.000000 optim3d-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:11:03.000000 optim3d-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-04-13 13:10:16.000000 optim3d-0.2.7/setup.py
```

### Comparing `optim3d-0.2.6/COPYING` & `optim3d-0.2.7/COPYING`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/LICENSE` & `optim3d-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/optim3d/config/reconstruct.json` & `optim3d-0.2.7/optim3d/config/reconstruct.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/optim3d/config/reconstruct_.json` & `optim3d-0.2.7/optim3d/config/reconstruct_.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/optim3d/main.py` & `optim3d-0.2.7/optim3d/main.py`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/optim3d.egg-info/PKG-INFO` & `optim3d-0.2.7/optim3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.6
+Version: 0.2.7
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `optim3d-0.2.6/PKG-INFO` & `optim3d-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.6
+Version: 0.2.7
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `optim3d-0.2.6/README.md` & `optim3d-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.6/setup.py` & `optim3d-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="optim3d",
-    version='0.2.6',
+    version='0.2.7',
     description="CLI application for efficient and optimized reconstruction of large-scale 3D building models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause BSD 3-Clause "New" or "Revised" License',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/Optim3D',
```

