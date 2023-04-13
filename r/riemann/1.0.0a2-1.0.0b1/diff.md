# Comparing `tmp/riemann-1.0.0a2.tar.gz` & `tmp/riemann-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riemann-1.0.0a2.tar", last modified: Thu Apr 13 03:27:00 2023, max compression
+gzip compressed data, was "riemann-1.0.0b1.tar", last modified: Thu Apr 13 15:15:24 2023, max compression
```

## Comparing `riemann-1.0.0a2.tar` & `riemann-1.0.0b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:27:00.351694 riemann-1.0.0a2/
--rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-1.0.0a2/LICENSE
--rw-rw-rw-   0        0        0     3494 2023-04-13 03:27:00.351694 riemann-1.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     2506 2023-04-13 03:23:56.000000 riemann-1.0.0a2/README.md
--rw-rw-rw-   0        0        0     1078 2023-04-13 03:25:27.000000 riemann-1.0.0a2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-13 03:27:00.351694 riemann-1.0.0a2/riemann.egg-info/
--rw-rw-rw-   0        0        0     3494 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8190 2023-04-13 01:14:25.000000 riemann-1.0.0a2/riemann.py
--rw-rw-rw-   0        0        0       42 2023-04-13 03:27:00.351694 riemann-1.0.0a2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 15:15:24.778990 riemann-1.0.0b1/
+-rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-1.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0     3494 2023-04-13 15:15:24.778990 riemann-1.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2506 2023-04-13 03:30:51.000000 riemann-1.0.0b1/README.md
+-rw-rw-rw-   0        0        0     1078 2023-04-13 15:13:49.000000 riemann-1.0.0b1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-13 15:15:24.774989 riemann-1.0.0b1/riemann.egg-info/
+-rw-rw-rw-   0        0        0     3494 2023-04-13 15:15:24.000000 riemann-1.0.0b1/riemann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-04-13 15:15:24.000000 riemann-1.0.0b1/riemann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:15:24.000000 riemann-1.0.0b1/riemann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 15:15:24.000000 riemann-1.0.0b1/riemann.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8190 2023-04-13 03:30:51.000000 riemann-1.0.0b1/riemann.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:15:24.783005 riemann-1.0.0b1/setup.cfg
```

### Comparing `riemann-1.0.0a2/LICENSE` & `riemann-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `riemann-1.0.0a2/PKG-INFO` & `riemann-1.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riemann
-Version: 1.0.0a2
+Version: 1.0.0b1
 Summary: A package for computing Riemann summations in n-dimensional space
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 Project-URL: Homepage, https://github.com/JacobLee23/riemann
 Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `riemann-1.0.0a2/README.md` & `riemann-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `riemann-1.0.0a2/pyproject.toml` & `riemann-1.0.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel >= 0.29.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "riemann"
-version = "1.0.0-a.2"
+version = "1.0.0-b.1"
 authors = [
   { name="Jacob Lee", email="Jacob.J.Lee@outlook.com" },
 ]
 description = "A package for computing Riemann summations in n-dimensional space"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `riemann-1.0.0a2/riemann.egg-info/PKG-INFO` & `riemann-1.0.0b1/riemann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riemann
-Version: 1.0.0a2
+Version: 1.0.0b1
 Summary: A package for computing Riemann summations in n-dimensional space
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 Project-URL: Homepage, https://github.com/JacobLee23/riemann
 Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `riemann-1.0.0a2/riemann.py` & `riemann-1.0.0b1/riemann.py`

 * *Files identical despite different names*

