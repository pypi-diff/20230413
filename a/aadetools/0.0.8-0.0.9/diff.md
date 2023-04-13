# Comparing `tmp/aadetools-0.0.8.tar.gz` & `tmp/aadetools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.0.8.tar", last modified: Wed Apr 12 21:07:42 2023, max compression
+gzip compressed data, was "aadetools-0.0.9.tar", last modified: Thu Apr 13 11:14:27 2023, max compression
```

## Comparing `aadetools-0.0.8.tar` & `aadetools-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:07:42.970946 aadetools-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-12 21:07:42.969967 aadetools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:07:42.947726 aadetools-0.0.8/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-12 21:07:42.000000 aadetools-0.0.8/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-04-12 21:07:42.000000 aadetools-0.0.8/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:07:42.000000 aadetools-0.0.8/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-12 21:07:42.000000 aadetools-0.0.8/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 21:07:42.000000 aadetools-0.0.8/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      674 2023-04-10 21:58:24.000000 aadetools-0.0.8/instructions.txt
--rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.0.8/req.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 21:07:42.971967 aadetools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1728 2023-04-12 21:07:16.000000 aadetools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:07:42.950285 aadetools-0.0.8/src/
--rw-rw-rw-   0        0        0        0 2023-04-12 19:35:56.000000 aadetools-0.0.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:07:42.964425 aadetools-0.0.8/src/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.0.8/src/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.0.8/src/morph/charsets.py
--rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.0.8/src/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.0.8/src/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.0.8/src/morph/settings.py
--rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.0.8/src/morph/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:07:42.967950 aadetools-0.0.8/src/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.0.8/src/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.0.8/src/parse/parser.py
--rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.0.8/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.191533 aadetools-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:14:27.191085 aadetools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.9/README.md
+-rw-rw-rw-   0        0        0      739 2023-04-12 21:20:08.000000 aadetools-0.0.9/instructions.txt
+-rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.0.9/req.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:14:27.193078 aadetools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2023-04-13 11:14:14.000000 aadetools-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.145192 aadetools-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:14:27.188226 aadetools-0.0.9/src/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 11:14:27.000000 aadetools-0.0.9/src/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.0.9/tox.ini
```

### Comparing `aadetools-0.0.8/LICENSE.txt` & `aadetools-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.8/PKG-INFO` & `aadetools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.8/aadetools.egg-info/PKG-INFO` & `aadetools-0.0.9/src/aadetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.8/instructions.txt` & `aadetools-0.0.9/instructions.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 
 python setup.py sdist bdist_wheel
+ls dist/
 py -m setup.py sdist bdist_wheel
 py -m pip install torchtext==0.14.0
 py -m pip install -e .
 from demo_sna.morph import morph_tagger
 morph_tagger.tagger("ذهب الولد الى المدرسة")
 from sina_tools import aned
 aned.ANED("بايثون",{"Qَ25":"بغة برمجية كائنية التوجه","Q55":"أفعى بايثون تعيش في الامازو"})
 
 
 aned.disambiguate("بايثون",{"Qَ25":"بغة برمجية كائنية التوجه","Q55":"أفعى بايثون تعيش في الامازو"})
 disambiguate
 
 
+tar tzf dist/.....tar.gz (test all files are there)
+
 upload to pypi instructions
 
 py -m setup sdist
 twine upload dist/*
 2bFGM6UWJP7ekeh
```

### Comparing `aadetools-0.0.8/req.txt` & `aadetools-0.0.9/req.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.8/setup.py` & `aadetools-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.0.8",                        # The initial release version
+    version="0.0.9",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     #packages=find_packages(include=['src','src.*']),    # List of all python modules to be installed
@@ -25,19 +25,16 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.9',                # Minimum version requirement of the package
-    py_modules=["aadetools"],             # Name of the python package
-    packages=['src',
-              'src.morph',
-              'src.parse',
-             ],    
+    py_modules=["morph, parse"],             # Name of the python package
+    package_dir={"": "src"},
     install_requires=requirements,         # Install other dependencies if any
     extras_require = {
         "dev": [
             "pytest >= 3.7",
             "check-manifest",
             "twine",
         ],
```

