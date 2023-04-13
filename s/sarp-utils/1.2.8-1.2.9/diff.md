# Comparing `tmp/sarp_utils-1.2.8.tar.gz` & `tmp/sarp_utils-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sarp_utils-1.2.8.tar", last modified: Sun May  9 01:02:41 2021, max compression
+gzip compressed data, was "dist\sarp_utils-1.2.9.tar", last modified: Wed May 19 01:48:17 2021, max compression
```

## Comparing `sarp_utils-1.2.8.tar` & `sarp_utils-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2021-05-09 01:02:41.485799 sarp_utils-1.2.8/
--rw-rw-rw-   0        0        0     1076 2020-11-20 21:08:48.000000 sarp_utils-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     1299 2021-05-09 01:02:41.485494 sarp_utils-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      658 2021-04-27 20:56:08.000000 sarp_utils-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2021-05-09 01:02:41.477024 sarp_utils-1.2.8/sarp_utils/
--rw-rw-rw-   0        0        0        0 2020-12-01 21:14:58.000000 sarp_utils-1.2.8/sarp_utils/__init__.py
--rw-rw-rw-   0        0        0      765 2021-03-26 16:03:45.000000 sarp_utils-1.2.8/sarp_utils/bitfield_utils.py
--rw-rw-rw-   0        0        0      987 2021-02-19 01:14:25.000000 sarp_utils-1.2.8/sarp_utils/codec.py
--rw-rw-rw-   0        0        0      510 2021-05-05 00:44:26.000000 sarp_utils-1.2.8/sarp_utils/fill_command_codec.py
--rw-rw-rw-   0        0        0      854 2021-04-26 22:55:13.000000 sarp_utils-1.2.8/sarp_utils/fill_telem_codec.py
--rw-rw-rw-   0        0        0      814 2021-05-06 17:32:12.000000 sarp_utils-1.2.8/sarp_utils/flight_data_codec.py
--rw-rw-rw-   0        0        0     1864 2021-03-26 16:18:15.000000 sarp_utils-1.2.8/sarp_utils/network_node.py
--rw-rw-rw-   0        0        0      508 2021-05-05 00:44:44.000000 sarp_utils-1.2.8/sarp_utils/prop_command_codec.py
--rw-rw-rw-   0        0        0      860 2021-04-30 00:13:37.000000 sarp_utils-1.2.8/sarp_utils/prop_telem_codec.py
--rw-rw-rw-   0        0        0      477 2020-12-02 01:10:20.000000 sarp_utils-1.2.8/sarp_utils/template_codec.py
-drwxrwxrwx   0        0        0        0 2021-05-09 01:02:41.484478 sarp_utils-1.2.8/sarp_utils.egg-info/
--rw-rw-rw-   0        0        0     1299 2021-05-09 01:02:41.000000 sarp_utils-1.2.8/sarp_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2021-05-09 01:02:41.000000 sarp_utils-1.2.8/sarp_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-09 01:02:41.000000 sarp_utils-1.2.8/sarp_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-05-09 01:02:41.000000 sarp_utils-1.2.8/sarp_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-09 01:02:41.485799 sarp_utils-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      684 2021-05-09 01:01:58.000000 sarp_utils-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-19 01:48:17.371147 sarp_utils-1.2.9/
+-rw-rw-rw-   0        0        0     1076 2020-11-20 21:08:48.000000 sarp_utils-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     1299 2021-05-19 01:48:17.370164 sarp_utils-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2021-04-27 20:56:08.000000 sarp_utils-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2021-05-19 01:48:17.359426 sarp_utils-1.2.9/sarp_utils/
+-rw-rw-rw-   0        0        0        0 2020-12-01 21:14:58.000000 sarp_utils-1.2.9/sarp_utils/__init__.py
+-rw-rw-rw-   0        0        0      765 2021-03-26 16:03:45.000000 sarp_utils-1.2.9/sarp_utils/bitfield_utils.py
+-rw-rw-rw-   0        0        0      987 2021-02-19 01:14:25.000000 sarp_utils-1.2.9/sarp_utils/codec.py
+-rw-rw-rw-   0        0        0      510 2021-05-05 00:44:26.000000 sarp_utils-1.2.9/sarp_utils/fill_command_codec.py
+-rw-rw-rw-   0        0        0      854 2021-04-26 22:55:13.000000 sarp_utils-1.2.9/sarp_utils/fill_telem_codec.py
+-rw-rw-rw-   0        0        0      814 2021-05-06 17:32:12.000000 sarp_utils-1.2.9/sarp_utils/flight_data_codec.py
+-rw-rw-rw-   0        0        0     1864 2021-03-26 16:18:15.000000 sarp_utils-1.2.9/sarp_utils/network_node.py
+-rw-rw-rw-   0        0        0      531 2021-05-19 01:44:25.000000 sarp_utils-1.2.9/sarp_utils/prop_command_codec.py
+-rw-rw-rw-   0        0        0      883 2021-05-19 01:44:22.000000 sarp_utils-1.2.9/sarp_utils/prop_telem_codec.py
+-rw-rw-rw-   0        0        0      477 2020-12-02 01:10:20.000000 sarp_utils-1.2.9/sarp_utils/template_codec.py
+drwxrwxrwx   0        0        0        0 2021-05-19 01:48:17.368210 sarp_utils-1.2.9/sarp_utils.egg-info/
+-rw-rw-rw-   0        0        0     1299 2021-05-19 01:48:17.000000 sarp_utils-1.2.9/sarp_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2021-05-19 01:48:17.000000 sarp_utils-1.2.9/sarp_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-19 01:48:17.000000 sarp_utils-1.2.9/sarp_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2021-05-19 01:48:17.000000 sarp_utils-1.2.9/sarp_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-05-19 01:48:17.371147 sarp_utils-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      684 2021-05-19 01:47:09.000000 sarp_utils-1.2.9/setup.py
```

### Comparing `sarp_utils-1.2.8/LICENSE` & `sarp_utils-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/PKG-INFO` & `sarp_utils-1.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarp_utils
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package to encode network communication for SARP
 Home-page: https://gitlab.com/SARP_UW/codecs
 Author: Josh Sherbrooke
 Author-email: jsherbro@gmail.com
 License: UNKNOWN
 Description: ## __Codecs for SARP__
