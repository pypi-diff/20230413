# Comparing `tmp/napari-sam-0.3.3.tar.gz` & `tmp/napari-sam-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.3.tar", last modified: Wed Apr 12 10:10:14 2023, max compression
+gzip compressed data, was "napari-sam-0.3.4.tar", last modified: Thu Apr 13 07:47:00 2023, max compression
```

## Comparing `napari-sam-0.3.3.tar` & `napari-sam-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.540764 napari-sam-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 10:09:51.000000 napari-sam-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 10:09:51.000000 napari-sam-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:10:14.540764 napari-sam-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 10:09:51.000000 napari-sam-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 10:09:51.000000 napari-sam-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 10:10:14.540764 napari-sam-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.536764 napari-sam-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.536764 napari-sam-0.3.3/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36427 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.540764 napari-sam-0.3.3/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 07:46:43.000000 napari-sam-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 07:46:43.000000 napari-sam-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 07:47:00.200459 napari-sam-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 07:46:43.000000 napari-sam-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 07:46:43.000000 napari-sam-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 07:47:00.204459 napari-sam-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.196459 napari-sam-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36427 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.3/LICENSE` & `napari-sam-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.3/PKG-INFO` & `napari-sam-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.3
+Version: 0.3.4
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.3 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.4 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.3/README.md` & `napari-sam-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.3/setup.cfg` & `napari-sam-0.3.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	napari
 	vispy
 	tqdm
+	napari-medical-image-formats
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari-sam-0.3.3/src/napari_sam/_widget.py` & `napari-sam-0.3.4/src/napari_sam/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.3/src/napari_sam/utils.py` & `napari-sam-0.3.4/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.3/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.4/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.3
+Version: 0.3.4
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.3 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.4 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

