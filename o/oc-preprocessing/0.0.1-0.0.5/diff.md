# Comparing `tmp/oc_preprocessing-0.0.1.tar.gz` & `tmp/oc_preprocessing-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_preprocessing-0.0.1.tar", last modified: Wed Apr 12 08:37:35 2023, max compression
+gzip compressed data, was "oc_preprocessing-0.0.5.tar", last modified: Wed Apr 12 22:58:29 2023, max compression
```

## Comparing `oc_preprocessing-0.0.1.tar` & `oc_preprocessing-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,33 @@
-drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 08:37:35.052533 oc_preprocessing-0.0.1/
--rw-r--r--   0 ariannamorettj   (501) staff       (20)      761 2023-02-21 08:51:37.000000 oc_preprocessing-0.0.1/LICENSE
--rw-r--r--   0 ariannamorettj   (501) staff       (20)     2235 2023-04-12 08:37:35.052293 oc_preprocessing-0.0.1/PKG-INFO
--rw-r--r--   0 ariannamorettj   (501) staff       (20)     1513 2023-02-21 02:33:51.000000 oc_preprocessing-0.0.1/README.md
-drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 08:37:35.051892 oc_preprocessing-0.0.1/oc_preprocessing.egg-info/
--rw-r--r--   0 ariannamorettj   (501) staff       (20)     2235 2023-04-12 08:37:35.000000 oc_preprocessing-0.0.1/oc_preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 ariannamorettj   (501) staff       (20)      192 2023-04-12 08:37:35.000000 oc_preprocessing-0.0.1/oc_preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 ariannamorettj   (501) staff       (20)        1 2023-04-12 08:37:35.000000 oc_preprocessing-0.0.1/oc_preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 ariannamorettj   (501) staff       (20)       14 2023-04-12 08:37:35.000000 oc_preprocessing-0.0.1/oc_preprocessing.egg-info/top_level.txt
--rw-r--r--   0 ariannamorettj   (501) staff       (20)     1042 2023-04-12 08:35:03.000000 oc_preprocessing-0.0.1/pyproject.toml
--rw-r--r--   0 ariannamorettj   (501) staff       (20)       38 2023-04-12 08:37:35.052593 oc_preprocessing-0.0.1/setup.cfg
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.837400 oc_preprocessing-0.0.5/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)      761 2023-02-21 08:51:37.000000 oc_preprocessing-0.0.5/LICENSE
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)       38 2023-04-12 22:54:48.000000 oc_preprocessing-0.0.5/MANIFEST.in
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     2368 2023-04-12 22:58:29.837243 oc_preprocessing-0.0.5/PKG-INFO
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     1513 2023-02-21 02:33:51.000000 oc_preprocessing-0.0.5/README.md
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.833978 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     2368 2023-04-12 22:58:29.000000 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)      716 2023-04-12 22:58:29.000000 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)        1 2023-04-12 22:58:29.000000 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)      154 2023-04-12 22:58:29.000000 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/requires.txt
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)       14 2023-04-12 22:58:29.000000 oc_preprocessing-0.0.5/oc_preprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.835434 oc_preprocessing-0.0.5/preprocessing/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)        0 2023-01-08 18:42:19.000000 oc_preprocessing-0.0.5/preprocessing/__init__.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     7978 2023-04-12 22:08:22.000000 oc_preprocessing-0.0.5/preprocessing/base.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)    11221 2023-04-12 00:11:36.000000 oc_preprocessing-0.0.5/preprocessing/crossref.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)    20355 2023-04-11 20:24:07.000000 oc_preprocessing-0.0.5/preprocessing/datacite.py
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.836254 oc_preprocessing-0.0.5/preprocessing/datasource/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)        0 2023-03-05 23:47:48.000000 oc_preprocessing-0.0.5/preprocessing/datasource/__init__.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)      224 2023-03-06 18:24:58.000000 oc_preprocessing-0.0.5/preprocessing/datasource/config.ini
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     1290 2023-03-07 06:27:48.000000 oc_preprocessing-0.0.5/preprocessing/datasource/datasource.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     2558 2023-04-12 22:16:54.000000 oc_preprocessing-0.0.5/preprocessing/datasource/redis.py
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.836559 oc_preprocessing-0.0.5/preprocessing/finder/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)        0 2022-11-10 11:58:50.000000 oc_preprocessing-0.0.5/preprocessing/finder/__init__.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     4570 2023-04-04 13:52:22.000000 oc_preprocessing-0.0.5/preprocessing/finder/nih.py
+drwxr-xr-x   0 ariannamorettj   (501) staff       (20)        0 2023-04-12 22:58:29.836926 oc_preprocessing-0.0.5/preprocessing/identifier_manager/
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)        0 2023-04-07 11:14:14.000000 oc_preprocessing-0.0.5/preprocessing/identifier_manager/__init__.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     6874 2023-04-07 11:15:15.000000 oc_preprocessing-0.0.5/preprocessing/identifier_manager/jid.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)    10767 2023-04-12 06:43:50.000000 oc_preprocessing-0.0.5/preprocessing/jalc.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)    11026 2023-04-11 15:17:38.000000 oc_preprocessing-0.0.5/preprocessing/openaire.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)    14156 2023-04-12 06:42:10.000000 oc_preprocessing-0.0.5/preprocessing/pubmed.py
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     1038 2023-04-12 22:49:59.000000 oc_preprocessing-0.0.5/pyproject.toml
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)       38 2023-04-12 22:58:29.837439 oc_preprocessing-0.0.5/setup.cfg
+-rw-r--r--   0 ariannamorettj   (501) staff       (20)     1473 2023-04-12 22:48:30.000000 oc_preprocessing-0.0.5/setup.py
```

### Comparing `oc_preprocessing-0.0.1/LICENSE` & `oc_preprocessing-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oc_preprocessing-0.0.1/PKG-INFO` & `oc_preprocessing-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: oc_preprocessing
-Version: 0.0.1
+Version: 0.0.5
 Summary: This package is meant to preprocess OpenCitations source dumps so to make them easily usable in OpenCitations main processes, by deleting unused information, splitting big files, and validating identifiers
