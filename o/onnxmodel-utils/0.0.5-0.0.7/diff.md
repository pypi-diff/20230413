# Comparing `tmp/onnxmodel-utils-0.0.5.tar.gz` & `tmp/onnxmodel-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxmodel-utils-0.0.5.tar", last modified: Thu Oct 13 04:31:20 2022, max compression
+gzip compressed data, was "onnxmodel-utils-0.0.7.tar", last modified: Thu Apr 13 02:20:20 2023, max compression
```

## Comparing `onnxmodel-utils-0.0.5.tar` & `onnxmodel-utils-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.451875 onnxmodel-utils-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.447875 onnxmodel-utils-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.447875 onnxmodel-utils-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-10-13 04:31:20.451875 onnxmodel-utils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-13 04:31:20.451875 onnxmodel-utils-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.447875 onnxmodel-utils-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.447875 onnxmodel-utils-0.0.5/src/onnxmodel_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)    77056 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.451875 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3601 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/decompose_sln.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/fuse_mulmatmul.py
--rw-r--r--   0 runner    (1001) docker     (121)     4063 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/merge_matmul.py
--rw-r--r--   0 runner    (1001) docker     (121)    10130 2022-10-13 04:31:01.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 04:31:20.451875 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-13 04:31:20.000000 onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.538002 onnxmodel-utils-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.530001 onnxmodel-utils-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.534001 onnxmodel-utils-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 02:20:20.538002 onnxmodel-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 02:20:20.538002 onnxmodel-utils-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.530001 onnxmodel-utils-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.534001 onnxmodel-utils-0.0.7/src/onnxmodel_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77056 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.538002 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/decompose_sln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/fuse_mulmatmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/merge_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-13 02:20:09.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:20:20.538002 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 02:20:20.000000 onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/top_level.txt
```

### Comparing `onnxmodel-utils-0.0.5/.github/workflows/build.yaml` & `onnxmodel-utils-0.0.7/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/.gitignore` & `onnxmodel-utils-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/LICENSE` & `onnxmodel-utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/PKG-INFO` & `onnxmodel-utils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxmodel-utils
-Version: 0.0.5
+Version: 0.0.7
 Summary: utils for working with onnx models
 Home-page: https://github.com/atksh/onnxmodel-utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2022 atksh
```

### Comparing `onnxmodel-utils-0.0.5/README.md` & `onnxmodel-utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/pyproject.toml` & `onnxmodel-utils-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "onnx-simplifier>=0.4.8",
+    "onnxsim>=0.4.8",
     "onnxruntime>=1.12.1",
     "onnx>=1.12.0",
     "numpy>=1.21.2",
     "pandas>=1.3.3",
     "tqdm>=4.62.3",
 ]
 dynamic = ["version"]
```

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/container.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/container.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/dtype.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/dtype.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/model.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/model.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/base.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/base.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/decompose_sln.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/decompose_sln.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/fuse_mulmatmul.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/fuse_mulmatmul.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/transform/merge_matmul.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/transform/merge_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils/utils.py` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/PKG-INFO` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxmodel-utils
-Version: 0.0.5
+Version: 0.0.7
 Summary: utils for working with onnx models
 Home-page: https://github.com/atksh/onnxmodel-utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2022 atksh
```

### Comparing `onnxmodel-utils-0.0.5/src/onnxmodel_utils.egg-info/SOURCES.txt` & `onnxmodel-utils-0.0.7/src/onnxmodel_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

