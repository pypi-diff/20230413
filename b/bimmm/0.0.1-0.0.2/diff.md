# Comparing `tmp/bimmm-0.0.1.tar.gz` & `tmp/bimmm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bimmm-0.0.1.tar", last modified: Thu Apr 13 09:13:23 2023, max compression
+gzip compressed data, was "dist/bimmm-0.0.2.tar", last modified: Thu Apr 13 09:19:57 2023, max compression
```

## Comparing `bimmm-0.0.1.tar` & `bimmm-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:13:23.366135 bimmm-0.0.1/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:13:23.365996 bimmm-0.0.1/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     2315 2023-04-13 09:12:10.000000 bimmm-0.0.1/README.md
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:13:23.365198 bimmm-0.0.1/bimmm/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 bimmm-0.0.1/bimmm/__init__.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 bimmm-0.0.1/bimmm/analyse_mmm_models.py
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:13:23.365804 bimmm-0.0.1/bimmm.egg-info/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:13:23.000000 bimmm-0.0.1/bimmm.egg-info/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)      208 2023-04-13 09:13:23.000000 bimmm-0.0.1/bimmm.egg-info/SOURCES.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-04-13 09:13:23.000000 bimmm-0.0.1/bimmm.egg-info/dependency_links.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       62 2023-04-13 09:13:23.000000 bimmm-0.0.1/bimmm.egg-info/requires.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        6 2023-04-13 09:13:23.000000 bimmm-0.0.1/bimmm.egg-info/top_level.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-04-13 09:13:23.366175 bimmm-0.0.1/setup.cfg
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     1499 2023-04-13 09:12:10.000000 bimmm-0.0.1/setup.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.787352 bimmm-0.0.2/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:19:57.787213 bimmm-0.0.2/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     2315 2023-04-13 09:16:57.000000 bimmm-0.0.2/README.md
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.786408 bimmm-0.0.2/bimmm/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 bimmm-0.0.2/bimmm/__init__.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 bimmm-0.0.2/bimmm/analyse_mmm_models.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.787020 bimmm-0.0.2/bimmm.egg-info/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)      208 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/SOURCES.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/dependency_links.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       52 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/requires.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        6 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/top_level.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-04-13 09:19:57.787394 bimmm-0.0.2/setup.cfg
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     1486 2023-04-13 09:19:29.000000 bimmm-0.0.2/setup.py
```

### Comparing `bimmm-0.0.1/PKG-INFO` & `bimmm-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bimmm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that makes it a bit easier to visualize and analyse Marketing Mix Models
 Home-page: UNKNOWN
 Author: Simon Teggelaar
 Author-email: simonteggelaar@gmail.com
 License: MIT
-Description: # `bixai`
+Description: # `bimmm`
         
         The `bimmm` is a package to analyse MMM models and visualize them
         
         ## Installation
         
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
```

### Comparing `bimmm-0.0.1/README.md` & `bimmm-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `bixai`
+# `bimmm`
 
 The `bimmm` is a package to analyse MMM models and visualize them
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
```

### Comparing `bimmm-0.0.1/bimmm/analyse_mmm_models.py` & `bimmm-0.0.2/bimmm/analyse_mmm_models.py`

 * *Files identical despite different names*

### Comparing `bimmm-0.0.1/bimmm.egg-info/PKG-INFO` & `bimmm-0.0.2/bimmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bimmm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that makes it a bit easier to visualize and analyse Marketing Mix Models
 Home-page: UNKNOWN
 Author: Simon Teggelaar
 Author-email: simonteggelaar@gmail.com
 License: MIT
-Description: # `bixai`
+Description: # `bimmm`
         
         The `bimmm` is a package to analyse MMM models and visualize them
         
         ## Installation
         
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
```

### Comparing `bimmm-0.0.1/setup.py` & `bimmm-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="bimmm",
 
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
 
     # Name of Author
     author="Simon Teggelaar",
 
     # your Email address
     author_email="simonteggelaar@gmail.com",
 
@@ -31,15 +31,15 @@
     # url="https://github.com/username/",
     packages=setuptools.find_packages(),
 
     # if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-         "pandas", "numpy", "itertools", "scipy", "plotly", "statsmodels", "tqdm", "requests"
+         "pandas", "numpy", "scipy", "plotly", "statsmodels", "tqdm", "requests"
        ],
 
     license="MIT",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
         "Programming Language :: Python :: 3",
```

