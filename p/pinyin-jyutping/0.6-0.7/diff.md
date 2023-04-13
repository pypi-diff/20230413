# Comparing `tmp/pinyin_jyutping-0.6.tar.gz` & `tmp/pinyin_jyutping-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinyin_jyutping-0.6.tar", last modified: Thu Apr 13 03:39:11 2023, max compression
+gzip compressed data, was "pinyin_jyutping-0.7.tar", last modified: Thu Apr 13 03:41:48 2023, max compression
```

## Comparing `pinyin_jyutping-0.6.tar` & `pinyin_jyutping-0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:39:11.289983 pinyin_jyutping-0.6/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/MANIFEST.in
--rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:39:11.288983 pinyin_jyutping-0.6/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     2158 2023-04-13 03:37:57.000000 pinyin_jyutping-0.6/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:39:11.287983 pinyin_jyutping-0.6/pinyin_jyutping/
--rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-04-13 03:37:57.000000 pinyin_jyutping-0.6/pinyin_jyutping/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/cache.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7157 2023-04-13 03:37:57.000000 pinyin_jyutping-0.6/pinyin_jyutping/conversion.py
--rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/data.py
--rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/dict.txt.big
--rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-04-13 03:37:57.000000 pinyin_jyutping-0.6/pinyin_jyutping/logic.py
--rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/parser.py
--rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-04-13 03:39:09.000000 pinyin_jyutping-0.6/pinyin_jyutping/pinyin_jyutping.pkl
--rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-03-31 01:12:26.000000 pinyin_jyutping-0.6/pinyin_jyutping/syllables.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:39:11.288983 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:39:10.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-04-13 03:39:11.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/not-zip-safe
--rw-r--r--   0 luc       (1000) luc       (1000)        6 2023-04-13 03:39:11.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-04-13 03:39:11.000000 pinyin_jyutping-0.6/pinyin_jyutping.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 03:39:11.289983 pinyin_jyutping-0.6/setup.cfg
--rw-r--r--   0 luc       (1000) luc       (1000)      796 2023-04-13 03:38:31.000000 pinyin_jyutping-0.6/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.470336 pinyin_jyutping-0.7/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/MANIFEST.in
+-rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:41:48.469336 pinyin_jyutping-0.7/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     2158 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.468336 pinyin_jyutping-0.7/pinyin_jyutping/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/cache.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7157 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/conversion.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/data.py
+-rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/dict.txt.big
+-rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-04-13 03:37:57.000000 pinyin_jyutping-0.7/pinyin_jyutping/logic.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/parser.py
+-rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-04-13 03:41:46.000000 pinyin_jyutping-0.7/pinyin_jyutping/pinyin_jyutping.pkl
+-rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-03-31 01:12:26.000000 pinyin_jyutping-0.7/pinyin_jyutping/syllables.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:41:48.469336 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2515 2023-04-13 03:41:47.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:41:47.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/not-zip-safe
+-rw-r--r--   0 luc       (1000) luc       (1000)        6 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-04-13 03:41:48.000000 pinyin_jyutping-0.7/pinyin_jyutping.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 03:41:48.470336 pinyin_jyutping-0.7/setup.cfg
+-rw-r--r--   0 luc       (1000) luc       (1000)      796 2023-04-13 03:41:08.000000 pinyin_jyutping-0.7/setup.py
```

### Comparing `pinyin_jyutping-0.6/LICENSE` & `pinyin_jyutping-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/PKG-INFO` & `pinyin_jyutping-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin_jyutping
-Version: 0.6
+Version: 0.7
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pinyin_jyutping-0.6/README.rst` & `pinyin_jyutping-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/__init__.py` & `pinyin_jyutping-0.7/pinyin_jyutping/__init__.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/cache.py` & `pinyin_jyutping-0.7/pinyin_jyutping/cache.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/constants.py` & `pinyin_jyutping-0.7/pinyin_jyutping/constants.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/conversion.py` & `pinyin_jyutping-0.7/pinyin_jyutping/conversion.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/dict.txt.big` & `pinyin_jyutping-0.7/pinyin_jyutping/dict.txt.big`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/logic.py` & `pinyin_jyutping-0.7/pinyin_jyutping/logic.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/parser.py` & `pinyin_jyutping-0.7/pinyin_jyutping/parser.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/pinyin_jyutping.pkl` & `pinyin_jyutping-0.7/pinyin_jyutping/pinyin_jyutping.pkl`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping/syllables.py` & `pinyin_jyutping-0.7/pinyin_jyutping/syllables.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping.egg-info/PKG-INFO` & `pinyin_jyutping-0.7/pinyin_jyutping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin-jyutping
-Version: 0.6
+Version: 0.7
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pinyin_jyutping-0.6/pinyin_jyutping.egg-info/SOURCES.txt` & `pinyin_jyutping-0.7/pinyin_jyutping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.6/setup.py` & `pinyin_jyutping-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # build instructions
 #  python3 setup.py sdist
 # twine upload dist/*
 
 setup(name='pinyin_jyutping',
-      version='0.6',
+      version='0.7',
       description='Convert a Chinese sentence to Pinyin or Jyutping',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/pinyin-jyutping',
       author='LucW',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

