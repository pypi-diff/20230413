# Comparing `tmp/PolyRound-0.2.7.tar.gz` & `tmp/PolyRound-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PolyRound-0.2.7.tar", last modified: Tue Mar 14 14:23:30 2023, max compression
+gzip compressed data, was "PolyRound-0.2.8.tar", last modified: Thu Apr 13 08:52:16 2023, max compression
```

## Comparing `PolyRound-0.2.7.tar` & `PolyRound-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.390073 PolyRound-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)    34667 2023-03-14 14:23:15.000000 PolyRound-0.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5811 2023-03-14 14:23:30.386072 PolyRound-0.2.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.370071 PolyRound-0.2.7/PolyRound/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/api.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.377072 PolyRound-0.2.7/PolyRound/mutable_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/mutable_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5190 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/mutable_classes/polytope.py
--rw-rw-rw-   0 root         (0) root         (0)     3916 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.382072 PolyRound-0.2.7/PolyRound/static_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7488 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/constraint_removal_reduction.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/csv_io.py
--rw-rw-rw-   0 root         (0) root         (0)    12846 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/lp_interfacing.py
--rw-rw-rw-   0 root         (0) root         (0)     2501 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/lp_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/parse_sbml_stoichiometry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.386072 PolyRound-0.2.7/PolyRound/static_classes/rounding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/rounding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3138 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/rounding/geometric_mean_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)    10569 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
--rw-rw-rw-   0 root         (0) root         (0)    20225 2023-03-14 14:23:15.000000 PolyRound-0.2.7/PolyRound/unit_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:23:30.374071 PolyRound-0.2.7/PolyRound.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5811 2023-03-14 14:23:30.000000 PolyRound-0.2.7/PolyRound.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-03-14 14:23:30.000000 PolyRound-0.2.7/PolyRound.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 14:23:30.000000 PolyRound-0.2.7/PolyRound.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-03-14 14:23:30.000000 PolyRound-0.2.7/PolyRound.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-14 14:23:30.000000 PolyRound-0.2.7/PolyRound.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5310 2023-03-14 14:23:15.000000 PolyRound-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-14 14:23:30.390073 PolyRound-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-03-14 14:23:15.000000 PolyRound-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.964647 PolyRound-0.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)    34667 2023-04-13 08:52:08.000000 PolyRound-0.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-04-13 08:52:16.961647 PolyRound-0.2.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.944646 PolyRound-0.2.8/PolyRound/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-04-13 08:52:08.000000 PolyRound-0.2.8/PolyRound/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.951646 PolyRound-0.2.8/PolyRound/mutable_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/mutable_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/mutable_classes/polytope.py
+-rw-rw-rw-   0 root         (0) root         (0)     3916 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.956647 PolyRound-0.2.8/PolyRound/static_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7488 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/constraint_removal_reduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/csv_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    12846 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/lp_interfacing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/lp_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/parse_sbml_stoichiometry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.961647 PolyRound-0.2.8/PolyRound/static_classes/rounding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/geometric_mean_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10569 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
+-rw-rw-rw-   0 root         (0) root         (0)    20225 2023-04-13 08:52:09.000000 PolyRound-0.2.8/PolyRound/unit_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:52:16.949646 PolyRound-0.2.8/PolyRound.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 08:52:16.000000 PolyRound-0.2.8/PolyRound.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2023-04-13 08:52:09.000000 PolyRound-0.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 08:52:16.964647 PolyRound-0.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-04-13 08:52:09.000000 PolyRound-0.2.8/setup.py
```

### Comparing `PolyRound-0.2.7/LICENSE` & `PolyRound-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PKG-INFO` & `PolyRound-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PolyRound
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for rounding polytopes.
 Home-page: https://gitlab.com/csb.ethz/PolyRound
 Author: Axel Theorell
 Author-email: atheorell@ethz.ch
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PolyRound-0.2.7/PolyRound/__init__.py` & `PolyRound-0.2.8/PolyRound/__init__.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/api.py` & `PolyRound-0.2.8/PolyRound/api.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/main.py` & `PolyRound-0.2.8/PolyRound/main.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/mutable_classes/polytope.py` & `PolyRound-0.2.8/PolyRound/mutable_classes/polytope.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/settings.py` & `PolyRound-0.2.8/PolyRound/settings.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/constraint_removal_reduction.py` & `PolyRound-0.2.8/PolyRound/static_classes/constraint_removal_reduction.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/csv_io.py` & `PolyRound-0.2.8/PolyRound/static_classes/csv_io.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/lp_interfacing.py` & `PolyRound-0.2.8/PolyRound/static_classes/lp_interfacing.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/lp_utils.py` & `PolyRound-0.2.8/PolyRound/static_classes/lp_utils.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/parse_sbml_stoichiometry.py` & `PolyRound-0.2.8/PolyRound/static_classes/parse_sbml_stoichiometry.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/rounding/geometric_mean_scaling.py` & `PolyRound-0.2.8/PolyRound/static_classes/rounding/geometric_mean_scaling.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py` & `PolyRound-0.2.8/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py` & `PolyRound-0.2.8/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound/unit_tests.py` & `PolyRound-0.2.8/PolyRound/unit_tests.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/PolyRound.egg-info/PKG-INFO` & `PolyRound-0.2.8/PolyRound.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PolyRound
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for rounding polytopes.
 Home-page: https://gitlab.com/csb.ethz/PolyRound
 Author: Axel Theorell
 Author-email: atheorell@ethz.ch
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PolyRound-0.2.7/PolyRound.egg-info/SOURCES.txt` & `PolyRound-0.2.8/PolyRound.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/README.md` & `PolyRound-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.7/setup.py` & `PolyRound-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="PolyRound",
-    version="0.2.7",
+    version="0.2.8",
     description="A python package for rounding polytopes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/csb.ethz/PolyRound",
     author="Axel Theorell",
     author_email="atheorell@ethz.ch",
     license="GPL-3.0",
```