+Home-page: https://github.com/opencitations/preprocess
+Author: OpenCitations authors
 Author-email: OpenCitations authors <contact@opencitations.net>
+License: BSD
 Project-URL: Homepage, https://github.com/opencitations/preprocess
 Project-URL: Bug Tracker, https://github.com/opencitations/preprocess/issues
+Keywords: preprocessing data dumps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oc_preprocessing-0.0.1/README.md` & `oc_preprocessing-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oc_preprocessing-0.0.1/oc_preprocessing.egg-info/PKG-INFO` & `oc_preprocessing-0.0.5/oc_preprocessing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: oc-preprocessing
-Version: 0.0.1
+Version: 0.0.5
 Summary: This package is meant to preprocess OpenCitations source dumps so to make them easily usable in OpenCitations main processes, by deleting unused information, splitting big files, and validating identifiers
+Home-page: https://github.com/opencitations/preprocess
+Author: OpenCitations authors
 Author-email: OpenCitations authors <contact@opencitations.net>
+License: BSD
 Project-URL: Homepage, https://github.com/opencitations/preprocess
 Project-URL: Bug Tracker, https://github.com/opencitations/preprocess/issues
+Keywords: preprocessing data dumps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oc_preprocessing-0.0.1/pyproject.toml` & `oc_preprocessing-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,27 @@
     "oc_idmanager==0.2.6",
     "pandas==1.5.3",
     "requests==2.28.2",
     "tqdm==4.64.1",
     "zstandard==0.19.0"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools]
-py-modules = ["preprocessing"]
-
 [project]
 name = "oc_preprocessing"
-version = "0.0.1"
+version = "0.0.5"
 authors = [
       { name="OpenCitations authors", email="contact@opencitations.net" },
 ]
 description = "This package is meant to preprocess OpenCitations source dumps so to make them easily usable in OpenCitations main processes, by deleting unused information, splitting big files, and validating identifiers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: ISC License (ISCL)",
     "Operating System :: OS Independent",
 ]
-
 [project.urls]
 "Homepage" = "https://github.com/opencitations/preprocess"
-"Bug Tracker" = "https://github.com/opencitations/preprocess/issues"
+"Bug Tracker" = "https://github.com/opencitations/preprocess/issues"
+
+[tool.setuptools]
+include-package-data = true
```

