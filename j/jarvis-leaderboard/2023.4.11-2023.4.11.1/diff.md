# Comparing `tmp/jarvis_leaderboard-2023.4.11.tar.gz` & `tmp/jarvis_leaderboard-2023.4.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_leaderboard-2023.4.11.tar", last modified: Wed Apr 12 02:43:49 2023, max compression
+gzip compressed data, was "jarvis_leaderboard-2023.4.11.1.tar", last modified: Thu Apr 13 21:40:47 2023, max compression
```

## Comparing `jarvis_leaderboard-2023.4.11.tar` & `jarvis_leaderboard-2023.4.11.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:51.033417 jarvis_leaderboard-2023.4.11/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1064 2023-02-25 21:44:25.000000 jarvis_leaderboard-2023.4.11/LICENSE
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-12 02:43:51.031426 jarvis_leaderboard-2023.4.11/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     5978 2023-04-11 22:13:11.000000 jarvis_leaderboard-2023.4.11/README.md
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:50.972418 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       49 2023-04-12 02:21:11.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/__init__.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3297 2023-04-07 21:22:48.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_populate_data.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      112 2023-04-12 00:54:55.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_serve.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     2918 2023-04-12 02:08:02.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_upload.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)    29738 2023-04-12 02:35:25.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/rebuild.py
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:51.020424 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      410 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/SOURCES.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/dependency_links.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      142 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/requires.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       19 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/top_level.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-04-12 02:43:51.034428 jarvis_leaderboard-2023.4.11/setup.cfg
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1303 2023-04-12 02:21:03.000000 jarvis_leaderboard-2023.4.11/setup.py
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.747073 jarvis_leaderboard-2023.4.11.1/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1064 2023-02-25 21:44:25.000000 jarvis_leaderboard-2023.4.11.1/LICENSE
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6423 2023-04-13 21:40:46.745073 jarvis_leaderboard-2023.4.11.1/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     5978 2023-04-11 22:13:11.000000 jarvis_leaderboard-2023.4.11.1/README.md
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.687073 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       51 2023-04-13 18:41:59.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/__init__.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3297 2023-04-07 21:22:48.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_populate_data.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      135 2023-04-12 02:59:35.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_serve.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     2942 2023-04-12 03:01:25.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_upload.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)    29761 2023-04-12 03:00:01.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/rebuild.py
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.735074 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6423 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      410 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      142 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/requires.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       19 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/top_level.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-04-13 21:40:46.748074 jarvis_leaderboard-2023.4.11.1/setup.cfg
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1305 2023-04-13 18:41:46.000000 jarvis_leaderboard-2023.4.11.1/setup.py
```

### Comparing `jarvis_leaderboard-2023.4.11/LICENSE` & `jarvis_leaderboard-2023.4.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11/PKG-INFO` & `jarvis_leaderboard-2023.4.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_leaderboard
-Version: 2023.4.11
+Version: 2023.4.11.1
 Summary: jarvis_leaderboard
 Home-page: https://github.com/knc6/jarvis_leaderboard
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jarvis_leaderboard-2023.4.11/README.md` & `jarvis_leaderboard-2023.4.11.1/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_populate_data.py` & `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_populate_data.py`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_upload.py` & `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#! /usr/bin/env python
 import argparse
 import os
 import sys
 import requests
 
 parser = argparse.ArgumentParser(description="Add data to JARVIS-Leaderboard.")
 
@@ -60,15 +61,15 @@
         print(cmd)
         os.system(cmd)
     if os.path.exists(your_benchmark_directory):
         print("Note: adding to existing directory.")
     cmd = (
         "rsync -r "
         + your_benchmark_directory
-        + " jarvis_leaderboard/jarvis_leaderboard/benchmarks"
+        + " jarvis_leaderboard/jarvis_leaderboard/benchmarks/"
     )
     print(cmd)
     os.system(cmd)
     # cmd='cd '+upstream_repo_name
     os.chdir(upstream_repo_name)
     add_dir = "jarvis_leaderboard/benchmarks/" + your_benchmark_directory
     cmd = "ls ./" + add_dir
```

### Comparing `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/rebuild.py` & `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/rebuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#! /usr/bin/env python
 import os
 from jarvis.db.jsonutils import loadjson
 from sklearn.metrics import mean_absolute_error, accuracy_score
 import pandas as pd
 import glob
 import zipfile
 import json
```

### Comparing `jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/PKG-INFO` & `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-leaderboard
-Version: 2023.4.11
+Version: 2023.4.11.1
 Summary: jarvis_leaderboard
 Home-page: https://github.com/knc6/jarvis_leaderboard
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jarvis_leaderboard-2023.4.11/setup.py` & `jarvis_leaderboard-2023.4.11.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jarvis_leaderboard",  # Replace with your own username
-    version="2023.04.11",
+    version="2023.04.11.1",
     author="Kamal Choudhary",
     author_email="kamal.choudhary@nist.gov",
     description="jarvis_leaderboard",
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
```

