# Comparing `tmp/numba_aot_compiler-0.11.tar.gz` & `tmp/numba_aot_compiler-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_aot_compiler-0.11.tar", last modified: Thu Apr 13 02:44:06 2023, max compression
+gzip compressed data, was "numba_aot_compiler-0.12.tar", last modified: Thu Apr 13 02:45:32 2023, max compression
```

## Comparing `numba_aot_compiler-0.11.tar` & `numba_aot_compiler-0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:44:06.382285 numba_aot_compiler-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-13 02:44:03.000000 numba_aot_compiler-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      161 2023-04-13 02:44:02.000000 numba_aot_compiler-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     6928 2023-04-13 02:44:06.382285 numba_aot_compiler-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:44:06.378296 numba_aot_compiler-0.11/numba_aot_compiler/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 numba_aot_compiler-0.11/numba_aot_compiler/LICENSE
--rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.11/numba_aot_compiler/README.MD
--rw-rw-rw-   0        0        0     2926 2023-04-12 16:47:50.000000 numba_aot_compiler-0.11/numba_aot_compiler/__init__.py
--rw-rw-rw-   0        0        0       43 2023-04-13 02:44:05.000000 numba_aot_compiler-0.11/numba_aot_compiler/requirements.txt
--rw-rw-rw-   0        0        0     3886 2023-04-13 02:44:05.000000 numba_aot_compiler-0.11/numba_aot_compiler/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-13 02:44:06.381287 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/
--rw-rw-rw-   0        0        0     6928 2023-04-13 02:44:06.000000 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-13 02:44:06.000000 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:44:06.000000 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 02:44:06.000000 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-13 02:44:06.000000 numba_aot_compiler-0.11/numba_aot_compiler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-13 02:44:06.382285 numba_aot_compiler-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-04-13 02:44:05.000000 numba_aot_compiler-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:45:32.648932 numba_aot_compiler-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-13 02:45:27.000000 numba_aot_compiler-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      161 2023-04-13 02:45:27.000000 numba_aot_compiler-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     7004 2023-04-13 02:45:32.648932 numba_aot_compiler-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:45:32.642948 numba_aot_compiler-0.12/numba_aot_compiler/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 numba_aot_compiler-0.12/numba_aot_compiler/LICENSE
+-rw-rw-rw-   0        0        0     6032 2023-04-13 02:43:50.000000 numba_aot_compiler-0.12/numba_aot_compiler/README.MD
+-rw-rw-rw-   0        0        0     2926 2023-04-12 16:47:50.000000 numba_aot_compiler-0.12/numba_aot_compiler/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-04-13 02:45:31.000000 numba_aot_compiler-0.12/numba_aot_compiler/requirements.txt
+-rw-rw-rw-   0        0        0     3886 2023-04-13 02:45:31.000000 numba_aot_compiler-0.12/numba_aot_compiler/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-13 02:45:32.647935 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/
+-rw-rw-rw-   0        0        0     7004 2023-04-13 02:45:32.000000 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-13 02:45:32.000000 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:45:32.000000 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 02:45:32.000000 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-13 02:45:32.000000 numba_aot_compiler-0.12/numba_aot_compiler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-13 02:45:32.649929 numba_aot_compiler-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-04-13 02:45:31.000000 numba_aot_compiler-0.12/setup.py
```

### Comparing `numba_aot_compiler-0.11/LICENSE.rst` & `numba_aot_compiler-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/PKG-INFO` & `numba_aot_compiler-0.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: numba_aot_compiler
-Version: 0.11
+Version: 0.12
+Summary: A function to facilitate the Ahead-of-time compilation with Numba
 Home-page: https://github.com/hansalemaos/numba_aot_compiler
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numba,aot,compile
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `numba_aot_compiler-0.11/README.md` & `numba_aot_compiler-0.12/README.md`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/numba_aot_compiler/LICENSE` & `numba_aot_compiler-0.12/numba_aot_compiler/LICENSE`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/numba_aot_compiler/README.MD` & `numba_aot_compiler-0.12/numba_aot_compiler/README.MD`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/numba_aot_compiler/__init__.py` & `numba_aot_compiler-0.12/numba_aot_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/numba_aot_compiler/thirdparty.json` & `numba_aot_compiler-0.12/numba_aot_compiler/thirdparty.json`

 * *Files identical despite different names*

### Comparing `numba_aot_compiler-0.11/numba_aot_compiler.egg-info/PKG-INFO` & `numba_aot_compiler-0.12/numba_aot_compiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: numba-aot-compiler
-Version: 0.11
+Version: 0.12
+Summary: A function to facilitate the Ahead-of-time compilation with Numba
 Home-page: https://github.com/hansalemaos/numba_aot_compiler
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numba,aot,compile
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `numba_aot_compiler-0.11/setup.py` & `numba_aot_compiler-0.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.11'
+VERSION = '0.12'
 DESCRIPTION = "A function to facilitate the Ahead-of-time compilation with Numba"
 
 # Setting up
 setup(
     name="numba_aot_compiler",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/numba_aot_compiler',
     author="Johannes Fischer",
     author_email="<aulasparticularesdealemaosp@gmail.com>",
-    desc=DESCRIPTION,
+    description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     #packages=['deepcopyall', 'numba', 'ordered_set', 'touchtouch'],
     keywords=['numba', 'aot', 'compile'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['deepcopyall', 'numba', 'ordered_set', 'touchtouch'],
     include_package_data=True
```

