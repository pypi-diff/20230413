# Comparing `tmp/cbig_network_correspondence-0.0.5.tar.gz` & `tmp/cbig_network_correspondence-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.0.5.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.0.6.tar", max compression
```

## Comparing `cbig_network_correspondence-0.0.5.tar` & `cbig_network_correspondence-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     3180 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/README.md
--rw-r--r--   0        0        0     2436 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      105 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0      245 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/__install__.py
--rw-r--r--   0        0        0    10455 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     2189 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0     5442 2023-04-13 10:19:33.066640 cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3180 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/README.md
+-rw-r--r--   0        0        0     2376 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      445 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    10455 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     2189 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0     5442 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.6/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.0.5/README.md` & `cbig_network_correspondence-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.5/pyproject.toml` & `cbig_network_correspondence-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.0.5"
+version = "0.0.6"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -32,17 +32,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1, <4.0"
 natsort = "^8.3.1"
 numpy = "^1.20.3"
 nibabel = "^5.0.1"
 scipy = "^1.5.3"
 seaborn = "^0.11.2"
-
-[tool.poetry.scripts]
-my-script = "cbig_network_correspondence.__install__:main"
+gitpython = "^3.1.27"
 
 [tool.poetry.dev-dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-builtins = "*"
```

### Comparing `cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.5/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.5/PKG-INFO` & `cbig_network_correspondence-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbig-network-correspondence
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolbox for exploring network correspondence across atlases
 Home-page: https://rubykong.github.io/cbig_network_correspondence
 License: MIT
 Author: Ruby Kong
 Author-email: roo.cone@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: gitpython (>=3.1.27,<4.0.0)
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
 Requires-Dist: nibabel (>=5.0.1,<6.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: scipy (>=1.5.3,<2.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
 Project-URL: Documentation, https://rubykong.github.io/cbig_network_correspondence
 Project-URL: Repository, https://github.com/rubykong/cbig_network_correspondence
```

