# Comparing `tmp/limacharlie-4.4.1.tar.gz` & `tmp/limacharlie-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.4.1.tar", last modified: Wed Apr 12 23:51:02 2023, max compression
+gzip compressed data, was "limacharlie-4.4.2.tar", last modified: Thu Apr 13 18:15:45 2023, max compression
```

## Comparing `limacharlie-4.4.1.tar` & `limacharlie-4.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.299804 limacharlie-4.4.1/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.1/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 23:51:02.299804 limacharlie-4.4.1/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.1/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.296804 limacharlie-4.4.1/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     4570 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Extensions.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.1/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-02-09 00:21:23.000000 limacharlie-4.4.1/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.1/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.1/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.1/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.1/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.1/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.1/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.1/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.1/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.298804 limacharlie-4.4.1/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.1/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-12 23:51:02.299804 limacharlie-4.4.1/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-12 23:50:48.000000 limacharlie-4.4.1/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.299804 limacharlie-4.4.1/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.1/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.1/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-13 18:15:45.571983 limacharlie-4.4.2/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.2/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-13 18:15:45.571983 limacharlie-4.4.2/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.2/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-13 18:15:45.567983 limacharlie-4.4.2/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.2/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.2/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4562 2023-04-13 18:15:26.000000 limacharlie-4.4.2/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.2/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-02-09 00:21:23.000000 limacharlie-4.4.2/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.2/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.2/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-12 22:28:28.000000 limacharlie-4.4.2/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.2/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.2/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.2/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.2/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.2/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.2/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.2/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.2/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.2/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.2/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-13 18:15:26.000000 limacharlie-4.4.2/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.2/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.2/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-13 18:15:45.569983 limacharlie-4.4.2/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-13 18:15:45.000000 limacharlie-4.4.2/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.2/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-13 18:15:45.572983 limacharlie-4.4.2/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-13 18:15:26.000000 limacharlie-4.4.2/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-13 18:15:45.571983 limacharlie-4.4.2/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.2/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.2/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.2/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.2/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.2/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.2/tests/test_sync.py
```

### Comparing `limacharlie-4.4.1/LICENSE` & `limacharlie-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/README.md` & `limacharlie-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Configs.py` & `limacharlie-4.4.2/limacharlie/Configs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/DRCli.py` & `limacharlie-4.4.2/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Extensions.py` & `limacharlie-4.4.2/limacharlie/Extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,12 +126,12 @@
                          required = False,
                          action = 'store_true',
                          dest = 'impersonated',
                          help = 'whether to ask the extension to impersonate you.' )
 
     args = parser.parse_args( sourceArgs )
 
-    ext = Extension( Manager.Manager( None, None ) )
+    ext = Extension( Manager( None, None ) )
     actions[ args.action.lower() ]( args, ext )
 
 if '__main__' == __name__:
     main()
```

### Comparing `limacharlie-4.4.1/limacharlie/Firehose.py` & `limacharlie-4.4.2/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Hive.py` & `limacharlie-4.4.2/limacharlie/Hive.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Jobs.py` & `limacharlie-4.4.2/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Logs.py` & `limacharlie-4.4.2/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Manager.py` & `limacharlie-4.4.2/limacharlie/Manager.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Payloads.py` & `limacharlie-4.4.2/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Query.py` & `limacharlie-4.4.2/limacharlie/Query.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Replay.py` & `limacharlie-4.4.2/limacharlie/Replay.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Replicants.py` & `limacharlie-4.4.2/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Search.py` & `limacharlie-4.4.2/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Sensor.py` & `limacharlie-4.4.2/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/SpotCheck.py` & `limacharlie-4.4.2/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Spout.py` & `limacharlie-4.4.2/limacharlie/Spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Sync.py` & `limacharlie-4.4.2/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/Webhook.py` & `limacharlie-4.4.2/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/__init__.py` & `limacharlie-4.4.2/limacharlie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.4.1"
+__version__ = "4.4.2"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
```

### Comparing `limacharlie-4.4.1/limacharlie/__main__.py` & `limacharlie-4.4.2/limacharlie/__main__.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie/utils.py` & `limacharlie-4.4.2/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.2/limacharlie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/setup.py` & `limacharlie-4.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.4.1"
+__version__ = "4.4.2"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.4.1/tests/test_artifacts.py` & `limacharlie-4.4.2/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/tests/test_core.py` & `limacharlie-4.4.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/tests/test_insight.py` & `limacharlie-4.4.2/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/tests/test_spout.py` & `limacharlie-4.4.2/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.1/tests/test_sync.py` & `limacharlie-4.4.2/tests/test_sync.py`

 * *Files identical despite different names*

