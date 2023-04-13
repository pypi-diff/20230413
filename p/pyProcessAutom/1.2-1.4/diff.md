# Comparing `tmp/pyProcessAutom-1.2.tar.gz` & `tmp/pyProcessAutom-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.2.tar", last modified: Thu Apr 13 04:05:31 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.tar", last modified: Thu Apr 13 04:17:21 2023, max compression
```

## Comparing `pyProcessAutom-1.2.tar` & `pyProcessAutom-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:05:31.590506 pyProcessAutom-1.2/
--rw-rw-rw-   0        0        0     1883 2023-04-13 04:05:31.589502 pyProcessAutom-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1658 2023-04-13 03:07:54.000000 pyProcessAutom-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:05:31.571501 pyProcessAutom-1.2/auto_preprocess/
--rw-rw-rw-   0        0        0        0 2023-04-13 03:01:11.000000 pyProcessAutom-1.2/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0       49 2023-04-13 03:02:13.000000 pyProcessAutom-1.2/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:05:31.588503 pyProcessAutom-1.2/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1883 2023-04-13 04:05:31.000000 pyProcessAutom-1.2/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-13 04:05:31.000000 pyProcessAutom-1.2/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:05:31.000000 pyProcessAutom-1.2/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 04:05:31.000000 pyProcessAutom-1.2/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 04:05:31.000000 pyProcessAutom-1.2/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 04:05:31.590506 pyProcessAutom-1.2/setup.cfg
--rw-rw-rw-   0        0        0      454 2023-04-13 04:04:59.000000 pyProcessAutom-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:17:21.905314 pyProcessAutom-1.4/
+-rw-rw-rw-   0        0        0     1883 2023-04-13 04:17:21.904314 pyProcessAutom-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1658 2023-04-13 03:07:54.000000 pyProcessAutom-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 04:17:21.883316 pyProcessAutom-1.4/auto_preprocess/
+-rw-rw-rw-   0        0        0       47 2023-04-13 04:09:05.000000 pyProcessAutom-1.4/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:17:21.902314 pyProcessAutom-1.4/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1883 2023-04-13 04:17:21.000000 pyProcessAutom-1.4/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-13 04:17:21.000000 pyProcessAutom-1.4/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 04:17:21.000000 pyProcessAutom-1.4/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-13 04:17:21.000000 pyProcessAutom-1.4/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 04:17:21.000000 pyProcessAutom-1.4/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 04:17:21.905314 pyProcessAutom-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      454 2023-04-13 04:17:16.000000 pyProcessAutom-1.4/setup.py
```

### Comparing `pyProcessAutom-1.2/PKG-INFO` & `pyProcessAutom-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.2
+Version: 1.4
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyProcessAutom-1.2/README.md` & `pyProcessAutom-1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyProcessAutom-1.2/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.2
+Version: 1.4
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

