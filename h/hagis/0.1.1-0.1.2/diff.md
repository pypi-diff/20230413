# Comparing `tmp/hagis-0.1.1.tar.gz` & `tmp/hagis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.1.1.tar", last modified: Thu Apr 13 11:47:55 2023, max compression
+gzip compressed data, was "hagis-0.1.2.tar", last modified: Thu Apr 13 14:31:36 2023, max compression
```

## Comparing `hagis-0.1.1.tar` & `hagis-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.259671 hagis-0.1.1/
--rw-rw-rw-   0        0        0      958 2023-04-13 11:47:55.245970 hagis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.1/README.md
--rw-rw-rw-   0        0        0      589 2023-04-13 11:44:46.000000 hagis-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 11:47:55.259671 hagis-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.178067 hagis-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.211055 hagis-0.1.1/src/hagis/
--rw-rw-rw-   0        0        0        0 2023-04-13 11:39:40.000000 hagis-0.1.1/src/hagis/__init__.py
--rw-rw-rw-   0        0        0     8706 2023-04-12 12:19:11.000000 hagis-0.1.1/src/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.245970 hagis-0.1.1/src/hagis.egg-info/
--rw-rw-rw-   0        0        0      958 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:36.230678 hagis-0.1.2/
+-rw-rw-rw-   0        0        0      958 2023-04-13 14:31:36.228783 hagis-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.2/README.md
+-rw-rw-rw-   0        0        0      589 2023-04-13 14:27:34.000000 hagis-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:31:36.230678 hagis-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:36.200899 hagis-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:36.209937 hagis-0.1.2/src/hagis/
+-rw-rw-rw-   0        0        0       21 2023-04-13 14:27:27.000000 hagis-0.1.2/src/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8706 2023-04-12 12:19:11.000000 hagis-0.1.2/src/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:36.226643 hagis-0.1.2/src/hagis.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-04-13 14:31:36.000000 hagis-0.1.2/src/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-13 14:31:36.000000 hagis-0.1.2/src/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:31:36.000000 hagis-0.1.2/src/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 14:31:36.000000 hagis-0.1.2/src/hagis.egg-info/top_level.txt
```

### Comparing `hagis-0.1.1/PKG-INFO` & `hagis-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.1.1/pyproject.toml` & `hagis-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hagis-0.1.1/src/hagis/hagis.py` & `hagis-0.1.2/src/hagis/hagis.py`

 * *Files identical despite different names*

### Comparing `hagis-0.1.1/src/hagis.egg-info/PKG-INFO` & `hagis-0.1.2/src/hagis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

