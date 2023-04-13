# Comparing `tmp/sklearn-0.0.post2.tar.gz` & `tmp/sklearn-0.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-0.0.post2.tar", last modified: Wed Jan 25 15:07:08 2023, max compression
+gzip compressed data, was "sklearn-0.0.post4.tar", last modified: Thu Apr 13 12:50:40 2023, max compression
```

## Comparing `sklearn-0.0.post2.tar` & `sklearn-0.0.post4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-01-25 15:07:08.456756 sklearn-0.0.post2/
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3437 2023-01-25 15:07:08.456756 sklearn-0.0.post2/PKG-INFO
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3279 2023-01-25 15:02:30.000000 sklearn-0.0.post2/README.md
--rw-r--r--   0 lesteve  (202587) sed      (26082)       38 2023-01-25 15:07:08.456756 sklearn-0.0.post2/setup.cfg
--rw-r--r--   0 lesteve  (202587) sed      (26082)     4789 2023-01-25 15:05:11.000000 sklearn-0.0.post2/setup.py
-drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-01-25 15:07:08.456756 sklearn-0.0.post2/sklearn.egg-info/
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3437 2023-01-25 15:07:07.000000 sklearn-0.0.post2/sklearn.egg-info/PKG-INFO
--rw-r--r--   0 lesteve  (202587) sed      (26082)      159 2023-01-25 15:07:08.000000 sklearn-0.0.post2/sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)        1 2023-01-25 15:07:07.000000 sklearn-0.0.post2/sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)       14 2023-01-25 15:07:08.000000 sklearn-0.0.post2/sklearn.egg-info/top_level.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3735 2022-11-07 13:41:13.000000 sklearn-0.0.post2/test_brownout.py
+drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-04-13 12:50:40.738130 sklearn-0.0.post4/
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-04-13 12:50:40.738130 sklearn-0.0.post4/PKG-INFO
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3340 2023-04-13 12:50:09.000000 sklearn-0.0.post4/README.md
+-rw-r--r--   0 lesteve  (202587) sed      (26082)       38 2023-04-13 12:50:40.738130 sklearn-0.0.post4/setup.cfg
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     4085 2023-04-13 12:50:23.000000 sklearn-0.0.post4/setup.py
+drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-04-13 12:50:40.738130 sklearn-0.0.post4/sklearn.egg-info/
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 lesteve  (202587) sed      (26082)      159 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)        1 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)       14 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/top_level.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3735 2022-11-07 13:41:13.000000 sklearn-0.0.post4/test_brownout.py
```

### Comparing `sklearn-0.0.post2/PKG-INFO` & `sklearn-0.0.post4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sklearn
-Version: 0.0.post2
+Version: 0.0.post4
 Summary: deprecated sklearn package, use scikit-learn instead
 Description-Content-Type: text/markdown
 
-# Goal
+# ⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
 
-This repo implements the brownout strategy for deprecating the `sklearn`
-package on PyPI.
+⚠️⚠️⚠️ The **`sklearn` PyPI package is deprecated use `scikit-learn` instead** ⚠️⚠️⚠️
 
 # How to fix the error for the main use cases
 
 - use `pip install scikit-learn` rather than `pip install sklearn`
 - replace `sklearn` by `scikit-learn` in your pip requirements files
   (`requirements.txt`, `setup.py,` `setup.cfg`, `Pipfile`, etc ...)
 - if the `sklearn` package is used by one of your dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sklearn-0.0.post2/README.md` & `sklearn-0.0.post4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# Goal
+# ⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
 
-This repo implements the brownout strategy for deprecating the `sklearn`
-package on PyPI.
+⚠️⚠️⚠️ The **`sklearn` PyPI package is deprecated use `scikit-learn` instead** ⚠️⚠️⚠️
 
 # How to fix the error for the main use cases
 
 - use `pip install scikit-learn` rather than `pip install sklearn`
 - replace `sklearn` by `scikit-learn` in your pip requirements files
   (`requirements.txt`, `setup.py,` `setup.cfg`, `Pipfile`, etc ...)
 - if the `sklearn` package is used by one of your dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sklearn-0.0.post2/setup.py` & `sklearn-0.0.post4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,14 @@
 import os
 import sys
 from datetime import datetime, MAXYEAR
 from collections import namedtuple
-import setuptools
 
-try:
-    from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
+from setuptools import setup
 
-    class bdist_wheel(_bdist_wheel):
-        def run(self):
-            message = "\n".join(
-                [
-                    "This is an expected error. Building wheel is disabled "
-                    "for the deprecated sklearn PyPI package to avoid pip caching.",
-                    "For more details about the sklearn PyPI package deprecation, see:",
-                    "https://github.com/scikit-learn/sklearn-pypi-package",
-                ]
-            )
-            raise setuptools.errors.ClassError(message)
-
-    cmdclass = {"bdist_wheel": bdist_wheel}
-
-except ImportError:
-    cmdclass = {}
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 
 def get_brownout_schedule():
     all_start_dates = [datetime(2022, 12, 1)] + [
@@ -114,15 +96,14 @@
         if datetime_str is None:
             checked_datetime = datetime.now()
         else:
             checked_datetime = datetime.fromisoformat(datetime_str)
 
         maybe_raise_error(checked_datetime)
 
-    setuptools.setup(
+    setup(
         description="deprecated sklearn package, use scikit-learn instead",
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         name="sklearn",
-        version="0.0.post2",
-        cmdclass=cmdclass,
+        version="0.0.post4",
     )
```

### Comparing `sklearn-0.0.post2/sklearn.egg-info/PKG-INFO` & `sklearn-0.0.post4/sklearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sklearn
-Version: 0.0.post2
+Version: 0.0.post4
 Summary: deprecated sklearn package, use scikit-learn instead
 Description-Content-Type: text/markdown
 
-# Goal
+# ⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
 
-This repo implements the brownout strategy for deprecating the `sklearn`
-package on PyPI.
+⚠️⚠️⚠️ The **`sklearn` PyPI package is deprecated use `scikit-learn` instead** ⚠️⚠️⚠️
 
 # How to fix the error for the main use cases
 
 - use `pip install scikit-learn` rather than `pip install sklearn`
 - replace `sklearn` by `scikit-learn` in your pip requirements files
   (`requirements.txt`, `setup.py,` `setup.cfg`, `Pipfile`, etc ...)
 - if the `sklearn` package is used by one of your dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sklearn-0.0.post2/test_brownout.py` & `sklearn-0.0.post4/test_brownout.py`

 * *Files identical despite different names*