```

### Comparing `sarp_utils-1.2.8/README.md` & `sarp_utils-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/bitfield_utils.py` & `sarp_utils-1.2.9/sarp_utils/bitfield_utils.py`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/codec.py` & `sarp_utils-1.2.9/sarp_utils/codec.py`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/fill_telem_codec.py` & `sarp_utils-1.2.9/sarp_utils/fill_telem_codec.py`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/flight_data_codec.py` & `sarp_utils-1.2.9/sarp_utils/flight_data_codec.py`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/network_node.py` & `sarp_utils-1.2.9/sarp_utils/network_node.py`

 * *Files identical despite different names*

### Comparing `sarp_utils-1.2.8/sarp_utils/prop_telem_codec.py` & `sarp_utils-1.2.9/sarp_utils/prop_telem_codec.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     ("pc_adc1_c4", "f"),
     ("pc_adc2_c1", "f"),
     ("pc_adc2_c2", "f"),
     ("pc_adc2_c3", "f"),
     ("pc_adc2_c4", "f"),
     ("pc_hard_armed", "?"),
     ("pc_soft_armed", "?"),
+    ("pc_fire", "?"),
     ("pc_redlines_armed", "?"),
     ("pc_state", "h"),
     ("pc_scr_tag", "h")
 ])
 
 class PropTelemCodec(Codec):
     def __init__(self):
```

### Comparing `sarp_utils-1.2.8/sarp_utils.egg-info/PKG-INFO` & `sarp_utils-1.2.9/sarp_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarp-utils
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package to encode network communication for SARP
 Home-page: https://gitlab.com/SARP_UW/codecs
 Author: Josh Sherbrooke
 Author-email: jsherbro@gmail.com
 License: UNKNOWN
 Description: ## __Codecs for SARP__
```

### Comparing `sarp_utils-1.2.8/setup.py` & `sarp_utils-1.2.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sarp_utils",
-    version="1.2.8",
+    version="1.2.9",
     author="Josh Sherbrooke",
     author_email="jsherbro@gmail.com",
     description="A package to encode network communication for SARP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/SARP_UW/codecs",
     packages=setuptools.find_packages(),
```

