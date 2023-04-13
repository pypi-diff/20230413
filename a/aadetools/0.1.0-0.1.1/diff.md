# Comparing `tmp/aadetools-0.1.0.tar.gz` & `tmp/aadetools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.1.0.tar", last modified: Thu Apr 13 11:19:55 2023, max compression
+gzip compressed data, was "aadetools-0.1.1.tar", last modified: Thu Apr 13 11:38:01 2023, max compression
```

## Comparing `aadetools-0.1.0.tar` & `aadetools-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.643181 aadetools-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-13 11:19:55.642941 aadetools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.616405 aadetools-0.1.0/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-13 11:19:55.000000 aadetools-0.1.0/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.1.0/instructions.txt
--rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.1.0/req.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:19:55.644278 aadetools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1651 2023-04-13 11:19:50.000000 aadetools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.619173 aadetools-0.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-04-12 19:35:56.000000 aadetools-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.634412 aadetools-0.1.0/src/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.1.0/src/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.1.0/src/morph/charsets.py
--rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.1.0/src/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.1.0/src/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.1.0/src/morph/settings.py
--rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.1.0/src/morph/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:19:55.638458 aadetools-0.1.0/src/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.1.0/src/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.1.0/src/parse/parser.py
--rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 11:38:01.965548 aadetools-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:38:01.965037 aadetools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 11:38:01.943049 aadetools-0.1.1/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:38:01.000000 aadetools-0.1.1/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-13 11:38:01.000000 aadetools-0.1.1/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:38:01.000000 aadetools-0.1.1/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 11:38:01.000000 aadetools-0.1.1/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:38:01.000000 aadetools-0.1.1/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.1.1/instructions.txt
+-rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.1.1/req.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:38:01.966593 aadetools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-04-13 11:37:58.000000 aadetools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:38:01.911401 aadetools-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:38:01.958835 aadetools-0.1.1/src/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.1.1/src/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.1.1/src/morph/charsets.py
+-rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.1.1/src/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.1.1/src/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.1.1/src/morph/settings.py
+-rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.1.1/src/morph/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:38:01.962077 aadetools-0.1.1/src/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.1.1/src/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.1.1/src/parse/parser.py
+-rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.1.1/tox.ini
```

### Comparing `aadetools-0.1.0/LICENSE.txt` & `aadetools-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/PKG-INFO` & `aadetools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.1.0/aadetools.egg-info/PKG-INFO` & `aadetools-0.1.1/aadetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.1.0/instructions.txt` & `aadetools-0.1.1/instructions.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/req.txt` & `aadetools-0.1.1/req.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/setup.py` & `aadetools-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,31 @@
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.1.0",                        # The initial release version
+    version="0.1.1",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    #packages=find_packages(include=['src','src.*']),    # List of all python modules to be installed
+    #packages=find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.9',                # Minimum version requirement of the package
-    packages=['src',
-              'src.morph',
-              'src.parse'
-             ],
+    packages=find_packages(),
     install_requires=requirements,         # Install other dependencies if any
     extras_require = {
         "dev": [
             "pytest >= 3.7",
             "check-manifest",
             "twine",
         ],
```

### Comparing `aadetools-0.1.0/src/morph/charsets.py` & `aadetools-0.1.1/src/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/src/morph/lemmatizeSentence.py` & `aadetools-0.1.1/src/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/src/morph/morph_tagger.py` & `aadetools-0.1.1/src/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/src/morph/tokenizers_words.py` & `aadetools-0.1.1/src/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.1.0/src/parse/parser.py` & `aadetools-0.1.1/src/parse/parser.py`

 * *Files identical despite different names*

