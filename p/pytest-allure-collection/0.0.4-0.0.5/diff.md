# Comparing `tmp/pytest_allure_collection-0.0.4-py3-none-any.whl.zip` & `tmp/pytest_allure_collection-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3779 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2529 b- defN 22-Oct-21 03:07 pytest_allure_collection/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Oct-21 03:11 pytest_allure_collection/__version__.py
--rw-r--r--  2.0 unx     1065 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      536 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      769 b- defN 22-Oct-21 03:12 pytest_allure_collection-0.0.4.dist-info/RECORD
-8 files, 5102 bytes uncompressed, 2397 bytes compressed:  53.0%
+Zip file size: 3783 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2576 b- defN 23-Apr-13 07:22 pytest_allure_collection/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-13 07:22 pytest_allure_collection/__version__.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      513 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      769 b- defN 23-Apr-13 07:23 pytest_allure_collection-0.0.5.dist-info/RECORD
+8 files, 5125 bytes uncompressed, 2401 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pytest_allure_collection/__init__.py
 Comment: 
 
 Filename: pytest_allure_collection/__version__.py
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/LICENSE
+Filename: pytest_allure_collection-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/METADATA
+Filename: pytest_allure_collection-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/WHEEL
+Filename: pytest_allure_collection-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/entry_points.txt
+Filename: pytest_allure_collection-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/top_level.txt
+Filename: pytest_allure_collection-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pytest_allure_collection-0.0.4.dist-info/RECORD
+Filename: pytest_allure_collection-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_allure_collection/__init__.py

```diff
@@ -32,14 +32,15 @@
                 if platform.system().lower() == "windows"
                 else file_path
             )
             test_dict = {
                 "name": test.name,
                 "location": f"{file_path}::{method_name.replace('.', '::')}",
                 "markers": {},
+                "source": test.fspath.strpath,
             }
             markers = test.iter_markers()
             title = getattr(test._obj, "__allure_display_name__", None)
             if title:
                 test_dict["markers"]["allure_title"] = title
             for marker in markers:
                 if marker.name in (
```

## pytest_allure_collection/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `pytest_allure_collection-0.0.4.dist-info/LICENSE` & `pytest_allure_collection-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytest_allure_collection-0.0.4.dist-info/METADATA` & `pytest_allure_collection-0.0.5.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-allure-collection
-Version: 0.0.4
+Version: 0.0.5
 Summary: pytest plugin to collect allure markers without running any tests
 Home-page: https://github.com/jnhyperion/pytest-allure-collection
 Author: Johnny Huang
 Author-email: jnhyperion@gmail.com
-License: UNKNOWN
 Keywords: pytest allure
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
+License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: allure-pytest
 
-UNKNOWN
-
-
```

