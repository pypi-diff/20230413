# Comparing `tmp/tdfextractor-0.1.4.tar.gz` & `tmp/tdfextractor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfextractor-0.1.4.tar", last modified: Thu Apr 13 16:27:30 2023, max compression
+gzip compressed data, was "tdfextractor-0.1.5.tar", last modified: Thu Apr 13 19:46:38 2023, max compression
```

## Comparing `tdfextractor-0.1.4.tar` & `tdfextractor-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.336149 tdfextractor-0.1.4/
--rw-rw-rw-   0        0        0      453 2023-04-13 16:27:30.335958 tdfextractor-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 16:27:30.336149 tdfextractor-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-04-13 16:25:55.000000 tdfextractor-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.322522 tdfextractor-0.1.4/tdfextractor/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.4/tdfextractor/__init__.py
--rw-rw-rw-   0        0        0       50 2022-09-29 06:07:39.000000 tdfextractor-0.1.4/tdfextractor/constants.py
--rw-rw-rw-   0        0        0     5365 2023-04-13 16:11:10.000000 tdfextractor-0.1.4/tdfextractor/ms2_extractor.py
--rw-rw-rw-   0        0        0     1498 2022-11-21 00:49:16.000000 tdfextractor-0.1.4/tdfextractor/string_templates.py
--rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.4/tdfextractor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.333536 tdfextractor-0.1.4/tdfextractor.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.334522 tdfextractor-0.1.4/test/
--rw-rw-rw-   0        0        0     2440 2023-04-12 23:55:45.000000 tdfextractor-0.1.4/test/test_ms2_extractor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.431476 tdfextractor-0.1.5/
+-rw-rw-rw-   0        0        0      453 2023-04-13 19:46:38.431476 tdfextractor-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:46:38.432477 tdfextractor-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-04-13 18:53:55.000000 tdfextractor-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.411356 tdfextractor-0.1.5/tdfextractor/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.5/tdfextractor/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.5/tdfextractor/constants.py
+-rw-rw-rw-   0        0        0     8936 2023-04-13 19:46:08.000000 tdfextractor-0.1.5/tdfextractor/ms2_extractor.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.5/tdfextractor/string_templates.py
+-rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.5/tdfextractor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.425010 tdfextractor-0.1.5/tdfextractor.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.430456 tdfextractor-0.1.5/test/
+-rw-rw-rw-   0        0        0     2440 2023-04-12 23:55:45.000000 tdfextractor-0.1.5/test/test_ms2_extractor.py
```

### Comparing `tdfextractor-0.1.4/setup.py` & `tdfextractor-0.1.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='tdfextractor',
-    version='0.1.4',
+    version='0.1.5',
     description='extract mass spec files from bruker d folder',
     url='https://github.com/pgarrett-scripps/tdfextractor.git',
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     license='MIT',
     packages=['tdfextractor'],
-    install_requires=['tdfpy==0.1.2', 'serenipy==0.2.6'],
+    install_requires=['tdfpy==0.1.2', 'serenipy==0.2.6', 'tqdm==4.64.1'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

### Comparing `tdfextractor-0.1.4/tdfextractor/string_templates.py` & `tdfextractor-0.1.5/tdfextractor/string_templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 header_ms2_template = 'H\tExtractor\tTimsTOF_extractor\n' \
                  'H\tExtractorVersion\t{version}\n' \
                  'H\tPublicationDate\t20-02-2020\n' \
                  'H\tDate Converted\t{date_of_creation}\n' \
                  'H\tComments\tTimsTOF_extractor written by Yu Gao, 2018\n' \
                  'H\tComments\tTimsTOF_extractor modified by Titus Jung, 2019\n' \
-                 'H\tComments\tTimsTOF_extractor modified by Patrick Garrett, 2023\n' \
+                 'H\tComments\tTimsTOF_extractor modified by Patrick Garrett, April 13th 2023\n' \
                  'H\tExtractorOptions\tMSn\n' \
                  'H\tAcquisitionMethod\tData-Dependent\n' \
                  'H\tInstrumentType\tTIMSTOF\n' \
                  'H\tDataType\tCentroid\n' \
                  'H\tScanType\tMS2\n' \
                  'H\tResolution\n' \
                  'H\tIsolationWindow\n' \
```

### Comparing `tdfextractor-0.1.4/tdfextractor/utils.py` & `tdfextractor-0.1.5/tdfextractor/utils.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.4/test/test_ms2_extractor.py` & `tdfextractor-0.1.5/test/test_ms2_extractor.py`

 * *Files identical despite different names*

