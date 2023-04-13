# Comparing `tmp/lantools-nsa-0.0.1.tar.gz` & `tmp/lantools-nsa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantools-nsa-0.0.1.tar", last modified: Thu Apr 13 11:03:16 2023, max compression
+gzip compressed data, was "lantools-nsa-0.0.2.tar", last modified: Thu Apr 13 11:10:02 2023, max compression
```

## Comparing `lantools-nsa-0.0.1.tar` & `lantools-nsa-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:03:16.197270 lantools-nsa-0.0.1/
--rw-rw-rw-   0        0        0     7813 2023-04-12 21:11:29.000000 lantools-nsa-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-04-12 21:11:29.000000 lantools-nsa-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      564 2023-04-13 11:03:16.195855 lantools-nsa-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-12 21:11:29.000000 lantools-nsa-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 11:03:16.197956 lantools-nsa-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-04-13 11:00:26.000000 lantools-nsa-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:03:16.181433 lantools-nsa-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:03:16.192578 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/
--rw-rw-rw-   0        0        0      564 2023-04-13 11:03:15.000000 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 11:03:15.000000 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:03:15.000000 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 11:03:15.000000 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 11:03:15.000000 lantools-nsa-0.0.1/src/lantools_nsa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-04-13 11:02:24.000000 lantools-nsa-0.0.1/src/parser.py
--rw-rw-rw-   0        0        0       73 2023-04-12 21:11:29.000000 lantools-nsa-0.0.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 11:10:02.064410 lantools-nsa-0.0.2/
+-rw-rw-rw-   0        0        0     7813 2023-04-12 21:11:29.000000 lantools-nsa-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-04-12 21:11:29.000000 lantools-nsa-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      564 2023-04-13 11:10:02.062895 lantools-nsa-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-12 21:11:29.000000 lantools-nsa-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:10:02.064410 lantools-nsa-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-04-13 11:09:56.000000 lantools-nsa-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:10:02.045880 lantools-nsa-0.0.2/src/
+-rw-rw-rw-   0        0        0      134 2023-04-13 11:02:24.000000 lantools-nsa-0.0.2/src/arabic_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:10:02.058519 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-04-13 11:10:01.000000 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-13 11:10:01.000000 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:10:01.000000 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 11:10:01.000000 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 11:10:01.000000 lantools-nsa-0.0.2/src/lantools_nsa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2023-04-12 21:11:29.000000 lantools-nsa-0.0.2/tox.ini
```

### Comparing `lantools-nsa-0.0.1/LICENSE.txt` & `lantools-nsa-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lantools-nsa-0.0.1/PKG-INFO` & `lantools-nsa-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantools-nsa
-Version: 0.0.1
+Version: 0.0.2
 Home-page: 
 Author: Alaa' Omar
 Author-email: 
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `lantools-nsa-0.0.1/setup.py` & `lantools-nsa-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="lantools-nsa",
-    version="0.0.1",
+    version="0.0.2",
     description="",
-    py_modules=["parser"],
+    py_modules=["arabic_parser"],
     package_dir={"": "src"},
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Alaa' Omar",
     author_email="",
```

### Comparing `lantools-nsa-0.0.1/src/lantools_nsa.egg-info/PKG-INFO` & `lantools-nsa-0.0.2/src/lantools_nsa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantools-nsa
-Version: 0.0.1
+Version: 0.0.2
 Home-page: 
 Author: Alaa' Omar
 Author-email: 
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

