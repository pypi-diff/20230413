# Comparing `tmp/teklia-line-image-extractor-0.2.8rc1.tar.gz` & `tmp/teklia-line-image-extractor-0.2.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teklia-line-image-extractor-0.2.8rc1.tar", last modified: Fri Mar  3 10:47:01 2023, max compression
+gzip compressed data, was "teklia-line-image-extractor-0.2.8rc2.tar", last modified: Thu Apr 13 09:27:19 2023, max compression
```

## Comparing `teklia-line-image-extractor-0.2.8rc1.tar` & `teklia-line-image-extractor-0.2.8rc2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 10:47:01.699632 teklia-line-image-extractor-0.2.8rc1/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2308 2023-03-03 10:47:01.699632 teklia-line-image-extractor-0.2.8rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1500 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-03 10:46:17.000000 teklia-line-image-extractor-0.2.8rc1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 10:47:01.699632 teklia-line-image-extractor-0.2.8rc1/line_image_extractor/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/line_image_extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/line_image_extractor/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     7197 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/line_image_extractor/image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/line_image_extractor/main.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-03-03 10:44:40.000000 teklia-line-image-extractor-0.2.8rc1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-03 10:47:01.699632 teklia-line-image-extractor-0.2.8rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1444 2023-03-03 10:43:39.000000 teklia-line-image-extractor-0.2.8rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 10:47:01.699632 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2308 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-03 10:47:01.000000 teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.351626 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7197 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/main.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1444 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/top_level.txt
```

### Comparing `teklia-line-image-extractor-0.2.8rc1/LICENSE` & `teklia-line-image-extractor-0.2.8rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/PKG-INFO` & `teklia-line-image-extractor-0.2.8rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.com/teklia/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `teklia-line-image-extractor-0.2.8rc1/README.md` & `teklia-line-image-extractor-0.2.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/line_image_extractor/extractor.py` & `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/line_image_extractor/image_utils.py` & `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/image_utils.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/line_image_extractor/main.py` & `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/main.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/setup.py` & `teklia-line-image-extractor-0.2.8rc2/setup.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc1/teklia_line_image_extractor.egg-info/PKG-INFO` & `teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.com/teklia/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

