# Comparing `tmp/aadetools-0.0.9.tar.gz` & `tmp/aadetools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.0.9.tar", last modified: Thu Apr 13 11:14:27 2023, max compression
+gzip compressed data, was "aadetools-0.1.0.tar", last modified: Thu Apr 13 11:19:55 2023, max compression
```

## Comparing `aadetools-0.0.9.tar` & `aadetools-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.191533 aadetools-0.0.9/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-13 11:14:27.191085 aadetools-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.9/README.md
--rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.0.9/instructions.txt
--rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.0.9/req.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:14:27.193078 aadetools-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1662 2023-04-13 11:14:14.000000 aadetools-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.145192 aadetools-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.188226 aadetools-0.0.9/src/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.0.9/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.643181 aadetools-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:19:55.642941 aadetools-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.616405 aadetools-0.1.0/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.1.0/instructions.txt
+-rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.1.0/req.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:19:55.644278 aadetools-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1651 2023-04-13 11:19:50.000000 aadetools-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.619173 aadetools-0.1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-04-12 19:35:56.000000 aadetools-0.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.634412 aadetools-0.1.0/src/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.1.0/src/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.1.0/src/morph/charsets.py
+-rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.1.0/src/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.1.0/src/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.1.0/src/morph/settings.py
+-rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.1.0/src/morph/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.638458 aadetools-0.1.0/src/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.1.0/src/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.1.0/src/parse/parser.py
+-rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.1.0/tox.ini
```

### Comparing `aadetools-0.0.9/LICENSE.txt` & `aadetools-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.9/PKG-INFO` & `aadetools-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.9
+Version: 0.1.0
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.9/instructions.txt` & `aadetools-0.1.0/instructions.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.9/req.txt` & `aadetools-0.1.0/req.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.9/setup.py` & `aadetools-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.0.9",                        # The initial release version
+    version="0.1.0",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     #packages=find_packages(include=['src','src.*']),    # List of all python modules to be installed
@@ -25,16 +25,18 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.9',                # Minimum version requirement of the package
-    py_modules=["morph, parse"],             # Name of the python package
-    package_dir={"": "src"},
+    packages=['src',
+              'src.morph',
+              'src.parse'
+             ],
     install_requires=requirements,         # Install other dependencies if any
     extras_require = {
         "dev": [
             "pytest >= 3.7",
             "check-manifest",
             "twine",
         ],
```

### Comparing `aadetools-0.0.9/src/aadetools.egg-info/PKG-INFO` & `aadetools-0.1.0/aadetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.9
+Version: 0.1.0
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

