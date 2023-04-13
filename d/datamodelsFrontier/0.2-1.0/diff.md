# Comparing `tmp/datamodelsFrontier-0.2.tar.gz` & `tmp/datamodelsFrontier-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamodelsFrontier-0.2.tar", last modified: Thu Apr 13 09:34:52 2023, max compression
+gzip compressed data, was "datamodelsFrontier-1.0.tar", last modified: Thu Apr 13 09:49:58 2023, max compression
```

## Comparing `datamodelsFrontier-0.2.tar` & `datamodelsFrontier-1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:34:52.394852 datamodelsFrontier-0.2/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-06 10:34:10.000000 datamodelsFrontier-0.2/.coveragerc
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1069 2023-04-12 16:30:40.000000 datamodelsFrontier-0.2/LICENSE.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       75 2023-04-12 15:31:53.000000 datamodelsFrontier-0.2/MANIFEST.in
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1440 2023-04-13 09:34:52.394611 datamodelsFrontier-0.2/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1032 2023-04-12 15:19:17.000000 datamodelsFrontier-0.2/README.md
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       38 2023-04-13 09:34:52.394977 datamodelsFrontier-0.2/setup.cfg
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      827 2023-04-13 09:34:48.000000 datamodelsFrontier-0.2/setup.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:34:52.390787 datamodelsFrontier-0.2/src/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:09:59.000000 datamodelsFrontier-0.2/src/__init__.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:34:52.392516 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1440 2023-04-13 09:34:52.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      374 2023-04-13 09:34:52.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/SOURCES.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        1 2023-04-13 09:34:52.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/dependency_links.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       40 2023-04-13 09:34:52.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/requires.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-13 09:34:52.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/top_level.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      733 2023-04-13 08:18:00.000000 datamodelsFrontier-0.2/src/datamodelsFrontier.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:34:52.393909 datamodelsFrontier-0.2/test/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:29:31.000000 datamodelsFrontier-0.2/test/__init__.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1626 2023-04-13 09:33:14.000000 datamodelsFrontier-0.2/test/test_datamodelsFrontier.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.664609 datamodelsFrontier-1.0/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-06 10:34:10.000000 datamodelsFrontier-1.0/.coveragerc
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1069 2023-04-12 16:30:40.000000 datamodelsFrontier-1.0/LICENSE.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       75 2023-04-12 15:31:53.000000 datamodelsFrontier-1.0/MANIFEST.in
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1456 2023-04-13 09:49:58.664417 datamodelsFrontier-1.0/PKG-INFO
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1048 2023-04-13 09:48:54.000000 datamodelsFrontier-1.0/README.md
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       38 2023-04-13 09:49:58.664662 datamodelsFrontier-1.0/setup.cfg
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      827 2023-04-13 09:34:48.000000 datamodelsFrontier-1.0/setup.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.660840 datamodelsFrontier-1.0/src/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:09:59.000000 datamodelsFrontier-1.0/src/__init__.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.662493 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1456 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/PKG-INFO
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      374 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        1 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       40 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/requires.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/top_level.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      733 2023-04-13 09:49:33.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.663869 datamodelsFrontier-1.0/test/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:29:31.000000 datamodelsFrontier-1.0/test/__init__.py
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1626 2023-04-13 09:33:14.000000 datamodelsFrontier-1.0/test/test_datamodelsFrontier.py
```

### Comparing `datamodelsFrontier-0.2/LICENSE.txt` & `datamodelsFrontier-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-0.2/PKG-INFO` & `datamodelsFrontier-1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 0.2
+Version: 1.0
 Summary: Datamodels needed for Frontier API
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -21,19 +21,19 @@
 This package is a simple package with three pydantic data models. 
 The module is called datamodels.
 
 **Example imports:**
 
 *Command Line*
 ```bash
-$ pip install datamodels
+$ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodels import barcode
+from datamodelsFrontier import barcode
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
```

### Comparing `datamodelsFrontier-0.2/README.md` & `datamodelsFrontier-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This package is a simple package with three pydantic data models. 
 The module is called datamodels.
 
 **Example imports:**
 
 *Command Line*
 ```bash
-$ pip install datamodels
+$ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodels import barcode
+from datamodelsFrontier import barcode
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
```

### Comparing `datamodelsFrontier-0.2/setup.py` & `datamodelsFrontier-1.0/setup.py`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-0.2/src/datamodelsFrontier.egg-info/PKG-INFO` & `datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 0.2
+Version: 1.0
 Summary: Datamodels needed for Frontier API
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -21,19 +21,19 @@
 This package is a simple package with three pydantic data models. 
 The module is called datamodels.
 
 **Example imports:**
 
 *Command Line*
 ```bash
-$ pip install datamodels
+$ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodels import barcode
+from datamodelsFrontier import barcode
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
```

### Comparing `datamodelsFrontier-0.2/src/datamodelsFrontier.py` & `datamodelsFrontier-1.0/src/datamodelsFrontier.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     # if this inventory item is out of stock then use the first on in this
     # list at is in stock
     alternative_inventory_items: list[str]
     thg_id: str
     status: str
 
 
-__version__ = '0.2'
+__version__ = '1.0'
```

### Comparing `datamodelsFrontier-0.2/test/test_datamodelsFrontier.py` & `datamodelsFrontier-1.0/test/test_datamodelsFrontier.py`

 * *Files identical despite different names*

