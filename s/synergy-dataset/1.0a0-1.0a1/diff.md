# Comparing `tmp/synergy-dataset-1.0a0.tar.gz` & `tmp/synergy-dataset-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synergy-dataset-1.0a0.tar", last modified: Wed Apr 12 08:25:45 2023, max compression
+gzip compressed data, was "synergy-dataset-1.0a1.tar", last modified: Thu Apr 13 10:51:16 2023, max compression
```

## Comparing `synergy-dataset-1.0a0.tar` & `synergy-dataset-1.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/synergy_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/synergy_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/synergy_dataset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/synergy_dataset/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/synergy_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 08:25:45.000000 synergy-dataset-1.0a0/synergy_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:25:45.732738 synergy-dataset-1.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 08:25:32.000000 synergy-dataset-1.0a0/tests/test_synergy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/synergy_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/synergy_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/synergy_dataset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/synergy_dataset/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/synergy_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 10:51:16.000000 synergy-dataset-1.0a1/synergy_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:51:16.675127 synergy-dataset-1.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:51:04.000000 synergy-dataset-1.0a1/tests/test_synergy.py
```

### Comparing `synergy-dataset-1.0a0/.github/workflows/python-package.yml` & `synergy-dataset-1.0a1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/.github/workflows/python-publish.yml` & `synergy-dataset-1.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/.gitignore` & `synergy-dataset-1.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/LICENSE` & `synergy-dataset-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/PKG-INFO` & `synergy-dataset-1.0a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a0
+Version: 1.0a1
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,16 +30,16 @@
 
 ```sh
 pip install synergy-dataset
 ```
 
 ## Getting started
 
-See [https://github.com/asreview/systematic-review-datasets](https://github.com/asreview/systematic-review-datasets) for documentation and getting started.
+See [https://github.com/asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) for documentation and getting started.
 
 ## License
 
 [MIT](/LICENSE)
 
 ## Contact
 
-See [https://github.com/asreview/systematic-review-datasets](https://github.com/asreview/systematic-review-datasets) for contact details.
+See [https://github.com/asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) for contact details.
```

### Comparing `synergy-dataset-1.0a0/pyproject.toml` & `synergy-dataset-1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/synergy_dataset/__main__.py` & `synergy-dataset-1.0a1/synergy_dataset/__main__.py`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a0/synergy_dataset/base.py` & `synergy-dataset-1.0a1/synergy_dataset/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,15 @@
     if not _dataset_available():
         download_raw_dataset()
 
     for dataset in sorted(
         glob.glob(str(Path(_get_path_raw_dataset(), "*", "metadata.json"))),
         key=lambda x: x.lower(),
     ):
-
-        yield Dataset(dataset.split("/")[-2])
+        yield Dataset(Path(dataset).parts[-2])
 
 
 class Dataset(object):
     """Dataset object belonging to a systematic review"""
 
     def __init__(self, name):
         super(Dataset, self).__init__()
```

### Comparing `synergy-dataset-1.0a0/synergy_dataset.egg-info/PKG-INFO` & `synergy-dataset-1.0a1/synergy_dataset.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a0
+Version: 1.0a1
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,16 +30,16 @@
 
 ```sh
 pip install synergy-dataset
 ```
 
 ## Getting started
 
-See [https://github.com/asreview/systematic-review-datasets](https://github.com/asreview/systematic-review-datasets) for documentation and getting started.
+See [https://github.com/asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) for documentation and getting started.
 
 ## License
 
 [MIT](/LICENSE)
 
 ## Contact
 
-See [https://github.com/asreview/systematic-review-datasets](https://github.com/asreview/systematic-review-datasets) for contact details.
+See [https://github.com/asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) for contact details.
```

### Comparing `synergy-dataset-1.0a0/synergy_dataset.egg-info/SOURCES.txt` & `synergy-dataset-1.0a1/synergy_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

