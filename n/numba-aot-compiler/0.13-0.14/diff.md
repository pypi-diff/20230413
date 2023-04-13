# Comparing `tmp/numba_aot_compiler-0.13.tar.gz` & `tmp/numba_aot_compiler-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_aot_compiler-0.13.tar", last modified: Thu Apr 13 02:48:27 2023, max compression
+gzip compressed data, was "numba_aot_compiler-0.14.tar", last modified: Thu Apr 13 02:55:03 2023, max compression
```

## Comparing `numba_aot_compiler-0.13.tar` & `numba_aot_compiler-0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:48:27.978615 numba_aot_compiler-0.13/
--rw-rw-rw-   0        0        0     1148 2023-04-13 02:48:24.000000 numba_aot_compiler-0.13/LICENSE.rst
--rw-rw-rw-   0        0        0      161 2023-04-13 02:48:23.000000 numba_aot_compiler-0.13/MANIFEST.in
--rw-rw-rw-   0        0        0     7004 2023-04-13 02:48:27.978615 numba_aot_compiler-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:48:27.973627 numba_aot_compiler-0.13/numba_aot_compiler/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 numba_aot_compiler-0.13/numba_aot_compiler/LICENSE
--rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.13/numba_aot_compiler/README.MD
--rw-rw-rw-   0        0        0     2926 2023-04-12 16:47:50.000000 numba_aot_compiler-0.13/numba_aot_compiler/__init__.py
--rw-rw-rw-   0        0        0       43 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler/requirements.txt
--rw-rw-rw-   0        0        0     3886 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-13 02:48:27.977617 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/
--rw-rw-rw-   0        0        0     7004 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/numba_aot_compiler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 02:48:27.978615 numba_aot_compiler-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-04-13 02:48:27.000000 numba_aot_compiler-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:55:03.570634 numba_aot_compiler-0.14/
+-rw-rw-rw-   0        0        0     1148 2023-04-13 02:54:58.000000 numba_aot_compiler-0.14/LICENSE.rst
+-rw-rw-rw-   0        0        0      161 2023-04-13 02:54:58.000000 numba_aot_compiler-0.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     7004 2023-04-13 02:55:03.570634 numba_aot_compiler-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:55:03.566644 numba_aot_compiler-0.14/numba_aot_compiler/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 numba_aot_compiler-0.14/numba_aot_compiler/LICENSE
+-rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.14/numba_aot_compiler/README.md
+-rw-rw-rw-   0        0        0     2926 2023-04-12 16:47:50.000000 numba_aot_compiler-0.14/numba_aot_compiler/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-04-13 02:55:02.000000 numba_aot_compiler-0.14/numba_aot_compiler/requirements.txt
+-rw-rw-rw-   0        0        0     3886 2023-04-13 02:55:02.000000 numba_aot_compiler-0.14/numba_aot_compiler/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-13 02:55:03.569636 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/
+-rw-rw-rw-   0        0        0     7004 2023-04-13 02:55:03.000000 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-13 02:55:03.000000 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:55:03.000000 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 02:55:03.000000 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-13 02:55:03.000000 numba_aot_compiler-0.14/numba_aot_compiler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 02:55:03.571631 numba_aot_compiler-0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-04-13 02:55:02.000000 numba_aot_compiler-0.14/setup.py
```

### Comparing `numba_aot_compiler-0.13/LICENSE.rst` & `numba_aot_compiler-0.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/PKG-INFO` & `numba_aot_compiler-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba_aot_compiler
-Version: 0.13
+Version: 0.14
 Summary: A function to facilitate the Ahead-of-time compilation with Numba
 Home-page: https://github.com/hansalemaos/numba_aot_compiler
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numba,aot,compile
 Classifier: Development Status :: 4 - Beta
```

### Comparing `numba_aot_compiler-0.13/README.md` & `numba_aot_compiler-0.14/README.md`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/numba_aot_compiler/LICENSE` & `numba_aot_compiler-0.14/numba_aot_compiler/LICENSE`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/numba_aot_compiler/README.MD` & `numba_aot_compiler-0.14/numba_aot_compiler/README.md`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/numba_aot_compiler/__init__.py` & `numba_aot_compiler-0.14/numba_aot_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/numba_aot_compiler/thirdparty.json` & `numba_aot_compiler-0.14/numba_aot_compiler/thirdparty.json`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.13/numba_aot_compiler.egg-info/PKG-INFO` & `numba_aot_compiler-0.14/numba_aot_compiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-aot-compiler
-Version: 0.13
+Version: 0.14
 Summary: A function to facilitate the Ahead-of-time compilation with Numba
 Home-page: https://github.com/hansalemaos/numba_aot_compiler
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numba,aot,compile
 Classifier: Development Status :: 4 - Beta
```

### Comparing `numba_aot_compiler-0.13/setup.py` & `numba_aot_compiler-0.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.13'
+VERSION = '0.14'
 DESCRIPTION = "A function to facilitate the Ahead-of-time compilation with Numba"
 
 # Setting up
 setup(
     name="numba_aot_compiler",
     version=VERSION,
     license='MIT',
```

