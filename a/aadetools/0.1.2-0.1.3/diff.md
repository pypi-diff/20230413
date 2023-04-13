# Comparing `tmp/aadetools-0.1.2.tar.gz` & `tmp/aadetools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.1.2.tar", last modified: Thu Apr 13 15:25:41 2023, max compression
+gzip compressed data, was "aadetools-0.1.3.tar", last modified: Thu Apr 13 15:28:40 2023, max compression
```

## Comparing `aadetools-0.1.2.tar` & `aadetools-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:25:41.797196 aadetools-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-13 15:25:41.796606 aadetools-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 15:25:41.793892 aadetools-0.1.2/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-13 15:25:41.000000 aadetools-0.1.2/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-13 15:25:41.000000 aadetools-0.1.2/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:25:41.000000 aadetools-0.1.2/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 15:25:41.000000 aadetools-0.1.2/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:25:41.000000 aadetools-0.1.2/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.1.2/instructions.txt
--rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.1.2/req.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 15:25:41.814417 aadetools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-04-13 15:25:37.000000 aadetools-0.1.2/setup.py
--rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.1.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 15:28:40.628208 aadetools-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-13 15:28:40.627083 aadetools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 15:28:40.625034 aadetools-0.1.3/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-13 15:28:40.000000 aadetools-0.1.3/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-13 15:28:40.000000 aadetools-0.1.3/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:28:40.000000 aadetools-0.1.3/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 15:28:40.000000 aadetools-0.1.3/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:28:40.000000 aadetools-0.1.3/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.1.3/instructions.txt
+-rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.1.3/req.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:28:40.628208 aadetools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-04-13 15:28:35.000000 aadetools-0.1.3/setup.py
+-rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.1.3/tox.ini
```

### Comparing `aadetools-0.1.2/LICENSE.txt` & `aadetools-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.2/PKG-INFO` & `aadetools-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.1.2/aadetools.egg-info/PKG-INFO` & `aadetools-0.1.3/aadetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.1.2/instructions.txt` & `aadetools-0.1.3/instructions.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.2/req.txt` & `aadetools-0.1.3/req.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.2/setup.py` & `aadetools-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.1.2",                        # The initial release version
+    version="0.1.3",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(where=['my_package','my_package.*']),    # List of all python modules to be installed
```

