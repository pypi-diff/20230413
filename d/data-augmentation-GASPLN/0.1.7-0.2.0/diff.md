# Comparing `tmp/data_augmentation_GASPLN-0.1.7.tar.gz` & `tmp/data_augmentation_GASPLN-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_augmentation_GASPLN-0.1.7.tar", last modified: Mon Apr 10 14:56:57 2023, max compression
+gzip compressed data, was "data_augmentation_GASPLN-0.2.0.tar", last modified: Thu Apr 13 02:42:20 2023, max compression
```

## Comparing `data_augmentation_GASPLN-0.1.7.tar` & `data_augmentation_GASPLN-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.767888 data_augmentation_GASPLN-0.1.7/
--rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-04-10 14:56:57.768888 data_augmentation_GASPLN-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5226 2023-04-09 23:28:39.000000 data_augmentation_GASPLN-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.698629 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/
--rw-rw-rw-   0        0        0        0 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.753888 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/
--rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
--rw-rw-rw-   0        0        0     6150 2023-04-09 23:26:15.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.752890 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-10 14:56:57.769890 data_augmentation_GASPLN-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-10 14:56:51.000000 data_augmentation_GASPLN-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:42:20.195554 data_augmentation_GASPLN-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-04-13 02:42:20.195554 data_augmentation_GASPLN-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9506 2023-04-13 02:40:18.000000 data_augmentation_GASPLN-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:42:20.182858 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN/
+-rw-rw-rw-   0        0        0     9624 2023-04-13 02:10:00.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:42:20.189107 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN/data/
+-rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
+drwxrwxrwx   0        0        0        0 2023-04-13 02:42:20.187603 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-04-13 02:42:20.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-13 02:42:20.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:42:20.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-13 02:42:20.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-13 02:42:20.000000 data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 02:42:20.197555 data_augmentation_GASPLN-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-13 02:41:59.000000 data_augmentation_GASPLN-0.2.0/setup.py
```

### Comparing `data_augmentation_GASPLN-0.1.7/LICENSE` & `data_augmentation_GASPLN-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet` & `data_augmentation_GASPLN-0.2.0/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.7/setup.py` & `data_augmentation_GASPLN-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_augmentation_GASPLN',
-    version='0.1.7',
+    version='0.2.0',
     author='Artur Melchiori Cerri',
     author_email='arturmelchiori@gmail.com',
     description='Data augmentation for Portuguese language',
     install_requires=[
         "spacy",
         "nltk",
         "pandas",
```

