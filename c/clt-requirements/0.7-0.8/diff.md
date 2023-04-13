# Comparing `tmp/clt_requirements-0.7.tar.gz` & `tmp/clt_requirements-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clt_requirements-0.7.tar", last modified: Mon Apr  3 23:48:12 2023, max compression
+gzip compressed data, was "clt_requirements-0.8.tar", last modified: Thu Apr 13 03:51:26 2023, max compression
```

## Comparing `clt_requirements-0.7.tar` & `clt_requirements-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-03 23:48:12.698162 clt_requirements-0.7/
--rw-r--r--   0 luc       (1000) luc       (1000)      416 2023-04-03 23:48:12.698162 clt_requirements-0.7/PKG-INFO
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-03 23:48:12.697162 clt_requirements-0.7/clt_requirements/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-03-28 05:23:58.000000 clt_requirements-0.7/clt_requirements/__init__.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-03 23:48:12.698162 clt_requirements-0.7/clt_requirements.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      416 2023-04-03 23:48:12.000000 clt_requirements-0.7/clt_requirements.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      236 2023-04-03 23:48:12.000000 clt_requirements-0.7/clt_requirements.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-03 23:48:12.000000 clt_requirements-0.7/clt_requirements.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)      194 2023-04-03 23:48:12.000000 clt_requirements-0.7/clt_requirements.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       17 2023-04-03 23:48:12.000000 clt_requirements-0.7/clt_requirements.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-03 23:48:12.698162 clt_requirements-0.7/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)     1038 2023-04-03 23:47:12.000000 clt_requirements-0.7/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:51:26.951636 clt_requirements-0.8/
+-rw-r--r--   0 luc       (1000) luc       (1000)      416 2023-04-13 03:51:26.950636 clt_requirements-0.8/PKG-INFO
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:51:26.949636 clt_requirements-0.8/clt_requirements/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-03-28 05:23:58.000000 clt_requirements-0.8/clt_requirements/__init__.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-13 03:51:26.950636 clt_requirements-0.8/clt_requirements.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      416 2023-04-13 03:51:26.000000 clt_requirements-0.8/clt_requirements.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      236 2023-04-13 03:51:26.000000 clt_requirements-0.8/clt_requirements.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:51:26.000000 clt_requirements-0.8/clt_requirements.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)      194 2023-04-13 03:51:26.000000 clt_requirements-0.8/clt_requirements.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       17 2023-04-13 03:51:26.000000 clt_requirements-0.8/clt_requirements.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-13 03:51:26.951636 clt_requirements-0.8/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)     1038 2023-04-13 03:50:43.000000 clt_requirements-0.8/setup.py
```

### Comparing `clt_requirements-0.7/setup.py` & `clt_requirements-0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='clt_requirements',
-      version='0.7',
+      version='0.8',
       description='Helper module for Cloud Language Tools, additional dependencies',
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
@@ -22,13 +22,13 @@
           'requests',
           'google-cloud-texttospeech',
           'google-cloud-translate',
           'boto3',
           'epitran==1.22',
           'pythainlp[thai2rom,ipa]',
           'jieba',
-          'pinyin_jyutping>=0.5',
+          'pinyin_jyutping>=0.7',
           'cryptography',
           'pydub',
           'openai'
       ],
       )
```

